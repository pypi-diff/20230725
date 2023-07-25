# Comparing `tmp/env_star-2.0.0.tar.gz` & `tmp/env_star-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_star-2.0.0.tar", max compression
+gzip compressed data, was "env_star-2.1.0.tar", max compression
```

## Comparing `env_star-2.0.0.tar` & `env_star-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2023-07-18 19:51:05.220720 env_star-2.0.0/LICENSE
--rw-r--r--   0        0        0      280 2023-07-18 19:51:05.220720 env_star-2.0.0/README.md
--rw-r--r--   0        0        0      495 2023-07-19 13:37:50.704759 env_star-2.0.0/config/__init__.py
--rw-r--r--   0        0        0     4128 2023-07-19 13:37:50.704759 env_star-2.0.0/config/_helpers.py
--rw-r--r--   0        0        0     3407 2023-07-19 13:37:50.704759 env_star-2.0.0/config/config.py
--rw-r--r--   0        0        0      812 2023-07-19 13:37:50.704759 env_star-2.0.0/config/enums.py
--rw-r--r--   0        0        0     2682 2023-07-19 13:37:50.704759 env_star-2.0.0/config/envconfig.py
--rw-r--r--   0        0        0      501 2023-07-19 13:37:50.704759 env_star-2.0.0/config/exceptions.py
--rw-r--r--   0        0        0      926 2023-07-19 13:37:50.704759 env_star-2.0.0/config/interface.py
--rw-r--r--   0        0        0        0 2023-07-18 19:51:05.220720 env_star-2.0.0/config/py.typed
--rw-r--r--   0        0        0     1224 2023-07-19 13:37:50.704759 env_star-2.0.0/config/utils.py
--rw-r--r--   0        0        0     1015 2023-07-19 14:11:30.576403 env_star-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 env_star-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-18 19:51:05.220720 env_star-2.1.0/LICENSE
+-rw-r--r--   0        0        0      280 2023-07-18 19:51:05.220720 env_star-2.1.0/README.md
+-rw-r--r--   0        0        0      610 2023-07-25 18:58:04.867672 env_star-2.1.0/config/__init__.py
+-rw-r--r--   0        0        0     4129 2023-07-25 18:24:41.544340 env_star-2.1.0/config/_helpers.py
+-rw-r--r--   0        0        0     4102 2023-07-25 18:49:08.522482 env_star-2.1.0/config/config.py
+-rw-r--r--   0        0        0      812 2023-07-19 13:37:50.704759 env_star-2.1.0/config/enums.py
+-rw-r--r--   0        0        0     2682 2023-07-19 13:37:50.704759 env_star-2.1.0/config/envconfig.py
+-rw-r--r--   0        0        0      587 2023-07-25 17:35:39.530082 env_star-2.1.0/config/exceptions.py
+-rw-r--r--   0        0        0      926 2023-07-19 13:37:50.704759 env_star-2.1.0/config/interface.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:51:05.220720 env_star-2.1.0/config/py.typed
+-rw-r--r--   0        0        0     3705 2023-07-25 18:47:21.015429 env_star-2.1.0/config/utils.py
+-rw-r--r--   0        0        0     1279 2023-07-25 18:58:01.679645 env_star-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 env_star-2.1.0/PKG-INFO
```

### Comparing `env_star-2.0.0/LICENSE` & `env_star-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `env_star-2.0.0/config/_helpers.py` & `env_star-2.1.0/config/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         _obj_setattr(instance, self.private_name, value)
 
 
 ExcT = typing.TypeVar("ExcT", bound=Exception)
 
 
 def panic(exc: type[ExcT], message: str, *excargs) -> ExcT:
-    raise exc(f"{message.removesuffix('!')}!", *excargs)
+    return exc(f"{message.removesuffix('!')}!", *excargs)
 
 
 def clean_dotenv_value(value: str) -> str:
     """clean_dotenv_value removes leading and trailing whitespace and removes
     wrapping quotes from the value."""
     # Remove leading and trailing whitespace
     value = value.strip()
```

### Comparing `env_star-2.0.0/config/config.py` & `env_star-2.1.0/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Union,
     overload,
 )
 
 from gyver.attrs import define, info
 
 from config._helpers import clean_dotenv_value, lazyfield, panic
-from config.exceptions import InvalidCast, MissingName
+from config.exceptions import InvalidCast, InvalidEnv, MissingName
 from config.interface import MISSING, _default_cast
 
 T = TypeVar("T")
 
 
 @define
 class EnvMapping(MutableMapping[str, str]):
@@ -64,17 +64,35 @@
     @lazyfield
     def file_values(self):
         return {}
 
     def _read_file(self, env_file: Union[str, Path]):
         with open(env_file, "r") as buf:
             for line in buf:
-                if line.startswith("#"):
+                line = (
+                    line.strip()
+                )  # Remove leading/trailing whitespaces and newlines
+                if not line or line.startswith(
+                    "#"
+                ):  # Skip empty lines and full-line comments
                     continue
+
+                # Handle lines with comments after the value
+
                 name, value = line.split("=", 1)
+                if " #" in value:
+                    value, comment = value.strip().split(" #", 1)
+                    maybe_quote = value[0]
+                    if (
+                        maybe_quote in "'\""
+                        and value[-1] != maybe_quote
+                        and comment[-1] == maybe_quote
+                    ):
+                        value = f"{value} #{comment}"
+
                 yield name.strip(), clean_dotenv_value(value)
 
     def _cast(self, name: str, val: Any, cast: Callable) -> Any:
         try:
             val = cast(val)
         except Exception as e:
             raise panic(
```

### Comparing `env_star-2.0.0/config/enums.py` & `env_star-2.1.0/config/enums.py`

 * *Files identical despite different names*

### Comparing `env_star-2.0.0/config/envconfig.py` & `env_star-2.1.0/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `env_star-2.0.0/config/interface.py` & `env_star-2.1.0/config/interface.py`

 * *Files identical despite different names*

### Comparing `env_star-2.0.0/pyproject.toml` & `env_star-2.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 line_length = 79
 
 [tool.black]
 line_length = 79
 
 [tool.poetry]
 name = "env-star"
-version = "2.0.0"
+version = "2.1.0"
 description = "a minimalist config manager"
 authors = ["Gustavo Correa <self.gustavocardoso@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gustcorrea/env-vars"
 packages = [{ include = "config" }]
 license = "MIT"
 classifiers = [
@@ -36,10 +36,25 @@
 [tool.poetry.group.lint.dependencies]
 flake8 = "^6.0.0"
 black = "^23.7.0"
 isort = "^5.12.0"
 autoflake = "^2.2.0"
 docformatter = "^1.7.5"
 
+
+[tool.poetry.group.test.dependencies]
+pytest-cov = "^4.1.0"
+coverage = "^7.2.7"
+
+[tool.pytest.ini_options]
+addopts = [
+    "--cov=config/",
+    "--cov-report=html",
+    "--cov-config=.coveragerc",
+    "--no-cov-on-fail",
+    "--cov-fail-under=80",
+    "--nf",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `env_star-2.0.0/PKG-INFO` & `env_star-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-star
-Version: 2.0.0
+Version: 2.1.0
 Summary: a minimalist config manager
 Home-page: https://github.com/gustcorrea/env-vars
 License: MIT
 Author: Gustavo Correa
 Author-email: self.gustavocardoso@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

