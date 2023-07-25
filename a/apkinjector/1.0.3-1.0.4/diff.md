# Comparing `tmp/apkinjector-1.0.3.tar.gz` & `tmp/apkinjector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinjector-1.0.3.tar", last modified: Tue Jul 25 21:26:20 2023, max compression
+gzip compressed data, was "apkinjector-1.0.4.tar", last modified: Tue Jul 25 21:40:39 2023, max compression
```

## Comparing `apkinjector-1.0.3.tar` & `apkinjector-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:26:20.879838 apkinjector-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:26:09.000000 apkinjector-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:26:20.879838 apkinjector-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-25 21:26:09.000000 apkinjector-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:26:20.879838 apkinjector-1.0.3/apkinjector/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/apktool.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/gadget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/uber_apk_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 21:26:09.000000 apkinjector-1.0.3/apkinjector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:26:20.879838 apkinjector-1.0.3/apkinjector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:26:20.000000 apkinjector-1.0.3/apkinjector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:26:20.879838 apkinjector-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-25 21:26:09.000000 apkinjector-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:40:28.000000 apkinjector-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:40:39.084815 apkinjector-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-25 21:40:28.000000 apkinjector-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/apkinjector/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/apktool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/uber_apk_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/apkinjector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:40:39.084815 apkinjector-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 21:40:28.000000 apkinjector-1.0.4/setup.py
```

### Comparing `apkinjector-1.0.3/LICENSE` & `apkinjector-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/PKG-INFO` & `apkinjector-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.3/README.md` & `apkinjector-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/__init__.py` & `apkinjector-1.0.4/apkinjector/__init__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/__main__.py` & `apkinjector-1.0.4/apkinjector/__main__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/adb.py` & `apkinjector-1.0.4/apkinjector/adb.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/apktool.py` & `apkinjector-1.0.4/apkinjector/apktool.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/bundle.py` & `apkinjector-1.0.4/apkinjector/bundle.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/dependencies.py` & `apkinjector-1.0.4/apkinjector/dependencies.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/download.py` & `apkinjector-1.0.4/apkinjector/download.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/frida.py` & `apkinjector-1.0.4/apkinjector/frida.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/gadget.py` & `apkinjector-1.0.4/apkinjector/gadget.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/injector.py` & `apkinjector-1.0.4/apkinjector/injector.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/java.py` & `apkinjector-1.0.4/apkinjector/java.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/logger.py` & `apkinjector-1.0.4/apkinjector/logger.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/plugins.py` & `apkinjector-1.0.4/apkinjector/plugins.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/uber_apk_signer.py` & `apkinjector-1.0.4/apkinjector/uber_apk_signer.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector/utils.py` & `apkinjector-1.0.4/apkinjector/utils.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/apkinjector.egg-info/PKG-INFO` & `apkinjector-1.0.4/apkinjector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.3/apkinjector.egg-info/SOURCES.txt` & `apkinjector-1.0.4/apkinjector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.3/setup.py` & `apkinjector-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='apkinjector',
-    version='1.0.3',
+    version='1.0.4',
     description='Utilities to help injecting libraries and frida in apks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Marcel Alexandru Nitan',
     author_email='nitan.marcel@gmail.com',
     url='https://nitanmarcel.github.io/apkinjector',
     keywords=['FRIDA', 'APK', 'INJECTION', 'INJECT'],
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'apkinjector = apkinjector.__main__:start'
         ]
     },
     install_requires=[
-        'requests'
+        'requests',
         'appdirs',
         'install-jdk',
         'click',
         'pyaxmlparser',
         'pyelftools',
         'colorama'
     ],
```

