# Comparing `tmp/invest_life-0.0.1.tar.gz` & `tmp/invest_life-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_life-0.0.1.tar", last modified: Tue Jul 25 13:33:57 2023, max compression
+gzip compressed data, was "invest_life-0.0.2.tar", last modified: Tue Jul 25 14:26:47 2023, max compression
```

## Comparing `invest_life-0.0.1.tar` & `invest_life-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 13:33:57.115581 invest_life-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-25 13:33:57.115256 invest_life-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-25 13:09:08.000000 invest_life-0.0.1/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-25 13:33:57.115718 invest_life-0.0.1/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 13:33:57.112774 invest_life-0.0.1/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.1/src/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 13:33:57.114761 invest_life-0.0.1/src/invest_life.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-25 13:33:57.000000 invest_life-0.0.1/src/invest_life.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      222 2023-07-25 13:33:57.000000 invest_life-0.0.1/src/invest_life.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-25 13:33:57.000000 invest_life-0.0.1/src/invest_life.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-25 13:33:57.000000 invest_life-0.0.1/src/invest_life.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      454 2023-07-25 12:59:34.000000 invest_life-0.0.1/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 14:26:47.749421 invest_life-0.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.2/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-25 14:26:47.749004 invest_life-0.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-25 14:23:55.000000 invest_life-0.0.2/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-25 14:26:47.749616 invest_life-0.0.2/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 14:26:47.745386 invest_life-0.0.2/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.2/src/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 14:26:47.747285 invest_life-0.0.2/src/invest_life.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-25 14:26:47.000000 invest_life-0.0.2/src/invest_life.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-25 14:26:47.000000 invest_life-0.0.2/src/invest_life.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-25 14:26:47.000000 invest_life-0.0.2/src/invest_life.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-25 14:26:47.000000 invest_life-0.0.2/src/invest_life.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)      704 2023-07-25 14:21:58.000000 invest_life-0.0.2/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-25 14:26:47.747994 invest_life-0.0.2/tests/
+-rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.2/tests/test.py
```

### Comparing `invest_life-0.0.1/LICENSE` & `invest_life-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_life-0.0.1/PKG-INFO` & `invest_life-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_life
-Version: 0.0.1
+Version: 0.0.2
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.1/src/invest_life.egg-info/PKG-INFO` & `invest_life-0.0.2/src/invest_life.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-life
-Version: 0.0.1
+Version: 0.0.2
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

