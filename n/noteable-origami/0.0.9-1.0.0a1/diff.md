# Comparing `tmp/noteable_origami-0.0.9.tar.gz` & `tmp/noteable_origami-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteable_origami-0.0.9.tar", max compression
+gzip compressed data, was "noteable_origami-1.0.0a1.tar", max compression
```

## Comparing `noteable_origami-0.0.9.tar` & `noteable_origami-1.0.0a1.tar`

### file list

```diff
@@ -1,21 +1,39 @@
--rw-r--r--   0        0        0     1516 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/LICENSE
--rw-r--r--   0        0        0     1824 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/README.md
--rw-r--r--   0        0        0        0 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/__init__.py
--rw-r--r--   0        0        0       18 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/_version.py
--rw-r--r--   0        0        0    35727 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/client.py
--rw-r--r--   0        0        0     3154 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/format.py
--rw-r--r--   0        0        0      400 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/pathing.py
--rw-r--r--   0        0        0      208 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/__init__.py
--rw-r--r--   0        0        0     6534 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/test_client.py
--rw-r--r--   0        0        0        0 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/types/__init__.py
--rw-r--r--   0        0        0     1813 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/tests/types/test_kernels.py
--rw-r--r--   0        0        0     4549 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/access_levels.py
--rw-r--r--   0        0        0    12013 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/deltas.py
--rw-r--r--   0        0        0    13889 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/files.py
--rw-r--r--   0        0        0     6788 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/jobs.py
--rw-r--r--   0        0        0     9512 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/kernels.py
--rw-r--r--   0        0        0     1517 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/models.py
--rw-r--r--   0        0        0    21180 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/origami/types/rtu.py
--rw-r--r--   0        0        0     2551 2022-10-29 03:57:31.785576 noteable_origami-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 noteable_origami-0.0.9/setup.py
--rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 noteable_origami-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4589 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/README.md
+-rw-r--r--   0        0        0       82 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/__init__.py
+-rw-r--r--   0        0        0    14228 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/api.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/cache.py
+-rw-r--r--   0        0        0    39670 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/rtu.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/models/api/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/base.py
+-rw-r--r--   0        0        0      649 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/datasources.py
+-rw-r--r--   0        0        0      924 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/files.py
+-rw-r--r--   0        0        0      659 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/outputs.py
+-rw-r--r--   0        0        0      475 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/projects.py
+-rw-r--r--   0        0        0      437 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/spaces.py
+-rw-r--r--   0        0        0      681 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/users.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/__init__.py
+-rw-r--r--   0        0        0      803 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/base.py
+-rw-r--r--   0        0        0      953 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_contents.py
+-rw-r--r--   0        0        0     1120 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_execute.py
+-rw-r--r--   0        0        0     1222 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_metadata.py
+-rw-r--r--   0        0        0      703 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_output_collection.py
+-rw-r--r--   0        0        0     1115 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_cells.py
+-rw-r--r--   0        0        0      588 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_metadata.py
+-rw-r--r--   0        0        0      850 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/discriminators.py
+-rw-r--r--   0        0        0      451 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/kernels.py
+-rw-r--r--   0        0        0     4010 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/notebook.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/base.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/__init__.py
+-rw-r--r--   0        0        0     7730 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/files.py
+-rw-r--r--   0        0        0     2508 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/kernels.py
+-rw-r--r--   0        0        0     2640 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/system.py
+-rw-r--r--   0        0        0     1210 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/discriminators.py
+-rw-r--r--   0        0        0     1073 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/errors.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/notebook/__init__.py
+-rw-r--r--   0        0        0    11988 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/notebook/builder.py
+-rw-r--r--   0        0        0     2715 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a1/PKG-INFO
```

### Comparing `noteable_origami-0.0.9/LICENSE` & `noteable_origami-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `noteable_origami-0.0.9/pyproject.toml` & `noteable_origami-1.0.0a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "noteable-origami"
-version = "0.0.9"
+version = "1.0.0-alpha.1"
 description = "The Noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/origami"
 # old setup.cfg had a bdist_wheel option.
@@ -29,37 +29,37 @@
 
 # Manifest.in is subsumed by poetry here
 # https://python-poetry.org/docs/pyproject/#include-and-exclude
 include = []
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<4.0"
 bitmath = "^1.3.3"
-httpx = "^0.23.0"
+httpx = ">=0.22"
 jwt = "^1.3.1"
 nbformat = "^5.4.0"
-orjson = "^3.6.8"
-pydantic = "^1.9.0"
-structlog = "^22.1.0"
-websockets = "^10.3"
+orjson = "^3.8.7"
+pydantic = "^1.10.5"
+websockets = ">=11.0"
 backoff = "^2.1.2"
-
-[tool.poetry.dev-dependencies]
-black = {version = "^22.3.0", allow-prereleases = true}
-isort = "^5.10.1"
-boto = "^2.49.0"
+cryptography = ">=40.0"
+diff-match-patch = "^20200713"
+sending = "^0.3.0"
+importlib-metadata = ">=6.8.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.1"
+pytest-cov = "^4.0.0"
+black = "^23.1.0"
+isort = "^5.12.0"
 flake8-docstrings = "^1.6.0"
 notebook = "^6.4.11"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
 pytest-asyncio = "^0.19.0"
-nox = "^2022.1.7"
-nox-poetry = "^1.0.0"
-pytest-httpx = "^0.21.0"
+structlog = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
@@ -88,19 +88,27 @@
 
 [tool.isort]
 line_length = 100
 multi_line_output = 3
 include_trailing_comma = true
 known_third_party = []
 
+[tool.ruff]
+line-length = 100
+
 [tool.coverage.run]
 branch = false
 omit = ["origami/_version.py", "*/tests/*"]
 
 [tool.coverage.report]
 exclude_lines = ["if self.debug:",
                  "pragma: no cover",
                  "raise AssertionError",
                  "raise NotImplementedError",
                  "if __name__ == '__main__':"]
-ignore_errors = true
-omit = ["origami/_version.py"]
+
+[tool.pytest.ini_options]
+testpaths = [
+    "origami/tests",
+]
+# https://pytest-asyncio.readthedocs.io/en/latest/reference/configuration.html#configuration
+asyncio_mode = "auto"
```

