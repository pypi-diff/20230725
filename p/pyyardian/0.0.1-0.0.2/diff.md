# Comparing `tmp/pyyardian-0.0.1.tar.gz` & `tmp/pyyardian-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyardian-0.0.1.tar", last modified: Tue Jul 25 08:34:38 2023, max compression
+gzip compressed data, was "pyyardian-0.0.2.tar", last modified: Tue Jul 25 08:44:45 2023, max compression
```

## Comparing `pyyardian-0.0.1.tar` & `pyyardian-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:34:38.828797 pyyardian-0.0.1/
--rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-0.0.1/LICENSE
--rw-r--r--   0 guang      (501) staff       (20)      459 2023-07-25 08:34:38.829032 pyyardian-0.0.1/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-0.0.1/README.md
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:34:38.812459 pyyardian-0.0.1/pyyardian/
--rw-r--r--   0 guang      (501) staff       (20)       44 2023-07-25 08:17:24.000000 pyyardian-0.0.1/pyyardian/__init__.py
--rw-r--r--   0 guang      (501) staff       (20)     2364 2023-07-25 07:51:46.000000 pyyardian-0.0.1/pyyardian/async_client.py
--rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-0.0.1/pyyardian/const.py
-drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:34:38.827060 pyyardian-0.0.1/pyyardian.egg-info/
--rw-r--r--   0 guang      (501) staff       (20)      459 2023-07-25 08:34:38.000000 pyyardian-0.0.1/pyyardian.egg-info/PKG-INFO
--rw-r--r--   0 guang      (501) staff       (20)      235 2023-07-25 08:34:38.000000 pyyardian-0.0.1/pyyardian.egg-info/SOURCES.txt
--rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-25 08:34:38.000000 pyyardian-0.0.1/pyyardian.egg-info/dependency_links.txt
--rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-25 08:34:38.000000 pyyardian-0.0.1/pyyardian.egg-info/top_level.txt
--rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-25 08:34:38.839442 pyyardian-0.0.1/setup.cfg
--rw-r--r--   0 guang      (501) staff       (20)      483 2023-07-25 08:13:10.000000 pyyardian-0.0.1/setup.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:44:45.288077 pyyardian-0.0.2/
+-rw-r--r--   0 guang      (501) staff       (20)     1072 2023-07-25 08:04:44.000000 pyyardian-0.0.2/LICENSE
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-25 08:44:45.288279 pyyardian-0.0.2/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      150 2023-07-25 08:09:39.000000 pyyardian-0.0.2/README.md
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:44:45.283522 pyyardian-0.0.2/pyyardian/
+-rw-r--r--   0 guang      (501) staff       (20)       44 2023-07-25 08:17:24.000000 pyyardian-0.0.2/pyyardian/__init__.py
+-rw-r--r--   0 guang      (501) staff       (20)     2364 2023-07-25 07:51:46.000000 pyyardian-0.0.2/pyyardian/async_client.py
+-rw-r--r--   0 guang      (501) staff       (20)      365 2023-07-25 08:17:15.000000 pyyardian-0.0.2/pyyardian/const.py
+drwxr-xr-x   0 guang      (501) staff       (20)        0 2023-07-25 08:44:45.287037 pyyardian-0.0.2/pyyardian.egg-info/
+-rw-r--r--   0 guang      (501) staff       (20)      454 2023-07-25 08:44:45.000000 pyyardian-0.0.2/pyyardian.egg-info/PKG-INFO
+-rw-r--r--   0 guang      (501) staff       (20)      235 2023-07-25 08:44:45.000000 pyyardian-0.0.2/pyyardian.egg-info/SOURCES.txt
+-rw-r--r--   0 guang      (501) staff       (20)        1 2023-07-25 08:44:45.000000 pyyardian-0.0.2/pyyardian.egg-info/dependency_links.txt
+-rw-r--r--   0 guang      (501) staff       (20)       10 2023-07-25 08:44:45.000000 pyyardian-0.0.2/pyyardian.egg-info/top_level.txt
+-rw-r--r--   0 guang      (501) staff       (20)      107 2023-07-25 08:44:45.289426 pyyardian-0.0.2/setup.cfg
+-rw-r--r--   0 guang      (501) staff       (20)      570 2023-07-25 08:43:24.000000 pyyardian-0.0.2/setup.py
```

### Comparing `pyyardian-0.0.1/LICENSE` & `pyyardian-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyardian-0.0.1/pyyardian/async_client.py` & `pyyardian-0.0.2/pyyardian/async_client.py`

 * *Files identical despite different names*

