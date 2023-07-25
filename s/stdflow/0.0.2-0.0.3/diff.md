# Comparing `tmp/stdflow-0.0.2.tar.gz` & `tmp/stdflow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.2.tar", last modified: Tue Jul 25 02:25:11 2023, max compression
+gzip compressed data, was "stdflow-0.0.3.tar", last modified: Tue Jul 25 14:38:09 2023, max compression
```

## Comparing `stdflow-0.0.2.tar` & `stdflow-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,23 @@
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.425492 stdflow-0.0.2/
--rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.2/LICENSE
--rw-r--r--   0 cyprien    (501) staff       (20)     6450 2023-07-25 02:25:11.425347 stdflow-0.0.2/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)     5931 2023-07-24 15:39:08.000000 stdflow-0.0.2/README.md
--rw-r--r--   0 cyprien    (501) staff       (20)      829 2023-07-25 02:25:04.000000 stdflow-0.0.2/pyproject.toml
--rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-25 02:25:11.425539 stdflow-0.0.2/setup.cfg
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.421778 stdflow-0.0.2/stdflow/
--rw-r--r--   0 cyprien    (501) staff       (20)     3363 2023-07-25 02:24:34.000000 stdflow-0.0.2/stdflow/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)       81 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/config.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.422899 stdflow-0.0.2/stdflow/loaders/
--rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/loaders/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)     1156 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/loaders/csv.py
--rw-r--r--   0 cyprien    (501) staff       (20)     2980 2023-07-24 15:19:12.000000 stdflow-0.0.2/stdflow/metadata.py
--rw-r--r--   0 cyprien    (501) staff       (20)     6526 2023-07-24 15:58:05.000000 stdflow-0.0.2/stdflow/path.py
--rw-r--r--   0 cyprien    (501) staff       (20)    12681 2023-07-24 15:26:56.000000 stdflow-0.0.2/stdflow/step.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.423211 stdflow-0.0.2/stdflow/utils/
--rw-r--r--   0 cyprien    (501) staff       (20)     7383 2023-07-24 14:48:55.000000 stdflow-0.0.2/stdflow/utils/__init__.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.422557 stdflow-0.0.2/stdflow.egg-info/
--rw-r--r--   0 cyprien    (501) staff       (20)     6450 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)      480 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 cyprien    (501) staff       (20)       83 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/requires.txt
--rw-r--r--   0 cyprien    (501) staff       (20)        8 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/top_level.txt
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.425055 stdflow-0.0.2/tests/
--rw-r--r--   0 cyprien    (501) staff       (20)     3430 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_load.py
--rw-r--r--   0 cyprien    (501) staff       (20)      490 2023-07-22 02:45:55.000000 stdflow-0.0.2/tests/test_package_vesion.py
--rw-r--r--   0 cyprien    (501) staff       (20)     5681 2023-07-24 15:20:46.000000 stdflow-0.0.2/tests/test_save.py
--rw-r--r--   0 cyprien    (501) staff       (20)     2089 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_src.py
--rw-r--r--   0 cyprien    (501) staff       (20)      751 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_utils.py
--rw-r--r--   0 cyprien    (501) staff       (20)      628 2023-07-25 02:24:34.000000 stdflow-0.0.2/tests/test_version.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 14:38:09.728139 stdflow-0.0.3/
+-rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.3/LICENSE
+-rw-r--r--   0 cyprien    (501) staff       (20)     6493 2023-07-25 14:38:09.727990 stdflow-0.0.3/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)     5931 2023-07-24 15:39:08.000000 stdflow-0.0.3/README.md
+-rw-r--r--   0 cyprien    (501) staff       (20)      930 2023-07-25 11:56:50.000000 stdflow-0.0.3/pyproject.toml
+-rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-25 14:38:09.728181 stdflow-0.0.3/setup.cfg
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 14:38:09.726225 stdflow-0.0.3/stdflow/
+-rw-r--r--   0 cyprien    (501) staff       (20)     5530 2023-07-25 13:32:51.000000 stdflow-0.0.3/stdflow/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)      135 2023-07-25 05:16:26.000000 stdflow-0.0.3/stdflow/config.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 14:38:09.727410 stdflow-0.0.3/stdflow/loaders/
+-rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.3/stdflow/loaders/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     1134 2023-07-25 03:46:32.000000 stdflow-0.0.3/stdflow/loaders/csv.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     3139 2023-07-25 07:20:59.000000 stdflow-0.0.3/stdflow/metadata.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     6483 2023-07-25 07:16:02.000000 stdflow-0.0.3/stdflow/path.py
+-rw-r--r--   0 cyprien    (501) staff       (20)    15929 2023-07-25 12:54:14.000000 stdflow-0.0.3/stdflow/step.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 14:38:09.727667 stdflow-0.0.3/stdflow/utils/
+-rw-r--r--   0 cyprien    (501) staff       (20)     7526 2023-07-25 07:52:54.000000 stdflow-0.0.3/stdflow/utils/__init__.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 14:38:09.727033 stdflow-0.0.3/stdflow.egg-info/
+-rw-r--r--   0 cyprien    (501) staff       (20)     6493 2023-07-25 14:38:09.000000 stdflow-0.0.3/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)      353 2023-07-25 14:38:09.000000 stdflow-0.0.3/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-25 14:38:09.000000 stdflow-0.0.3/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)       83 2023-07-25 14:38:09.000000 stdflow-0.0.3/stdflow.egg-info/requires.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        8 2023-07-25 14:38:09.000000 stdflow-0.0.3/stdflow.egg-info/top_level.txt
```

### Comparing `stdflow-0.0.2/LICENSE` & `stdflow-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.2/PKG-INFO` & `stdflow-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
+Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stdflow-0.0.2/README.md` & `stdflow-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.2/pyproject.toml` & `stdflow-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+py-modules = ["stdflow"]
+
 [project]
 name = "stdflow"
