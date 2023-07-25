# Comparing `tmp/pythonperlin-0.0.6.tar.gz` & `tmp/pythonperlin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonperlin-0.0.6.tar", last modified: Tue Jul 11 14:11:49 2023, max compression
+gzip compressed data, was "pythonperlin-0.0.7.tar", last modified: Tue Jul 25 15:49:33 2023, max compression
```

## Comparing `pythonperlin-0.0.6.tar` & `pythonperlin-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-11 14:11:49.588186 pythonperlin-0.0.6/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.6/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-11 14:11:49.588077 pythonperlin-0.0.6/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4648 2023-07-10 14:34:06.000000 pythonperlin-0.0.6/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-11 14:11:49.587359 pythonperlin-0.0.6/pythonperlin/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      172 2023-07-11 14:05:32.000000 pythonperlin-0.0.6/pythonperlin/__init__.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     8488 2023-07-11 14:04:52.000000 pythonperlin-0.0.6/pythonperlin/perlin.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-11 14:11:49.587931 pythonperlin-0.0.6/pythonperlin.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-11 14:11:49.000000 pythonperlin-0.0.6/pythonperlin.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-11 14:11:49.000000 pythonperlin-0.0.6/pythonperlin.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-11 14:11:49.000000 pythonperlin-0.0.6/pythonperlin.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-11 14:11:49.000000 pythonperlin-0.0.6/pythonperlin.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-11 14:11:49.000000 pythonperlin-0.0.6/pythonperlin.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-11 14:11:49.588225 pythonperlin-0.0.6/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-11 14:06:38.000000 pythonperlin-0.0.6/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.660013 pythonperlin-0.0.7/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.7/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-25 15:49:33.659854 pythonperlin-0.0.7/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     4648 2023-07-10 14:34:06.000000 pythonperlin-0.0.7/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.658601 pythonperlin-0.0.7/pythonperlin/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      172 2023-07-11 14:05:32.000000 pythonperlin-0.0.7/pythonperlin/__init__.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     8488 2023-07-25 15:46:10.000000 pythonperlin-0.0.7/pythonperlin/perlin.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.659622 pythonperlin-0.0.7/pythonperlin.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-25 15:49:33.660071 pythonperlin-0.0.7/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-25 15:46:36.000000 pythonperlin-0.0.7/setup.py
```

### Comparing `pythonperlin-0.0.6/LICENSE` & `pythonperlin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.6/PKG-INFO` & `pythonperlin-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythonperlin-0.0.6/README.md` & `pythonperlin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.6/pythonperlin/perlin.py` & `pythonperlin-0.0.7/pythonperlin/perlin.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         m = x.shape[axis]
         l = np.linspace(0, 1, m)
         f = interp1d(l, x, kind, axis)
         l = np.linspace(0, 1, (n + 1) * (m - 1) + 1)
         x_ = f(l)
         if mode == 'same':
             slc = [slice(None)] * x.ndim
-            slc[axis] = slice(0, n)
+            slc[axis] = slice(0, m)
             x_ = x_[tuple(slc)]
     return x_
```

### Comparing `pythonperlin-0.0.6/pythonperlin.egg-info/PKG-INFO` & `pythonperlin-0.0.7/pythonperlin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythonperlin-0.0.6/setup.py` & `pythonperlin-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="pythonperlin",
-    version="0.0.6",
+    version="0.0.7",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Perlin noise in python - seamlessly tile in any dimensions",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/pythonperlin",
```

