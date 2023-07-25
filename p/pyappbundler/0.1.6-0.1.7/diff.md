# Comparing `tmp/pyappbundler-0.1.6.tar.gz` & `tmp/pyappbundler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.6.tar", last modified: Sun Jul  9 05:49:49 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.7.tar", last modified: Tue Jul 25 21:23:38 2023, max compression
```

## Comparing `pyappbundler-0.1.6.tar` & `pyappbundler-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.259959 pyappbundler-0.1.6/pyappbundler/
--rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.6/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.6/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-09 05:48:46.000000 pyappbundler-0.1.6/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     5182 2023-07-09 05:48:02.000000 pyappbundler-0.1.6/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.263959 pyappbundler-0.1.6/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1705 2023-07-08 10:54:08.000000 pyappbundler-0.1.6/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.262958 pyappbundler-0.1.6/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:23:38.102176 pyappbundler-0.1.7/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-25 21:23:38.102176 pyappbundler-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 21:23:38.097176 pyappbundler-0.1.7/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.7/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.7/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-25 21:23:20.000000 pyappbundler-0.1.7/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     5187 2023-07-25 21:22:53.000000 pyappbundler-0.1.7/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:23:38.101176 pyappbundler-0.1.7/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1705 2023-07-08 10:54:08.000000 pyappbundler-0.1.7/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-25 21:23:38.100175 pyappbundler-0.1.7/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-25 21:23:38.000000 pyappbundler-0.1.7/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 21:23:38.000000 pyappbundler-0.1.7/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:23:38.000000 pyappbundler-0.1.7/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-25 21:23:38.000000 pyappbundler-0.1.7/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 21:23:38.000000 pyappbundler-0.1.7/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 21:23:38.102176 pyappbundler-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.7/setup.py
```

### Comparing `pyappbundler-0.1.6/LICENSE` & `pyappbundler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.6/PKG-INFO` & `pyappbundler-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.6
+Version: 0.1.7
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.6/pyappbundler/__main__.py` & `pyappbundler-0.1.7/pyappbundler/__main__.py`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.6/pyappbundler/pyappbundler.py` & `pyappbundler-0.1.7/pyappbundler/pyappbundler.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         logging.info(f'Cleaning "{self.dist}" directory...')
 
         if not self.dist.exists():
             self.dist.mkdir(parents=True)
             logging.info(
                 f'"{self.dist}" directory doesn\'t exist!'
                 ' The new one has been created.')
-            return
+            return self
 
         if not self.dist.is_dir():
             raise FileNotFoundError(
                 f'Directory expected, but "{self.dist}" is not!')
 
         for path in self.dist.iterdir():
             if path.is_file():
```

### Comparing `pyappbundler-0.1.6/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.7/pyappbundler/templates/iss.tmpl`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.6/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.7/pyappbundler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.6
+Version: 0.1.7
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.6/pyproject.toml` & `pyappbundler-0.1.7/pyproject.toml`

 * *Files identical despite different names*

