# Comparing `tmp/apkinjector-1.0.1.tar.gz` & `tmp/apkinjector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinjector-1.0.1.tar", last modified: Tue Jul 25 19:56:15 2023, max compression
+gzip compressed data, was "apkinjector-1.0.2.tar", last modified: Tue Jul 25 21:17:28 2023, max compression
```

## Comparing `apkinjector-1.0.1.tar` & `apkinjector-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:56:15.349197 apkinjector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 19:56:06.000000 apkinjector-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 19:56:15.349197 apkinjector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-25 19:56:06.000000 apkinjector-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:56:15.349197 apkinjector-1.0.1/apkinjector/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/apktool.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/gadget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/uber_apk_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 19:56:06.000000 apkinjector-1.0.1/apkinjector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:56:15.349197 apkinjector-1.0.1/apkinjector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 19:56:15.000000 apkinjector-1.0.1/apkinjector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:56:15.349197 apkinjector-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-25 19:56:06.000000 apkinjector-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:28.914580 apkinjector-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:17:18.000000 apkinjector-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:17:28.910580 apkinjector-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-25 21:17:18.000000 apkinjector-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:28.910580 apkinjector-1.0.2/apkinjector/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/apktool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/uber_apk_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 21:17:18.000000 apkinjector-1.0.2/apkinjector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:28.910580 apkinjector-1.0.2/apkinjector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:17:28.000000 apkinjector-1.0.2/apkinjector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:17:28.914580 apkinjector-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-25 21:17:18.000000 apkinjector-1.0.2/setup.py
```

### Comparing `apkinjector-1.0.1/LICENSE` & `apkinjector-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/PKG-INFO` & `apkinjector-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.1/README.md` & `apkinjector-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/__init__.py` & `apkinjector-1.0.2/apkinjector/__init__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/__main__.py` & `apkinjector-1.0.2/apkinjector/__main__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/adb.py` & `apkinjector-1.0.2/apkinjector/adb.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/apktool.py` & `apkinjector-1.0.2/apkinjector/apktool.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/bundle.py` & `apkinjector-1.0.2/apkinjector/bundle.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/dependencies.py` & `apkinjector-1.0.2/apkinjector/dependencies.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/download.py` & `apkinjector-1.0.2/apkinjector/download.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/frida.py` & `apkinjector-1.0.2/apkinjector/frida.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/gadget.py` & `apkinjector-1.0.2/apkinjector/gadget.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/injector.py` & `apkinjector-1.0.2/apkinjector/injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .arch import ARCH
 from .utils import arch_to_abi
 
 
 class Injector:
     @staticmethod
-    def inject_library(source: str, unpack_path: str, smali_path: str = None, extra_files: List[str] = None) ->:
+    def inject_library(source: str, unpack_path: str, smali_path: str = None, extra_files: List[str] = None) -> None:
         """Inject library into unpacked apk
 
         Args:
             source (str): Path to shared library to inject.
             unpack_path (str): Path to apktool unpacked apk.
             smali_path (str, optional): _description_. Path to smali file to inject into. Leave empty to skip this step
             extra_files (List[str], optional): _description_. Extra files to copy over the the apk lib/ folder
```

### Comparing `apkinjector-1.0.1/apkinjector/java.py` & `apkinjector-1.0.2/apkinjector/java.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/logger.py` & `apkinjector-1.0.2/apkinjector/logger.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/plugins.py` & `apkinjector-1.0.2/apkinjector/plugins.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/uber_apk_signer.py` & `apkinjector-1.0.2/apkinjector/uber_apk_signer.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector/utils.py` & `apkinjector-1.0.2/apkinjector/utils.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/apkinjector.egg-info/PKG-INFO` & `apkinjector-1.0.2/apkinjector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.1/apkinjector.egg-info/SOURCES.txt` & `apkinjector-1.0.2/apkinjector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.1/setup.py` & `apkinjector-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
 setup(
     name='apkinjector',
-    version='1.0.1',
+    version='1.0.2',
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
-        'requests',
+        'requests'
         'appdirs',
         'install-jdk',
         'click',
         'pyaxmlparser',
-        'pyelftools'
+        'pyelftools',
+        'colorama'
     ],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