-version = "0.0.2"
+version = "0.0.3"
 description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
 readme = "README.md"
 authors = [
     { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
 ]
+keywords = ["data science", "data", "flow", "data flow"]
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     'License :: OSI Approved :: MIT License',
     "Programming Language :: Python :: 3.9",
 ]
```

### Comparing `stdflow-0.0.2/stdflow/loaders/csv.py` & `stdflow-0.0.3/stdflow/loaders/csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 
 # Converter function
 def convert_data(data, return_type):
     if return_type == "dict":
         return data
     elif return_type == "list":
-        return list(
-            map(namedtuple("NamedDataFrame", ["name", "dataframe"])._make, data.items())
-        )
+        return list(map(namedtuple("NamedDataFrame", ["name", "dataframe"])._make, data.items()))
     elif return_type == "dotdict":
         return Box(data)
     else:
         raise ValueError('return_type must be either "dict", "list", or "dotdict"')
 
 
 # Load CSV files
```

### Comparing `stdflow-0.0.2/stdflow/metadata.py` & `stdflow-0.0.3/stdflow/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,47 +63,50 @@
     @classmethod
     def from_data(
         cls,
         path: Path,
         data: pd.DataFrame,
         export_method_used: str = "unknown",
         input_files: list["MetaData"] = None,
+        descriptions: dict[str, str] = None,
     ):
         if input_files is not None:
             input_files = list({"uuid": file.uuid} for file in input_files)
         columns = list(
-            {"name": c, "type": t.name, "description": None}
+            {
+                "name": c,
+                "type": t.name,
+                "description": (
+                    descriptions.get(c, None) if isinstance(descriptions, dict) else None
+                ),
+            }
             for c, t in zip(data.columns, data.dtypes)
         )
         return cls(path, columns, export_method_used, input_files or [], uuid_=None)
 
     def __eq__(self, other):
         if isinstance(other, Path):
             return self.path == other
         if isinstance(other, MetaData):
             return self.uuid == other.uuid
         raise ValueError(f"other must be of type Path or str, got {type(other)}")
 
     def __str__(self):
