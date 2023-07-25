# Comparing `tmp/ccp-performance-0.3.3.tar.gz` & `tmp/ccp-performance-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-wlwizsf7/ccp-performance-0.3.3.tar", last modified: Fri May 26 00:26:01 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-_plnr9zu/ccp-performance-0.3.4.tar", last modified: Tue Jul 25 20:36:14 2023, max compression
```

## Comparing `ccp-performance-0.3.3.tar` & `ccp-performance-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47176 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/compressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/config/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/fluids.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/new_units.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/data_io/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/read_xl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/fo.py
--rw-r--r--   0 runner    (1001) docker     (123)    39930 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/impeller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    57872 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/normal-head.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/app/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    54302 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/assets/ccp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/ccp_app_back_to_back.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    82488 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/ccp_app_back_to_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/ccp_app_straight_through.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    62886 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/ccp_app_straight_through.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/app/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/data/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/example_straight.ccp
+-rw-r--r--   0 runner    (1001) docker     (123)  4283651 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/app/p77_export_a.ccp
+-rw-r--r--   0 runner    (1001) docker     (123)    47176 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/config/fluids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/config/new_units.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/config/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/config/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/data_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/data_io/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/data_io/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/data_io/read_xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/fo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43936 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/impeller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58508 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24672 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-25 20:36:04.000000 ccp-performance-0.3.4/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:36:14.000000 ccp-performance-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-25 20:36:05.000000 ccp-performance-0.3.4/setup.py
```

### Comparing `ccp-performance-0.3.3/LICENSE` & `ccp-performance-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/PKG-INFO` & `ccp-performance-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.3
+Version: 0.3.4
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
```

### Comparing `ccp-performance-0.3.3/README.md` & `ccp-performance-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/__init__.py` & `ccp-performance-0.3.4/ccp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     _shared_library = "REFPRP64.DLL"
 
 _library_path = _path / _shared_library
 
 if not _library_path.is_file():
     _warnings.warn(f"{_library_path}.\nREFPROP not configured.")
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 __version__full = (
     f"ccp: {__version__} | "
     + f'CP : {_CP.get_global_param_string("version")} | '
     + f'REFPROP : {_CP.get_global_param_string("REFPROP_version")}'
 )
```

### Comparing `ccp-performance-0.3.3/ccp/compressor.py` & `ccp-performance-0.3.4/ccp/compressor.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/config/fluids.py` & `ccp-performance-0.3.4/ccp/config/fluids.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/config/units.py` & `ccp-performance-0.3.4/ccp/config/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "flow_m": "kilogram/second",
     "fit": "m",
     "viscosity": "pascal*s",
     "h": "joule/kilogram",
     "s": "joule/(kelvin kilogram)",
     "b": "meter",
     "D": "meter",
+    "d": "meter",
     "roughness": "meter",
     "head": "joule/kilogram",
     "eff": "dimensionless",
     "power": "watt",
 }
 for i, unit in zip(["k", "c"], ["N/m", "N*s/m"]):
     for j in ["x", "y", "z"]:
```

### Comparing `ccp-performance-0.3.3/ccp/curve.py` & `ccp-performance-0.3.4/ccp/curve.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/data_io/processing.py` & `ccp-performance-0.3.4/ccp/data_io/processing.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         .rolling(
             window=window,
         )
         .apply(fluctuation)
         .fillna(0.0)
     )
     fluctuation_df = fluctuation_df[window - 1 :]
-    fluctuation_df.reset_index(drop=True, inplace=True)
     return fluctuation_df
 
 
 def mean_data(df, window=3):
     """Calculate the mean of dataframe columns.
 
     The mean is calculated using a rolling window.
@@ -115,31 +114,38 @@
         df.apply(pd.to_numeric)
         .rolling(
             window=window,
         )
         .mean()
     )
     mean_df = mean_df[window - 1 :]
-    mean_df.reset_index(drop=True, inplace=True)
     return mean_df
 
 
 def filter_data(
     df,
     window=3,
     data_type=None,
     temperature_fluctuation=0.5,
     pressure_fluctuation=2,
     speed_fluctuation=0.5,
 ):
     """Filter data according to fluctuation values.
 
