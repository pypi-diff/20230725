# Comparing `tmp/playcode-0.0.4.tar.gz` & `tmp/playcode-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playcode-0.0.4.tar", last modified: Sat Jul 22 02:36:44 2023, max compression
+gzip compressed data, was "playcode-0.0.5.tar", last modified: Tue Jul 25 14:42:21 2023, max compression
```

## Comparing `playcode-0.0.4.tar` & `playcode-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.816451 playcode-0.0.4/
--rw-rw-rw-   0        0        0      410 2023-07-22 02:36:44.815517 playcode-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.4/README
-drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.800577 playcode-0.0.4/playcode/
--rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.4/playcode/__init__.py
--rw-rw-rw-   0        0        0       85 2023-01-21 12:07:02.000000 playcode-0.0.4/playcode/test.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.812614 playcode-0.0.4/playcode.egg-info/
--rw-rw-rw-   0        0        0      410 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 02:36:44.816451 playcode-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-07-22 02:27:44.000000 playcode-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.677254 playcode-0.0.5/
+-rw-rw-rw-   0        0        0      410 2023-07-25 14:42:21.675262 playcode-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.5/README
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.654315 playcode-0.0.5/playcode/
+-rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.5/playcode/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-07-25 14:40:12.000000 playcode-0.0.5/playcode/pycode.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:21.670274 playcode-0.0.5/playcode.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 14:42:21.000000 playcode-0.0.5/playcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:42:21.678255 playcode-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-07-25 14:40:11.000000 playcode-0.0.5/setup.py
```

### Comparing `playcode-0.0.4/setup.py` & `playcode-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="playcode", # Replace with your own PyPI username(id)
-    version="0.0.4",
+    version="0.0.5",
     author="Seungjun Min",
     author_email="sjmin213@gmail.com",
     description="Creating password",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sjmin/",
     packages=setuptools.find_packages(),
```

