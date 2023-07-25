# Comparing `tmp/suta_ble_bed-0.3.2.tar.gz` & `tmp/suta_ble_bed-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suta_ble_bed-0.3.2.tar", last modified: Mon Apr 10 22:02:19 2023, max compression
+gzip compressed data, was "suta_ble_bed-0.3.3.tar", last modified: Tue Jul 25 02:21:27 2023, max compression
```

## Comparing `suta_ble_bed-0.3.2.tar` & `suta_ble_bed-0.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/
--rw-r--r--   0 simon     (1000) simon     (1002)     3581 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/CONTRIBUTING.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      888 2023-04-10 21:50:37.000000 suta_ble_bed-0.3.2/HISTORY.rst
--rw-r--r--   0 simon     (1000) simon     (1002)     1069 2023-03-04 01:55:36.000000 suta_ble_bed-0.3.2/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1002)      242 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1002)     3919 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1002)     2239 2023-04-10 22:02:04.000000 suta_ble_bed-0.3.2/README.rst
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.228831 suta_ble_bed-0.3.2/docs/
--rw-r--r--   0 simon     (1000) simon     (1002)      613 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/Makefile
--rwxr-xr-x   0 simon     (1000) simon     (1002)     4843 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/conf.py
--rw-r--r--   0 simon     (1000) simon     (1002)       33 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/contributing.rst
--rw-r--r--   0 simon     (1000) simon     (1002)       28 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/history.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      298 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/index.rst
--rw-r--r--   0 simon     (1000) simon     (1002)     1150 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/installation.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      810 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/make.bat
--rw-r--r--   0 simon     (1000) simon     (1002)       27 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/readme.rst
--rw-r--r--   0 simon     (1000) simon     (1002)       79 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/usage.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      384 2023-04-10 22:02:19.231831 suta_ble_bed-0.3.2/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1002)     1543 2023-04-10 22:00:37.000000 suta_ble_bed-0.3.2/setup.py
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.229831 suta_ble_bed-0.3.2/suta_ble_bed/
--rw-r--r--   0 simon     (1000) simon     (1002)      320 2023-04-10 21:47:02.000000 suta_ble_bed-0.3.2/suta_ble_bed/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1002)      234 2023-03-24 02:10:42.000000 suta_ble_bed-0.3.2/suta_ble_bed/__main__.py
--rwxr-xr-x   0 simon     (1000) simon     (1002)     1727 2023-04-10 21:43:38.000000 suta_ble_bed-0.3.2/suta_ble_bed/cli.py
--rw-r--r--   0 simon     (1000) simon     (1002)     4199 2023-04-10 21:43:38.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed.py
--rw-r--r--   0 simon     (1000) simon     (1002)     3219 2023-03-24 21:42:50.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed_controller.py
--rw-r--r--   0 simon     (1000) simon     (1002)     1656 2023-03-24 21:25:34.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_consts.py
--rw-r--r--   0 simon     (1000) simon     (1002)     1322 2023-03-24 20:28:13.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_scanner.py
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1002)     3919 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1002)      728 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1002)       56 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-03-22 00:41:32.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/not-zip-safe
--rw-r--r--   0 simon     (1000) simon     (1002)       43 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1002)       13 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/tests/
--rw-r--r--   0 simon     (1000) simon     (1002)       42 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/tests/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1002)      412 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/tests/test_suta_ble_bed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/suta_ble_bed/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1727 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_bed_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 02:21:27.000000 suta_ble_bed-0.3.3/suta_ble_bed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:21:27.479868 suta_ble_bed-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 02:21:16.000000 suta_ble_bed-0.3.3/tests/test_suta_ble_bed.py
```

### Comparing `suta_ble_bed-0.3.2/CONTRIBUTING.rst` & `suta_ble_bed-0.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/HISTORY.rst` & `suta_ble_bed-0.3.3/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
 
+0.3.3 (2023-07-24)
+------------------
+* Added release pipeline
+
 0.3.2 (2023-04-10)
 ------------------
 * Fix disconnect callback
 * Correct comment on BLE characteristics
 
 0.3.1 (2023-03-23)
 ------------------
```

### Comparing `suta_ble_bed-0.3.2/LICENSE` & `suta_ble_bed-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/PKG-INFO` & `suta_ble_bed-0.3.3/suta_ble_bed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: suta_ble_bed
-Version: 0.3.2
+Name: suta-ble-bed
+Version: 0.3.3
 Summary: Handle BLE communications for a SUTA bed frame such as the i500 or i800.
 Home-page: https://github.com/sredman/suta_ble_bed
 Author: Simon Redman
 Author-email: simon@ergotech.com
 License: MIT license
 Keywords: SUTA,sleepmotion,i500,i900,i200
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -83,27 +82,31 @@
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Inspirired by:
+Inspired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.3.3 (2023-07-24)
+------------------
+* Added release pipeline
+
 0.3.2 (2023-04-10)
 ------------------
 * Fix disconnect callback
 * Correct comment on BLE characteristics
 
 0.3.1 (2023-03-23)
 ------------------
@@ -143,9 +146,7 @@
 
 * Trying to get packaging correct
 
 0.1 (2023-03-05)
 ----------------
 
 * First release on PyPI.
-
-
```

### Comparing `suta_ble_bed-0.3.2/README.rst` & `suta_ble_bed-0.3.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Inspirired by:
+Inspired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `suta_ble_bed-0.3.2/docs/Makefile` & `suta_ble_bed-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/docs/conf.py` & `suta_ble_bed-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/docs/installation.rst` & `suta_ble_bed-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/docs/make.bat` & `suta_ble_bed-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/setup.py` & `suta_ble_bed-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     include_package_data=True,
     keywords=['SUTA','sleepmotion','i500','i900','i200'],
     name='suta_ble_bed',
     packages=find_packages(include=['suta_ble_bed', 'suta_ble_bed.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/sredman/suta_ble_bed',
-    version='0.3.2',
+    version='0.3.3',
     zip_safe=False,
 )
```

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed/cli.py` & `suta_ble_bed-0.3.3/suta_ble_bed/cli.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed.py` & `suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_bed.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed_controller.py` & `suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_bed_controller.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_consts.py` & `suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_consts.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_scanner.py` & `suta_ble_bed-0.3.3/suta_ble_bed/suta_ble_scanner.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed.egg-info/PKG-INFO` & `suta_ble_bed-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: suta-ble-bed
-Version: 0.3.2
+Name: suta_ble_bed
+Version: 0.3.3
 Summary: Handle BLE communications for a SUTA bed frame such as the i500 or i800.
 Home-page: https://github.com/sredman/suta_ble_bed
 Author: Simon Redman
 Author-email: simon@ergotech.com
 License: MIT license
 Keywords: SUTA,sleepmotion,i500,i900,i200
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -83,27 +82,31 @@
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Inspirired by:
+Inspired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.3.3 (2023-07-24)
+------------------
+* Added release pipeline
+
 0.3.2 (2023-04-10)
 ------------------
 * Fix disconnect callback
 * Correct comment on BLE characteristics
 
 0.3.1 (2023-03-23)
 ------------------
@@ -143,9 +146,7 @@
 
 * Trying to get packaging correct
 
 0.1 (2023-03-05)
 ----------------
 
 * First release on PyPI.
-
-
```

### Comparing `suta_ble_bed-0.3.2/suta_ble_bed.egg-info/SOURCES.txt` & `suta_ble_bed-0.3.3/suta_ble_bed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