-    This function filters the data according to the fluctuation values of the
-    columns and returns the mean value for set of values defined by the window size.
+    This function performs two filters:
+        1. Remove rows where the speed is zero.
+        2. Remove rows where the fluctuation of the data is higher than the
+        maximum fluctuation defined by the user.
+
+    After filtering, it returns the mean value for set of values defined by
+    the window size.
     Default values for maximum fluctuation are based on ASME PTC 10-1997.
+    As per ASME PTC 10-1997, the minimum duration of a test point is 15 minutes.
+    Assuming that we need a minimum of 3 measurements to calculate the fluctuation, the
+    time span between each measurement is 7.5 minutes.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Dataframe with data to be filtered.
     window : int, optional
         Window size for rolling calculation, meaning how many rolls will be used
@@ -169,21 +175,27 @@
     >>> df = pd.DataFrame({'a': [1, 2, 3, 4, 4.01, 4.02], 'b': [4, 5, 6, 6.01, 6.02, 6.03]})
     >>> data_type = {'a': 'pressure', 'b': 'temperature'}
     >>> filter_data(df, window=3, data_type=data_type)
     """
     fluctuation_df = fluctuation_data(df, window=window)
     mean_df = mean_data(df, window=window)
     # filter mean_df based on fluctuation_df max values
-    for column in fluctuation_df.columns:
-        if data_type[column] == "pressure":
+    for column, property_type in data_type.items():
+        if property_type == "pressure":
             max_fluctuation = pressure_fluctuation
-        elif data_type[column] == "temperature":
+            # remove pressure values below 0
+            mean_df.loc[mean_df[column] < 0, column] = None
+        elif property_type == "temperature":
             max_fluctuation = temperature_fluctuation
-        elif data_type[column] == "speed":
+            # remove temperature values below 0
+            mean_df.loc[mean_df[column] < 0, column] = None
+        elif property_type == "speed":
             max_fluctuation = speed_fluctuation
+            # remove speed values below 1
+            mean_df.loc[mean_df[column] < 1, column] = None
         else:
             raise ValueError(
                 f"Invalid data type for column {column}. "
                 "Valid data types are: pressure, temperature and speed."
             )
         mean_df.loc[fluctuation_df[column] > max_fluctuation, column] = None
     mean_df = mean_df.dropna()
```

### Comparing `ccp-performance-0.3.3/ccp/data_io/read_csv.py` & `ccp-performance-0.3.4/ccp/data_io/read_csv.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/impeller.py` & `ccp-performance-0.3.4/ccp/impeller.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from scipy.interpolate import interp1d, UnivariateSpline
 from scipy.optimize import fsolve
 
 from ccp import Q_, State, Point, Curve
 from ccp.config.units import check_units
 from ccp.config.utilities import r_getattr, r_setattr
 from ccp.data_io.read_csv import read_data_from_engauge_csv
+from ccp.plotly_theme import tableau_colors
 
 
 class ImpellerStateParameter:
     def __init__(self, impeller_state_object, attr):
         self.impeller_state_object = impeller_state_object
         self.attr = attr
 
@@ -59,30 +60,30 @@
         self.impeller_object = impeller_object
         self.attr = attr
 
     @check_units
     def __call__(self, *args, flow_v=None, speed=None, plot_kws=None, **kwargs):
         """Plot parameter versus volumetric flow.
 
