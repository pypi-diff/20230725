# Comparing `tmp/remotion_lambda-4.0.1.tar.gz` & `tmp/remotion_lambda-4.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.1.tar", last modified: Tue Jul 25 01:55:09 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.10.tar", last modified: Tue Jul 25 00:58:21 2023, max compression
```

## Comparing `remotion_lambda-4.0.1.tar` & `remotion_lambda-4.0.10.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 01:55:09.123223 remotion_lambda-4.0.1/
--rw-r--r--   0 codedev    (503) staff       (20)     2512 2023-07-21 08:40:48.000000 remotion_lambda-4.0.1/LICENSE
--rw-r--r--   0 codedev    (503) staff       (20)      390 2023-07-25 01:55:09.123047 remotion_lambda-4.0.1/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)       26 2023-07-21 08:40:48.000000 remotion_lambda-4.0.1/README.md
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 01:55:09.120455 remotion_lambda-4.0.1/remotion_lambda/
--rw-r--r--   0 codedev    (503) staff       (20)      202 2023-07-21 08:40:48.000000 remotion_lambda-4.0.1/remotion_lambda/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)     5252 2023-07-21 08:40:48.000000 remotion_lambda-4.0.1/remotion_lambda/models.py
--rw-r--r--   0 codedev    (503) staff       (20)     6182 2023-07-23 00:48:40.000000 remotion_lambda-4.0.1/remotion_lambda/remotionclient.py
--rw-r--r--   0 codedev    (503) staff       (20)       84 2023-07-25 01:54:59.000000 remotion_lambda-4.0.1/remotion_lambda/version.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 01:55:09.121782 remotion_lambda-4.0.1/remotion_lambda.egg-info/
--rw-r--r--   0 codedev    (503) staff       (20)      390 2023-07-25 01:55:09.000000 remotion_lambda-4.0.1/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)      384 2023-07-25 01:55:09.000000 remotion_lambda-4.0.1/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 codedev    (503) staff       (20)        1 2023-07-25 01:55:09.000000 remotion_lambda-4.0.1/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 01:55:09.000000 remotion_lambda-4.0.1/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 01:55:09.123270 remotion_lambda-4.0.1/setup.cfg
--rw-r--r--   0 codedev    (503) staff       (20)      753 2023-07-25 01:10:20.000000 remotion_lambda-4.0.1/setup.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 01:55:09.122672 remotion_lambda-4.0.1/tests/
--rw-r--r--   0 codedev    (503) staff       (20)      131 2023-07-21 08:40:48.000000 remotion_lambda-4.0.1/tests/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)      474 2023-07-21 22:55:58.000000 remotion_lambda-4.0.1/tests/test_get_render_progress_client.py
--rw-r--r--   0 codedev    (503) staff       (20)      764 2023-07-21 22:55:55.000000 remotion_lambda-4.0.1/tests/test_render_client.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787713 remotion_lambda-4.0.10/
+-rw-r--r--   0 codedev    (503) staff       (20)     2512 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/LICENSE
+-rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.787545 remotion_lambda-4.0.10/PKG-INFO
+-rw-r--r--   0 codedev    (503) staff       (20)       26 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/README.md
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786093 remotion_lambda-4.0.10/remotion_lambda/
+-rw-r--r--   0 codedev    (503) staff       (20)      202 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/__init__.py
+-rw-r--r--   0 codedev    (503) staff       (20)     5252 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/models.py
+-rw-r--r--   0 codedev    (503) staff       (20)     6182 2023-07-23 00:48:40.000000 remotion_lambda-4.0.10/remotion_lambda/remotionclient.py
+-rw-r--r--   0 codedev    (503) staff       (20)       85 2023-07-25 00:58:16.000000 remotion_lambda-4.0.10/remotion_lambda/version.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786610 remotion_lambda-4.0.10/remotion_lambda.egg-info/
+-rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 codedev    (503) staff       (20)      384 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 codedev    (503) staff       (20)        1 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 codedev    (503) staff       (20)       42 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 00:58:21.787756 remotion_lambda-4.0.10/setup.cfg
+-rw-r--r--   0 codedev    (503) staff       (20)      684 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/setup.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787180 remotion_lambda-4.0.10/tests/
+-rw-r--r--   0 codedev    (503) staff       (20)      131 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/tests/__init__.py
+-rw-r--r--   0 codedev    (503) staff       (20)      474 2023-07-21 22:55:58.000000 remotion_lambda-4.0.10/tests/test_get_render_progress_client.py
+-rw-r--r--   0 codedev    (503) staff       (20)      764 2023-07-21 22:55:55.000000 remotion_lambda-4.0.10/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.1/LICENSE` & `remotion_lambda-4.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.1/remotion_lambda/models.py` & `remotion_lambda-4.0.10/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.1/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.10/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.1/setup.py` & `remotion_lambda-4.0.10/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     author_email="jonny@remotion.dev",
     description="Remotion Lambda client",
     long_description_content_type="text/markdown",
     url="https://github.com/remotion-dev/remotion/tree/main/packages/lambda-python",
     classifiers=[
 
     ],
-    long_description="Remotion is a framework for creating videos programmatically using React.",
+    long_description="",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     # Name of the python package
-    py_modules=["remotion-lambda"],
+    py_modules=["remotion-lambda-sdk"],
 
 )
```

### Comparing `remotion_lambda-4.0.1/tests/test_render_client.py` & `remotion_lambda-4.0.10/tests/test_render_client.py`

 * *Files identical despite different names*

