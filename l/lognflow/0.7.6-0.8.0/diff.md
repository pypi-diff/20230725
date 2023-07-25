# Comparing `tmp/lognflow-0.7.6.tar.gz` & `tmp/lognflow-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.6.tar", last modified: Mon Jul 17 02:29:51 2023, max compression
+gzip compressed data, was "lognflow-0.8.0.tar", last modified: Tue Jul 25 12:09:07 2023, max compression
```

## Comparing `lognflow-0.7.6.tar` & `lognflow-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 02:29:40.000000 lognflow-0.7.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-17 02:29:40.000000 lognflow-0.7.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-17 02:29:40.000000 lognflow-0.7.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 02:29:40.000000 lognflow-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-17 02:29:40.000000 lognflow-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-17 02:29:51.787692 lognflow-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-17 02:29:40.000000 lognflow-0.7.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.783692 lognflow-0.7.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 02:29:40.000000 lognflow-0.7.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.783692 lognflow-0.7.6/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67409 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-17 02:29:40.000000 lognflow-0.7.6/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 02:29:51.000000 lognflow-0.7.6/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-17 02:29:51.787692 lognflow-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-17 02:29:40.000000 lognflow-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:29:51.787692 lognflow-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-17 02:29:40.000000 lognflow-0.7.6/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 12:08:55.000000 lognflow-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-25 12:08:55.000000 lognflow-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-25 12:08:55.000000 lognflow-0.8.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 12:08:55.000000 lognflow-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-25 12:08:55.000000 lognflow-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 12:09:07.586255 lognflow-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-25 12:08:55.000000 lognflow-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64082 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 12:09:07.586255 lognflow-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-25 12:08:55.000000 lognflow-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.6/CONTRIBUTING.rst` & `lognflow-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/HISTORY.rst` & `lognflow-0.8.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -111,8 +111,15 @@
 * Added complex numbers to log_imshow
 
 0.7.6 (2023-07-17)
 ------------------
 * printprogress can handle up to 99 days
 * log_text takes any save_as
 * If variable name has escape key is alright
-* If variable name is splitable, we replace them with _
+* If variable name is splitable, we replace them with _
+
+0.8.0 (2023-07-25)
+------------------
+* logger.save and savez are set to be identical to log_single.
+* logged.load is set to be identical to get_single.
+* utils.py is added to contain all misc functions.
+* replace_all added to utils
```

### Comparing `lognflow-0.7.6/LICENSE` & `lognflow-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/PKG-INFO` & `lognflow-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.6
+Version: 0.8.0
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -205,7 +205,14 @@
 
 0.7.6 (2023-07-17)
 ------------------
 * printprogress can handle up to 99 days
 * log_text takes any save_as
 * If variable name has escape key is alright
 * If variable name is splitable, we replace them with _
+
+0.8.0 (2023-07-25)
+------------------
+* logger.save and savez are set to be identical to log_single.
+* logged.load is set to be identical to get_single.
+* utils.py is added to contain all misc functions.
+* replace_all added to utils
```

### Comparing `lognflow-0.7.6/README.rst` & `lognflow-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/docs/Makefile` & `lognflow-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/docs/conf.py` & `lognflow-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/docs/installation.rst` & `lognflow-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/docs/make.bat` & `lognflow-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.6/lognflow/lognflow.py` & `lognflow-0.8.0/lognflow/lognflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,16 @@
 
 """
 
 import pathlib
 import time
 import itertools
 from   dataclasses import dataclass
-from re import sub as re_sub
-from unicodedata import normalize as unicodedata_normalize
-from   os import sep as os_sep
 import numpy as np
+
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from   matplotlib import animation
 
 from .logviewer import logviewer
 
 @dataclass
@@ -64,41 +62,15 @@
     to_be_logged        : str   
     log_fpath           : pathlib.Path         
     log_size_limit      : int 
     log_size            : int     
     last_log_flush_time : float
     log_flush_period    : int
 
-def repr_raw(text):
-    """Returns a raw string representation of a text with escape charachters"""
-    escape_dict={'\a':r'\a',
-                 '\b':r'\b',
-                 '\c':r'\c',
-                 '\f':r'\f',
-                 '\n':r'\n',
-                 '\r':r'\r',
-                 '\t':r'\t',
-                 '\v':r'\v',
-                 '\'':r'\'',
-                 '\"':r'\"'}
-    new_string=''
-    for char in text:
-        try: 
-            new_string += escape_dict[char]
-        except KeyError: 
-            new_string += char
-    return new_string
-
-def replace_all(text, pattern, fill_value):
-    while (len(text.split(pattern)) > 1):
-        text = text.replace(pattern, fill_value)
-    return text
-
-if __name__ == '__main__':
-    name = 'asdfkyt sdyufg%^&*()'
+from .utils import repr_raw, replace_all
 
 class lognflow:
     """Initialization
         
         lognflow creates a directory/attribute called log_dir and puts all 
         stored data in there, if logs_root is given. Otherwise give it log_dir
         to use. If you type
