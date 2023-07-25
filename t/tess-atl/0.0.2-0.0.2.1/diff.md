# Comparing `tmp/tess-atl-0.0.2.tar.gz` & `tmp/tess-atl-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tess-atl-0.0.2.tar", last modified: Tue Jul 25 06:59:55 2023, max compression
+gzip compressed data, was "tess-atl-0.0.2.1.tar", last modified: Tue Jul 25 07:14:55 2023, max compression
```

## Comparing `tess-atl-0.0.2.tar` & `tess-atl-0.0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804406 tess-atl-0.0.2/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.804230 tess-atl-0.0.2/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.802944 tess-atl-0.0.2/atl/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2/atl/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2/atl/atl.py
--rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2/atl/cli.py
--rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2/atl/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2/atl/noise.py
--rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2/atl/query.py
--rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2/atl/scaling.py
--rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2/atl/tess_stars2px.py
--rw-r--r--   0 daniel     (501) staff       (20)       22 2023-07-25 06:58:59.000000 tess-atl-0.0.2/atl/version.py
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.804451 tess-atl-0.0.2/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      959 2023-07-25 06:42:18.000000 tess-atl-0.0.2/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804012 tess-atl-0.0.2/tess_atl.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/entry_points.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.009324 tess-atl-0.0.2.1/
+-rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:14:55.009117 tess-atl-0.0.2.1/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.007780 tess-atl-0.0.2.1/atl/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2.1/atl/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2.1/atl/atl.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2.1/atl/cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2.1/atl/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2.1/atl/noise.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2.1/atl/query.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2.1/atl/scaling.py
+-rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2.1/atl/tess_stars2px.py
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-07-25 07:14:52.000000 tess-atl-0.0.2.1/atl/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:14:55.009453 tess-atl-0.0.2.1/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      951 2023-07-25 07:12:45.000000 tess-atl-0.0.2.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.008785 tess-atl-0.0.2.1/tess_atl.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/top_level.txt
```

### Comparing `tess-atl-0.0.2/atl/atl.py` & `tess-atl-0.0.2.1/atl/atl.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/cli.py` & `tess-atl-0.0.2.1/atl/cli.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/noise.py` & `tess-atl-0.0.2.1/atl/noise.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/query.py` & `tess-atl-0.0.2.1/atl/query.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/scaling.py` & `tess-atl-0.0.2.1/atl/scaling.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/tess_stars2px.py` & `tess-atl-0.0.2.1/atl/tess_stars2px.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/setup.py` & `tess-atl-0.0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 # Prepare and send a new release to PyPI
 if "release" in sys.argv[-1]:
     os.system("python setup.py sdist")
     os.system("twine upload dist/*")
     os.system("rm -rf dist/tess-atl*")
     sys.exit()
 
-with open("requirements.txt") as f:
-    install_requires = f.read().splitlines()
+INSTALL_REQUIRES = ["numpy", "pandas", "astroquery", "astropy", "scipy"]
 
 # Load the __version__ variable without importing the package already
 exec(open("atl/version.py").read())
 
 setup(
     name="tess-atl",
     version=__version__,
@@ -24,14 +23,14 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
-    install_requires=install_requires,
+    install_requires=INSTALL_REQUIRES,
     entry_points={
         "console_scripts": [
             "atl=atl.cli:main",
         ],
     },
 )
```

