# Comparing `tmp/pycivitai-0.0.1.tar.gz` & `tmp/pycivitai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycivitai-0.0.1.tar", last modified: Tue Jul 25 04:49:36 2023, max compression
+gzip compressed data, was "pycivitai-0.0.2.tar", last modified: Tue Jul 25 14:17:21 2023, max compression
```

## Comparing `pycivitai-0.0.1.tar` & `pycivitai-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.421267 pycivitai-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 04:49:06.000000 pycivitai-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 04:49:06.000000 pycivitai-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-25 04:49:36.421267 pycivitai-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-25 04:49:06.000000 pycivitai-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.417266 pycivitai-0.0.1/pycivitai/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.417266 pycivitai-0.0.1/pycivitai/client/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/client/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/client/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.421267 pycivitai-0.0.1/pycivitai/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/config/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.421267 pycivitai-0.0.1/pycivitai/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/manager/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/manager/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.421267 pycivitai-0.0.1/pycivitai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-25 04:49:06.000000 pycivitai-0.0.1/pycivitai/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.417266 pycivitai-0.0.1/pycivitai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 04:49:36.000000 pycivitai-0.0.1/pycivitai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 04:49:06.000000 pycivitai-0.0.1/requirements-cli.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 04:49:06.000000 pycivitai-0.0.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-25 04:49:06.000000 pycivitai-0.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 04:49:06.000000 pycivitai-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 04:49:36.421267 pycivitai-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-25 04:49:06.000000 pycivitai-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:36.421267 pycivitai-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-25 04:49:06.000000 pycivitai-0.0.1/test/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-25 04:49:06.000000 pycivitai-0.0.1/test/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 04:49:06.000000 pycivitai-0.0.1/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.381308 pycivitai-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 14:16:46.000000 pycivitai-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 14:16:46.000000 pycivitai-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-25 14:17:21.381308 pycivitai-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-25 14:16:46.000000 pycivitai-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.377308 pycivitai-0.0.2/pycivitai/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.377308 pycivitai-0.0.2/pycivitai/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/client/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.377308 pycivitai-0.0.2/pycivitai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/config/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.377308 pycivitai-0.0.2/pycivitai/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/manager/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/manager/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.381308 pycivitai-0.0.2/pycivitai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-25 14:16:46.000000 pycivitai-0.0.2/pycivitai/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.377308 pycivitai-0.0.2/pycivitai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 14:17:21.000000 pycivitai-0.0.2/pycivitai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 14:16:46.000000 pycivitai-0.0.2/requirements-cli.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 14:16:46.000000 pycivitai-0.0.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-25 14:16:46.000000 pycivitai-0.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 14:16:46.000000 pycivitai-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:17:21.381308 pycivitai-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-25 14:16:46.000000 pycivitai-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:21.381308 pycivitai-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-25 14:16:46.000000 pycivitai-0.0.2/test/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-25 14:16:46.000000 pycivitai-0.0.2/test/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:16:46.000000 pycivitai-0.0.2/test/test_main.py
```

### Comparing `pycivitai-0.0.1/LICENSE` & `pycivitai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/PKG-INFO` & `pycivitai-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycivitai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Client and Model Management for CivitAI.
 Home-page: https://github.com/narugo1992/pycivitai
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Python Client and Model Management for CivitAI.
 Classifier: Development Status :: 5 - Production/Stable
@@ -89,14 +89,24 @@
     # It contains a safetensors and a vae, the safetensors is primary.
     # Homepage of this model: https://civitai.com/models/6755/cetus-mix
     print(civitai_download('Cetus-Mix'))  # the safetensors file (when file not specified, primary file will be chosen)
     print(civitai_download('Cetus-Mix', file='*.vae.pt'))  # get the vae file
 
 ```
 
+If you are using command line, you can get the models with the following commands
+
+```shell
+pycivitai get -m 'DEN_barbucci_artstyle'           # get model, use primary file of the latest version
+pycivitai get -m 'DEN_barbucci_artstyle' -v 'v1.0' # get model, use primary file the v1.0 version
+pycivitai get -m 'Cetus-Mix'                       # get the safetensors file of Cetus-Mix
+pycivitai get -m 'Cetus-Mix' -f '*.vae.pt'         # get the vae file of Cetus-Mix
+
+```
+
 ### Get Information of Model Resource
 
 If you only need to obtain information about the model's resource files, for example, if you need to download the files
 yourself, you can use the `civitai_find_online` function, which will return a `Resource` object.
 
 ```python
 from pycivitai import civitai_find_online, Resource
