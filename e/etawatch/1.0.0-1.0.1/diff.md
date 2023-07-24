# Comparing `tmp/etawatch-1.0.0.tar.gz` & `tmp/etawatch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etawatch-1.0.0.tar", last modified: Mon Jul 24 21:24:22 2023, max compression
+gzip compressed data, was "etawatch-1.0.1.tar", last modified: Mon Jul 24 22:48:32 2023, max compression
```

## Comparing `etawatch-1.0.0.tar` & `etawatch-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 21:24:22.028202 etawatch-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-07-23 16:38:43.000000 etawatch-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    42584 2023-07-24 21:24:22.026203 etawatch-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-07-23 16:59:01.000000 etawatch-1.0.0/README.md
--rw-rw-rw-   0        0        0      694 2023-07-24 21:24:04.000000 etawatch-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 21:24:22.028202 etawatch-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 21:24:22.011203 etawatch-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 21:24:22.019204 etawatch-1.0.0/src/etawatch/
--rw-rw-rw-   0        0        0      268 2023-07-24 21:19:00.000000 etawatch-1.0.0/src/etawatch/__init__.py
--rw-rw-rw-   0        0        0      907 2023-07-23 17:16:11.000000 etawatch-1.0.0/src/etawatch/etawatch.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:24:22.024202 etawatch-1.0.0/src/etawatch.egg-info/
--rw-rw-rw-   0        0        0    42584 2023-07-24 21:24:21.000000 etawatch-1.0.0/src/etawatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-24 21:24:22.000000 etawatch-1.0.0/src/etawatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 21:24:22.000000 etawatch-1.0.0/src/etawatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 21:24:22.000000 etawatch-1.0.0/src/etawatch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 22:48:32.006123 etawatch-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-23 16:38:43.000000 etawatch-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    42584 2023-07-24 22:48:32.005123 etawatch-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-07-23 16:59:01.000000 etawatch-1.0.1/README.md
+-rw-rw-rw-   0        0        0      694 2023-07-24 22:47:39.000000 etawatch-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 22:48:32.007124 etawatch-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 22:48:31.989124 etawatch-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 22:48:31.997123 etawatch-1.0.1/src/etawatch/
+-rw-rw-rw-   0        0        0      295 2023-07-24 22:47:30.000000 etawatch-1.0.1/src/etawatch/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-07-23 17:16:11.000000 etawatch-1.0.1/src/etawatch/etawatch.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:48:32.003124 etawatch-1.0.1/src/etawatch.egg-info/
+-rw-rw-rw-   0        0        0    42584 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/top_level.txt
```

### Comparing `etawatch-1.0.0/LICENSE` & `etawatch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etawatch-1.0.0/PKG-INFO` & `etawatch-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etawatch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Like a stopwatch, but it also gives you an ETA
 Author-email: "Rick D. Gray" <rickdgray@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `etawatch-1.0.0/README.md` & `etawatch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `etawatch-1.0.0/pyproject.toml` & `etawatch-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "etawatch"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name = "Rick D. Gray", email = "rickdgray@outlook.com"},
 ]
 description = "Like a stopwatch, but it also gives you an ETA"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `etawatch-1.0.0/src/etawatch/etawatch.py` & `etawatch-1.0.1/src/etawatch/etawatch.py`

 * *Files identical despite different names*

### Comparing `etawatch-1.0.0/src/etawatch.egg-info/PKG-INFO` & `etawatch-1.0.1/src/etawatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etawatch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Like a stopwatch, but it also gives you an ETA
 Author-email: "Rick D. Gray" <rickdgray@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