-        You can plot an specific point in the plot giving its flow_v and speed.
+        You can plot a specific point in the plot giving its flow_v and speed.
 
         You can choose units with the arguments flow_v_units='...' and
         {attr}_units='...'. For the speed you can use speed_units='...'.
 
         Parameters
         ----------
         flow_v : pint.Quantity, float, optional
             Volumetric flow (m³/s) for a specific point in the plot.
         speed : pint.Quantity, float, optional
             Speed (rad/s) for a specific point in the plot.
         flow_v_units : str, optional
             Flow units used for the plot. Default is m³/s.
         {attr}_units : str, optional
             Units for the parameter being plotted (e.g. for a head plot we could use
-            head_units='J/kg' or head_units='J/g'. Default is SI.
+            head_units='J/kg' or head_units='J/g'). Default is SI.
         speed_units : str, optional
             Speed units for the plot. Default is 'rad/s'.
 
         Returns
         -------
         fig : plotly.Figure
             Plotly figure that can be customized.
@@ -137,14 +138,115 @@
         return fig
 
 
 def impeller_plot_function(impeller_object, attr):
     return ImpellerPlotFunction(impeller_object, attr)
 
 
+class CompareImpellerPlotFunction:
+    def __init__(self, impeller_object, attr):
+        self.impeller_object = impeller_object
+        self.attr = attr
+
+    @check_units
+    def __call__(
+        self, other_impeller, flow_v=None, speed=None, plot_kws=None, **kwargs
+    ):
+        """Plot parameter versus volumetric flow.
+
+        You can plot a specific point in the plot giving its flow_v and speed.
+
+        You can choose units with the arguments flow_v_units='...' and
+        {attr}_units='...'. For the speed you can use speed_units='...'.
+
+        Parameters
+        ----------
+        flow_v : pint.Quantity, float, optional
+            Volumetric flow (m³/s) for a specific point in the plot.
+        speed : pint.Quantity, float, optional
+            Speed (rad/s) for a specific point in the plot.
+        flow_v_units : str, optional
+            Flow units used for the plot. Default is m³/s.
+        {attr}_units : str, optional
+            Units for the parameter being plotted (e.g. for a head plot we could use
+            head_units='J/kg' or head_units='J/g'). Default is SI.
+        speed_units : str, optional
+            Speed units for the plot. Default is 'rad/s'.
+
+        Returns
+        -------
+        fig : plotly.Figure
+            Plotly figure that can be customized.
+
+        Examples
+        --------
+        >>> import ccp
+        >>> imp = ccp.impeller_example()
+        >>> fig = imp.plot_head(
+        ...    flow_v=5.5,
+        ...    speed=900,
+        ...    flow_v_units='m³/h',
+        ...    head_units='j/kg',
+        ...    speed_units='RPM'
+        ... )
+
+        """
+        impeller_object = self.impeller_object
+        attr = self.attr
+        fig = kwargs.pop("fig", None)
+
+        if fig is None:
+            fig = go.Figure()
+
+        if plot_kws is None:
+            plot_kws = {}
+
+        p0 = impeller_object.points[0]
+        flow_v_units = kwargs.get("flow_v_units", p0.flow_v.units)
+
+        for curve, color in zip(impeller_object.curves, tableau_colors):
+            other_curve = other_impeller.curve(speed=curve.speed)
+            fig = r_getattr(other_curve, attr + "_plot")(
+                fig=fig, plot_kws=plot_kws, **kwargs
+            )
+            # change line to dash
+            fig.data[-1].update(
+                line=dict(dash="dash", color=color),
+                showlegend=False,
+            )
+
+        for curve, color in zip(impeller_object.curves, tableau_colors):
+            fig = r_getattr(curve, attr + "_plot")(fig=fig, plot_kws=plot_kws, **kwargs)
+            fig.data[-1].update(line=dict(color=color))
+
+        if speed:
+            current_curve = impeller_object.curve(speed=speed)
+            fig = r_getattr(current_curve, attr + "_plot")(
+                fig=fig, plot_kws=plot_kws, **kwargs
+            )
+            if flow_v:
+                current_point = impeller_object.point(flow_v=flow_v, speed=speed)
+                fig = r_getattr(current_point, attr + "_plot")(
+                    fig=fig, plot_kws=plot_kws, **kwargs
+                )
+
+        # extra x range
+        flow_values = [p.flow_v.to(flow_v_units) for p in impeller_object.points]
+        min_flow = min(flow_values)
+        max_flow = max(flow_values)
+        delta = 0.05 * (max_flow - min_flow)
+        fig.update_layout(xaxis=dict(range=[min_flow - delta, max_flow + delta]))
+
+        return fig
+
+
+def compare_impeller_plot_function(impeller_object, attr):
+    return CompareImpellerPlotFunction(impeller_object, attr)
+
+
 class Impeller:
     """An impeller with a performance map.
 
     Impeller instance is initialized with the list of points.
     The created instance will hold the dimensional points used in instantiation.
     Curves will be generated from points close in similarity.
 
@@ -193,15 +295,18 @@
             if "." not in attr:
                 for c in self.curves:
                     param = r_getattr(c, attr)
                     values.append(param.magnitude)
                 units = param.units
                 r_setattr(self, attr, Q_(values, units))
 
-            r_setattr(self, attr + "_plot", impeller_plot_function(self, attr))
+            r_setattr(self, f"{attr}_plot", impeller_plot_function(self, attr))
+            r_setattr(
+                self, f"{attr}_compare", compare_impeller_plot_function(self, attr)
+            )
 
     def __getitem__(self, item):
         return self.points.__getitem__(item)
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             points_other = sorted(other.points, key=lambda x: x.flow_v)
@@ -229,14 +334,20 @@
 
         Returns
         -------
         point : ccp.Point
             Point in the performance map.
         """
 
