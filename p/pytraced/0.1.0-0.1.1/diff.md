# Comparing `tmp/pytraced-0.1.0.tar.gz` & `tmp/pytraced-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytraced-0.1.0.tar", last modified: Sat Jul 22 08:31:32 2023, max compression
+gzip compressed data, was "pytraced-0.1.1.tar", last modified: Tue Jul 25 03:25:29 2023, max compression
```

## Comparing `pytraced-0.1.0.tar` & `pytraced-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.201329 pytraced-0.1.0/
--rw-rw-rw-   0        0        0    32746 2023-06-19 08:13:23.000000 pytraced-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0    45373 2023-07-22 08:31:32.201329 pytraced-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6886 2023-07-22 08:21:49.000000 pytraced-0.1.0/README.md
--rw-rw-rw-   0        0        0      146 2023-06-29 07:47:42.000000 pytraced-0.1.0/dev_requirements.txt
--rw-rw-rw-   0        0        0     1328 2023-07-11 21:03:09.000000 pytraced-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       15 2023-07-11 21:01:30.000000 pytraced-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0     1120 2023-07-22 08:31:32.206328 pytraced-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-07-05 23:12:07.000000 pytraced-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.054327 pytraced-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.128327 pytraced-0.1.0/src/pytraced/
--rw-rw-rw-   0        0        0     2866 2023-07-13 08:36:55.000000 pytraced-0.1.0/src/pytraced/__init__.py
--rw-rw-rw-   0        0        0     9289 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/_config.py
--rw-rw-rw-   0        0        0     6055 2023-07-22 06:28:10.000000 pytraced-0.1.0/src/pytraced/_formatter.py
--rw-rw-rw-   0        0        0     2415 2023-07-22 06:27:27.000000 pytraced-0.1.0/src/pytraced/_levels.py
--rw-rw-rw-   0        0        0    22708 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/_logger.py
--rw-rw-rw-   0        0        0     1610 2023-07-22 06:24:47.000000 pytraced-0.1.0/src/pytraced/_record.py
--rw-rw-rw-   0        0        0     3462 2023-07-22 06:24:42.000000 pytraced-0.1.0/src/pytraced/_sink.py
--rw-rw-rw-   0        0        0     1820 2023-07-22 06:24:27.000000 pytraced-0.1.0/src/pytraced/_traceback.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.150326 pytraced-0.1.0/src/pytraced/colours/
--rw-rw-rw-   0        0        0     1033 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/colours/__init__.py
--rw-rw-rw-   0        0        0     3658 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/colours/_colouriser.py
--rw-rw-rw-   0        0        0     2377 2023-07-22 06:29:11.000000 pytraced-0.1.0/src/pytraced/colours/_colours.py
--rw-rw-rw-   0        0        0        0 2023-06-19 08:13:23.000000 pytraced-0.1.0/src/pytraced/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.142327 pytraced-0.1.0/src/pytraced.egg-info/
--rw-rw-rw-   0        0        0    45373 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      838 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.197327 pytraced-0.1.0/tests/
--rw-rw-rw-   0        0        0     1284 2023-07-22 07:44:34.000000 pytraced-0.1.0/tests/test_colouriser.py
--rw-rw-rw-   0        0        0      713 2023-07-14 21:54:52.000000 pytraced-0.1.0/tests/test_colours.py
--rw-rw-rw-   0        0        0     3046 2023-07-22 07:44:34.000000 pytraced-0.1.0/tests/test_config.py
--rw-rw-rw-   0        0        0     6747 2023-07-22 06:28:40.000000 pytraced-0.1.0/tests/test_formatter.py
--rw-rw-rw-   0        0        0      609 2023-07-18 02:56:35.000000 pytraced-0.1.0/tests/test_level.py
--rw-rw-rw-   0        0        0    10555 2023-07-22 07:44:48.000000 pytraced-0.1.0/tests/test_logger.py
--rw-rw-rw-   0        0        0      567 2023-07-14 21:26:53.000000 pytraced-0.1.0/tests/test_metadata.py
--rw-rw-rw-   0        0        0      506 2023-07-18 20:28:35.000000 pytraced-0.1.0/tests/test_performance.py
--rw-rw-rw-   0        0        0     1265 2023-07-18 23:04:02.000000 pytraced-0.1.0/tests/test_record.py
--rw-rw-rw-   0        0        0     2155 2023-07-18 02:56:58.000000 pytraced-0.1.0/tests/test_sink.py
--rw-rw-rw-   0        0        0      798 2023-07-19 08:51:38.000000 pytraced-0.1.0/tests/test_traceback.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.542002 pytraced-0.1.1/
+-rw-rw-rw-   0        0        0    32746 2023-06-20 08:26:01.000000 pytraced-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    45373 2023-07-25 03:25:29.543007 pytraced-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6886 2023-07-25 00:26:21.000000 pytraced-0.1.1/README.md
+-rw-rw-rw-   0        0        0      146 2023-07-21 07:16:47.000000 pytraced-0.1.1/dev_requirements.txt
+-rw-rw-rw-   0        0        0     1218 2023-07-25 03:20:22.000000 pytraced-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       15 2023-07-21 07:16:47.000000 pytraced-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0     1120 2023-07-25 03:25:29.553523 pytraced-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-07-25 03:10:21.000000 pytraced-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.441967 pytraced-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.477165 pytraced-0.1.1/src/pytraced/
+-rw-rw-rw-   0        0        0     2866 2023-07-25 03:18:59.000000 pytraced-0.1.1/src/pytraced/__init__.py
+-rw-rw-rw-   0        0        0     9289 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_config.py
+-rw-rw-rw-   0        0        0     6055 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_formatter.py
+-rw-rw-rw-   0        0        0     2415 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_levels.py
+-rw-rw-rw-   0        0        0    22708 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_logger.py
+-rw-rw-rw-   0        0        0     1610 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_record.py
+-rw-rw-rw-   0        0        0     3462 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_sink.py
+-rw-rw-rw-   0        0        0     1820 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/_traceback.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.516034 pytraced-0.1.1/src/pytraced/colours/
+-rw-rw-rw-   0        0        0     1033 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/colours/__init__.py
+-rw-rw-rw-   0        0        0     3658 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/colours/_colouriser.py
+-rw-rw-rw-   0        0        0     2377 2023-07-22 08:40:31.000000 pytraced-0.1.1/src/pytraced/colours/_colours.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 08:26:01.000000 pytraced-0.1.1/src/pytraced/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.508754 pytraced-0.1.1/src/pytraced.egg-info/
+-rw-rw-rw-   0        0        0    45373 2023-07-25 03:25:29.000000 pytraced-0.1.1/src/pytraced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      838 2023-07-25 03:25:29.000000 pytraced-0.1.1/src/pytraced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:25:29.000000 pytraced-0.1.1/src/pytraced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-07-25 03:25:29.000000 pytraced-0.1.1/src/pytraced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 03:25:29.000000 pytraced-0.1.1/src/pytraced.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 03:25:29.540013 pytraced-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1284 2023-07-22 08:40:31.000000 pytraced-0.1.1/tests/test_colouriser.py
+-rw-rw-rw-   0        0        0      713 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_colours.py
+-rw-rw-rw-   0        0        0     3046 2023-07-22 08:40:31.000000 pytraced-0.1.1/tests/test_config.py
+-rw-rw-rw-   0        0        0     6747 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_formatter.py
+-rw-rw-rw-   0        0        0      609 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_level.py
+-rw-rw-rw-   0        0        0    10555 2023-07-22 08:40:31.000000 pytraced-0.1.1/tests/test_logger.py
+-rw-rw-rw-   0        0        0      567 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_metadata.py
+-rw-rw-rw-   0        0        0      506 2023-07-25 03:19:32.000000 pytraced-0.1.1/tests/test_performance.py
+-rw-rw-rw-   0        0        0     1265 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_record.py
+-rw-rw-rw-   0        0        0     2155 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_sink.py
+-rw-rw-rw-   0        0        0      798 2023-07-21 07:16:47.000000 pytraced-0.1.1/tests/test_traceback.py
```

### Comparing `pytraced-0.1.0/LICENSE.md` & `pytraced-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/PKG-INFO` & `pytraced-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytraced
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple, lightweight, & extensible logging library for python
 Author: Eris
 Author-email: Eris <theferretdetective@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