@@ -210,15 +182,20 @@
         self._print_text = print_text
         self._loggers_dict = {}
         self._vars_dict = {}
         self._single_var_call_cnt = 0
 
         self.log_name = main_log_name
         self.log_flush_period = log_flush_period
+        self.save = self.log_single
     
+    def savez(self, *args, **kwargs):
+        kwargs['save_as'] = 'npz'
+        return self.save(*args, **kwargs)
+        
     @property
     def time_stamp(self):
         """ Current time stamp
             Gives the time after the start of the lognflow
         """
         return time.time() - self._init_time
     
@@ -374,15 +351,15 @@
                  print_text = None,
                  log_size_limit: int = int(1e+7),
                  time_tag: bool = None,
                  log_flush_period: int = None,
                  flush = False,
                  end = '\n',
                  new_file = False,
-                 save_as = 'txt'):
+                 save_as = None):
         """ log a string into a text file
             You can shose a name for the log and give the text to put in it.
             Also you can pass a small numpy array. You can ask it to put time
             stamp in the log and in the log file name, you can disable
             printing the text. You can set the log size limit to split it into
             another file with a new time stamp.
             
@@ -415,23 +392,32 @@
                    it closees the current text file and overwrites on it.
             :param save_as: str
                    save_as is the suffix of the text file.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
+        
         log_name = self.log_name if (log_name is None) else log_name
 
+        if(save_as is None):
+            log_name_split = log_name.split('.')
+            if len(log_name_split) > 1:
+                save_as = log_name_split[-1]
+                log_name = '.'.join(log_name_split)
+        else:
+            save_as = 'txt'
+
         if((print_text is None) | (print_text is True)):
             print_text = self._print_text
         if(print_text):
             if(log_time_stamp):
                 print(f'T:{self.time_stamp:>6.6f}| ', end='')
             print(to_be_logged, end = end)
-                
+        
         if ( (not (log_name in self._loggers_dict)) or new_file):
             self._log_text_handler(log_name, 
                                    log_size_limit = log_size_limit,
                                    time_tag = time_tag,
                                    save_as = save_as)
 
         curr_textinlog = self._loggers_dict[log_name]
@@ -468,15 +454,15 @@
                         
 
     def _get_log_counter_limit(self, param, log_size_limit):
         cnt_limit = int(log_size_limit/(param.size*param.itemsize))
         return cnt_limit
 
     def log_var(self, parameter_name: str, parameter_value, 
-                save_as='npz', log_size_limit: int = int(1e+7)):
+                save_as = None, log_size_limit: int = int(1e+7)):
         """log a numpy array in buffer then dump
             It can be the case that we need to take snapshots of a numpy array
             over time. The size of the array would not change and this is hoing
             to happen frequently.
             This log_ver makes a buffer in RAM and keeps many instances of the
             array along with their time stamp and then when the size of the 
             array reaches a threhshold flushes it into HDD with a file that
@@ -498,14 +484,22 @@
                     
         """
         try:
             _ = parameter_value.shape
         except:
             parameter_value = np.array([parameter_value])
         
+        if(save_as is None):
+            parameter_name_split = parameter_name.split('.')
+            if len(parameter_name_split) > 1:
+                save_as = parameter_name_split[-1]
+                parameter_name = '.'.join(parameter_name_split)
+        else:
+            save_as = 'npz'
+        
         log_counter_limit = self._get_log_counter_limit(\
             parameter_value, log_size_limit)
 
         if(parameter_name in self._vars_dict):
             _var = self._vars_dict[parameter_name]
             data_array, time_array, curr_index, \
                 file_start_time, save_as, log_counter_limit = \
@@ -559,25 +553,28 @@
                     path like name such as myscript/myvar.
         """
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         
         _var = self._vars_dict[parameter_name]
         _var_data_array = _var.data_array[_var.time_array > 0]
         _var_time_array = _var.time_array[_var.time_array > 0]
-        if(_var.save_as == 'npz'):
+        if((_var.save_as == 'npz')):# | (_var.save_as == 'npy')):
             fpath = param_dir / f'{param_name}_{_var.file_start_time}.npz'
             np.savez(fpath,
                 time_array = _var_time_array,
                 data_array = _var_data_array)
-        elif(_var.save_as == 'txt'):
+        else:#if(_var.save_as == 'txt'):
             fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_time_array)
             fpath = param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_data_array)