+        # check if speed and flow are defined
+        if speed is None:
+            raise ValueError("Speed must be defined.")
+        if flow_v is None and flow_m is None:
+            raise ValueError("Either flow_v or flow_m must be defined.")
+
         current_curve = self.curve(speed)
         if flow_m:
             flow_v = current_curve.points[0].suc.v() * flow_m
 
         func_T = interp1d(
             current_curve.flow_v.m, current_curve.disch.T().m, fill_value="extrapolate"
         )
@@ -454,16 +565,16 @@
         cls,
         suc,
         head_curves=None,
         eff_curves=None,
         power_curves=None,
         pressure_ratio_curves=None,
         disch_T_curves=None,
-        b=None,
-        D=None,
+        b=Q_(0.005, "m"),
+        D=Q_(0.5, "m"),
         number_of_points=10,
         flow_units="m**3/s",
         flow_units_head=None,
         flow_units_eff=None,
         flow_units_power=None,
         flow_units_pressure_ratio=None,
         flow_units_disch_T=None,
@@ -496,17 +607,17 @@
         head_curves : dict
             Dict with head/flow values.
         eff_curves : dict
             Dict with eff/flow values.
         power_curves : dict
             Dict with power/flow values.
         b : float, pint.Quantity
-            Impeller width (m).
+            Impeller width at the outer blade diameter (m).
         D : float, pint.Quantity
-            Impeller diameter (m).
+            Impeller outer diameter (m).
         number_of_points : int
             Number of points that will be interpolated.
         flow_units : str
             Flow units used in the dict.
         flow_units_head: str
             Flow units used in the dict for head curves.
             Only needed when flow units for head curve differs from other curves.
