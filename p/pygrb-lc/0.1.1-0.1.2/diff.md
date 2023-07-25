# Comparing `tmp/pygrb_lc-0.1.1.tar.gz` & `tmp/pygrb_lc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.1.1.tar", last modified: Fri Jul  7 16:48:05 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.2.tar", last modified: Tue Jul 25 20:26:50 2023, max compression
```

## Comparing `pygrb_lc-0.1.1.tar` & `pygrb_lc-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.461765 pygrb_lc-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 16:48:05.000000 pygrb_lc-0.1.1/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:05.465765 pygrb_lc-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 16:47:56.000000 pygrb_lc-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.494186 pygrb_lc-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_utils.py
```

### Comparing `pygrb_lc-0.1.1/LICENSE` & `pygrb_lc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/PKG-INFO` & `pygrb_lc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb_lc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.1/README.md` & `pygrb_lc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/setup.cfg` & `pygrb_lc-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.1.1
+version = 0.1.2
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.2/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/catalogs.py` & `pygrb_lc-0.1.2/src/pygrb_lc/catalogs.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/config.py` & `pygrb_lc-0.1.2/src/pygrb_lc/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 if not os.path.exists(IMAGE_PATH):
     os.makedirs(IMAGE_PATH)
 
 LIGHT_CURVE_SAVE = f'{ROOT_PATH}light_curves/'
 if not os.path.exists(LIGHT_CURVE_SAVE):
     os.makedirs(LIGHT_CURVE_SAVE)
 
-ACS_DATA_PATH = 'E:/ACS/'
-
 DATA_PATH = f'{ROOT_PATH}data/'
 if not os.path.exists(DATA_PATH):
     os.makedirs(DATA_PATH)
 
 LOGS_PATH = f'{ROOT_PATH}logs/'
 if not os.path.exists(LOGS_PATH):
     os.makedirs(LOGS_PATH)
```

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.2/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.2/src/pygrb_lc/furie.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,20 +54,20 @@
         flux.append(np.mean(ps[mask1]) if len(ps[mask1])!=0 else 0)
         flux_err.append(chi2.ppf(0.67, 2*len(ps[mask1]))/len(ps[mask1]) if len(ps[mask1]) != 0 else 1)
     
     return np.array(time), np.array(time_err), np.array(flux), np.array(flux_err)
 
 class FurieLightCurve():
     def __init__(self, light_curve: LightCurve, 
-                       interval_t90: Iterable | None = None,
+                       interval_t90: Iterable = None,
                        bkg_substraction_resolution: float = 10,
                        bkg_polynom_degree: int = 3,
-                       bkg_intervals: Iterable | None = None,
-                       pad_size: int | None  = None,
-                       window: Callable | None = None
+                       bkg_intervals: Iterable = None,
+                       pad_size: int = None,
+                       window: Callable = None
                        ):
 
         '''
         Args:
             light_curve (LightCurve): light curve object
             interval_t90 (tuple, optional): time interval for t90. If None, uses 2 and 3 quartile of time
             bkg_substraction_resolution (float, optional): background substraction resolution, defaults to 10
@@ -85,15 +85,17 @@
                          (interval_t90[1],self.light_curve.times[-1]+self.light_curve.resolution)]
         else:
             bkg_intervals = bkg_intervals
         
         self.bkg_intervals = bkg_intervals
         self.interval_t90 = interval_t90
 
-        rebined_param = np.polyfit(self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).times,self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).signal,bkg_polynom_degree)
+        rebined_param = np.polyfit(self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).times,
+                                   self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).signal,
+                                   bkg_polynom_degree)
         rebined_param = rebined_param * (self.light_curve.original_resolution/self.light_curve.resolution)
         self.rebined_param = rebined_param
         self.N = np.sum(self.light_curve.rebin().set_intervals(*bkg_intervals).signal)
 
         signal = self.light_curve.rebin().substract_polynom(rebined_param).set_intervals(interval_t90).signal
```

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.2/src/pygrb_lc/light_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import requests
 import pandas as pd
 import datetime
 import numpy as np
-from .config import LIGHT_CURVE_SAVE, GBM_DETECTOR_CODES, logging, GBM_DETECTORS
+from .config import LIGHT_CURVE_SAVE, logging, GBM_DETECTORS
 from astropy.io import fits
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 from .time import change_fermi_seconds, change_utc
 from .utils import get_first_intersection, is_iterable, retry
 import pickle
-from .config import ACS_DATA_PATH
 
 logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
 
 class LightCurve():
     '''
     Base class for light curves from different sources
     '''
