# Comparing `tmp/tinyimagenet-0.6.tar.gz` & `tmp/tinyimagenet-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyimagenet-0.6.tar", last modified: Fri Jul 21 02:54:51 2023, max compression
+gzip compressed data, was "tinyimagenet-0.7.tar", last modified: Tue Jul 25 03:06:52 2023, max compression
```

## Comparing `tinyimagenet-0.6.tar` & `tinyimagenet-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-21 02:54:51.549855 tinyimagenet-0.6/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.6/LICENSE
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-21 02:54:51.549855 tinyimagenet-0.6/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      789 2023-07-11 15:17:51.000000 tinyimagenet-0.6/README.md
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)    13085 2023-07-11 15:24:08.000000 tinyimagenet-0.6/imagenet1k.py
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-21 02:54:51.549855 tinyimagenet-0.6/setup.cfg
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2964 2023-07-21 02:54:24.000000 tinyimagenet-0.6/setup.py
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-21 02:54:51.549855 tinyimagenet-0.6/tinyimagenet.egg-info/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      266 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/SOURCES.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/dependency_links.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/requires.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       24 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/top_level.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.6/tinyimagenet.egg-info/zip-safe
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     6235 2023-07-11 15:24:55.000000 tinyimagenet-0.6/tinyimagenet.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-25 03:06:52.626489 tinyimagenet-0.7/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.7/LICENSE
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1702 2023-07-25 03:06:52.626489 tinyimagenet-0.7/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      789 2023-07-11 15:17:51.000000 tinyimagenet-0.7/README.md
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)    13085 2023-07-11 15:24:08.000000 tinyimagenet-0.7/imagenet1k.py
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-25 03:06:52.626489 tinyimagenet-0.7/setup.cfg
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2964 2023-07-25 03:06:43.000000 tinyimagenet-0.7/setup.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-25 03:06:52.626489 tinyimagenet-0.7/tinyimagenet.egg-info/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1702 2023-07-25 03:06:52.000000 tinyimagenet-0.7/tinyimagenet.egg-info/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      266 2023-07-25 03:06:52.000000 tinyimagenet-0.7/tinyimagenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-25 03:06:52.000000 tinyimagenet-0.7/tinyimagenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-25 03:06:52.000000 tinyimagenet-0.7/tinyimagenet.egg-info/requires.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       24 2023-07-25 03:06:52.000000 tinyimagenet-0.7/tinyimagenet.egg-info/top_level.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.7/tinyimagenet.egg-info/zip-safe
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     6235 2023-07-11 15:24:55.000000 tinyimagenet-0.7/tinyimagenet.py
```

### Comparing `tinyimagenet-0.6/LICENSE` & `tinyimagenet-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.6/PKG-INFO` & `tinyimagenet-0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.6
+Version: 0.7
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
 Keywords: TinyImageNet ImageNet Dataset PyTorch torch torchvision
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,7 +42,9 @@
 print(f"Showing info of {n_samples} samples...")
 for i in range(0,n,n//n_samples):
     image,klass = dataset[i]
     print(f"Sample of class {klass:3d}, image {image}, words {dataset.idx_to_words[klass]}")
 ````
 
 You can also check the [quickstart notebook](https://colab.research.google.com/drive/1FCDsDJg86mCjyeAWOxDW9iF49goWCx4j?usp=sharing)
+
+
```

### Comparing `tinyimagenet-0.6/README.md` & `tinyimagenet-0.7/README.md`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.6/imagenet1k.py` & `tinyimagenet-0.7/imagenet1k.py`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.6/setup.py` & `tinyimagenet-0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 url="https://github.com/facundoq/tinyimagenet"
-VERSION="0.6"
+VERSION="0.7"
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
```

### Comparing `tinyimagenet-0.6/tinyimagenet.egg-info/PKG-INFO` & `tinyimagenet-0.7/tinyimagenet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.6
+Version: 0.7
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
 Keywords: TinyImageNet ImageNet Dataset PyTorch torch torchvision
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,7 +42,9 @@
 print(f"Showing info of {n_samples} samples...")
 for i in range(0,n,n//n_samples):
     image,klass = dataset[i]
     print(f"Sample of class {klass:3d}, image {image}, words {dataset.idx_to_words[klass]}")
 ````
 
 You can also check the [quickstart notebook](https://colab.research.google.com/drive/1FCDsDJg86mCjyeAWOxDW9iF49goWCx4j?usp=sharing)
+
+
```

### Comparing `tinyimagenet-0.6/tinyimagenet.py` & `tinyimagenet-0.7/tinyimagenet.py`

 * *Files identical despite different names*

