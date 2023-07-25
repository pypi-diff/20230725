# Comparing `tmp/playcode-0.0.5.tar.gz` & `tmp/playcode-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playcode-0.0.5.tar", last modified: Tue Jul 25 14:42:21 2023, max compression
+gzip compressed data, was "playcode-0.0.6.tar", last modified: Tue Jul 25 14:49:26 2023, max compression
```

## Comparing `playcode-0.0.5.tar` & `playcode-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.677254 playcode-0.0.5/
--rw-rw-rw-   0        0        0      410 2023-07-25 14:42:21.675262 playcode-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.5/README
-drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.654315 playcode-0.0.5/playcode/
--rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.5/playcode/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-07-25 14:40:12.000000 playcode-0.0.5/playcode/pycode.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.670274 playcode-0.0.5/playcode.egg-info/
--rw-rw-rw-   0        0        0      410 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:42:21.678255 playcode-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-07-25 14:40:11.000000 playcode-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:26.260305 playcode-0.0.6/
+-rw-rw-rw-   0        0        0      410 2023-07-25 14:49:26.258310 playcode-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.6/README
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:26.221410 playcode-0.0.6/playcode/
+-rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.6/playcode/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-07-25 14:40:12.000000 playcode-0.0.6/playcode/pycode.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:26.254322 playcode-0.0.6/playcode.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-25 14:49:25.000000 playcode-0.0.6/playcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-25 14:49:25.000000 playcode-0.0.6/playcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:49:25.000000 playcode-0.0.6/playcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 14:49:25.000000 playcode-0.0.6/playcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:49:26.260305 playcode-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-07-25 14:48:47.000000 playcode-0.0.6/setup.py
```

### Comparing `playcode-0.0.5/playcode/pycode.py` & `playcode-0.0.6/playcode/pycode.py`

 * *Files identical despite different names*

### Comparing `playcode-0.0.5/setup.py` & `playcode-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="playcode", # Replace with your own PyPI username(id)
-    version="0.0.5",
+    version="0.0.6",
     author="Seungjun Min",
     author_email="sjmin213@gmail.com",
     description="Creating password",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sjmin/",
     packages=setuptools.find_packages(),
```