@@ -129,14 +139,26 @@
 or use the TUI to choose which one to delete
 
 ```shell
 pip install pycivitai[cli]  # this step is necessary
 pycivitai delete-cache
 ```
 
+TUI is like this, build with [InquirerPy](https://github.com/kazhala/InquirerPy):
+
+```
+? Choose model versions to delete:
+  Model cetus_mix(ID: 6755, 2 files, size: 3.899 GiB):
+❯ ○ cetusmix_whalefall2(ID: 105924, 2 files, size: 3.899 GiB)
+
+  Model den_barbucci_artstyle(ID: 85716, 2 files, size: 17.181 KiB):
+  ○ v1_0(ID: 91158, 1 file, size: 7.160 KiB)
+  ○ v2_0(ID: 113049, 1 file, size: 10.021 KiB)
+```
+
 ## F.A.Q.
 
 ### Where will the downloaded model be saved?
 
 The downloaded model will be saved by default in the `~/.cache/civitai` directory. If you need to change the save path,
 you can set the value of the `CIVITAI_HOME` environment variable to your desired save path.
```

### Comparing `pycivitai-0.0.1/README.md` & `pycivitai-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,24 @@
     # It contains a safetensors and a vae, the safetensors is primary.
     # Homepage of this model: https://civitai.com/models/6755/cetus-mix
     print(civitai_download('Cetus-Mix'))  # the safetensors file (when file not specified, primary file will be chosen)
     print(civitai_download('Cetus-Mix', file='*.vae.pt'))  # get the vae file
 
 ```
 
+If you are using command line, you can get the models with the following commands
+
+```shell
+pycivitai get -m 'DEN_barbucci_artstyle'           # get model, use primary file of the latest version
+pycivitai get -m 'DEN_barbucci_artstyle' -v 'v1.0' # get model, use primary file the v1.0 version
+pycivitai get -m 'Cetus-Mix'                       # get the safetensors file of Cetus-Mix
+pycivitai get -m 'Cetus-Mix' -f '*.vae.pt'         # get the vae file of Cetus-Mix
+
+```
+
 ### Get Information of Model Resource
 
 If you only need to obtain information about the model's resource files, for example, if you need to download the files
 yourself, you can use the `civitai_find_online` function, which will return a `Resource` object.
 
 ```python
 from pycivitai import civitai_find_online, Resource
@@ -103,14 +113,26 @@
 or use the TUI to choose which one to delete
 
 ```shell
 pip install pycivitai[cli]  # this step is necessary
 pycivitai delete-cache
 ```
 
+TUI is like this, build with [InquirerPy](https://github.com/kazhala/InquirerPy):
+
+```
+? Choose model versions to delete:
+  Model cetus_mix(ID: 6755, 2 files, size: 3.899 GiB):
+❯ ○ cetusmix_whalefall2(ID: 105924, 2 files, size: 3.899 GiB)
+
+  Model den_barbucci_artstyle(ID: 85716, 2 files, size: 17.181 KiB):
+  ○ v1_0(ID: 91158, 1 file, size: 7.160 KiB)
+  ○ v2_0(ID: 113049, 1 file, size: 10.021 KiB)
+```
+
 ## F.A.Q.
 
 ### Where will the downloaded model be saved?
 
 The downloaded model will be saved by default in the `~/.cache/civitai` directory. If you need to change the save path,
 you can set the value of the `CIVITAI_HOME` environment variable to your desired save path.
```

### Comparing `pycivitai-0.0.1/pycivitai/client/http.py` & `pycivitai-0.0.2/pycivitai/client/http.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/client/resource.py` & `pycivitai-0.0.2/pycivitai/client/resource.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/dispatch.py` & `pycivitai-0.0.2/pycivitai/dispatch.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/entry.py` & `pycivitai-0.0.2/pycivitai/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,32 @@
 import os
 from functools import partial
 
 import click
 from hbutils.scale import size_to_bytes_str
 from hbutils.string import plural_word
 
-from .dispatch import _get_global_manager
+from .dispatch import _get_global_manager, civitai_download
 from .utils import GLOBAL_CONTEXT_SETTINGS
 from .utils import print_version as _origin_print_version
 
 try:
     import InquirerPy
 except (ModuleNotFoundError, ImportError):
     InquirerPy = None
 
+
+def _check_inquirerpy():
+    if InquirerPy is None:
+        raise OSError(
+            'TUI for models deletion not available, '
+            'please install CLI extra with `pip install pycivitiai[cli]`.'
+        )
+
+
 print_version = partial(_origin_print_version, 'pycivitai')
 
 
 @click.group(context_settings={**GLOBAL_CONTEXT_SETTINGS}, help='Command-Line Interface for pycivitai')
 @click.option('-v', '--version', is_flag=True,
               callback=print_version, expose_value=False, is_eager=True)
 def cli():
@@ -56,19 +65,15 @@
                               f'({size_to_bytes_str(model_size, precision=3)}) ...')
                 manager.delete_model(model.model_name_or_id)
                 total_size += model_size
 
             click.echo(f'All models deleted, total {size_to_bytes_str(total_size, precision=3)}.')
 
         else:
-            if InquirerPy is None:
-                raise OSError(
-                    'TUI for models deletion not available, '
-                    'please install CLI extra with `pip install pycivitiai[cli]`.'
-                )
+            _check_inquirerpy()
 
             from InquirerPy import inquirer
             from InquirerPy.base import Choice
             from InquirerPy.separator import Separator
 
             choices = []
             for model in manager.list_models():
@@ -113,7 +118,21 @@
                               f'will be released, confirm?'):
                     for model_name, version_name, _, _ in versions_to_detect:
                         manager.delete_version(model_name, version_name)
                     click.echo(click.style('Deletion complete!', fg='green'))
 
             else:
                 click.echo(click.style('No models found to delete.', fg='yellow'))