-        return fpath
+        try:
+            return fpath
+        except:
+            print('here')
     
     def get_var(self, parameter_name: str) -> tuple:
         """ Get the buffered numpy arrays
             If you need the buffered variable back.
             :param parameter_name: str
                 examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
@@ -608,33 +605,42 @@
             function.
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param parameter_value: np.array
-                    An np array whose size doesn't change
+                    Could be anything and np.save will be used. If it is a
+                    dictionary, np.savez will be used. As you may know, np.save
+                    can save all pickalables.
             :param save_as: str
                     can be 'npz', 'npy', 'mat', 'torch' for pytorch models
                     or 'txt' or anything else which will save it as text.
                     This includes 'json', 'pdb', or ...
             :param mat_field: str
                     when saving as 'mat' file, the field can be set.
                     otherwise it will be the parameter_name
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
-            
+
         if(save_as is None):
-            if isinstance(parameter_value, (np.ndarray, int, float)):
+            parameter_name_split = parameter_name.split('.')
+            if len(parameter_name_split) > 1:
+                save_as = parameter_name_split[-1]
+                #YOU CAN CHECK IF IT IS LEGITEMATE EXTENSION
+                parameter_name = '.'.join(parameter_name_split)
+            elif isinstance(parameter_value, (np.ndarray, int, float)):
                 save_as = 'npy'
-            if (isinstance(parameter_value, dict)):
+            elif (isinstance(parameter_value, dict)):
                 save_as = 'npz'
+            else:
+                save_as = 'txt'
         save_as = save_as.strip()
         save_as = save_as.strip('.')
 
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
         
         try:
@@ -712,14 +718,15 @@
         parameter_value: np.ndarray,
         frame_shape = None,
         image_format='jpeg', 
         dpi=1200, 
         time_tag: bool = None,
         add_colorbar = False,
         remove_axis_ticks = True,
+        return_figure = False,
         **kwargs):
         """log multiple images as a tiled square
             The image is logged using plt.imshow
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
@@ -737,26 +744,29 @@
         n_r, n_c, n_ch = parameter_value.shape
         
         if(frame_shape is None):
             n_ch_sq = int(np.ceil(n_ch ** 0.5))
             n_ch_r, n_ch_c = (n_ch_sq, n_ch_sq)
         else:
             n_ch_r, n_ch_c = frame_shape
-        _, ax = plt.subplots(n_ch_r,n_ch_c)
+        fig, ax = plt.subplots(n_ch_r,n_ch_c)
         if(remove_axis_ticks):
             plt.setp(ax, xticks=[], yticks=[])
         for rcnt in range(n_ch_r):
             for ccnt in range(n_ch_c):
                 im = parameter_value[:,:, ccnt + rcnt * n_ch_c]
                 im_ch = ax[rcnt, ccnt].imshow(im, **kwargs)
                 if(add_colorbar):
                     self.add_colorbar(im_ch)
-        return self.log_plt(parameter_name = parameter_name,
-                     image_format=image_format, dpi=dpi,
-                     time_tag = time_tag)
+        if not return_figure:
+            return self.log_plt(parameter_name = parameter_name,
+                         image_format=image_format, dpi=dpi,
+                         time_tag = time_tag)
+        else:
+            return fig
             
     def log_plot(self, parameter_name: str, 
                        parameter_value_list,
                        x_values = None,
                        image_format='jpeg', dpi=1200,
                        time_tag: bool = None,
                        **kwargs):
@@ -868,15 +878,15 @@
         except:
             self.log_text(self.log_name,
                 f'Cannot make the histogram for variable {parameter_name}.')
             return None
     
     def log_scatter3(self, parameter_name: str,
                        parameter_value, image_format='jpeg', dpi=1200,
-                       time_tag: bool = None):
+                       time_tag: bool = None, return_figure = False):
         """log a single scatter in 3D
             Scatter plotting in 3D
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
@@ -884,33 +894,30 @@
                     An np array of size 3 x n, to sctter n data points in 3D
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        try:
-            fig = plt.figure()
-            ax = fig.add_subplot(111, projection='3d')
-            ax.scatter(parameter_value[0], 
-                       parameter_value[1], 
-                       parameter_value[2])
-            fpath = self.log_plt(
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        ax.scatter(parameter_value[0], 
+                   parameter_value[1], 
+                   parameter_value[2])
+        if not return_figure:
+            return self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
-            return fpath
-        except:
-            self.log_text(self.log_name,
-                f'Cannot make the scatter3 for variable {parameter_name}.')
-            return None
+        else:
+            return fig
     
     def log_surface(self, parameter_name: str,
                        parameter_value, image_format='jpeg', dpi=1200,
-                       time_tag: bool = None, **kwargs):
+                       time_tag: bool = None, return_figure = False, **kwargs):
         """log a surface in 3D
             surface plotting in 3D exactly similar to imshow but in 3D
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
@@ -918,31 +925,29 @@
                     An np array of size n x m, to plot surface in 3D
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
             rest of the parameters (**kwargs) will be passed to plot_surface() 
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        try:
-            # from mpl_toolkits.mplot3d import Axes3D
-            n_r, n_c = parameter_value.shape
-            fig = plt.figure()
-            ax = fig.add_subplot(111, projection='3d')
-            X, Y = np.meshgrid(np.arange(n_r, dtype='int'), 
-                               np.arange(n_c, dtype='int'))
-            ax.plot_surface(X, Y, parameter_value, **kwargs)
+        from mpl_toolkits.mplot3d import Axes3D
+        n_r, n_c = parameter_value.shape
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        X, Y = np.meshgrid(np.arange(n_r, dtype='int'), 
+                           np.arange(n_c, dtype='int'))
+        ax.plot_surface(X, Y, parameter_value, **kwargs)
+        if not return_figure:
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
             return fpath
