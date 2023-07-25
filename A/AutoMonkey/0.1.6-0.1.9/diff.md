# Comparing `tmp/AutoMonkey-0.1.6.tar.gz` & `tmp/AutoMonkey-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoMonkey-0.1.6.tar", last modified: Tue Jul 25 19:50:47 2023, max compression
+gzip compressed data, was "AutoMonkey-0.1.9.tar", last modified: Tue Jul 25 20:16:41 2023, max compression
```

## Comparing `AutoMonkey-0.1.6.tar` & `AutoMonkey-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      178 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/AUTHORS.rst
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.127348 AutoMonkey-0.1.6/AutoMonkey.egg-info/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      729 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       51 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/not-zip-safe
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      242 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       11 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/top_level.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3556 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/CONTRIBUTING.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       89 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/HISTORY.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1582 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/LICENSE
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      279 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/MANIFEST.in
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    11362 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1098 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/README.rst
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/automonkey/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      177 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/automonkey/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4700 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/app_funcs.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     9336 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/automonkey.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1730 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/constants.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      589 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/exceptions.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    10013 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/img_funcs.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4263 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/mouse_tracker.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4706 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/utils.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/docs/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      611 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/Makefile
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/authors.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4901 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/conf.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       33 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/contributing.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/history.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      307 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/index.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1154 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/installation.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      772 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/make.bat
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       27 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/readme.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       75 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/usage.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      939 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      265 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/requirements.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      425 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1578 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      178 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/AUTHORS.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.873695 AutoMonkey-0.1.9/AutoMonkey.egg-info/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      729 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       51 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/not-zip-safe
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      237 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       11 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/top_level.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3556 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       89 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/HISTORY.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1582 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/LICENSE
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      279 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/MANIFEST.in
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    11362 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1098 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/README.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.873695 AutoMonkey-0.1.9/automonkey/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      177 2023-07-25 20:04:39.000000 AutoMonkey-0.1.9/automonkey/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4700 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/app_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     9336 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/automonkey.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1730 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/constants.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      589 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/exceptions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    10013 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/img_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4263 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/mouse_tracker.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4706 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/utils.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/docs/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      611 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/Makefile
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/authors.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4901 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/conf.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       33 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/contributing.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/history.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      307 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/index.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1154 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/installation.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      772 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/make.bat
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       27 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/readme.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       75 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/usage.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      943 2023-07-25 20:12:40.000000 AutoMonkey-0.1.9/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      259 2023-07-25 20:01:33.000000 AutoMonkey-0.1.9/requirements.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      425 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1578 2023-07-25 20:04:39.000000 AutoMonkey-0.1.9/setup.py
```

### Comparing `AutoMonkey-0.1.6/AutoMonkey.egg-info/PKG-INFO` & `AutoMonkey-0.1.9/AutoMonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMonkey
-Version: 0.1.6
+Version: 0.1.9
 Summary: Python Automation using Mouse and Keyboard, for the masses
 Home-page: https://github.com/MihailCosmin/automonkey
 Author: Mihail-Cosmin Munteanu
 Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
 Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.6 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.9 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `AutoMonkey-0.1.6/AutoMonkey.egg-info/SOURCES.txt` & `AutoMonkey-0.1.9/AutoMonkey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/CONTRIBUTING.rst` & `AutoMonkey-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/LICENSE` & `AutoMonkey-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/PKG-INFO` & `AutoMonkey-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMonkey
-Version: 0.1.6
+Version: 0.1.9
 Summary: Python Automation using Mouse and Keyboard, for the masses
 Home-page: https://github.com/MihailCosmin/automonkey
 Author: Mihail-Cosmin Munteanu
 Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
 Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.6 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.9 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `AutoMonkey-0.1.6/README.md` & `AutoMonkey-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/README.rst` & `AutoMonkey-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/app_funcs.py` & `AutoMonkey-0.1.9/automonkey/app_funcs.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/automonkey.py` & `AutoMonkey-0.1.9/automonkey/automonkey.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/constants.py` & `AutoMonkey-0.1.9/automonkey/constants.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/exceptions.py` & `AutoMonkey-0.1.9/automonkey/exceptions.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/img_funcs.py` & `AutoMonkey-0.1.9/automonkey/img_funcs.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/mouse_tracker.py` & `AutoMonkey-0.1.9/automonkey/mouse_tracker.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/automonkey/utils.py` & `AutoMonkey-0.1.9/automonkey/utils.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/docs/Makefile` & `AutoMonkey-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/docs/conf.py` & `AutoMonkey-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/docs/installation.rst` & `AutoMonkey-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/docs/make.bat` & `AutoMonkey-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.6/pyproject.toml` & `AutoMonkey-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
     "pyautogui>=0.9.53",
     "pytesseract>=0.3.9",
     "numpy>=1.21.5",
     "keyboard>=0.13.5",
     "clipboard>=0.0.4",
     "opencv-python==4.5.5.62",
     "pillow>=9.0.1",
-    "pywin32>=303",
-    "pywin32-ctypes>=0.2.0",
+    # "pywin32>=303",
+    # "pywin32-ctypes>=0.2.0",
     "screeninfo>=0.8",
     "pyperclip>=1.8.2",
     "PyScreeze>=0.1.27",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AutoMonkey"
-version = "0.1.6"
+version = "0.1.9"
 authors = [
   { name="Mihail-Cosmin Munteanu", email="munteanumihailcosmin@gmail.com" },
 ]
 description = "Python Automation using Mouse and Keyboard, for the masses"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `AutoMonkey-0.1.6/setup.py` & `AutoMonkey-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='automonkey',
     name='automonkey',
     packages=find_packages(include=['automonkey', 'automonkey.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MihailCosmin/automonkey',
-    version="0.1.6",
+    version="0.1.9",
     zip_safe=False,
 )
```