-    def __init__(self, event_time: str = None,duration: float = None, data: np.array = None):
+    def __init__(self, event_time: str = None, duration: float = None, data: np.array = None):
         '''
         Args:
             event_time (str, optional): time of the event in format 'YYYY-MM-DD HH:MM:SS'
             duration (int, optional): duration in seconds
             data (np.array, optional): data of the light curve, having 2 or 4 columns (time, time_err, signal, signal_err) in seconds.
         '''
         self.event_time = event_time
@@ -40,17 +39,17 @@
             self.original_times,self.original_signal = None, None
             self.original_resolution = None
 
     def __repr__(self):
         return f'{self.__class__.__name__}(event_time={self.event_time}, duration={self.duration}, original resolution={self.original_resolution})'
 
     def __eq__(self, other: object):
-        return isinstance(other, LightCurve) and self.__class__ == other.__class__ and self.event_time == other.event_time and self.duration == other.duration and self.original_resolution == other.original_resolution
+        return self.__class__ == other.__class__ and self.event_time == other.event_time and self.duration == other.duration and self.original_resolution == other.original_resolution
 
-    def plot(self,kind: str = 'plot',
+    def plot(self, kind: str = 'plot',
              logx: bool = None,
              logy: bool = None, 
              ax: mpl.axes.Axes = None, 
              **kwargs):
         '''
         Plot the light curve
         Args:
@@ -274,43 +273,44 @@
     Class for light curves from SPI-ACS/INTEGRAL
     '''
     def __init__(self, 
                  event_time: str,
                  duration: int, 
                  loading_method: str = 'web',
                  scale: str = 'utc',
+                 acs_path = 'E:/ACS/',
                  **kwargs):
         '''
         Args:
             event_time (str): date and time of event in ISO 8601 format
             duration (int): duration of light curve in seconds
             loading_method (str, optional): 'local' or 'web'
             scale (str, optional): 'utc' or 'ijd'
         '''
-        super().__init__(event_time,duration,**kwargs)
+        super().__init__(event_time, duration, **kwargs)
         self.event_time = self.event_time[:10] + ' ' + self.event_time[11:19]
         
         if self.original_times is None:
             if loading_method == 'local':
-                self.original_times,self.original_signal = self.__get_light_curve_from_file(scale = scale)
+                self.original_times,self.original_signal = self.__get_light_curve_from_file(scale = scale, acs_path = acs_path)
             elif loading_method =='web':
                 self.original_times,self.original_signal = self.__get_light_curve_from_web(scale = scale)
             else:
                 raise NotImplementedError(f'Loading method {loading_method} not supported')
 
             self.original_resolution = round(np.mean(self.original_times[1:] - self.original_times[:-1]), 3) # determine size of time window
             self._reset_light_curve()
 
-    def __get_light_curve_from_file(self,scale = 'utc'):
+    def __get_light_curve_from_file(self,scale = 'utc', acs_path = 'E:/ACS/'):
         '''
         Load a light curve from raw scw files
         Args:
             scale (str, optional): scale of light curve, 'utc' (seconds from trigger) or 'ijd' (days from J2000)
         '''
-        with open(f'{ACS_DATA_PATH}swg_infoc.dat','r') as f:
+        with open(f'{acs_path}swg_infoc.dat','r') as f:
             acs_scw_df = [line.split() for line in f]
 
         acs_scw_df = pd.DataFrame(acs_scw_df,columns=['scw_id','obt_start','obt_finish','ijd_start','ijd_finish','scw_duration','x','y','z','ra','dec'])
         acs_scw_df['scw_id'] = acs_scw_df['scw_id'].astype(str)
         acs_scw_df['ijd_start'] = acs_scw_df['ijd_start'].astype(float)
         acs_scw_df['ijd_finish'] = acs_scw_df['ijd_finish'].astype(float)
 
@@ -321,15 +321,15 @@
         if scw_needed.shape[0]==0:
             raise ValueError(f'No data found for {self.event_time}')
 
         current_data = []
         for _,row in scw_needed.iterrows():
             for i in range(5):
                 try:
-                    with open(f'{ACS_DATA_PATH}0.05s/{row["scw_id"][:4]}/{row["scw_id"]}.00{i}.dat','r') as f:
+                    with open(f'{acs_path}0.05s/{row["scw_id"][:4]}/{row["scw_id"]}.00{i}.dat','r') as f:
                         for line in f:
                             line = line.split()
                             if float(line[0]) > 0:
                                 current_data.append([row['ijd_start']+float(line[0])/(24*60*60),float(line[2])])
                     break
                 except FileNotFoundError:
                     continue
```

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/time.py` & `pygrb_lc-0.1.2/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.2/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.1/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.2/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.1/tests/test_utils.py` & `pygrb_lc-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

