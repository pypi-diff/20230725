# Comparing `tmp/uszipstats-0.1.tar.gz` & `tmp/uszipstats-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uszipstats-0.1.tar", last modified: Tue Jul 25 18:21:25 2023, max compression
+gzip compressed data, was "uszipstats-0.2.tar", last modified: Tue Jul 25 18:35:20 2023, max compression
```

## Comparing `uszipstats-0.1.tar` & `uszipstats-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:21:25.024683 uszipstats-0.1/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.1/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:21:25.024909 uszipstats-0.1/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-25 18:05:28.000000 uszipstats-0.1/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:21:25.018906 uszipstats-0.1/code_zip/
--rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 18:05:32.000000 uszipstats-0.1/code_zip/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)    40397 2023-07-25 18:05:52.000000 uszipstats-0.1/code_zip/irs_data.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-25 18:21:25.026069 uszipstats-0.1/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1679 2023-07-25 18:21:12.000000 uszipstats-0.1/setup.py
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:21:25.024274 uszipstats-0.1/uszipstats.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:21:24.000000 uszipstats-0.1/uszipstats.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-25 18:21:24.000000 uszipstats-0.1/uszipstats.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-25 18:21:24.000000 uszipstats-0.1/uszipstats.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       38 2023-07-25 18:21:24.000000 uszipstats-0.1/uszipstats.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-25 18:21:24.000000 uszipstats-0.1/uszipstats.egg-info/top_level.txt
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.022297 uszipstats-0.2/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.2/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:35:20.022526 uszipstats-0.2/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-25 18:05:28.000000 uszipstats-0.2/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.018427 uszipstats-0.2/code_zip/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 18:05:32.000000 uszipstats-0.2/code_zip/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)    40386 2023-07-25 18:32:05.000000 uszipstats-0.2/code_zip/irs_data.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-25 18:35:20.023264 uszipstats-0.2/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1663 2023-07-25 18:33:28.000000 uszipstats-0.2/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-25 18:35:20.022028 uszipstats-0.2/uszipstats.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      731 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       33 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-25 18:35:19.000000 uszipstats-0.2/uszipstats.egg-info/top_level.txt
```

### Comparing `uszipstats-0.1/LICENSE.txt` & `uszipstats-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uszipstats-0.1/PKG-INFO` & `uszipstats-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uszipstats
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/uszipstats.git
-Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: DATA,FUNCTIONS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `uszipstats-0.1/code_zip/irs_data.py` & `uszipstats-0.2/code_zip/irs_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     https://colab.research.google.com/drive/1uPT_N3tc_-1JnwddHGCj3qD-OPid0wT1
 """
 
 import pandas as pd
 import numpy as np
 import requests
 import matplotlib.pyplot as plt
-import json
+
 
 df_irs_totals = pd.DataFrame()
 for year in range(2015, 2021):
     url = f'https://us-central1-taxfiling-aggregation.cloudfunctions.net/filings-summary?parm_name=VW_tab_{year}_total_returns_and_amounts'
     response = requests.get(url)
     data = response.json()
     df = pd.DataFrame(data)
```

### Comparing `uszipstats-0.1/setup.py` & `uszipstats-0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 setuptools.setup(
     name='uszipstats',         # How you named your package
     packages=['code_zip'],   # Chose the same as "name"
-    version='0.1',      # Start with a small number and increase it with every change you make
+    version='0.2',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     description='sample package',   # Give a short description about your library
     author='VEDANT RATHI',                   # Type in your name
     author_email='vedrathi10@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/vrathi101/uszipstats.git',
     # I explain this later on
-    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_01.tar.gz',
+    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_02.tar.gz',
     keywords=['DATA', 'FUNCTIONS'],   # Keywords that define your package best
     install_requires=[
         'pandas',
         'numpy',
         'requests',
         'matplotlib',
-        'json',
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         # Define that your audience are developers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

### Comparing `uszipstats-0.1/uszipstats.egg-info/PKG-INFO` & `uszipstats-0.2/uszipstats.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uszipstats
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/uszipstats.git
-Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: DATA,FUNCTIONS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

