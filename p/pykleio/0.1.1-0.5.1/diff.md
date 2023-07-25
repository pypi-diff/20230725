# Comparing `tmp/pykleio-0.1.1.tar.gz` & `tmp/pykleio-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykleio-0.1.1.tar", last modified: Tue Feb  7 21:56:32 2023, max compression
+gzip compressed data, was "pykleio-0.5.1.tar", last modified: Tue Jul 25 16:07:56 2023, max compression
```

## Comparing `pykleio-0.1.1.tar` & `pykleio-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.098568 pykleio-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-07 21:56:14.000000 pykleio-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-07 21:56:32.098568 pykleio-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-07 21:56:14.000000 pykleio-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.094568 pykleio-0.1.1/kleio/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.094568 pykleio-0.1.1/kleio/stores/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/stores/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/stores/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/stores/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/stores/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.098568 pykleio-0.1.1/kleio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/utils/uid_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-02-07 21:56:14.000000 pykleio-0.1.1/kleio/utils/vc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.098568 pykleio-0.1.1/pykleio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-07 21:56:32.000000 pykleio-0.1.1/pykleio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-07 21:56:32.000000 pykleio-0.1.1/pykleio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:56:32.000000 pykleio-0.1.1/pykleio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-07 21:56:32.000000 pykleio-0.1.1/pykleio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-07 21:56:32.000000 pykleio-0.1.1/pykleio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-07 21:56:14.000000 pykleio-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-07 21:56:32.098568 pykleio-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:32.098568 pykleio-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:14.000000 pykleio-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-07 21:56:14.000000 pykleio-0.1.1/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-07 21:56:14.000000 pykleio-0.1.1/tests/test_vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-07 21:56:14.000000 pykleio-0.1.1/tests/test_write.py
+drwxr-xr-x   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 16:07:56.411394 pykleio-0.5.1/
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1457 2023-07-25 13:42:47.000000 pykleio-0.5.1/LICENSE
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1557 2023-07-25 16:07:56.411473 pykleio-0.5.1/PKG-INFO
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      986 2023-07-25 13:42:47.000000 pykleio-0.5.1/README.md
+drwxr-xr-x   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 16:07:56.408722 pykleio-0.5.1/kleio/
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        1 2023-07-25 13:42:47.000000 pykleio-0.5.1/kleio/__init__.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)       22 2023-07-25 15:30:57.000000 pykleio-0.5.1/kleio/config.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     9378 2023-07-25 15:35:12.000000 pykleio-0.5.1/kleio/stores.py
+drwxr-xr-x   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 16:07:56.409437 pykleio-0.5.1/kleio/utils/
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)       74 2023-07-25 15:02:44.000000 pykleio-0.5.1/kleio/utils/__init__.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1016 2023-07-25 14:06:05.000000 pykleio-0.5.1/kleio/utils/exceptions.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      716 2023-07-25 13:58:44.000000 pykleio-0.5.1/kleio/utils/util.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     4693 2023-07-25 15:38:42.000000 pykleio-0.5.1/kleio/utils/vc.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1582 2023-07-25 15:28:12.000000 pykleio-0.5.1/kleio/utils/version.py
+drwxr-xr-x   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 16:07:56.410158 pykleio-0.5.1/pykleio.egg-info/
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1557 2023-07-25 16:07:56.000000 pykleio-0.5.1/pykleio.egg-info/PKG-INFO
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      436 2023-07-25 16:07:56.000000 pykleio-0.5.1/pykleio.egg-info/SOURCES.txt
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        1 2023-07-25 16:07:56.000000 pykleio-0.5.1/pykleio.egg-info/dependency_links.txt
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)       50 2023-07-25 16:07:56.000000 pykleio-0.5.1/pykleio.egg-info/requires.txt
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)       12 2023-07-25 16:07:56.000000 pykleio-0.5.1/pykleio.egg-info/top_level.txt
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      103 2023-07-25 13:42:47.000000 pykleio-0.5.1/pyproject.toml
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      785 2023-07-25 16:07:56.411823 pykleio-0.5.1/setup.cfg
+drwxr-xr-x   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 16:07:56.411223 pykleio-0.5.1/tests/
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)        0 2023-07-25 13:42:47.000000 pykleio-0.5.1/tests/__init__.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1900 2023-07-25 13:42:47.000000 pykleio-0.5.1/tests/test_creation.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)      410 2023-07-25 13:42:47.000000 pykleio-0.5.1/tests/test_vcs.py
+-rw-r--r--   0 zouinkhim (898756248) HHMI\Domain Users (1899195968)     1114 2023-07-25 13:42:47.000000 pykleio-0.5.1/tests/test_write.py
```

### Comparing `pykleio-0.1.1/LICENSE` & `pykleio-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykleio-0.1.1/PKG-INFO` & `pykleio-0.5.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-Metadata-Version: 2.1
-Name: pykleio
-Version: 0.1.1
-Summary: Versioned Storage Python SDK - enable version management for nd data
-Home-page: https://github.com/JaneliaSciComp/KLEIO-Python-SDK
-Author: Marwan Zouinkhi
-Author-email: zouinkhi.marwan@gmail.com
-Project-URL: Bug Tracker, https://github.com/JaneliaSciComp/KLEIO-Python-SDK/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Versioned Storage Python SDK 
 | [JAVA SDK IS HERE](https://github.com/JaneliaSciComp/VersionedN5)
 
 
 ----
 #### Proposed solution:
 To enable block-based data versioning for nd data, a mix is created of:
 - Version block index using [Zarr](https://zarr.readthedocs.io/en/stable/) + [Git](https://git-scm.com/)
 - A key value store: using [N5](https://github.com/saalfeldlab/n5) for now
 
+### How to:
+```
+index_store = ZarrIndexStore(INDEX_PATH)
+store = VersionedFSStore(index_store, RAW_PATH)
+
+z = zarr.open(store, mode="a")
+
+# Commit
+store.vc.commit()
+
+# Push
+store.vc.push()
+
+# Create new branch
+store.vc.create_new_branch(BRANCH_NAME)
+
+# Checkout new branch
+store.vc.create_new_branch(BRANCH_NAME)
+```
+
 
 ### Features:
 - Multiple branches
 - Multiple collaborators
 - Can jump anytime to any historical point
 - Data is not replicated and no extra reading writing cost
```

### Comparing `pykleio-0.1.1/kleio/stores/zarr.py` & `pykleio-0.5.1/kleio/stores.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any, Union
 
 import numpy as np
-from ..utils.uid_rest import get_next_id
-from ..utils.exceptions import InvalidAccessModeError
-from ..utils import util
-from ..utils.vc import VCS
-
 import zarr
-from zarr.storage import NestedDirectoryStore, array_meta_key
-from zarr.n5 import N5FSStore, is_chunk_key
 from zarr.codecs import Zlib
 from zarr.meta import decode_array_metadata, encode_array_metadata, decode_dtype
+from zarr.n5 import N5FSStore, is_chunk_key
+from zarr.storage import NestedDirectoryStore, array_meta_key
+
+from kleio.utils import util
+from kleio.utils.exceptions import InvalidAccessModeError, TmpVersionException
+from kleio.utils.vc import VCS
 
 index_default_dtype = "i8"
 index_default_chunk = 64
 index_default_compressor = Zlib()
 
 
 def get_dataset_name(key, dimension_separator="/"):
@@ -148,32 +147,33 @@
 
 class VersionedFSStore(N5FSStore):
 
     def __init__(self, index_store: Union[ZarrIndexStore, N5FSIndexStore], *args, **kwargs):
         super().__init__(*args, **kwargs)
         # self.index_store = Array(index_store)
         self._index_store = index_store
-        self.__current_version: np.uint64 = None
+        # self.__current_version: np.uint64 = None
         self.__index_array = None
 
     @property
     def vc(self):
         return self._index_store.vc
 
     @property
     def _index_array(self):
         if self.__index_array is None:
             self.__index_array = zarr.open(self._index_store, mode="a")
         return self.__index_array
 
     @property
     def current_version(self):
-        if self.__current_version is None:
-            self.__current_version = self._increment_version()
-        return self.__current_version
+        current = self.vc.current_version.current
+        if current is None:
+            raise TmpVersionException("Current version is None")
+        return current
 
     # Arrays check is this method exist, if not, arrays load the chunk blocks implemented to append the version ID to
     # the path of the block dataset/VERSION/chunk_id
     # NB: add the version to the key should be done before normalizing
     # the key dataset/0.0 -> dataset/VERSION/0.0 won't work if block id is 0/0
     # z[dataset][:] will call this instead of __getitem__
 
@@ -214,18 +214,14 @@
         elif key.endswith(array_meta_key):
             self._index_store.create_dataset_for(key, value)
             # self._index_store.vc.commit_all("create :{}".format(key))
         else:
             self._index_store.__setitem__(key, value)
         super().__setitem__(key, value)
 
-    def _increment_version(self):
-        self.__current_version = get_next_id()
-        return self.current_version
-
     def _get_version_for(self, key):
         dataset, position = util.decode_key_into_dataset_position(key)
         return self._index_array[dataset][position]
 
     def __set_index_version_items(self, keys, version):
         print("set version index items: {} ".format(keys))
         to_be_updated = {}
```

### Comparing `pykleio-0.1.1/kleio/utils/exceptions.py` & `pykleio-0.5.1/kleio/utils/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 class BaseKleioError(Exception):
     _msg = ""
 
     def __init__(self, *args: object) -> None:
         super().__init__(self._msg.format(*args))
 
 
+class TmpVersionException(BaseKleioError):
+    _msg = "{}"
+
+
 class InvalidDataDaskFillError(BaseKleioError):
     _msg = "Invalid data type for fill: {0!r}"
 
 
 class InvalidCompressionIndexError(BaseKleioError):
     _msg = "compression index: {0!r} is not in (0, 9) range"
```

### Comparing `pykleio-0.1.1/kleio/utils/util.py` & `pykleio-0.5.1/kleio/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-
+import json
 
 def read_file(fn):
     with open(fn, 'rb') as f:
         return f.read()
 
 
 def write_file(a, fn):
@@ -19,7 +19,8 @@
     segments = list(key.split(dataset_separator))
     result_dataset = segments[:-1]
     if not isinstance(result_dataset, str):
         result_dataset = dataset_separator.join(result_dataset)
     last_part = segments[-1]
     grid_position = [int(k) for k in last_part.split(dimension_separator)]
     return result_dataset, tuple(grid_position)
+
```

### Comparing `pykleio-0.1.1/kleio/utils/vc.py` & `pykleio-0.5.1/kleio/utils/vc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import time
 
 from git import Repo, InvalidGitRepositoryError, NoSuchPathError
 
 from .exceptions import InvalidCompressionIndexError
+from .version import Version
 
 
 class VCS(object):
 
     def __init__(self, path: str, compression=0):
         """Create a new VCS instance
         :param path:
@@ -20,19 +21,21 @@
             can vary from 0 to 9. 9 is the slowest
         :return: ``vc.VCS`` """
         if not (0 <= compression <= 9):
             raise InvalidCompressionIndexError(compression)
         self._path = path
         self._compression = compression
         self._repo = None
+        self.current_version = None
 
     @property
     def repo(self):
         if self._repo is None:
             self._repo = Repo(self._path)
+            self.current_version = Version(self._path)
         return self._repo
 
     def is_git_repo(self):
         try:
             _ = self.repo.git_dir
             return True
         except InvalidGitRepositoryError:
@@ -55,15 +58,15 @@
             # Enable git push to this branch
             if not cw.has_section("receive"):
                 cw.add_section("receive")
             # because server git version is 1.8.0
             cw.set("receive", "denyCurrentBranch", "false")
             # for newer git version use (2.3.6)
             # cw.set("receive", "denyCurrentBranch", "updateInstead")
-
+        self.current_version = Version(self._path, create=True)
         # self.commit('Initial commit')
 
     def add_all(self):
         """stage all local changes to git index"""
         self.repo.git.add(all=True)
 
     def add(self, files: [str]):
@@ -75,23 +78,25 @@
                 """
         self.repo.index.add(files)
 
     def commit(self, message: str):
         """commit staged changes , need add() before
         :param message: commit message. """
         self.repo.index.commit(message)
+        self.current_version.increment()
 
     def commit_all(self, message: str = None):
         """commit staged changes , need add() before
         :param message: commit message. """
         if message is None:
             files = self.untracked_files()
             message = "-".join(files)
         self.repo.git.add(all=True)
         self.repo.index.commit(message)
+        self.current_version.increment()
 
     def show_history(self):
         """ Show git history """
         repo = Repo.init(self._path)
         commits = repo.iter_commits('--all')
         for commit in commits:
             print("Committed by %s on %s with sha %s" % (
@@ -112,47 +117,18 @@
         if create:
             print("Create new branch: {}".format(branch_name))
             repo.git.checkout('-b', branch_name)
         else:
             # print("Moved to branch: {}".format(branch_name))
             repo.git.checkout(branch_name)
 
-    def clone_to(self, dist_path):
-        Repo.clone_from(self._path, dist_path)
-        print("cloned.")
-
     def gc(self):
         """Collect garbage, to be run every while """
         repo = Repo.init(self._path)
         repo.git.gc()
 
-    @staticmethod
-    def push_repo(path):
-        repo = Repo(path)
-        repo.git.push()
-
-    # TODO remote change
-
-    # @staticmethod
-    # def push_repo(path, client: RemoteClient):
-    #     repo = Repo(path)
-    #     repo.git.push(env={
-    #         f"GIT_SSH_COMMAND": f"sshpass -p {client.password} ssh -l {client.user}"})
-    #
-    # @classmethod
-    # def remote_clone(cls, remote_client: RemoteClient, remote_path, path):
-    #     try:
-    #         repo = Repo.clone_from(f"ssh://{remote_client.host}:{remote_path}",
-    #                                path, env={
-    #                 "GIT_SSH_COMMAND": f"sshpass -p {remote_client.password} ssh -l {remote_client.user}"})
-    #     except Exception as e:
-    #         # TODO don't use Exception / raise or recover
-    #         print("Error!")
-    #         print(e)
-    #     else:
-    #         print("Repo cloned successfully!")
-
     @classmethod
     def make_bare(cls, path):
         repo = Repo(path)
         with repo.config_writer() as cw:
             cw.set("core", "bare", "true")
+
```

### Comparing `pykleio-0.1.1/setup.cfg` & `pykleio-0.5.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pykleio
-version = 0.1.1
+version = 0.5.1
 author = Marwan Zouinkhi
 author_email = zouinkhi.marwan@gmail.com
 description = Versioned Storage Python SDK - enable version management for nd data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JaneliaSciComp/KLEIO-Python-SDK
 project_urls = 
@@ -18,26 +18,20 @@
 packages = find:
 python_requires = >=3.6
 test_suite = tests
 install_requires = 
 	numpy
 	zarr
 	fsspec
-	tqdm
-	dask
-	paramiko
-	scp
-	requests
 	deprecation
 	numcodecs
 	GitPython
 
 [options.packages.find]
 exclude = 
 	examples*
-	versionedzarrlib*
 	img*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pykleio-0.1.1/tests/test_creation.py` & `pykleio-0.5.1/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `pykleio-0.1.1/tests/test_write.py` & `pykleio-0.5.1/tests/test_write.py`

 * *Files identical despite different names*