+
+
+@cli.command('get', context_settings={**GLOBAL_CONTEXT_SETTINGS},
+             help='Delete downloaded models from storage.')
+@click.option('--model', '-m', 'model', type=str, required=True,
+              help='Title or id of the model.')
+@click.option('--version', '-v', 'version', type=str, default=None,
+              help='Name or id of the version. Latest version will be used when not given.', show_default=True)
+@click.option('--file', '-f', 'file', type=str, default=None,
+              help='Name pattern of the model file. Primary file will be used when not given', show_default=True)
+@click.option('--offline', 'offline', is_flag=True, type=bool, default=False,
+              help='Offline mode. Default is disabled.', show_default=True)
+def get_(model, version, file, offline):
+    click.echo(civitai_download(model, version, file, offline))
```

### Comparing `pycivitai-0.0.1/pycivitai/manager/dispatch.py` & `pycivitai-0.0.2/pycivitai/manager/dispatch.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/manager/model.py` & `pycivitai-0.0.2/pycivitai/manager/model.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/manager/version.py` & `pycivitai-0.0.2/pycivitai/manager/version.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/utils/cli.py` & `pycivitai-0.0.2/pycivitai/utils/cli.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai/utils/download.py` & `pycivitai-0.0.2/pycivitai/utils/download.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai.egg-info/PKG-INFO` & `pycivitai-0.0.2/pycivitai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycivitai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Client and Model Management for CivitAI.
 Home-page: https://github.com/narugo1992/pycivitai
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Python Client and Model Management for CivitAI.
 Classifier: Development Status :: 5 - Production/Stable
@@ -89,14 +89,24 @@
     # It contains a safetensors and a vae, the safetensors is primary.
     # Homepage of this model: https://civitai.com/models/6755/cetus-mix
     print(civitai_download('Cetus-Mix'))  # the safetensors file (when file not specified, primary file will be chosen)
     print(civitai_download('Cetus-Mix', file='*.vae.pt'))  # get the vae file
 
 ```
 
+If you are using command line, you can get the models with the following commands
+
+```shell
+pycivitai get -m 'DEN_barbucci_artstyle'           # get model, use primary file of the latest version
+pycivitai get -m 'DEN_barbucci_artstyle' -v 'v1.0' # get model, use primary file the v1.0 version
+pycivitai get -m 'Cetus-Mix'                       # get the safetensors file of Cetus-Mix
+pycivitai get -m 'Cetus-Mix' -f '*.vae.pt'         # get the vae file of Cetus-Mix
+
+```
+
 ### Get Information of Model Resource
 
 If you only need to obtain information about the model's resource files, for example, if you need to download the files
 yourself, you can use the `civitai_find_online` function, which will return a `Resource` object.
 
 ```python
 from pycivitai import civitai_find_online, Resource
