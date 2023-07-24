# Comparing `tmp/lexset-4.0.8.tar.gz` & `tmp/lexset-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.8.tar", last modified: Fri Jul 21 19:28:10 2023, max compression
+gzip compressed data, was "lexset-4.0.9.tar", last modified: Mon Jul 24 23:36:29 2023, max compression
```

## Comparing `lexset-4.0.8.tar` & `lexset-4.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 19:28:10.700563 lexset-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 19:27:55.000000 lexset-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/review.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:28:10.700563 lexset-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 19:27:55.000000 lexset-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:36:29.102367 lexset-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 23:36:29.102367 lexset-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 23:36:11.000000 lexset-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:36:29.098367 lexset-4.0.9/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-24 23:36:11.000000 lexset-4.0.9/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-24 23:36:11.000000 lexset-4.0.9/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-24 23:36:11.000000 lexset-4.0.9/lexset/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-07-24 23:36:11.000000 lexset-4.0.9/lexset/review.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:36:29.098367 lexset-4.0.9/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 23:36:29.000000 lexset-4.0.9/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-24 23:36:29.000000 lexset-4.0.9/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:36:29.000000 lexset-4.0.9/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 23:36:29.000000 lexset-4.0.9/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 23:36:29.000000 lexset-4.0.9/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 23:36:29.102367 lexset-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 23:36:11.000000 lexset-4.0.9/setup.py
```

### Comparing `lexset-4.0.8/lexset/LexsetManager.py` & `lexset-4.0.9/lexset/LexsetManager.py`

 * *Files identical despite different names*

### Comparing `lexset-4.0.8/lexset/credentials.py` & `lexset-4.0.9/lexset/credentials.py`

 * *Files identical despite different names*

### Comparing `lexset-4.0.8/lexset/review.py` & `lexset-4.0.9/lexset/review.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 
     #performs relative size analysis on a dataset containing object annotations 
     # with bounding box information. The goal is to analyze the relative size 
     # of objects within each category and visualize the distribution of relative 
     # sizes using histograms.
 
-    def relative_scale(self):
+    def relative_scale(self,num_bins=50):
 
         # Load JSON data
         with open(self.dir + 'coco_annotations.json') as f:
             data = json.load(f)
 
         # Prepare a dictionary to hold relative sizes per category
         relative_sizes = {category['id']: [] for category in data['categories']}
@@ -146,15 +146,15 @@
         grid_size = math.ceil(math.sqrt(num_categories))
         fig, axs = plt.subplots(grid_size, grid_size, figsize=(15, 15))
 
         # Plot a histogram of relative sizes for each category
         for i, category in enumerate(data['categories']):
             row = i // grid_size
             col = i % grid_size
-            axs[row, col].hist(relative_sizes[category['id']], bins=50)
+            axs[row, col].hist(relative_sizes[category['id']], bins=num_bins)
             axs[row, col].set_title(category["name"])
 
         # Remove any unused subplots
         for j in range(i+1, grid_size*grid_size):
             fig.delaxes(axs.flatten()[j])
 
         plt.tight_layout()
```

### Comparing `lexset-4.0.8/setup.py` & `lexset-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='lexset',
-      version='4.0.8',
+      version='4.0.9',
       author='F. Bitonti',
       author_email='Francis@lexset.ai',
       license='Apache 2.0',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3'
       ],
```

