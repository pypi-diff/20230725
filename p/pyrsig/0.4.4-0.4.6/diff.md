# Comparing `tmp/pyrsig-0.4.4.tar.gz` & `tmp/pyrsig-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.4.4.tar", last modified: Fri Jun  9 15:49:01 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.6.tar", last modified: Tue Jul 25 15:47:24 2023, max compression
```

## Comparing `pyrsig-0.4.4.tar` & `pyrsig-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.4/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-09 15:49:01.000000 pyrsig-0.4.4/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.4/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-06-09 15:49:00.000000 pyrsig-0.4.4/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-06-09 15:49:01.000000 pyrsig-0.4.4/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.4/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.4/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3182 2023-06-07 12:10:43.000000 pyrsig-0.4.4/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.4/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.4.4/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.4/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.4/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)    50427 2023-06-08 20:40:23.000000 pyrsig-0.4.4/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-06-09 15:49:01.000000 pyrsig-0.4.4/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.4/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-07-25 15:47:24.000000 pyrsig-0.4.6/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.6/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-07-25 15:47:24.000000 pyrsig-0.4.6/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.6/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-07-25 15:47:24.000000 pyrsig-0.4.6/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-07-25 15:47:23.000000 pyrsig-0.4.6/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-07-25 15:47:23.000000 pyrsig-0.4.6/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-07-25 15:47:23.000000 pyrsig-0.4.6/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-07-25 15:47:23.000000 pyrsig-0.4.6/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-07-25 15:47:23.000000 pyrsig-0.4.6/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-07-25 15:47:24.000000 pyrsig-0.4.6/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-07-25 15:47:24.000000 pyrsig-0.4.6/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.6/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.6/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3182 2023-06-07 12:10:43.000000 pyrsig-0.4.6/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.6/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.4.6/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.6/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.6/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    51678 2023-07-25 15:40:26.000000 pyrsig-0.4.6/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-07-25 15:47:24.000000 pyrsig-0.4.6/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.6/README.md
```

### Comparing `pyrsig-0.4.4/setup.py` & `pyrsig-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/PKG-INFO` & `pyrsig-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.4
+Version: 0.4.6
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.4/LICENSE` & `pyrsig-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.6/pyrsig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.4.4
+Version: 0.4.6
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.4.4/pyrsig/tests/test_api.py` & `pyrsig-0.4.6/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.6/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.6/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig/tests/test_coards.py` & `pyrsig-0.4.6/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig/tests/test_gui.py` & `pyrsig-0.4.6/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.4.4/pyrsig/__init__.py` & `pyrsig-0.4.6/pyrsig/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
-__version__ = '0.4.4'
+__version__ = '0.4.6'
 
 import pandas as pd
-
+import requests
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
         XORIG=-2556000.0, YORIG=-1728000.0, XCELL=12000., YCELL=12000.,
         P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
     ),
@@ -112,32 +112,32 @@
     'pandora.L2_rsus1p1_8.sulfur_dioxide_air_mass_factor_uncertainty',
     'pandora.L2_rnvssp1_8.nitrogen_dioxide_vertical_column_amount',
     'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor',
     'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
     'purpleair.pm25_corrected',
     'purpleair.pm25_corrected_hourly', 'purpleair.pm25_corrected_daily',
     'purpleair.pm25_corrected_monthly', 'purpleair.pm25_corrected_yearly',
-    'tempo.proxy_l2.no2.vertical_column_total',
-    'tempo.proxy_l2.no2.vertical_column_total_uncertainty',
-    'tempo.proxy_l2.no2.vertical_column_troposphere',
-    'tempo.proxy_l2.no2.vertical_column_stratosphere',
-    'tempo.proxy_l2.no2.amf_total',
-    'tempo.proxy_l2.no2.amf_total_uncertainty',
-    'tempo.proxy_l2.no2.amf_troposphere',
-    'tempo.proxy_l2.no2.amf_stratosphere',
-    'tempo.proxy_l2.no2.ground_pixel_quality_flag'
-    'tempo.proxy_l2.hcho.vertical_column',
-    'tempo.proxy_l2.hcho.vertical_column_uncertainty',
-    'tempo.proxy_l2.hcho.amf',
-    'tempo.proxy_l2.hcho.amf_uncertainty',
-    'tempo.proxy_l2.o3p.total_ozone_column',
-    'tempo.proxy_l2.o3p.troposphere_ozone_column',
-    'tempo.proxy_l2.o3p.stratosphere_ozone_column',
-    'tempo.proxy_l2.o3p.ozone_information_content',
-    'tempo.proxy_l2.o3p.ground_pixel_quality_flag',
+    'tempo2.proxy_l2.no2.vertical_column_total',
+    'tempo2.proxy_l2.no2.vertical_column_total_uncertainty',
+    'tempo2.proxy_l2.no2.vertical_column_troposphere',
+    'tempo2.proxy_l2.no2.vertical_column_stratosphere',
+    'tempo2.proxy_l2.no2.amf_total',
+    'tempo2.proxy_l2.no2.amf_total_uncertainty',
+    'tempo2.proxy_l2.no2.amf_troposphere',
+    'tempo2.proxy_l2.no2.amf_stratosphere',
+    'tempo2.proxy_l2.no2.ground_pixel_quality_flag'
+    'tempo2.proxy_l2.hcho.vertical_column',
+    'tempo2.proxy_l2.hcho.vertical_column_uncertainty',
+    'tempo2.proxy_l2.hcho.amf',
+    'tempo2.proxy_l2.hcho.amf_uncertainty',
+    'tempo2.proxy_l2.o3p.total_ozone_column',
+    'tempo2.proxy_l2.o3p.troposphere_ozone_column',
+    'tempo2.proxy_l2.o3p.stratosphere_ozone_column',
+    'tempo2.proxy_l2.o3p.ozone_information_content',
+    'tempo2.proxy_l2.o3p.ground_pixel_quality_flag',
     'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
     'tropomi.offl.no2.air_mass_factor_troposphere',
     'tropomi.offl.hcho.formaldehyde_tropospheric_vertical_column',
     'tropomi.offl.co.carbonmonoxide_total_column',
     'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