-        except:
-            self.log_text(self.log_name,
-                f'Cannot make the surface plot for variable {parameter_name}.')
-            return None
+        else:
+            return fig
         
     def log_hexbin(self, parameter_name: str, parameter_value,
                    gridsize = 20, image_format='jpeg', dpi=1200,
                    time_tag: bool = None):
         """log a 2D histogram 
             The 2D histogram is made out of hexagonals
             
@@ -1058,80 +1063,16 @@
             self.log_text(
                 self.log_name,
                 f'Cannot plot variable {parameter_name} with shape' + \
                 f'{parameter_value.shape}')
             return
 
     def multichannel_to_square(self, stack, borders = 0):
-        """ turn a stack of multi-channel images into stack of square images
-            This is very useful when lots of images need to be tiled
-            against each other.
-        
-            :param stack: np.ndarray
-                    It must have the shape of either
-                    n_r x n_c x n_ch
-                    n_r x n_c x  3  x n_ch
-                    n_f x n_r x n_c x n_ch
-                    n_f x n_r x n_c x  3  x n_ch
-                    
-                In both cases n_ch will be turned into a square tile
-                Remember if you have N images to put into a square, the input
-                shape should be 1 x n_r x n_c x N
-            :param borders: literal or np.inf or np.nan
-                When plotting images with matplotlib.pyplot.imshow, there
-                needs to be a border between them. This is the value for the 
-                border elements.
-                
-            output
-            ---------
-                Since we have N channels to be laid into a square, the side
-                length woul be ceil(N**0.5)
-                it produces an np.array of shape n_f x n_r * S x n_c * S or
-                n_f x n_r * S x n_c * S x 3 in case of RGB input.
-        """
-        if(len(stack.shape) == 4):
-            if(stack.shape[3] == 3):
-                stack = np.array([stack])
-        if(len(stack.shape) == 3):
-            stack = np.array([stack])
-        
-        if((len(stack.shape) == 4) | (len(stack.shape) == 5)):
-            if(len(stack.shape) == 4):
-                n_imgs, n_R, n_C, n_ch = stack.shape
-            if(len(stack.shape) == 5):
-                n_imgs, n_R, n_C, is_rgb, n_ch = stack.shape
-                if(is_rgb != 3):
-                    return None
-            square_side = int(np.ceil(np.sqrt(n_ch)))
-            new_n_R = n_R * square_side
-            new_n_C = n_C * square_side
-            if(len(stack.shape) == 4):
-                canv = np.zeros((n_imgs, new_n_R, new_n_C), 
-                                dtype = stack.dtype)
-            if(len(stack.shape) == 5):
-                canv = np.zeros((n_imgs, new_n_R, new_n_C, 3),
-                                 dtype = stack.dtype)
-            used_ch_cnt = 0
-            if(borders is not None):
-                stack[:,   :1      ] = borders
-                stack[:,   : ,   :1] = borders
-                stack[:, -1:       ] = borders
-                stack[:,   : , -1: ] = borders
-            
-            for rcnt in range(square_side):
-                for ccnt in range(square_side):
-                    ch_cnt = rcnt + square_side*ccnt
-                    if (ch_cnt<n_ch):
-                        canv[:, rcnt*n_R: (rcnt + 1)*n_R,
-                                ccnt*n_C: (ccnt + 1)*n_C] = \
-                            stack[..., used_ch_cnt]
-                        used_ch_cnt += 1
-        else:
-            return None
-        return canv
+        return self.multichannel_to_frame(stack, 
+                              frame_shape = None, borders = borders)
 
     def multichannel_to_frame(self, stack, 
                               frame_shape : tuple = None, borders = 0):
         """ turn a stack of multi-channel images into a frame of images
             This is very useful when lots of images need to be tiled
             against each other.
         
@@ -1559,31 +1500,7 @@
             pass
         
     def __repr__(self):
         return f'{self.log_dir}'
 
     def __bool__(self):
         return self.log_dir.is_dir()
-
-def select_directory(default_directory = './'):
-    """ Open dialog to select a directory
-        It works for windows and Linux using PyQt5.
-    
-       :param default_directory: pathlib.Path
-                When dialog opens, it starts from this default directory.
-    """
-    from PyQt5.QtWidgets import QFileDialog, QApplication
-    _ = QApplication([])
-    log_dir = QFileDialog.getExistingDirectory(
-        None, "Select a directory", default_directory, QFileDialog.ShowDirsOnly)
-    return(log_dir)
-
-def select_file():
-    """ Open dialog to select a file
-        It works for windows and Linux using PyQt5.
-    """
-    from PyQt5.QtWidgets import QFileDialog, QApplication
-    from pathlib import Path
-    _ = QApplication([])
-    fpath = QFileDialog.getOpenFileName()
-    fpath = Path(fpath[0])
-    return(fpath)
```

### Comparing `lognflow-0.7.6/lognflow/logviewer.py` & `lognflow-0.8.0/lognflow/logviewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pathlib
 import numpy as np
