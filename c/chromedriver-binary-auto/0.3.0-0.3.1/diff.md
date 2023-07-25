# Comparing `tmp/chromedriver-binary-auto-0.3.0.tar.gz` & `tmp/chromedriver-binary-auto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-binary-auto-0.3.0.tar", last modified: Mon Jul 24 15:13:53 2023, max compression
+gzip compressed data, was "chromedriver-binary-auto-0.3.1.tar", last modified: Tue Jul 25 13:36:18 2023, max compression
```

## Comparing `chromedriver-binary-auto-0.3.0.tar` & `chromedriver-binary-auto-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2722 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/chromedriver_binary/
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6882 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2722 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:36:18.494929 chromedriver-binary-auto-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-25 13:36:17.000000 chromedriver-binary-auto-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-25 13:36:18.494929 chromedriver-binary-auto-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-25 13:36:17.000000 chromedriver-binary-auto-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:36:18.490929 chromedriver-binary-auto-0.3.1/chromedriver_binary/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-25 13:36:17.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6882 2023-07-25 13:36:17.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:36:18.494929 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-25 13:36:18.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-25 13:36:18.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:36:18.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 13:36:18.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-25 13:36:18.000000 chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:36:18.494929 chromedriver-binary-auto-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-25 13:36:17.000000 chromedriver-binary-auto-0.3.1/setup.py
```

### Comparing `chromedriver-binary-auto-0.3.0/LICENSE` & `chromedriver-binary-auto-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.3.0/PKG-INFO` & `chromedriver-binary-auto-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.3.0/README.md` & `chromedriver-binary-auto-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.3.0/chromedriver_binary/__init__.py` & `chromedriver-binary-auto-0.3.1/chromedriver_binary/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.3.0/chromedriver_binary/utils.py` & `chromedriver-binary-auto-0.3.1/chromedriver_binary/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     :param version: Major version number or None
     :return: Latest release for given version
     """
     try:
         if version is None:
             response = urlopen("https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions.json", context=ssl_context)
             return json.load(response)["channels"]["Stable"]["version"]
-        if int(version) < 113:
+        if int(version) < 115:
             return get_latest_legacy_release_for_version(version)
         response = urlopen("https://googlechromelabs.github.io/chrome-for-testing/latest-versions-per-milestone-with-downloads.json", context=ssl_context)
         return json.load(response)["milestones"][str(version)]["version"]
     except Exception:
         raise RuntimeError('Failed to find release information for version: {}'.format(version if version else "latest"))
```

### Comparing `chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/PKG-INFO` & `chromedriver-binary-auto-0.3.1/chromedriver_binary_auto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.3.0/setup.py` & `chromedriver-binary-auto-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             if not os.access(chromedriver_filename, os.X_OK):
                 os.chmod(chromedriver_filename, 0o744)
         build_py.run(self)
 
 
 setup(
     name="chromedriver-binary-auto",
-    version="0.3.0",
+    version="0.3.1",
     author="Daniel Kaiser",
     author_email="daniel.kaiser94@gmail.com",
     description="Installer for chromedriver.",
     license="MIT",
     keywords="chromedriver chrome browser selenium splinter",
     url="https://github.com/danielkaiser/python-chromedriver-binary",
     packages=['chromedriver_binary'],
```

