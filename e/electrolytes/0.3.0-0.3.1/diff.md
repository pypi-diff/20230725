# Comparing `tmp/electrolytes-0.3.0.tar.gz` & `tmp/electrolytes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.3.0.tar", last modified: Mon Jul 24 21:03:47 2023, max compression
+gzip compressed data, was "electrolytes-0.3.1.tar", last modified: Tue Jul 25 21:50:39 2023, max compression
```

## Comparing `electrolytes-0.3.0.tar` & `electrolytes-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-24 21:03:34.000000 electrolytes-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-24 21:03:47.855215 electrolytes-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-24 21:03:34.000000 electrolytes-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.851215 electrolytes-0.3.0/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/db1.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:34.000000 electrolytes-0.3.0/electrolytes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 21:03:47.000000 electrolytes-0.3.0/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-24 21:03:34.000000 electrolytes-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:03:47.855215 electrolytes-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:03:47.855215 electrolytes-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-24 21:03:34.000000 electrolytes-0.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-24 21:03:34.000000 electrolytes-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-25 21:50:28.000000 electrolytes-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 21:50:39.964221 electrolytes-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-25 21:50:28.000000 electrolytes-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/db1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-25 21:50:28.000000 electrolytes-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:50:39.964221 electrolytes-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-25 21:50:28.000000 electrolytes-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-25 21:50:28.000000 electrolytes-0.3.1/tests/test_cli.py
```

### Comparing `electrolytes-0.3.0/LICENSE.txt` & `electrolytes-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.0/PKG-INFO` & `electrolytes-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.0
+Version: 0.3.1
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
```

### Comparing `electrolytes-0.3.0/README.md` & `electrolytes-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.0/electrolytes/__init__.py` & `electrolytes-0.3.1/electrolytes/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 import pkgutil
 from pathlib import Path
 from typing import Iterable, Iterator, List, Sequence, Dict, Optional, Any
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
+if sys.version_info >= (3, 8):
+    from functools import cached_property
+else:
+    from backports.cached_property import cached_property
 from warnings import warn
 
 from pydantic import BaseModel, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from filelock import FileLock
 from typer import get_app_dir
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 class Constituent(BaseModel, populate_by_name=True, frozen=True):
     id: Optional[int] = None
     name: str
     u_neg: Annotated[List[float], Field(alias="uNeg")] = [] # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     u_pos: Annotated[List[float], Field(alias="uPos")] = [] # [+1, +2, +3, ..., +pos_count]
@@ -94,80 +98,74 @@
     def _counts(cls, v: Optional[int], info: FieldValidationInfo) -> int:
         if v is None:
             v = len(info.data[f"u_{info.field_name[:3]}"])
         elif v != len(info.data[f"u_{info.field_name[:3]}"]):
             raise ValueError(f"{info.field_name} != len(u_{info.field_name[:3]})")
         return v
 
-    @model_validator(mode="after") # type: ignore # https://github.com/pydantic/pydantic/issues/6709
+    @model_validator(mode="after")
     def _pkas_not_increasing(self) -> "Constituent":
         pkas = [*self.pkas_neg, *self.pkas_pos]
 
         if not all(x>=y for x, y in zip(pkas, pkas[1:])):
             raise ValueError("pKa values must not increase with charge")
 
-        return self # type: ignore # https://github.com/pydantic/pydantic/issues/6709
+        return self
 
 
 _StoredConstituents = TypeAdapter(Dict[str, List[Constituent]])
 
 def _load_constituents(data: bytes, context: Optional[Dict[str,str]]=None) -> List[Constituent]:
     return _StoredConstituents.validate_json(data, context=context)["constituents"]
 
 def _dump_constituents(constituents: List[Constituent]) -> bytes:
     return  _StoredConstituents.dump_json({"constituents": constituents}, by_alias=True, indent=4)
 
 
-class _Database:
-    def __init__(self) -> None:
-        self._loaded_default_constituents: Optional[Dict[str, Constituent]] = None
-        self._loaded_user_constituents: Optional[Dict[str, Constituent]] = None
+class _FileLock(FileLock):
+    def __enter__(self) -> Any:
+        Path(self.lock_file).parent.mkdir(parents=True, exist_ok=True) # https://github.com/tox-dev/py-filelock/issues/176
+        return super().__enter__()
 
-    @property
+
+class _Database:
+    @cached_property
     def _default_constituents(self) -> Dict[str, Constituent]:
-        if self._loaded_default_constituents is None:
-            data = pkgutil.get_data(__package__, "db1.json")
-            if data is None:
-                raise RuntimeError("failed to load default constituents")
-            constituents = _load_constituents(data, context={"fix": "db1"})
-            self._loaded_default_constituents = {c.name: c for c in constituents}
-        return self._loaded_default_constituents
-    
-    _USER_CONSTITUENTS_FILE = Path(get_app_dir(__package__), "user_constituents.json")
+        data = pkgutil.get_data(__package__, "db1.json")
+        if data is None:
+            raise RuntimeError("failed to load default constituents")
+        constituents = _load_constituents(data, context={"fix": "db1"})
+        return {c.name: c for c in constituents}
 