+from .utils import replace_all
 
 class logviewer:
     """ log viewer
         Since lognflow makes lots of files and folders, maybe it is nice
         to have a logviewer that loads those information. In this module we
         provide a set of functions for a logged object that can load variables,
         texts, file lists and etc.. Use it simply by::
@@ -15,15 +16,16 @@
     def __init__(self,
                  log_dir : pathlib.Path,
                  logger = print):
         self.log_dir = pathlib.Path(log_dir)
         assert self.log_dir.is_dir(), \
             f'lognflow.logviewer| No such directory: '+ str(self.log_dir)
         self.logger = logger
-        
+        self.load = self.get_single
+    
     def get_text(self, log_name='main_log'):
         """ get text log files
             Given the log_name, this function returns the text therein.
 
             Parameters
             ----------
             :param log_name:
@@ -37,33 +39,26 @@
             for fcnt in range(n_files):
                 with open(flist[fcnt]) as f_txt:
                     txt.append(f_txt.readlines())
             if(n_files == 1):
                 txt = txt[0]
             return txt
 
-    def get_single(self, var_name, single_shot_index = -1, 
-                     suffix = None):
-        """ get a single variable
-            return the value of a saved variable.
+    def get_flist(self, var_name, suffix = None):
+        """ get list of files
+            return the list of files for a saved variable.
 
             Parameters
             ----------
             :param var_name:
                 variable name
-            :param single_shot_index:
-                If there are many snapshots of a variable, this input can
-                limit the returned to a set of indices.
             :param suffix:
                 If there are different suffixes availble for a variable
                 this input needs to be set. npy, npz, mat, and torch are
                 supported.
-                
-            .. note::
-                when reading a MATLAB file, the output is a dictionary.
         """
         var_name = var_name.replace('\t', '\\t').replace('\n', '\\n')\
             .replace('\r', '\\r').replace('\b', '\\b')
         
         if suffix is None:
             if len(var_name.split('.')) > 1:
                 suffix = var_name.split('.')[-1]
@@ -73,89 +68,119 @@
                     var_name = '*'
                 else:
                     var_name = ('.').join(var_name.split('.')[:-1])
             else:
                 suffix = '.np*'
 
         suffix = suffix.strip('.')        
-        assert single_shot_index == int(single_shot_index), \
-                    f'single_shot_index {single_shot_index} must be an integer'
+
         flist = []            
         if((self.log_dir / var_name).is_file()):
             flist = [self.log_dir / var_name]
         elif((self.log_dir / f'{var_name}.{suffix}').is_file()):
             flist = [self.log_dir / f'{var_name}.{suffix}']
         else:
             _var_name = (self.log_dir / var_name).name
             _var_dir = (self.log_dir / var_name).parent
             search_patt = f'{_var_name}*.{suffix}'
-            while('**' in search_patt):
-                search_patt = search_patt.replace('**', '*')
+            search_patt = replace_all(search_patt, '**', '*')
             flist = list(_var_dir.glob(search_patt))
             if(len(flist) == 0):
-                flist = list(_var_dir.glob(f'{_var_name}*.*'))
+                search_patt = f'{_var_name}*.*'
+                search_patt = replace_all(search_patt, '**', '*')
+                flist = list(_var_dir.glob(search_patt))
                 if(len(flist) > 0):
-                    self.logger('Can not find the file with the given suffix, '\
-                                +'but found some with a different suffix, '\
-                                +f'one file is: {flist[single_shot_index]}')
+                    self.logger(
+                        'I Can not find the file with the given suffix, '\
+                        + 'but found some with a different suffix, '\
+                        + f'one file is: {flist[-1]}. This is what I'\
+                        + ' will return.' )
                     
         if(len(flist) > 0):
             flist.sort()
         else:
             var_dir = self.log_dir / var_name
             if(var_dir.is_dir()):
                 flist = list(var_dir.glob('*.*'))
             if(len(flist) > 0):
                 flist.sort()
-            else:
-                self.logger('No such variable')
-                return
-        var_path = flist[single_shot_index]
+        return flist
+            
+    def get_single(self, var_name, file_index = -1, suffix = None):
+        """ get a single variable
+            return the value of a saved variable.
+
+            Parameters
+            ----------
+            :param var_name:
+                variable name
+            :param file_index:
+                If there are many snapshots of a variable, this input can
+                limit the returned to a set of indices.
+            :param suffix:
+                If there are different suffixes availble for a variable
+                this input needs to be set. npy, npz, mat, and torch are
+                supported.
                 
