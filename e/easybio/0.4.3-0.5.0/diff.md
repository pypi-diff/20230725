# Comparing `tmp/easybio-0.4.3.tar.gz` & `tmp/easybio-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.4.3.tar", last modified: Sat Jul 15 13:06:20 2023, max compression
+gzip compressed data, was "easybio-0.5.0.tar", last modified: Tue Jul 25 05:26:55 2023, max compression
```

## Comparing `easybio-0.4.3.tar` & `easybio-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-15 13:06:20.789289 easybio-0.4.3/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easybio-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easyBio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easyBio/Utils/
--rw-rw-r--   0 root         (0) root         (0)      661 2023-07-07 11:47:13.000000 easybio-0.4.3/easyBio/Utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2854 2023-07-07 09:45:10.000000 easybio-0.4.3/easyBio/Utils/downLoadBAM.py
--rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-07 02:09:13.000000 easybio-0.4.3/easyBio/Utils/downLoadSRA.py
--rw-rw-r--   0 root         (0) root         (0)     8221 2023-07-07 02:07:55.000000 easybio-0.4.3/easyBio/Utils/download.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-07-07 11:51:19.000000 easybio-0.4.3/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     9077 2023-07-06 12:33:28.000000 easybio-0.4.3/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-07-06 13:07:59.000000 easybio-0.4.3/easyBio/Utils/easyCellranger.py
--rw-rw-r--   0 root         (0) root         (0)    12112 2023-07-14 10:32:06.000000 easybio-0.4.3/easyBio/Utils/gsaDownLoadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easybio-0.4.3/easyBio/Utils/netUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2594 2023-07-07 11:45:29.000000 easybio-0.4.3/easyBio/Utils/runvelocityc.py
--rw-rw-r--   0 root         (0) root         (0)     7773 2023-07-14 10:39:20.000000 easybio-0.4.3/easyBio/Utils/toFastq.py
--rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-07 09:45:19.000000 easybio-0.4.3/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 root         (0) root         (0)      426 2023-07-06 12:55:32.000000 easybio-0.4.3/easyBio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2023-07-12 07:12:26.000000 easybio-0.4.3/easyBio/changeSRAName.py
--rw-rw-r--   0 root         (0) root         (0)     2136 2023-07-14 04:32:24.000000 easybio-0.4.3/easyBio/downloadSRA.py
--rw-rw-r--   0 root         (0) root         (0)      200 2023-07-12 06:59:45.000000 easybio-0.4.3/easyBio/easyBio.py
--rw-rw-r--   0 root         (0) root         (0)     2636 2023-07-14 04:40:35.000000 easybio-0.4.3/easyBio/gsaPipline.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-14 10:32:46.000000 easybio-0.4.3/easyBio/pipline.py
--rw-rw-r--   0 root         (0) root         (0)     1324 2023-07-12 07:12:35.000000 easybio-0.4.3/easyBio/run_cellranger.py
--rw-rw-r--   0 root         (0) root         (0)      110 2023-07-12 11:04:38.000000 easybio-0.4.3/easyBio/run_test.py
--rw-rw-r--   0 root         (0) root         (0)     1247 2023-07-12 07:12:38.000000 easybio-0.4.3/easyBio/runvelocyto.py
--rw-rw-r--   0 root         (0) root         (0)     1479 2023-07-12 07:12:42.000000 easybio-0.4.3/easyBio/splitSRA.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easybio-0.4.3/easyBio/test.py
--rw-rw-r--   0 root         (0) root         (0)     2671 2023-07-12 07:12:49.000000 easybio-0.4.3/easyBio/tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easybio.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      538 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      831 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      345 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-14 10:41:43.000000 easybio-0.4.3/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)       27 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 13:06:20.789289 easybio-0.4.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1562 2023-07-15 13:05:23.000000 easybio-0.4.3/setup.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-07-25 05:26:55.715113 easybio-0.5.0/PKG-INFO
+-rwxrwxrwx   0 lei       (1003) lei       (1004)       30 2023-07-19 17:27:09.000000 easybio-0.5.0/README.md
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.711118 easybio-0.5.0/easyBio/
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3907 2023-07-22 14:54:20.000000 easybio-0.5.0/easyBio/SetupBioEnv.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/easyBio/Utils/
+-rwxrwxrwx   0 lei       (1003) lei       (1004)      661 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/__init__.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2854 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downLoadBAM.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2901 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downLoadSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     8221 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/download.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     4193 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downloadUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     9077 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/easyBioUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2216 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/easyCellranger.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)    12094 2023-07-21 16:38:47.000000 easybio-0.5.0/easyBio/Utils/gsaDownLoadUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2117 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/netUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2594 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/runvelocityc.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     7773 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/toFastq.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     4019 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/toolsUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)      426 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/__init__.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     6283 2023-07-21 16:36:07.000000 easybio-0.5.0/easyBio/changeSRAName.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2136 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/downloadSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5153 2023-07-19 18:23:11.000000 easybio-0.5.0/easyBio/easyBio.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2636 2023-07-21 16:35:25.000000 easybio-0.5.0/easyBio/gsaPipline.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     6740 2023-07-21 16:24:07.000000 easybio-0.5.0/easyBio/installConda copy.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5856 2023-07-22 14:54:29.000000 easybio-0.5.0/easyBio/installConda.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5024 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/pipline.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1324 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/run_cellranger.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1247 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/runvelocyto.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1454 2023-07-21 16:38:49.000000 easybio-0.5.0/easyBio/splitSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1006 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/test.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2671 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/tidy.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/easybio.egg-info/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1003) lei       (1004)      887 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)      433 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-07-25 05:26:55.715113 easybio-0.5.0/setup.cfg
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1690 2023-07-25 05:26:06.000000 easybio-0.5.0/setup.py
```

### Comparing `easybio-0.4.3/PKG-INFO` & `easybio-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.4.3
+Version: 0.5.0
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.4.3/easyBio/Utils/__init__.py` & `easybio-0.5.0/easyBio/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/downLoadBAM.py` & `easybio-0.5.0/easyBio/Utils/downLoadBAM.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/downLoadSRA.py` & `easybio-0.5.0/easyBio/Utils/downLoadSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/download.py` & `easybio-0.5.0/easyBio/Utils/download.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/downloadUtils.py` & `easybio-0.5.0/easyBio/Utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/easyBioUtils.py` & `easybio-0.5.0/easyBio/Utils/easyBioUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/easyCellranger.py` & `easybio-0.5.0/easyBio/Utils/easyCellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/gsaDownLoadUtils.py` & `easybio-0.5.0/easyBio/Utils/gsaDownLoadUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Author: Lei
 # Date: 2023-06-08
 # Description:
 from collections import defaultdict
 import os
 import re
 import shutil