@@ -699,16 +810,16 @@
 
     @classmethod
     def load_from_dict_isis(
         cls,
         suc,
         head_curves,
         eff_curves,
-        b=None,
-        D=None,
+        b=Q_(0.005, "m"),
+        D=Q_(0.5, "m"),
         number_of_points=10,
         flow_units="m**3/s",
         head_units="J/kg",
         speed_units="RPM",
     ):
         """Create points from dict object available in the ISIS platform.
 
@@ -731,17 +842,17 @@
         suc : ccp.State
             Suction state.
         head_curve : dict
             Dict with head/flow values.
         eff_curve : dict
             Dict with head/flow values.
         b : float, pint.Quantity
-            Impeller width (m).
+            Impeller width at the outer blade diameter (m).
         D : float, pint.Quantity
-            Impeller diameter (m).
+            Impeller outer diameter (m).
         number_of_points : int
             Number of points that will be interpolated.
         flow_units : str
             Flow units used in the dict.
         head_units : str
             Head units used in the dict.
             If the curve head units are in meter you can use: head_units="m*g0".
@@ -817,16 +928,16 @@
 
     @classmethod
     def load_from_engauge_csv(
         cls,
         suc,
         curve_name,
         curve_path,
-        b=None,
-        D=None,
+        b=Q_(0.005, "m"),
+        D=Q_(0.5, "m"),
         number_of_points=10,
         flow_units="m**3/s",
         flow_units_head=None,
         flow_units_eff=None,
         flow_units_power=None,
         flow_units_pressure_ratio=None,
         flow_units_disch_T=None,
@@ -840,80 +951,80 @@
         eff_interpolation_method="interp1d",
         power_interpolation_method="interp1d",
         pressure_ratio_interpolation_method="interp1d",
         disch_T_interpolation_method="interp1d",
     ):
         """Convert points from csv generated by engauge to csv with 6 points at same flow for use on hysys.
 
-         The csv files should be generated with engauge with the following procedure:
-         First, copy the image of the curve to your clipboard, then inside engauge digitizer:
-             - Edit -> Paste as new
-             - Name each curve with their respective speed value;
-             - On Axis Point -> add 3 reference points
-             - Select the curve (e.g. 10322 would be the curve for 10322 RPM)
-             - Select the points using the segment fill tool;
-             - Select the next curve and points...
-             - Settings -> Export Setup -> Select:
-             - Raws X's and Y's ; One curve on each line
-         Files should be saved with the following convention:
-             - <curve-name>-head.csv
-             - <curve-name>-eff.csv
-
-         suc : ccp.State
-             Suction state.
-         curve_path : pathlib.Path
-             Path to the curves.
-         curve_name : str
-             Name for head and efficiency curve.
-             Curves should have names <curve_name>-head.csv and <curve-name>-eff.csv.
-         b : float, pint.Quantity
-             Impeller width (m).
-         D : float, pint.Quantity
-             Impeller diameter (m).
-         number_of_points : int
-             Number of points that will be interpolated.
-         flow_units : str
-             Flow units used when extracting data with engauge.
-         flow_units_head: str
-             Flow units used when extracting data with engauge for head curves.
-             Only needed when flow units for head curve differs from other curves.
+        The csv files should be generated with engauge with the following procedure:
+        First, copy the image of the curve to your clipboard, then inside engauge digitizer:
+            - Edit -> Paste as new
+            - Name each curve with their respective speed value;
+            - On Axis Point -> add 3 reference points
+            - Select the curve (e.g. 10322 would be the curve for 10322 RPM)
+            - Select the points using the segment fill tool;
+            - Select the next curve and points...
+            - Settings -> Export Setup -> Select:
+            - Raws X's and Y's ; One curve on each line
+        Files should be saved with the following convention:
+            - <curve-name>-head.csv
+            - <curve-name>-eff.csv
+
+        suc : ccp.State
+            Suction state.
+        curve_path : pathlib.Path
+            Path to the curves.
+        curve_name : str
+            Name for head and efficiency curve.
+            Curves should have names <curve_name>-head.csv and <curve-name>-eff.csv.
+        b : float, pint.Quantity
+            Impeller width at the outer blade diameter (m).
+        D : float, pint.Quantity
+            Impeller outer diameter (m).
+        number_of_points : int
+            Number of points that will be interpolated.
+        flow_units : str
+            Flow units used when extracting data with engauge.
+        flow_units_head: str
+            Flow units used when extracting data with engauge for head curves.
+            Only needed when flow units for head curve differs from other curves.
         flow_units_eff: str