-    _USER_CONSTITUENTS_FILE.parent.mkdir(parents=True, exist_ok=True) # https://github.com/tox-dev/py-filelock/issues/176
-    _user_constituents_lock = FileLock(_USER_CONSTITUENTS_FILE.with_suffix(".lock"))
+    _USER_CONSTITUENTS_FILE = Path(get_app_dir(__package__), "user_constituents.json")
+    _user_constituents_file_lock = _FileLock(_USER_CONSTITUENTS_FILE.with_suffix(".lock"))
 
-    @_user_constituents_lock
-    def _reload_user_constituents(self) -> None:
+    @cached_property
+    def _user_constituents(self) -> Dict[str, Constituent]:
         try:
-            with self._USER_CONSTITUENTS_FILE.open("rb") as f:
+            with self._user_constituents_file_lock, self._USER_CONSTITUENTS_FILE.open("rb") as f:
                 data = f.read()
-        except FileNotFoundError:
-            self._loaded_user_constituents = {}
-            return
+        except OSError:
+            return {}
         try:
             constituents = _load_constituents(data)
         except Exception as e:
             warn(f"failed to load user constituents from {self._USER_CONSTITUENTS_FILE}: {type(e).__name__}", RuntimeWarning)
-            self._loaded_user_constituents = {}
-            return
-        self._loaded_user_constituents = {c.name: c for c in constituents}
-
-    @property
-    def _user_constituents(self) -> Dict[str, Constituent]:
-        if self._loaded_user_constituents is None:
-            self._reload_user_constituents()
-        assert self._loaded_user_constituents is not None
-        return self._loaded_user_constituents
+            return {}
+        return {c.name: c for c in constituents}
     
-    @_user_constituents_lock
+    def _invalidate_user_constituents(self) -> None:
+        try:
+            del self._user_constituents
+        except AttributeError:
+            pass
+
+    @_user_constituents_file_lock
     def _save_user_constituents(self) -> None:
-        assert self._loaded_user_constituents is not None
-        data = _dump_constituents(list(self._loaded_user_constituents.values()))
+        data = _dump_constituents(list(self._user_constituents.values()))
         self._USER_CONSTITUENTS_FILE.parent.mkdir(parents=True, exist_ok=True)
         with self._USER_CONSTITUENTS_FILE.open("wb") as f:
             f.write(data)
 
 
     def __iter__(self) -> Iterator[str]:
         yield from sorted([*self._default_constituents, *self._user_constituents])
@@ -175,28 +173,28 @@
     def __getitem__(self, name: str) -> Constituent:
         name = name.upper()
         try:
             return self._user_constituents[name]
         except KeyError:
             return self._default_constituents[name]
 
-    @_user_constituents_lock
+    @_user_constituents_file_lock
     def add(self, constituent: Constituent) -> None:
-        self._reload_user_constituents()
+        self._invalidate_user_constituents()
         if constituent.name not in self:
             self._user_constituents[constituent.name] = constituent
             self._save_user_constituents()
         else:
             warn(f"{constituent.name}: component was not added (name already exists in database)")
 
-    @_user_constituents_lock
+    @_user_constituents_file_lock
     def __delitem__(self, name: str) -> None:
         name = name.upper()
         try:
-            self._reload_user_constituents()
+            self._invalidate_user_constituents()
             del self._user_constituents[name]
             self._save_user_constituents()
         except KeyError:
             if name in self._default_constituents:
                 raise ValueError(f"{name}: cannot remove default component")
             else:
                 raise
```

### Comparing `electrolytes-0.3.0/electrolytes/__main__.py` & `electrolytes-0.3.1/electrolytes/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             any_omitted = True
         elif any_omitted:
             typer.echo(f"Error: missing charge -{i}", err=True)
             raise typer.Exit(code=1)
         else:
             pos.append(p)
 
-    with database._user_constituents_lock:
+    with database._user_constituents_file_lock:
         if not force and database.is_user_defined(name):
             typer.echo(f"Error: user-defined component {name} already exists (use -f to replace)", err=True)
             raise typer.Exit(code=1)
 
         try:
             constituent = Constituent(name=name,
                                     u_neg=[x[0] for x in neg],
```

### Comparing `electrolytes-0.3.0/electrolytes/db1.json` & `electrolytes-0.3.1/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.0/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.3.1/electrolytes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.0
+Version: 0.3.1
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
```

### Comparing `electrolytes-0.3.0/pyproject.toml` & `electrolytes-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ]
 
 dependencies = [
     "typer>=0.9.0,<0.10",
     "pydantic>=2.0.3,<3",
     "filelock==3.*",
     "typing-extensions>=3.7.4.3,<5; python_version<'3.9'",
+    "backports.cached_property>=1.0.2,<2; python_version<'3.8'",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 lint = [
     "mypy==1.*",
```

### Comparing `electrolytes-0.3.0/tests/test_api.py` & `electrolytes-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.0/tests/test_cli.py` & `electrolytes-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