-import subprocess
 import threading
 
 import pandas as pd
 
 from .toolsUtils import sraMd5Cal
 from .download import Download
 from .netUtils import requestGet
```

### Comparing `easybio-0.4.3/easyBio/Utils/netUtils.py` & `easybio-0.5.0/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/runvelocityc.py` & `easybio-0.5.0/easyBio/Utils/runvelocityc.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/toFastq.py` & `easybio-0.5.0/easyBio/Utils/toFastq.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/Utils/toolsUtils.py` & `easybio-0.5.0/easyBio/Utils/toolsUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Date: 2023-04-20
 # Description:
 import shutil
 import datetime
 import multiprocessing
 import os
 import hashlib
+import sys
 
 import psutil
 
 def calMd5(filename):
     with open(filename,"rb") as f:
         bytes = f.read() # read file as bytes
         readable_hash = hashlib.md5(bytes).hexdigest();
@@ -118,7 +119,19 @@
     for file_name in os.listdir(source_dir):
         source_file = os.path.join(source_dir, file_name)
         target_file = os.path.join(target_dir, file_name)
 
         if os.path.isfile(source_file):
             shutil.copy2(source_file, target_file)
             print(f"Copied {source_file} to {target_file}")
+
+
+def get_current_system():
+    platform = sys.platform
+    if platform.startswith('win'):
+        return 'Windows'
+    elif platform.startswith('linux'):
+        return 'Linux'
+    elif platform.startswith('darwin'):
+        return 'Mac'
+    else:
+        return 'Unknown'
```

### Comparing `easybio-0.4.3/easyBio/changeSRAName.py` & `easybio-0.5.0/easyBio/changeSRAName.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/downloadSRA.py` & `easybio-0.5.0/easyBio/downloadSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/gsaPipline.py` & `easybio-0.5.0/easyBio/gsaPipline.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/pipline.py` & `easybio-0.5.0/easyBio/pipline.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/run_cellranger.py` & `easybio-0.5.0/easyBio/run_cellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/runvelocyto.py` & `easybio-0.5.0/easyBio/runvelocyto.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/splitSRA.py` & `easybio-0.5.0/easyBio/splitSRA.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import os
-from pathlib import Path
 
 from .Utils import splitSRAfun
 from .Utils import get_num_threads
 
 def main():
     num_threads = get_num_threads()
    # Parse command line arguments
```

### Comparing `easybio-0.4.3/easyBio/test.py` & `easybio-0.5.0/easyBio/test.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easyBio/tidy.py` & `easybio-0.5.0/easyBio/tidy.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.3/easybio.egg-info/PKG-INFO` & `easybio-0.5.0/easybio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.4.3
+Version: 0.5.0
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.4.3/easybio.egg-info/SOURCES.txt` & `easybio-0.5.0/easybio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
 setup.py
+easyBio/SetupBioEnv.py
 easyBio/__init__.py
 easyBio/changeSRAName.py
 easyBio/downloadSRA.py
 easyBio/easyBio.py
 easyBio/gsaPipline.py
+easyBio/installConda copy.py
+easyBio/installConda.py
 easyBio/pipline.py
 easyBio/run_cellranger.py
-easyBio/run_test.py
 easyBio/runvelocyto.py
 easyBio/splitSRA.py
 easyBio/test.py
 easyBio/tidy.py
 easyBio/Utils/__init__.py
 easyBio/Utils/downLoadBAM.py
 easyBio/Utils/downLoadSRA.py
```

### Comparing `easybio-0.4.3/setup.py` & `easybio-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.4.3'
+VERSION = '0.5.0'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
@@ -24,23 +24,26 @@
             'easydownloadSRA=easyBio.downloadSRA:main',
             'easysplitSRA=easyBio.splitSRA:main',
             'easychangeSRAName=easyBio.changeSRAName:main',
             'easycellranger=easyBio.run_cellranger:main',
             'easyscGEOpipline=easyBio.pipline:main', 
             'easyVelocyto=easyBio.runvelocyto:main',
             'easyscGSEpipline=easyBio.gsaPipline:main',
+            'easyInstallConda=easyBio.installConda:main',
+            'easySetupBioEnv=easyBio.SetupBioEnv:main',
         ]
     },
     install_requires=[
         # 'biopython',
         'threadpool',
         'requests',
-        'pandas'
+        'psutil',
+        'pandas',
+        'bs4',
         # 'velocyto',
-        # 'psutil',
         # 'Cython'
         # Add more dependencies here
     ],
     package_data={
         'Utils': ['Utils/*']
     },
     classifiers=[
```