-        return (
-            f"MetaData(\n\t{self.uuid[:4]=}\n\t{self.path=}\n\t{self.input_files=}\n)"
-        )
+        return f"MetaData(\n\t{self.uuid[:6]=}\n\t{self.path=}\n\t{self.input_files=}\n)"
 
     def __repr__(self):
         return self.__str__()
 
 
 def get_file(files: list[dict], path: Path):
     return next(
         (
             f
             for f in files
-            if Path.from_dict(
-                f["step"], f["file_name"], f["file_type"]
-            ).full_path_from_root
+            if Path.from_dict(f["step"], f["file_name"], f["file_type"]).full_path_from_root
             == path.full_path_from_root
         ),
         None,
     )
 
 
 def get_file_md(files: list[MetaData], path: Path):
```

### Comparing `stdflow-0.0.2/stdflow/path.py` & `stdflow-0.0.3/stdflow/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 from __future__ import annotations
 
 import logging
 import os
-from typing import Optional
+from typing import Literal, Optional
 
-from stdflow.config import DATE_VERSION_FORMAT, STEP_PREFIX, VERSION_PREFIX
+from stdflow.config import STEP_PREFIX, VERSION_PREFIX
+from stdflow.types.strftime_type import Strftime
 from stdflow.utils import detect_folders, fstep, fv, remove_dir, retrieve_from_path
 
 logger = logging.getLogger(__name__)
 
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 
 logger.addHandler(ch)
 logger.setLevel(logging.DEBUG)
 
 
 class Path:
     def __init__(
         self,
-        data_root_path: str | None = "./data",
-        path=None,
-        step_name=None,
-        version="last",
-        file_name=None,
+        root: str | None = "./data",
+        attrs: list | None | str = None,
+        step_name: str | None = None,
+        version: str | Literal[":last", ":first"] = ":last",
+        file_name: str = None,
     ):
         """
         At this stage all information are present except the version which is to be detected if not specified
-        :param data_root_path: first part of the full_path
-        :param path: seconds parts of the full_path (optional)
+        :param root: first part of the full_path
+        :param attrs: seconds parts of the full_path (optional)
         :param step_name: third part of the full_path (optional)
-        :param version: last part of the full_path. one of ["last", "first", "<version_name>", None]
+        :param version: last part of the full_path. one of [":last", ":first", "<version_name>", None]
         :param file_name: file name (optional)
         """
         # if step is str and contains step_, remove it
         if isinstance(step_name, str) and step_name.startswith(STEP_PREFIX):
             step_name = step_name[len(STEP_PREFIX) :]
         # if version is str and contains v_, remove it
         if isinstance(version, str) and version.startswith(VERSION_PREFIX):
             version = version[len(VERSION_PREFIX) :]
 
-        self.data_root_path = data_root_path
-        self.path: str = "/".join(path) if isinstance(path, list) else path
+        self.root = root
+        self.path: str = "/".join(attrs) if isinstance(attrs, list) else attrs
         self.step_name = step_name
         self.file_name = file_name
 
         self.version = None
-        if version in ["last", "first"]:
+        if version in [":last", ":first"]:
             if not os.path.isdir(self.dir_path):
                 logger.error(f"Path {self.dir_path} does not exist")
             self.version = self.detect_version(self.dir_path, version)
         elif version is not None:
             self.version = version
 
     @property
@@ -71,38 +72,38 @@
     #
     #     path = os.path.dirname(path)
     #     path = remove_dir(path, file_name) if file_name else path
     #     path = remove_dir(path, fv(version)) if version else path
     #     path = remove_dir(path, fstep(step)) if step else path
     #
     #     return cls(
-    #         data_root_path=path, step_name=step, version=version, file_name=file_name
+    #         root=path, step_name=step, version=version, file_name=file_name
     #     )
 
     def detect_version(self, path, version_type):
