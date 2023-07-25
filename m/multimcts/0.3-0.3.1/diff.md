# Comparing `tmp/multimcts-0.3.tar.gz` & `tmp/multimcts-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.3.tar", last modified: Tue Jul 25 18:33:20 2023, max compression
+gzip compressed data, was "multimcts-0.3.1.tar", last modified: Tue Jul 25 18:52:12 2023, max compression
```

## Comparing `multimcts-0.3.tar` & `multimcts-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.536037 multimcts-0.3/
--rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.3/LICENSE
--rw-r--r--   0 taylorvance   (501) staff       (20)     2770 2023-07-25 18:33:20.535903 multimcts-0.3/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     2489 2023-07-25 16:42:00.000000 multimcts-0.3/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.535197 multimcts-0.3/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.3/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   430223 2023-07-25 17:39:23.000000 multimcts-0.3/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)     9693 2023-07-24 19:46:18.000000 multimcts-0.3/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.535714 multimcts-0.3/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2770 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      231 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.3/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-25 18:33:20.536083 multimcts-0.3/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      565 2023-07-25 18:33:14.000000 multimcts-0.3/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.032456 multimcts-0.3.1/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.3.1/LICENSE
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2805 2023-07-25 18:52:12.032320 multimcts-0.3.1/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2489 2023-07-25 16:42:00.000000 multimcts-0.3.1/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.031629 multimcts-0.3.1/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.3.1/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   430223 2023-07-25 17:39:23.000000 multimcts-0.3.1/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)     9693 2023-07-24 19:46:18.000000 multimcts-0.3.1/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.032128 multimcts-0.3.1/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2805 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      231 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.3.1/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-25 18:52:12.032501 multimcts-0.3.1/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      619 2023-07-25 18:51:52.000000 multimcts-0.3.1/setup.py
```

### Comparing `multimcts-0.3/LICENSE` & `multimcts-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multimcts-0.3/PKG-INFO` & `multimcts-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.3
+Version: 0.3.1
 Summary: Monte Carlo Tree Search for multiple teams
-Home-page: UNKNOWN
+Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `multimcts-0.3/README.md` & `multimcts-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multimcts-0.3/multimcts/mcts.c` & `multimcts-0.3.1/multimcts/mcts.c`

 * *Files identical despite different names*

### Comparing `multimcts-0.3/multimcts/mcts.pyx` & `multimcts-0.3.1/multimcts/mcts.pyx`

 * *Files identical despite different names*

### Comparing `multimcts-0.3/multimcts.egg-info/PKG-INFO` & `multimcts-0.3.1/multimcts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.3
+Version: 0.3.1
 Summary: Monte Carlo Tree Search for multiple teams
-Home-page: UNKNOWN
+Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `multimcts-0.3/setup.py` & `multimcts-0.3.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
 setup(
     name='multimcts',
-    version='0.3',
+    version='0.3.1',
     description='Monte Carlo Tree Search for multiple teams',
     author='Taylor Vance',
     author_email='mirrors.cities0w@icloud.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
+    url='https://github.com/taylorvance/multimcts',
     packages=find_packages(),
     ext_modules=cythonize([
         Extension('multimcts.mcts', ['multimcts/mcts.pyx']),
     ]),
     package_data={'multimcts': ['*.pyx']},
 )
```