-             Flow units used when extracting data with engauge for efficiency curves.
-             Only needed when flow units for efficiency curve differs from other curves.
-         flow_units_power: str
-             Flow units used when extracting data with engauge for power curves.
-             Only needed when flow units for power curve differs from other curves.
-         flow_units_pressure_ratio: str
-             Flow units used when extracting data with engauge for pressure ratio curves.
-             Only needed when flow units for power curve differs from other curves.
-         flow_units_disch_T: str
-             Flow units used when extracting data with engauge for discharge temperature curves.
-             Only needed when flow units for efficiency curve differs from other curves.
-         head_units : str
-             Head units used when extracting data with engauge.
-             If the curve head units are in meter you can use: head_units="m*g0".
-         eff_units : str
-             Dimensionless.
-         power_units : str
-             Power units used when extracting data with engauge.
-         pressure_ratio_units : str
-             Pressure ratio units used when extracting data with engauge.
-         disch_T_units : str
-             Discharge temperature units used when extracting data with engauge.
-         speed_units : str
-             Speed units used when extracting data with engauge.
-         head_interpolation_method : str, optional
-             Interpolation method from scipy. Can be interp1d or UnivariateSpline.
-             Default is interp1d.
-         eff_interpolation_method : str, optional
-             Interpolation method from scipy. Can be interp1d or UnivariateSpline.
-             Default is interp1d.
-         power_inte![](../../AppData/Local/Temp/logo.png)rpolation_method : str, optional
-             Interpolation method from scipy. Can be interp1d or UnivariateSpline.
-             Default is interp1d.
+            Flow units used when extracting data with engauge for efficiency curves.
+            Only needed when flow units for efficiency curve differs from other curves.
+        flow_units_power: str
+            Flow units used when extracting data with engauge for power curves.
+            Only needed when flow units for power curve differs from other curves.
+        flow_units_pressure_ratio: str
+            Flow units used when extracting data with engauge for pressure ratio curves.
+            Only needed when flow units for power curve differs from other curves.
+        flow_units_disch_T: str
+            Flow units used when extracting data with engauge for discharge temperature curves.
+            Only needed when flow units for efficiency curve differs from other curves.
+        head_units : str
+            Head units used when extracting data with engauge.
+            If the curve head units are in meter you can use: head_units="m*g0".
+        eff_units : str
+            Dimensionless.
+        power_units : str
+            Power units used when extracting data with engauge.
+        pressure_ratio_units : str
+            Pressure ratio units used when extracting data with engauge.
+        disch_T_units : str
+            Discharge temperature units used when extracting data with engauge.
+        speed_units : str
+            Speed units used when extracting data with engauge.
+        head_interpolation_method : str, optional
+            Interpolation method from scipy. Can be interp1d or UnivariateSpline.
+            Default is interp1d.
+        eff_interpolation_method : str, optional
+            Interpolation method from scipy. Can be interp1d or UnivariateSpline.
+            Default is interp1d.
+        power_interpolation_method : str, optional
+            Interpolation method from scipy. Can be interp1d or UnivariateSpline.
+            Default is interp1d.
         """
         curves_path_dict = {}
 
         for param in ["head", "eff", "power", "pressure_ratio", "disch_T"]:
             param_path = curve_path / (curve_name + f"-{param}.csv")
             if param_path.is_file():
                 curves_path_dict[f"{param}_curves"] = read_data_from_engauge_csv(
@@ -1003,15 +1114,17 @@
             "head": "kJ/kg",
             "eff": "percent",
         }
         curves_dict = {}
         for curve in self.curves:
             curves_dict[round(curve.speed.to("RPM").m)] = {
                 "flow": getattr(curve, "flow_v").m,
-                f"{parameter}": getattr(curve, parameter).to(parameters_units[parameter]).m,
+                f"{parameter}": getattr(curve, parameter)
+                .to(parameters_units[parameter])
+                .m,
             }
 
         with open(file, mode="w", newline="") as f:
             for idx, (key, values) in enumerate(curves_dict.items(), start=1):
                 f.write(f"curva{idx} {key}\n")
                 for flow, param in zip(values["flow"], values[parameter]):
                     f.write(f"{flow:.5f} {param:.5f}\n")
```

### Comparing `ccp-performance-0.3.3/ccp/plotly_theme.py` & `ccp-performance-0.3.4/ccp/plotly_theme.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/point.py` & `ccp-performance-0.3.4/ccp/point.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,18 @@
         Suction state, polytropic head and polytropic efficiency.
     suc, head, power : ccp.State, pint.Quantity or float, pint.Quantity or float
         Suction state, polytropic head (J/kg) and gas power (Watt).
     suc, eff, volume_ratio : ccp.State, float, float
         Suction state, polytropic efficiency and volume ratio.
     suc, pres_ratio, disch_T : ccp.State, float, pint.Quantity or float
         Suction state, pressure ration and discharge temperature.
-    b : pint.Quantity, optional
-        Impeller width (m).
-        This value is used to calculate the machine Mach and Reynolds numbers.
-    D : pint.Quantity, optional
-        Impeller diameter (m).
-        This value is used to calculate the machine Mach and Reynolds numbers.
+    b : float, pint.Quantity
+        Impeller width at the outer blade diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     surface_roughness : pint.Quantity, optional
         Gas passage mean surface roughness (m).
         Used in the reynolds correction calculation.
         Default value is 3.048e-6 m.
     casing_area : pint.Quantity, optional
         Compressor case area used to calculate case heat loss (m²).
     casing_temperature : pint.Quantity, optional
@@ -89,18 +87,18 @@
         Power (Watt).
     phi : pint.Quantity
         Volume flow coefficient (dimensionless).
     psi : pint.Quantity
         Polytropic head coefficient (dimensionless).
     volume_ratio : pint.Quantity
         Volume ratio - suc.v() / disch.v() (dimensionless).
-    b : pint.Quantity
-        Impeller width (m).
-    D : pint.Quantity
-        Impeller diameter (m).
+    b : float, pint.Quantity
+        Impeller width at the outer blade diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     casing_area : pint.Quantity
         Compressor case area used to calculate case heat loss (m²).
     casing_temperature : pint.Quantity
         Compressor case temperature used to calculate case heat loss (degK).
     ambient_temperature : pint.Quantity
         Ambient temperature used to calculate case heat loss (degK).
     convection_constant : pint.Quantity
@@ -1703,16 +1701,16 @@
 
 @check_units
 def u_calc(D, speed):
     """Calculate the impeller tip speed.
 
     Parameters
     ----------