-        if(var_path.is_file()):
-            self.logger(f'Loading {var_path}')
-            if(var_path.suffix == '.npz'):
-                buf = np.load(var_path)
+            .. note::
+                when reading a MATLAB file, the output is a dictionary.
+        """
+        assert file_index == int(file_index), \
+                    f'file_index {file_index} must be an integer'
+        flist = self.get_flist(var_name, suffix)
+        var_path = None
+        if flist:
+            var_path = flist[file_index]
+    
+            if(var_path.is_file()):
+                self.logger(f'Loading {var_path}')
+                if(var_path.suffix == '.npz'):
+                    buf = np.load(var_path)
+                    try:
+                        time_array = buf['time_array']
+                        n_logs = (time_array > 0).sum()
+                        time_array = time_array[:n_logs]
+                        data_array = buf['data_array']
+                        data_array = data_array[:n_logs]
+                        return((time_array, data_array))
+                    except:
+                        return(buf)
+                if(var_path.suffix == '.npy'):
+                    return(np.load(var_path))
+                if(var_path.suffix == '.mat'):
+                    from scipy.io import loadmat
+                    return(loadmat(var_path))
+                if( (var_path.suffix == '.txt')
+                   |(var_path.suffix == '.pdb')
+                   |(var_path.suffix == '.json')):
+                    with open(var_path) as f_txt:
+                        return(f_txt.read())
+                if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
+                    from tifffile import imread
+                    return(imread(var_path))
+                if(var_path.suffix == '.torch'):      
+                    from torch import load as torch_load 
+                    return(torch_load(var_path))
                 try:
-                    time_array = buf['time_array']
-                    n_logs = (time_array > 0).sum()
-                    time_array = time_array[:n_logs]
-                    data_array = buf['data_array']
-                    data_array = data_array[:n_logs]
-                    return((time_array, data_array))
+                    from matplotlib.pyplot import imread
+                    img = imread(var_path)
+                    return(img)
                 except:
-                    return(buf)
-            if(var_path.suffix == '.npy'):
-                return(np.load(var_path))
-            if(var_path.suffix == '.mat'):
-                from scipy.io import loadmat
-                return(loadmat(var_path))
-            if(var_path.suffix == '.txt'):
-                with open(var_path) as f_txt:
-                    return(f_txt.read())
-            if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
-                from tifffile import imread
-                return(imread(var_path))
-            if(var_path.suffix == '.torch'):      
-                from torch import load as torch_load 
-                return(torch_load(var_path))
-            try:
-                from matplotlib.pyplot import imread
-                img = imread(var_path)
-                return(img)
-            except:
-                pass
-        else:
-            self.logger(f'{var_name} not found.')
-            return
-   
-    def get_stack_of_files(self,
+                    var_path = None
+            else:
+                var_path = None
+                
+        if var_path is None:
+            self.logger(f'{var_name} does not resemble the name of any file '
+                        f'or directory in the log_dir: {self.log_dir}')
+    
+    def get_stack_of_files(self, 
         var_name = None, flist = [], suffix = None,
         return_data = False, return_flist = True, read_func = None,
-        data_makes_a_block = False, verbose = True):
+        data_makes_a_block = True, verbose = True):
        
         """ Get list or data of all files in a directory
        
             This function gives the list of paths of all files in a directory
             for a single variable.
 
             Parameters