@@ -129,14 +139,26 @@
 or use the TUI to choose which one to delete
 
 ```shell
 pip install pycivitai[cli]  # this step is necessary
 pycivitai delete-cache
 ```
 
+TUI is like this, build with [InquirerPy](https://github.com/kazhala/InquirerPy):
+
+```
+? Choose model versions to delete:
+  Model cetus_mix(ID: 6755, 2 files, size: 3.899 GiB):
+❯ ○ cetusmix_whalefall2(ID: 105924, 2 files, size: 3.899 GiB)
+
+  Model den_barbucci_artstyle(ID: 85716, 2 files, size: 17.181 KiB):
+  ○ v1_0(ID: 91158, 1 file, size: 7.160 KiB)
+  ○ v2_0(ID: 113049, 1 file, size: 10.021 KiB)
+```
+
 ## F.A.Q.
 
 ### Where will the downloaded model be saved?
 
 The downloaded model will be saved by default in the `~/.cache/civitai` directory. If you need to change the save path,
 you can set the value of the `CIVITAI_HOME` environment variable to your desired save path.
```

### Comparing `pycivitai-0.0.1/pycivitai.egg-info/SOURCES.txt` & `pycivitai-0.0.2/pycivitai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/pycivitai.egg-info/requires.txt` & `pycivitai-0.0.2/pycivitai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/setup.py` & `pycivitai-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/test/test_dispatch.py` & `pycivitai-0.0.2/test/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `pycivitai-0.0.1/test/test_entry.py` & `pycivitai-0.0.2/test/test_entry.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 @pytest.fixture()
 def sample_repo(sample_repo_dir):
     with isolated_directory({'repo': sample_repo_dir}):
         def _get_manager(offline):
             return DispatchManager('repo', offline)
 
-        with patch('pycivitai.entry._get_global_manager', _get_manager):
+        with patch('pycivitai.entry._get_global_manager', _get_manager), \
+                patch('pycivitai.dispatch._get_global_manager', _get_manager):
             yield DispatchManager('repo', offline=True)
 
 
 @pytest.fixture()
 def empty_repo():
     with isolated_directory():
         os.makedirs('repo', exist_ok=True)
 
         def _get_manager(offline):
             return DispatchManager('repo', offline)
 
-        with patch('pycivitai.entry._get_global_manager', _get_manager):
+        with patch('pycivitai.entry._get_global_manager', _get_manager), \
+                patch('pycivitai.dispatch._get_global_manager', _get_manager):
             yield DispatchManager('repo', offline=True)
 
 
 @pytest.fixture()
 def mock_all_choices():
     from InquirerPy.base import Choice
     def _get_choices(choices):
@@ -122,7 +124,31 @@
             result = simulate_entry(cli, ['cli', 'delete-cache'])
             assert result.exitcode == 0
             text_aligner.assert_equal(
                 'Deletion cancelled.',
                 result.stdout,
             )
         assert sample_repo.total_size == 25451
+
+    def test_get(self, sample_repo):
+        result = simulate_entry(cli, ['cli', 'get', '-m', 'amiya arknights (old)'])
+        assert result.exitcode == 0
+        assert os.path.samefile(
+            result.stdout.strip(),
+            os.path.join('repo', 'amiya_arknights_old__115427', 'v1_1__124885', 'files', 'amiya.pt'),
+        )
+
+    def test_get_offline(self, sample_repo):
+        result = simulate_entry(cli, ['cli', 'get', '-m', 'amiya arknights (old)', '--offline'])
+        assert result.exitcode == 0
+        assert os.path.samefile(
+            result.stdout.strip(),
+            os.path.join('repo', 'amiya_arknights_old__115427', 'v1_0__124870', 'files', 'amiya.pt'),
+        )
+
+    def test_get_specific_version(self, sample_repo):
+        result = simulate_entry(cli, ['cli', 'get', '-m', 'amiya arknights (old)', '-v', 'v1.0'])
+        assert result.exitcode == 0
+        assert os.path.samefile(
+            result.stdout.strip(),
+            os.path.join('repo', 'amiya_arknights_old__115427', 'v1_0__124870', 'files', 'amiya.pt'),
+        )
```