-        if version_type not in ["last", "first"]:
+        if version_type not in [":last", ":first"]:
             logger.warning(f"Unknown version type: {version_type}")
         # Check for versioned directories
         versions = detect_folders(path, VERSION_PREFIX)
 
         logger.debug(f"ordered versions: {versions}")
         if not versions:
             logger.warning(f"No versioned directories found in {path}")
 
-        if version_type == "last":
+        if version_type == ":last":
             return versions[-1] if versions else None
-        elif version_type == "first":
+        elif version_type == ":first":
             return versions[0] if versions else None
 
         return None
 
     @property
     def full_path(self):
         return Path.full_path_(
-            self.data_root_path,
+            self.root,
             self.path,
             fstep(self.step_name) if self.step_name else "",
             fv(self.version) if self.version else "",
             self.file_name,
         )
 
     @property
@@ -114,36 +115,34 @@
             fv(self.version) if self.version else "",
             self.file_name,
         )
 
     @property
     def dir_path(self):
         return Path.full_path_(
-            self.data_root_path,
+            self.root,
             self.path,
             fstep(self.step_name) if self.step_name else "",
             fv(self.version) if self.version else "",
             None,
         )
 
     @property
     def step_dir(self):
         return Path.full_path_(
-            self.data_root_path,
+            self.root,
             self.path,
             fstep(self.step_name) if self.step_name else None,
             None,
             None,
         )
 
     @staticmethod
-    def full_path_(data_root_path, path, step, version, file_name):
-        return os.path.join(
-            data_root_path or "", path or "", step or "", version or "", file_name or ""
-        )
+    def full_path_(root, path, step, version, file_name):
+        return os.path.join(root or "", path or "", step or "", version or "", file_name or "")
 
     @property
     def extension(self):
         return os.path.splitext(self.file_name)[-1][1:]
 
     @property
     def dict_step(self):
@@ -152,53 +151,51 @@
             step_name=self.step_name,
             version=self.version,
         )
 
     @classmethod
     def from_dict(cls, step_dict, file_name, file_type):
         return cls(
-            data_root_path=None,
-            path=step_dict["path"],
+            root=None,
+            attrs=step_dict["path"],
             step_name=step_dict["step_name"],
             version=step_dict["version"],
             file_name=f"{file_name}.{file_type}",
         )
 
     @property
     def metadata_path(self):
         return os.path.join(self.dir_path, "metadata.json")
 
     @classmethod
-    def from_input_params(cls, data_root_path, path, step, version, file_name):
+    def from_input_params(cls, root, attrs, step, version, file_name):
         # if step is True:
         #     # extract step from path
         #     step = retrieve_from_path(path, STEP_PREFIX)
         #     path = remove_dir(path, fstep(step))
         # if version is True:
         #     # extract version from path
         #     version = retrieve_from_path(path, VERSION_PREFIX)
         #     path = remove_dir(path, fv(version))
         # if file_name is True:
         #     # extract file_name from path
         #     file_name = os.path.basename(path)
         #     path = os.path.dirname(path)
 
         return cls(
-            data_root_path=data_root_path,
-            path=path,
+            root=root,
+            attrs=attrs,
             step_name=step,
             version=version,
             file_name=file_name,
         )
 
     def __str__(self):
         return self.full_path
 
     def __repr__(self):
         return self.full_path
 
 
 if __name__ == "__main__":
-    path = Path("./data", path="fr", step_name="raw", version="last")
-    assert (
-        path.full_path == "./data/fr/step_raw/v_2/"
-    ), f"src.full_path: {path.full_path}"
+    path = Path("./data", attrs="fr", step_name="raw", version=":last")
+    assert path.full_path == "./data/fr/step_raw/v_2/", f"src.full_path: {path.full_path}"
```

### Comparing `stdflow-0.0.2/stdflow/utils/__init__.py` & `stdflow-0.0.3/stdflow/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import re
 import shutil
 from typing import List, Union
 
 from graphviz import Digraph
 
 from stdflow.config import STEP_PREFIX, VERSION_PREFIX
