# Comparing `tmp/xclass_sdk-1.5.0.tar.gz` & `tmp/xclass_sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xclass_sdk-1.5.0.tar", last modified: Mon Jul 24 07:23:31 2023, max compression
+gzip compressed data, was "xclass_sdk-1.6.0.tar", last modified: Fri Jul 21 06:19:19 2023, max compression
```

## Comparing `xclass_sdk-1.5.0.tar` & `xclass_sdk-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 lantrungseo   (502) staff       (20)        0 2023-07-24 07:23:31.067317 xclass_sdk-1.5.0/
--rw-r--r--   0 lantrungseo   (502) staff       (20)    35148 2023-06-08 11:12:49.000000 xclass_sdk-1.5.0/LICENSE.txt
--rw-r--r--   0 lantrungseo   (502) staff       (20)      535 2023-07-24 07:23:31.067124 xclass_sdk-1.5.0/PKG-INFO
--rw-r--r--   0 lantrungseo   (502) staff       (20)       39 2023-06-08 11:29:08.000000 xclass_sdk-1.5.0/README.md
--rw-r--r--   0 lantrungseo   (502) staff       (20)      607 2023-07-24 07:22:52.000000 xclass_sdk-1.5.0/pyproject.toml
--rw-r--r--   0 lantrungseo   (502) staff       (20)       38 2023-07-24 07:23:31.067375 xclass_sdk-1.5.0/setup.cfg
-drwxr-xr-x   0 lantrungseo   (502) staff       (20)        0 2023-07-24 07:23:31.062492 xclass_sdk-1.5.0/src/
-drwxr-xr-x   0 lantrungseo   (502) staff       (20)        0 2023-07-24 07:23:31.063835 xclass_sdk-1.5.0/src/browser_sdk/
--rw-r--r--   0 lantrungseo   (502) staff       (20)      748 2023-07-24 07:22:52.000000 xclass_sdk-1.5.0/src/browser_sdk/math_app_browser.py
-drwxr-xr-x   0 lantrungseo   (502) staff       (20)        0 2023-07-24 07:23:31.065541 xclass_sdk-1.5.0/src/xclass_sdk/
--rw-r--r--   0 lantrungseo   (502) staff       (20)       26 2023-06-08 10:49:21.000000 xclass_sdk-1.5.0/src/xclass_sdk/__init__.py
--rw-r--r--   0 lantrungseo   (502) staff       (20)     1028 2023-07-24 07:22:52.000000 xclass_sdk-1.5.0/src/xclass_sdk/math_app.py
--rw-r--r--   0 lantrungseo   (502) staff       (20)      980 2023-07-24 07:22:52.000000 xclass_sdk-1.5.0/src/xclass_sdk/profile.py
--rw-r--r--   0 lantrungseo   (502) staff       (20)      833 2023-06-09 08:22:20.000000 xclass_sdk-1.5.0/src/xclass_sdk/xclass_helpers.py
-drwxr-xr-x   0 lantrungseo   (502) staff       (20)        0 2023-07-24 07:23:31.066866 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/
--rw-r--r--   0 lantrungseo   (502) staff       (20)      535 2023-07-24 07:23:31.000000 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lantrungseo   (502) staff       (20)      374 2023-07-24 07:23:31.000000 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lantrungseo   (502) staff       (20)        1 2023-07-24 07:23:31.000000 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lantrungseo   (502) staff       (20)       15 2023-07-24 07:23:31.000000 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/requires.txt
--rw-r--r--   0 lantrungseo   (502) staff       (20)       23 2023-07-24 07:23:31.000000 xclass_sdk-1.5.0/src/xclass_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.896246 xclass_sdk-1.6.0/
+-rw-r--r--   0 hansle     (501) staff       (20)    35148 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/LICENSE.txt
+-rw-r--r--   0 hansle     (501) staff       (20)      535 2023-07-21 06:19:19.896113 xclass_sdk-1.6.0/PKG-INFO
+-rw-r--r--   0 hansle     (501) staff       (20)       39 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/README.md
+-rw-r--r--   0 hansle     (501) staff       (20)      607 2023-07-21 06:19:13.000000 xclass_sdk-1.6.0/pyproject.toml
+-rw-r--r--   0 hansle     (501) staff       (20)       38 2023-07-21 06:19:19.896287 xclass_sdk-1.6.0/setup.cfg
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.892928 xclass_sdk-1.6.0/src/
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.894332 xclass_sdk-1.6.0/src/browser_sdk/
+-rw-r--r--   0 hansle     (501) staff       (20)     1528 2023-07-17 18:12:05.000000 xclass_sdk-1.6.0/src/browser_sdk/general_app_browser.py
+-rw-r--r--   0 hansle     (501) staff       (20)      748 2023-07-16 10:30:50.000000 xclass_sdk-1.6.0/src/browser_sdk/math_app_browser.py
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.895210 xclass_sdk-1.6.0/src/xclass_sdk/
+-rw-r--r--   0 hansle     (501) staff       (20)       26 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/src/xclass_sdk/__init__.py
+-rw-r--r--   0 hansle     (501) staff       (20)     2294 2023-07-20 09:05:01.000000 xclass_sdk-1.6.0/src/xclass_sdk/general_app.py
+-rw-r--r--   0 hansle     (501) staff       (20)     1028 2023-07-16 10:30:50.000000 xclass_sdk-1.6.0/src/xclass_sdk/math_app.py
+-rw-r--r--   0 hansle     (501) staff       (20)      980 2023-07-07 02:12:24.000000 xclass_sdk-1.6.0/src/xclass_sdk/profile.py
+-rw-r--r--   0 hansle     (501) staff       (20)      833 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/src/xclass_sdk/xclass_helpers.py
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.895946 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/
+-rw-r--r--   0 hansle     (501) staff       (20)      535 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 hansle     (501) staff       (20)      443 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 hansle     (501) staff       (20)        1 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 hansle     (501) staff       (20)       15 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/requires.txt
+-rw-r--r--   0 hansle     (501) staff       (20)       23 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/top_level.txt
```

### Comparing `xclass_sdk-1.5.0/LICENSE.txt` & `xclass_sdk-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.5.0/PKG-INFO` & `xclass_sdk-1.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xclass_sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: X-Class SDK
 Author-email: Trung Nguyen <lantrungseo@gmail.com>
 Project-URL: Homepage, https://github.com/lantrungseo/xclass-sdk
 Project-URL: Bug Tracker, https://github.com/lantrungseo/xclass-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xclass_sdk-1.5.0/pyproject.toml` & `xclass_sdk-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xclass_sdk"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
   { name="Trung Nguyen", email="lantrungseo@gmail.com" },
 ]
 description = "X-Class SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xclass_sdk-1.5.0/src/browser_sdk/math_app_browser.py` & `xclass_sdk-1.6.0/src/browser_sdk/math_app_browser.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.5.0/src/xclass_sdk/math_app.py` & `xclass_sdk-1.6.0/src/xclass_sdk/math_app.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.5.0/src/xclass_sdk/profile.py` & `xclass_sdk-1.6.0/src/xclass_sdk/profile.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.5.0/src/xclass_sdk/xclass_helpers.py` & `xclass_sdk-1.6.0/src/xclass_sdk/xclass_helpers.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.5.0/src/xclass_sdk.egg-info/PKG-INFO` & `xclass_sdk-1.6.0/src/xclass_sdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xclass-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: X-Class SDK
 Author-email: Trung Nguyen <lantrungseo@gmail.com>
 Project-URL: Homepage, https://github.com/lantrungseo/xclass-sdk
 Project-URL: Bug Tracker, https://github.com/lantrungseo/xclass-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

