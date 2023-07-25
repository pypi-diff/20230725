# Comparing `tmp/flexible_dict-1.1.0.tar.gz` & `tmp/flexible_dict-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-1.1.0.tar", last modified: Mon Jul 24 10:41:32 2023, max compression
+gzip compressed data, was "flexible_dict-1.1.1.tar", last modified: Tue Jul 25 03:24:28 2023, max compression
```

## Comparing `flexible_dict-1.1.0.tar` & `flexible_dict-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-24 10:41:32.156435 flexible_dict-1.1.0/
--rw-r--r--   0 bytedance   (501) staff       (20)      802 2023-07-24 10:41:32.156297 flexible_dict-1.1.0/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      518 2023-07-24 08:29:14.000000 flexible_dict-1.1.0/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-24 10:41:32.154525 flexible_dict-1.1.0/flexible_dict/
--rw-r--r--   0 bytedance   (501) staff       (20)      182 2023-07-24 08:27:54.000000 flexible_dict-1.1.0/flexible_dict/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      508 2023-07-24 09:58:30.000000 flexible_dict-1.1.0/flexible_dict/__main__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-07-24 09:33:31.000000 flexible_dict-1.1.0/flexible_dict/about.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5203 2023-07-24 08:26:14.000000 flexible_dict-1.1.0/flexible_dict/json_object.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-24 10:41:32.155716 flexible_dict-1.1.0/flexible_dict/script/
--rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-24 09:41:19.000000 flexible_dict-1.1.0/flexible_dict/script/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1532 2023-07-24 10:02:21.000000 flexible_dict-1.1.0/flexible_dict/script/class_builder.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-24 10:41:32.155434 flexible_dict-1.1.0/flexible_dict.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      802 2023-07-24 10:41:32.000000 flexible_dict-1.1.0/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-07-24 10:41:32.000000 flexible_dict-1.1.0/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-24 10:41:32.000000 flexible_dict-1.1.0/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-07-24 10:41:32.000000 flexible_dict-1.1.0/flexible_dict.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-24 10:41:32.156481 flexible_dict-1.1.0/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)      965 2023-07-24 09:37:15.000000 flexible_dict-1.1.0/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-24 10:41:32.155971 flexible_dict-1.1.0/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)      212 2023-07-24 10:01:59.000000 flexible_dict-1.1.0/tests/test_build_class.py
--rw-r--r--   0 bytedance   (501) staff       (20)      410 2023-07-24 08:27:54.000000 flexible_dict-1.1.0/tests/test_json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475708 flexible_dict-1.1.1/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1248 2023-07-25 03:24:28.475598 flexible_dict-1.1.1/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      959 2023-07-24 11:06:26.000000 flexible_dict-1.1.1/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.473820 flexible_dict-1.1.1/flexible_dict/
+-rw-r--r--   0 bytedance   (501) staff       (20)      182 2023-07-24 08:27:54.000000 flexible_dict-1.1.1/flexible_dict/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      508 2023-07-24 09:58:30.000000 flexible_dict-1.1.1/flexible_dict/__main__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-07-25 03:17:53.000000 flexible_dict-1.1.1/flexible_dict/about.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5203 2023-07-24 08:26:14.000000 flexible_dict-1.1.1/flexible_dict/json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475002 flexible_dict-1.1.1/flexible_dict/script/
+-rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-24 09:41:19.000000 flexible_dict-1.1.1/flexible_dict/script/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5360 2023-07-25 03:14:12.000000 flexible_dict-1.1.1/flexible_dict/script/class_builder.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.474628 flexible_dict-1.1.1/flexible_dict.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1248 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-25 03:24:28.475750 flexible_dict-1.1.1/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)      970 2023-07-24 10:52:09.000000 flexible_dict-1.1.1/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475279 flexible_dict-1.1.1/tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)      625 2023-07-25 03:17:01.000000 flexible_dict-1.1.1/tests/test_build_class.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      410 2023-07-24 08:27:54.000000 flexible_dict-1.1.1/tests/test_json_object.py
```

### Comparing `flexible_dict-1.1.0/flexible_dict/json_object.py` & `flexible_dict-1.1.1/flexible_dict/json_object.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.0/setup.py` & `flexible_dict-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     exec(f.read(), about)
 
 setup(
     name=name,
     version=about['__version__'],
     description=description,
     long_description=long_description,
-    long_description_content_type='markdown',
+    long_description_content_type='text/markdown',
     author='darkpeath',
     author_email='darkpeath@gmail.com',
     url="https://github.com/darkpeath/flexible_dict",
     packages=packages,
     include_package_data=True,
     platforms="any",
     tests_require=["pytest"],
```

