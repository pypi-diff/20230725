# Comparing `tmp/tess-atl-0.0.2.1.tar.gz` & `tmp/tess-atl-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tess-atl-0.0.2.1.tar", last modified: Tue Jul 25 07:14:55 2023, max compression
+gzip compressed data, was "tess-atl-0.0.2.2.tar", last modified: Tue Jul 25 07:26:46 2023, max compression
```

## Comparing `tess-atl-0.0.2.1.tar` & `tess-atl-0.0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.009324 tess-atl-0.0.2.1/
--rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:14:55.009117 tess-atl-0.0.2.1/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.007780 tess-atl-0.0.2.1/atl/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2.1/atl/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2.1/atl/atl.py
--rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2.1/atl/cli.py
--rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2.1/atl/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2.1/atl/noise.py
--rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2.1/atl/query.py
--rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2.1/atl/scaling.py
--rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2.1/atl/tess_stars2px.py
--rw-r--r--   0 daniel     (501) staff       (20)       24 2023-07-25 07:14:52.000000 tess-atl-0.0.2.1/atl/version.py
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:14:55.009453 tess-atl-0.0.2.1/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      951 2023-07-25 07:12:45.000000 tess-atl-0.0.2.1/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:14:55.008785 tess-atl-0.0.2.1/tess_atl.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/entry_points.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 07:14:54.000000 tess-atl-0.0.2.1/tess_atl.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:26:46.788634 tess-atl-0.0.2.2/
+-rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:26:46.788450 tess-atl-0.0.2.2/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:26:46.786813 tess-atl-0.0.2.2/atl/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2.2/atl/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7245 2023-07-25 07:25:05.000000 tess-atl-0.0.2.2/atl/atl.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3192 2023-07-25 07:25:19.000000 tess-atl-0.0.2.2/atl/cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2.2/atl/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2.2/atl/noise.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2.2/atl/query.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2.2/atl/scaling.py
+-rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2.2/atl/tess_stars2px.py
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-07-25 07:26:43.000000 tess-atl-0.0.2.2/atl/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:26:46.788718 tess-atl-0.0.2.2/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      951 2023-07-25 07:12:45.000000 tess-atl-0.0.2.2/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:26:46.788069 tess-atl-0.0.2.2/tess_atl.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      297 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 07:26:46.000000 tess-atl-0.0.2.2/tess_atl.egg-info/top_level.txt
```

### Comparing `tess-atl-0.0.2.1/atl/atl.py` & `tess-atl-0.0.2.2/atl/atl.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,27 @@
 from .tess_stars2px import tess_stars2px_function_entry
 from .scaling import *
 from .query import *
 from .noise import *
 
 
 def granulation(nu0, DILUTION, VNYQ):
-    # calculate the granulation at a set of frequencies from (7) eqn 2 model F
-    # Divide by DILUTION squared as it affects stars in the time series.
-    # The units of DILUTION change from ppm to ppm^2 microHz^-1 when going from the
-    # time series to frequency. p6: c=4 and zeta = 2*sqrt(2)/pi
+    """Calculate the granulation at a set of frequencies from (7) eqn 2 model F
+    Divide by DILUTION squared as it affects stars in the time series.
+    The units of DILUTION change from ppm to ppm^2 microHz^-1 when going from the
+    time series to frequency. p6: c=4 and zeta = 2*sqrt(2)/pi
+
+    Args:
+        nu0 (_type_): _description_
+        DILUTION (_type_): _description_
+        VNYQ (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
 
     a_nomass = 0.85 * 3382 * nu0**-0.609
     b1 = 0.317 * nu0**0.970
     b2 = 0.948 * nu0**0.992
     Pgran = (
         ((2 * np.sqrt(2)) / np.pi) * (a_nomass**2 / b1) / (1 + ((nu0 / b1) ** 4))
         + ((2 * np.sqrt(2)) / np.pi) * (a_nomass**2 / b2) / (1 + ((nu0 / b2) ** 4))
@@ -141,15 +150,15 @@
     nbins = int((2.0 * env_width / bw))  # from (11)
     snrthresh = stats.chi2.ppf(pdet, 2.0 * nbins) / (2.0 * nbins) - 1.0
 
     pfinal = stats.chi2.sf((snrthresh + 1.0) / (snr + 1.0) * 2.0 * nbins, 2.0 * nbins)
     return pfinal, snr, numax, dnu  # , snrthresh # snr is needed in TESS_telecon2.py
 
 
-def get_sectors(vals):  #
+def get_sectors(vals):
     (
         outID,
         outEclipLong,
         outEclipLat,
         outSec,
         outCam,
         outCcd,
```

### Comparing `tess-atl-0.0.2.1/atl/cli.py` & `tess-atl-0.0.2.2/atl/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,20 +29,19 @@
         required=False,
         default=0.05,
         help="The false alarm probability level above which the probability of detection is measured.",
     )
     parser.add_argument(
         "--cadence",
         type=int,
-        required=True,
+        required=False,
         default=20,
         help="The observational cadence, either 20 or 120. Default is 20.",
     )
 
-    # magnitude, teff, radius, logg, sectors, cadence,
     args = parser.parse_args()
 
     # Query the TIC first for magnitudes, positions.
     if args.target is not None:
         ticid = None  # this is awful but i can't be bothered.
         q = Simbad.query_objectids(args.target)
         for ids in q["ID"]:
```

### Comparing `tess-atl-0.0.2.1/atl/noise.py` & `tess-atl-0.0.2.2/atl/noise.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2.1/atl/query.py` & `tess-atl-0.0.2.2/atl/query.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2.1/atl/scaling.py` & `tess-atl-0.0.2.2/atl/scaling.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2.1/atl/tess_stars2px.py` & `tess-atl-0.0.2.2/atl/tess_stars2px.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2.1/setup.py` & `tess-atl-0.0.2.2/setup.py`

 * *Files identical despite different names*