@@ -265,14 +265,49 @@
     else:
         if blocknum == 0:
             print('Retrieving .', end='', flush=True)
         if (blocknum % pblocks) == 0:
             print('.', end='', flush=True)
 
 
+def _create_unverified_tls_context(*args, **kwds):
+    """
+    Thin wrapper around ssl._create_unverified_context that adds the option to
+    use TLS negotiation, which is currently used by RSIG servers.
+    """
+    import ssl
+    # Set up SSL context to allow legacy TLS versions
+    ctx = ssl._create_unverified_context(*args, **kwds)
+    ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
+    return ctx
+
+
+class LegacyAdapter(requests.adapters.HTTPAdapter):
+    # "Transport adapter" that allows us to use custom ssl_context.
+
+    def __init__(self, **kwargs):
+        import ssl
+        ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
+        ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
+        self.ssl_context = ctx
+        super().__init__(**kwargs)
+
+    def init_poolmanager(self, connections, maxsize, block=False):
+        import urllib3
+        self.poolmanager = urllib3.poolmanager.PoolManager(
+            num_pools=connections, maxsize=maxsize,
+            block=block, ssl_context=self.ssl_context)
+
+
+def legacy_get(*args, **kwds):
+    session = requests.session()
+    session.mount('https://', LegacyAdapter())
+    return session.get(*args, **kwds)
+
+
 def _getfile(url, outpath, maxtries=5, verbose=1, overwrite=False):
     """
     Download file from RSIG using fault tolerance and optional caching
     when overwrite is False.
 
     Arguments
     ---------
@@ -293,28 +328,29 @@
     None
     """
     import time
     from urllib.request import urlretrieve
     import ssl
     import os
 
-    ssl._create_default_https_context = ssl._create_unverified_context
-
     # If the file exists, get the current size
     if not overwrite and os.path.exists(outpath):
         stat = os.stat(outpath)
         dlsize = stat.st_size
     else:
         dlsize = 0
 
     # if the size is non-zero, assume it is good
     if dlsize > 0:
         print('Using cached:', outpath)
         return
 
+    _def_https_context = ssl._create_default_https_context
+    ssl._create_default_https_context = _create_unverified_tls_context
+
     # Try to download the file maxtries times
     tries = 0
     if verbose > 0:
         reporthook = _progress
     else:
         reporthook = None
     while dlsize <= 0 and tries < maxtries:
@@ -339,14 +375,16 @@
         if dlsize == 0:
             print('Failed', url, t1 - t0)
         tries += 1
 
         if verbose > 0:
             print('')
 
+    ssl._create_default_https_context = _def_https_context
+
 
 def get_proj4(attrs, earth_radius=6370000.):
     """
     Create a proj4 formatted grid definition using IOAPI attrs and earth_radius
 
     Arguments
     ---------
@@ -697,19 +735,18 @@
         -------
             df = rsigapi.describe('airnow.no2')
             print(df.to_csv())
             # ,name,label,description,bbox_str,beginPosition,timeResolution
             # 0,no2,no2(ppb),UTC hourly mean surface measured nitrogen ...,
             # ... -157 21 -51 64,2003-01-02T00:00:00Z,PT1H
         """
-        import requests
         import warnings
 
         if key not in self._description:
-            r = requests.get(
+            r = legacy_get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 f'1.0.0&REQUEST=DescribeCoverage&COVERAGE={key}&compress=1'
             )
             self._description[key] = r.text
 
         if raw:
             return self._description[key]
@@ -766,23 +803,22 @@
             # ['tropomi.nrti.no2.nitrogendioxide_tropospheric_column'
             #  ... 43 other name here
             #  'tropomi.rpro.ch4.methane_mixing_ratio_bias_corrected']
         """
         import re
         import pandas as pd
         import warnings
-        import requests
 
         if as_dataframe and self._coveragesdf is not None:
             return self._coveragesdf
 
         if self._describecoverages is None:
             if verbose > 1:
                 print('Requesting...', flush=True)
-            self._describecoverages = requests.get(
+            self._describecoverages = legacy_get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 '1.0.0&REQUEST=DescribeCoverage&compress=1'
             ).text
 
         ctext = self._describecoverages
 
         # Start Cleaning Section
@@ -886,17 +922,16 @@
         return coverages
 
     def capabilities(self):
         """
         At this time, the capabilities does not list cmaq.*
 
         """
-        import requests
         if self._capabilities is None:
-            self._capabilities = requests.get(
+            self._capabilities = legacy_get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 '1.0.0&REQUEST=GetCapabilities&compress=1'
             )
 
         return self._capabilities
 
     def keys(self, offline=True):
```

### Comparing `pyrsig-0.4.4/README.md` & `pyrsig-0.4.6/README.md`

 * *Files identical despite different names*