+from stdflow.html.template import template
+
+
+def get_arg_value(arg, default):
+    if arg == ":default":
+        return default
+    return arg
 
 
 def detect_folders(path: str, prefix: str) -> list:
     full_path_versions = sorted(glob.glob(os.path.join(path, f"{prefix}*")))
-    suffixes = [
-        os.path.basename(v)[len(prefix) :]
-        for v in full_path_versions
-        if os.path.isdir(v)
-    ]
+    suffixes = [os.path.basename(v)[len(prefix) :] for v in full_path_versions if os.path.isdir(v)]
     return suffixes
 
 
 def retrieve_from_path(path: str, prefix: str) -> str:
-    version = [
-        part[len(prefix) :] for part in path.split(os.sep) if part.startswith(prefix)
-    ]
+    version = [part[len(prefix) :] for part in path.split(os.sep) if part.startswith(prefix)]
     return version[-1] if version else None
 
 
 def fv(version):
     """fv: format version"""
     return f"{VERSION_PREFIX}{version}" if version else None
 
@@ -42,17 +43,15 @@
     :param path: Initial path
     :param dir_to_remove: Directory to be removed
     :return: Corrected path
     """
     path_parts = []
 
     # Keep splitting the path until you reach the top
-    while path != os.path.dirname(
-        path
-    ):  # os.path.dirname(path) returns the directory part of path
+    while path != os.path.dirname(path):  # os.path.dirname(path) returns the directory part of path
         path, tail = os.path.split(path)
         if tail == dir_to_remove:
             # Skip the directory to be removed
             break
         path_parts.insert(0, tail)
 
     return os.path.join(path, *path_parts)
@@ -66,17 +65,15 @@
         dot.node(file["file_name"])
         for input_file in file.get("input_files", []):
             # find the file in the list of files using uuid
             print(f"{dest=}")
             print(f"{input_file['uuid']=}")
             print([f["uuid"] for f in metadata["files"]])
 
-            input_file = [
-                f for f in metadata["files"] if f["uuid"] == input_file["uuid"]
-            ][0]
+            input_file = [f for f in metadata["files"] if f["uuid"] == input_file["uuid"]][0]
             dot.edge(input_file["file_name"], file["file_name"])
 
     # Save the graph in DOT format
     dot.save(os.path.join(dest, "pipeline.dot"))
     os.system("dot -Tpng pipeline.dot -o pipeline.png")
     dot.format = "svg"
     dot.render("pipeline")
@@ -90,26 +87,27 @@
     # Load metadata
     with open(metadata_file) as f:
         metadata = json.load(f)
 
     # get_pipeline(metadata, dest)
 
     # Set up Jinja2 environment
-    env = Environment(loader=FileSystemLoader("."))
-    template = env.get_template("stdflow/html/template.html")
+    # env = Environment(loader=FileSystemLoader("."))
+    # template = env.get_template("stdflow/html/template.html")
 
     # Convert to JavaScript
     js_data = json.dumps(metadata)
 
     # Write JS data into HTML file
     with open(os.path.join(dest, "data.js"), "w") as js_file:
         js_file.write(f"var data = {js_data};")
 
-    # cp html/template.html dest
-    shutil.copy("stdflow/html/template.html", dest)
+    # dump the content of template variable in dest/template.html
+    with open(os.path.join(dest, "template.html"), "w") as html_file:
+        html_file.write(template)
 
 
 #     # Write output to HTML file
 #     with open(os.path.join(dest, "pipeline.html"), "w") as html_file:
 #         # html_file.write(output)
 #         html_file.write(
 #             """
```

### Comparing `stdflow-0.0.2/stdflow.egg-info/PKG-INFO` & `stdflow-0.0.3/stdflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
+Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