@@ -190,56 +215,23 @@
            
                 It returns a tuple, (dataset, flist),
                 dataset will be a list of files contains or numpy array in
                 case all files produce same shape numpy arrays.
                 flist is type pathlib.Path
            
         """
-        if suffix is None:
-            var_name_split = var_name.split('.')
-            if len(var_name_split) > 1:
-                suffix = var_name_split[-1]
-                name_before_suffix = var_name_split[:-1]
-                if((len(name_before_suffix) == 1) &
-                   (name_before_suffix[0] == '')):
-                    var_name = '*'
-                else:
-                    var_name = ('.').join(var_name_split[:-1])
-            else:
-                suffix = '*'
-
-        suffix = suffix.strip('.')
         if not flist:
-            assert var_name is not None, \
-                ' The file list is empty. Please provide the ' \
-                + 'variable name or a non-empty file list.'
-            var_dir = self.log_dir / var_name
-            if(var_dir.is_dir()):
-                var_fname = None
-                flist = list(var_dir.glob(f'*.{suffix}'))
-            else:
-                var_fname = var_dir.name
-                var_dir = var_dir.parent
-                patt = f'{var_fname}*.{suffix}'
-                while('**' in patt):
-                    patt = patt.replace('**', '*')
-                flist = list(var_dir.glob(patt))
-        else:
-            var_dir = flist[0].parent
-            assert var_dir.is_dir(),\
-                f'The directory {var_dir} for the '\
-                + 'provided list cannot be accessed.'
-           
+            flist = self.get_flist(var_name, suffix)
+        
         if flist:
             flist.sort()
             n_files = len(flist)
             if((not return_data) & return_flist):
                 return(flist)
            
-            ######### asked for data ########
             if(read_func is None):
                 try:
                     fdata = np.load(flist[0])
                     read_func = np.load
                 except:
                     pass
             if(read_func is None):
@@ -253,18 +245,28 @@
                 assert callable(read_func), \
                     f'given read_func: {read_func} is not callable.'
                 fdata = read_func(flist[0])
                 if(data_makes_a_block):
                     dataset = np.zeros((n_files, ) + fdata.shape,
                                        dtype=fdata.dtype)
                     if(verbose):
-                        self.logger(f'logviewer: Reading dataset from {var_dir}'
+                        self.logger(f'logviewer: Reading dataset from '
+                                    f'{flist[0].parent}'
                                     f', the shape would be: {dataset.shape}')
                     for fcnt, fpath in enumerate(flist):
-                        dataset[fcnt] = read_func(fpath)
+                        try:
+                            dataset[fcnt] = read_func(fpath)
+                        except e:
+                            self.logger(
+                                'I cannot concatenate the data I just read on'
+                                ' top of last files data. You need to set'
+                                ' data_makes_a_block = False in the input'
+                                f' of get_stack_of_files({var_name}, ...)'
+                                ' This will return a list of data of files')
+                            raise e
                 else:
                     dataset = [read_func(fpath) for fpath in flist]
                 if(return_flist):
                     return(dataset, flist)
                 else:
                     return(dataset)
             else:
@@ -310,51 +312,8 @@
 
         return(flist_A_new, flist_B_new)
     
     def __repr__(self):
         return f'{self.log_dir}'
 
     def __bool__(self):
-        return self.log_dir.is_dir()
-
-def str2type(_element):
-    if _element[0] == '\'':
-        return _element[1:-1]
-    else:
-        try:
-            return int(_element)
-        except ValueError:
-            try:
-                return float(_element)
-            except ValueError:
-                pass
-    return _element
-
-def text_to_object(txt):
-    """ Read a list or dict that was sent to write to text e.g. via log_single:
-    As you may have tried, it is possible to send a Pythonic list to a text file
-    the list will be typed there with [ and ] and ' and ' for strings with ', '
-    in between. In this function we will merely return the actual content
-    of the original list.
-    Now if the type the element of the list was string, it would put ' and ' in
-    the text file. But if it is a number, no kind of punctuation or sign is 
-    used. by write(). We support int or float. Otherwise the written text
-    will be returned as string with any other wierd things attached to it.
-    
-    """
-    if(txt[0] == '['):
-        txt = txt.strip('[').strip(']')
-        txt = txt.split(', ')
-        obj_out = txt
-        for cnt, _element in enumerate(txt):
-            obj_out[cnt] = str2type(_element)
-    elif(txt[0] == '{'):
-        txt = txt.strip('{').strip('}')
-        txt = txt.split(', ')
-        obj_out = dict()
-        for cnt, _element in enumerate(txt):
-            _element_key = str2type(_element.split(': ')[0])
-            _element_value = str2type(_element.split(': ')[1])
-            obj_out[_element_key] = _element_value
-    else:
-        obj_out = txt
-    return obj_out
+        return self.log_dir.is_dir()
```

### Comparing `lognflow-0.7.6/lognflow/printprogress.py` & `lognflow-0.8.0/lognflow/printprogress.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     looking progress bar with a simple title and limits and 
     is very simple to use. Define the object with number of steps of the loop 
     and then call it in every iteration of the loop. If you'd like it
     to go faster, call it with give number of steps that have passed.
     """
     def __init__(self, 
                  n_steps, 
-                 numTicks = 80,
+                 numTicks = 78,
                  title = None,
                  method = 'linear',
                  print_function = print,
                  **print_function_kwargs):
         """
             n_steps: int
                 Number of iterations in the for loop
@@ -67,15 +67,15 @@
         self._print_func(' ', end='')
         self._print_func('_'*self.numTicks, end='')
         self._print_func(' ')
         
         self._print_func('/', end='')
         self._print_func(' '*int((self.numTicks - len(title))/2), end='')
         self._print_func(title, end='')
-        self._print_func(' '*int((self.numTicks - len(title))/2), end='')
+        self._print_func(' '*int(ceil((self.numTicks-len(title))/2)-1), end='')
         self._print_func(' \\')
         
         self._print_func(' ', end = '')
     
     def _print_func(self, text, end='\n'):
         if (self.in_print_function is not None):
             if (self.in_print_function == print):
```

### Comparing `lognflow-0.7.6/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.0/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.6
+Version: 0.8.0
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -205,7 +205,14 @@
 
 0.7.6 (2023-07-17)
 ------------------
 * printprogress can handle up to 99 days
 * log_text takes any save_as
 * If variable name has escape key is alright
 * If variable name is splitable, we replace them with _
+
+0.8.0 (2023-07-25)
+------------------
+* logger.save and savez are set to be identical to log_single.
+* logged.load is set to be identical to get_single.
+* utils.py is added to contain all misc functions.
+* replace_all added to utils
```

### Comparing `lognflow-0.7.6/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.0/lognflow.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 lognflow/__init__.py
 lognflow/lognflow.py
 lognflow/logviewer.py
 lognflow/printprogress.py
+lognflow/utils.py
 lognflow.egg-info/PKG-INFO
 lognflow.egg-info/SOURCES.txt
 lognflow.egg-info/dependency_links.txt
 lognflow.egg-info/not-zip-safe
 lognflow.egg-info/requires.txt
 lognflow.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `lognflow-0.7.6/setup.py` & `lognflow-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.6'
+__version__ = '0.8.0'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.6/tests/test_lognflow.py` & `lognflow-0.8.0/tests/test_lognflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Tests for `lognflow` package."""
 
 import time
+import pytest
 import numpy as np
 import matplotlib.pyplot as plt
-import pytest
 
 from lognflow import lognflow, logviewer, printprogress, select_directory
 
 import tempfile
 temp_dir = tempfile.gettempdir()
 
 @pytest.fixture