-    D : pint.Quantity, float
-        Impeller diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     speed : pint.Quantity, float
         Impeller speed (rad/s).
 
     Returns
     -------
     u_calc : pint.Quantity
         Impeller tip speed (m/s).
@@ -1727,16 +1725,16 @@
 
     Parameters
     ----------
     head : pint.Quantity, float
         Polytropic head (J/kg).
     speed : pint.Quantity, float
         Impeller speed (rad/s).
-    D : pint.Quantity, float
-        Impeller diameter.
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
 
     Returns
     -------
     psi : pint.Quantity
         Polytropic head coefficient (dimensionless).
     """
     u = u_calc(D, speed)
@@ -1767,16 +1765,16 @@
 
 @check_units
 def speed_from_psi(D, head, psi):
     """Calculate speed from non dimensional psi.
 
     Parameters
     ----------
-    D : pint.Quantity, float
-        Impeller diameter.
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     head : pint.Quantity, float
         Polytropic head.
     psi : pint.Quantity, float
         Head coefficient.
 
     Returns
     -------
@@ -1788,15 +1786,30 @@
     speed = 2 * u / D
 
     return speed.to("rad/s")
 
 
 @check_units
 def phi(flow_v, speed, D):
-    """Flow coefficient."""
+    """Flow coefficient.
+
+    Parameters
+    ----------
+    flow_v : float, pint.Quantity
+        Impeller flow (m³/s).
+    speed : float, pint.Quantity
+        Impeller speed (rad/s).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
+
+    Returns
+    -------
+    phi : pint.Quantity
+        Flow coefficient (dimensionless).
+    """
     u = u_calc(D, speed)
 
     phi = flow_v * 4 / (np.pi * D**2 * u)
 
     return phi.to("dimensionless")
 
 