```

### Comparing `pytraced-0.1.0/README.md` & `pytraced-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/setup.cfg` & `pytraced-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/__init__.py` & `pytraced-0.1.1/src/pytraced/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 pytraced:
 
-version: 0.1.0
+version: 0.1.1
 
 A simple, lightweight, & extensible logging library for python. This library provides an out of the
 box logger which prints to `stderr`, however it is extremely customizable to fit a wide range of 
 needs.
 
 Globals:
     - `__version__` - The current version of this package.
@@ -60,15 +60,15 @@
 from . import colours
 from ._config import Config
 from ._levels import Level, LevelDoesNotExistError
 from ._logger import Logger
 from ._record import Record
 from ._sink import Sink, SinkDoesNotExistError
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __all__ = (
     "logger",
     "Logger",
     "Level",
     "LevelDoesNotExistError",
     "Sink",
     "SinkDoesNotExistError",
```

### Comparing `pytraced-0.1.0/src/pytraced/_config.py` & `pytraced-0.1.1/src/pytraced/_config.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_formatter.py` & `pytraced-0.1.1/src/pytraced/_formatter.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_levels.py` & `pytraced-0.1.1/src/pytraced/_levels.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_logger.py` & `pytraced-0.1.1/src/pytraced/_logger.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_record.py` & `pytraced-0.1.1/src/pytraced/_record.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_sink.py` & `pytraced-0.1.1/src/pytraced/_sink.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/_traceback.py` & `pytraced-0.1.1/src/pytraced/_traceback.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/colours/__init__.py` & `pytraced-0.1.1/src/pytraced/colours/__init__.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/colours/_colouriser.py` & `pytraced-0.1.1/src/pytraced/colours/_colouriser.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced/colours/_colours.py` & `pytraced-0.1.1/src/pytraced/colours/_colours.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/src/pytraced.egg-info/PKG-INFO` & `pytraced-0.1.1/src/pytraced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytraced
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple, lightweight, & extensible logging library for python
 Author: Eris
 Author-email: Eris <theferretdetective@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
```

### Comparing `pytraced-0.1.0/src/pytraced.egg-info/SOURCES.txt` & `pytraced-0.1.1/src/pytraced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_colouriser.py` & `pytraced-0.1.1/tests/test_colouriser.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_colours.py` & `pytraced-0.1.1/tests/test_colours.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_config.py` & `pytraced-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_formatter.py` & `pytraced-0.1.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_level.py` & `pytraced-0.1.1/tests/test_level.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_logger.py` & `pytraced-0.1.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_metadata.py` & `pytraced-0.1.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_record.py` & `pytraced-0.1.1/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_sink.py` & `pytraced-0.1.1/tests/test_sink.py`

 * *Files identical despite different names*

### Comparing `pytraced-0.1.0/tests/test_traceback.py` & `pytraced-0.1.1/tests/test_traceback.py`

 * *Files identical despite different names*