@@ -277,14 +277,38 @@
     logger('This is a test for test_log_imshow_complex', flush = True)
     
     mat = np.random.rand(100, 100) + 10 * 1j * np.random.rand(100, 100)
     
     logger(f'mat is complex? {np.iscomplexobj(mat)}')
     logger.log_imshow('mat', mat)
     
+def test_replace_time_with_index():
+    logger = lognflow(temp_dir)
+    logger('Well this is a test for logviewer')
+    
+    for _ in range(5):
+        logger.log_single('test_param', np.array([_]))
+        logger.log_single('testy/t', np.array([_]))
+    
+    logged = logviewer(logger.log_dir, logger)
+
+    data_in, flist = logged.get_stack_of_files(
+        'test_param', return_data=True, return_flist=True)
+    
+    logger(flist)
+
+    logger.replace_time_with_index('test_param')
+    
+    data_out, flist = logged.get_stack_of_files(
+        'test_param', return_data=True, return_flist=True)
+    
+    logger(flist)
+    
+    logger(data_in)
+    logger(data_out)
     
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
     test_log_single_text()
@@ -304,7 +328,8 @@
     test_log_animation()
     test_log_hist()
     test_log_scatter3()
     test_log_plt()
     test_log_hexbin()
     test_log_canvas()
     test_log_confusion_matrix()
+    test_replace_time_with_index()
```

### Comparing `lognflow-0.7.6/tests/test_logviewer.py` & `lognflow-0.8.0/tests/test_logviewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python
 
 """Tests for `lognflow` package."""
 
 import pytest
 import re
-from lognflow import lognflow, select_directory, logviewer, printprogress
-
 import numpy as np
 
+from lognflow import (lognflow, select_directory, 
+                      logviewer, printprogress,
+                      text_to_object)
+
 import tempfile
 temp_dir = tempfile.gettempdir()
 
 @pytest.fixture
 def response():
     """Sample pytest fixture.
 
@@ -85,42 +87,15 @@
             flist = flist_B_AB, return_data = True, return_flist = False)
         
         logger.log_canvas('data_samples', [dataset_A, dataset_B], dpi = 300)
         _ = logger._loggers_dict['main_log'].log_size
         logger('Size of the log file in bytes is: ' \
                + f'{_}')
 
-def test_replace_time_with_index():
-    logger = lognflow(temp_dir)
-    logger('Well this is a test for logviewer')
-    
-    for _ in range(5):
-        logger.log_single('test_param', np.array([_]))
-        logger.log_single('testy/t', np.array([_]))
-    
-    logged = logviewer(logger.log_dir, logger)
-
-    data_in, flist = logged.get_stack_of_files(
-        'test_param', return_data=True, return_flist=True)
-    
-    logger(flist)
-
-    logger.replace_time_with_index('test_param')
-    
-    data_out, flist = logged.get_stack_of_files(
-        'test_param', return_data=True, return_flist=True)
-    
-    logger(flist)
-    
-    logger(data_in)
-    logger(data_out)
-
 def test_text_to_object():
-    from lognflow.logviewer import text_to_object
-    
     logger = lognflow(temp_dir, time_tag = False)
     test_list = ['asdf', 1243, "dd"]
     logger.log_single('test_list', test_list, save_as = 'txt')
     
     test_dict = {"one": "asdf", 'two': 1243, 'thre': "dd"}
     logger.log_single('test_dict', test_dict, save_as = 'txt')
     
@@ -154,12 +129,9 @@
     
     assert vec_out == vec
 
 if __name__ == '__main__':
     temp_dir = select_directory()
     test_get_single_specific_fname()
     test_get_images_as_stack()
-    test_replace_time_with_index()
     test_logviewer()
-    test_text_to_object()
-    exit()
-    
+    test_text_to_object()
```

### Comparing `lognflow-0.7.6/tests/test_printprogress.py` & `lognflow-0.8.0/tests/test_printprogress.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 def test_content(response):
     """Sample pytest test function with the pytest fixture as an argument."""
     # from bs4 import BeautifulSoup
     # assert 'GitHub' in BeautifulSoup(response.content).title.string
 
 def test_printprogress():
-    N = 15000000
+    N = 3000000
     pprog = printprogress(N)
     for _ in range(N):
         pprog()
     # assert input('Did it show you a progress bar? (y for yes)')=='y'
 
-def test_with_logger():
+def test_printprogress_with_logger():
     logger = lognflow()
     N = 1500000
     pprog = printprogress(N, print_function = logger, log_time_stamp = False)
     for _ in range(N):
         pprog()
         
-def test_ETA():
+def test_printprogress_ETA():
     logger = lognflow()
-    N = 1500000
+    N = 500000
     pprog = printprogress(N, print_function = None)
     for _ in range(N):
         ETA = pprog()
         print(ETA)
     
 
 if __name__ == '__main__':
-    test_ETA()
+    test_printprogress_with_logger()
+    test_printprogress_ETA()
     test_printprogress()
-    test_with_logger()
     exit()
```

