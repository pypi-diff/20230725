# Comparing `tmp/tess-atl-0.0.1.tar.gz` & `tmp/tess-atl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tess-atl-0.0.1.tar", last modified: Tue Jul 25 06:41:55 2023, max compression
+gzip compressed data, was "tess-atl-0.0.2.tar", last modified: Tue Jul 25 06:59:55 2023, max compression
```

## Comparing `tess-atl-0.0.1.tar` & `tess-atl-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:41:55.272779 tess-atl-0.0.1/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:41:55.272619 tess-atl-0.0.1/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:41:55.271482 tess-atl-0.0.1/atl/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.1/atl/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:31:13.000000 tess-atl-0.0.1/atl/atl.py
--rw-r--r--   0 daniel     (501) staff       (20)     3210 2023-07-25 06:39:52.000000 tess-atl-0.0.1/atl/cli.py
--rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.1/atl/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.1/atl/noise.py
--rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.1/atl/query.py
--rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.1/atl/scaling.py
--rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.1/atl/tess_stars2px.py
--rw-r--r--   0 daniel     (501) staff       (20)       22 2023-07-25 02:45:01.000000 tess-atl-0.0.1/atl/version.py
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:41:55.272826 tess-atl-0.0.1/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      958 2023-07-25 06:38:37.000000 tess-atl-0.0.1/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:41:55.272393 tess-atl-0.0.1/tess_atl.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/entry_points.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 06:41:55.000000 tess-atl-0.0.1/tess_atl.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804406 tess-atl-0.0.2/
+-rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.804230 tess-atl-0.0.2/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.802944 tess-atl-0.0.2/atl/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2/atl/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2/atl/atl.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2/atl/cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2/atl/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2/atl/noise.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2/atl/query.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2/atl/scaling.py
+-rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2/atl/tess_stars2px.py
+-rw-r--r--   0 daniel     (501) staff       (20)       22 2023-07-25 06:58:59.000000 tess-atl-0.0.2/atl/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.804451 tess-atl-0.0.2/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      959 2023-07-25 06:42:18.000000 tess-atl-0.0.2/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804012 tess-atl-0.0.2/tess_atl.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/top_level.txt
```

### Comparing `tess-atl-0.0.1/atl/atl.py` & `tess-atl-0.0.2/atl/atl.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.1/atl/cli.py` & `tess-atl-0.0.2/atl/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         default=0.05,
         help="The false alarm probability level above which the probability of detection is measured.",
     )
     parser.add_argument(
         "--cadence",
         type=int,
         required=True,
-        help="The observational cadence, either 20 or 120",
+        default=20,
+        help="The observational cadence, either 20 or 120. Default is 20.",
     )
 
     # magnitude, teff, radius, logg, sectors, cadence,
     args = parser.parse_args()
 
     # Query the TIC first for magnitudes, positions.
     if args.target is not None:
```

### Comparing `tess-atl-0.0.1/atl/noise.py` & `tess-atl-0.0.2/atl/noise.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.1/atl/query.py` & `tess-atl-0.0.2/atl/query.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.1/atl/scaling.py` & `tess-atl-0.0.2/atl/scaling.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.1/atl/tess_stars2px.py` & `tess-atl-0.0.2/atl/tess_stars2px.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.1/setup.py` & `tess-atl-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from setuptools import setup
 
 # Prepare and send a new release to PyPI
 if "release" in sys.argv[-1]:
     os.system("python setup.py sdist")
     os.system("twine upload dist/*")
-    os.system("rm -rf dist/echelle*")
+    os.system("rm -rf dist/tess-atl*")
     sys.exit()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 # Load the __version__ variable without importing the package already
 exec(open("atl/version.py").read())
```