@@ -1806,30 +1819,41 @@
 
     Eq. 5.13 from :cite:`ludtke2004process`
 
     Parameters
     ----------
     flow_v : float, pint.Quantity
         Impeller exit flow (m³/s).
+    speed : float, pint.Quantity
+        Impeller speed (rad/s).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
+    b : float, pint.Quantity
+        Impeller width at the outer blade diameter (m).
+
+    Returns
+    -------
+    phi : pint.Quantity
+        Discharge flow coefficient (dimensionless).
     """
     u = u_calc(D, speed)
 
     phi = flow_v / (np.pi * D * b * u)
 
     return phi.to("dimensionless")
 
 
 @check_units
 def flow_from_phi(D, phi, speed):
     """Calculate flow from non dimensional phi.
 
     Parameters
     ----------
-    D : pint.Quantity, float
-        Impeller diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     phi : pint.Quantity, float
         Flow coefficient (m³/s).
     speed : pint.Quantity, float
         Speed (rad/s).
 
     Returns
     -------
@@ -1844,16 +1868,16 @@
 
 
 def head_from_psi(D, psi, speed):
     """Calculate head from non dimensional psi.
 
     Parameters
     ----------
-    D : pint.Quantity, float
-        Impeller diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
     psi : pint.Quantity, float
         Head coefficient.
     speed : pint.Quantity, float
         Speed (rad/s).
 
     Returns
     -------
@@ -1944,18 +1968,18 @@
 
     Parameters
     ----------
     suc : ccp.State
         Suction state.
     speed : pint.Quantity, float
         Impeller speed (rad/s).
-    b : pint.Quantity, float
-        Impeller width (m).
-    D : pint.Quantity, float
-        Impeller diameter (m).
+    b : float, pint.Quantity
+        Impeller width at the outer blade diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
 
     Returns
     -------
     reynolds : pint.Quantity
         Reynolds number (dimensionless).
     """
     u = u_calc(D, speed)
@@ -1970,16 +1994,16 @@
 
     Parameters
     ----------
     suc : ccp.State
         Suction state.
     speed : pint.Quantity, float
         Impeller speed (rad/s).
-    D : pint.Quantity, float
-        Impeller diameter (m).
+    D : float, pint.Quantity
+        Impeller outer diameter (m).
 
     Returns
     -------
     mach : pint.Quantity
         Mach number (dimensionless).
     """
     u = u_calc(D, speed)
```

### Comparing `ccp-performance-0.3.3/ccp/similarity.py` & `ccp-performance-0.3.4/ccp/similarity.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/state.py` & `ccp-performance-0.3.4/ccp/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,14 +662,21 @@
             args_dict = {}
             for k in args:
                 args_dict[k] = locals()[k]
             raise ValueError(
                 f"Could not define state with {args_dict} and {self.fluid}"
             ) from e
 
+    def get_coolprop_state(self):
+        """Return a CoolProp state object."""
+        EOS = self.EOS
+        if EOS is None:
+            EOS = ccp.config.EOS
+        return CP.AbstractState(EOS, self._fluid)
+
     def plot_envelope(
         self, T_units="degK", p_units="Pa", dew_point_margin=20, fig=None, **kwargs
     ):
         """Plot phase envelope.
 
         Plots the phase envelope and dew point limit.
```

### Comparing `ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.3.4/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.3.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.3.4/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.3.4/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.3.4/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp/tests/data/normal-head.csv` & `ccp-performance-0.3.4/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.3/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.3.4/ccp_performance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.3
+Version: 0.3.4
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
```

### Comparing `ccp-performance-0.3.3/setup.py` & `ccp-performance-0.3.4/setup.py`

 * *Files identical despite different names*

