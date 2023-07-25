# Comparing `tmp/plotguy-1.2.4.tar.gz` & `tmp/plotguy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.2.4.tar", last modified: Tue Jun 20 03:49:06 2023, max compression
+gzip compressed data, was "plotguy-1.2.5.tar", last modified: Tue Jul 25 08:44:54 2023, max compression
```

## Comparing `plotguy-1.2.4.tar` & `plotguy-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.858642 plotguy-1.2.4/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-20 03:49:06.858485 plotguy-1.2.4/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.4/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.857545 plotguy-1.2.4/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    26203 2023-06-20 03:47:28.000000 plotguy-1.2.4/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.4/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    65962 2023-06-09 02:59:05.000000 plotguy-1.2.4/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    38129 2023-06-13 02:24:31.000000 plotguy-1.2.4/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.4/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.858286 plotguy-1.2.4/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-20 03:49:06.858694 plotguy-1.2.4/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-20 03:48:00.000000 plotguy-1.2.4/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-25 08:44:54.253894 plotguy-1.2.5/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-07-25 08:44:54.253668 plotguy-1.2.5/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.5/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-25 08:44:54.252168 plotguy-1.2.5/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    26360 2023-07-25 08:43:03.000000 plotguy-1.2.5/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.5/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    65962 2023-06-09 02:59:05.000000 plotguy-1.2.5/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    38129 2023-06-13 02:24:31.000000 plotguy-1.2.5/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.5/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-25 08:44:54.253388 plotguy-1.2.5/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-07-25 08:44:53.000000 plotguy-1.2.5/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-07-25 08:44:53.000000 plotguy-1.2.5/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-07-25 08:44:53.000000 plotguy-1.2.5/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-07-25 08:44:53.000000 plotguy-1.2.5/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-07-25 08:44:53.000000 plotguy-1.2.5/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-25 08:44:54.253965 plotguy-1.2.5/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-07-25 08:43:59.000000 plotguy-1.2.5/setup.py
```

### Comparing `plotguy-1.2.4/plotguy/__init__.py` & `plotguy-1.2.5/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,16 +379,22 @@
 
     intraday = para_combination['intraday']
     freq = para_combination['freq']
     file_format = para_combination['file_format']
     sec_profile = para_combination['sec_profile']
 
     if sectype == 'FUT':
+        for key in sec_profile:
+            if 'margin_req' in key:
+                sec_profile['margin_req'] = sec_profile.pop(key)
+                break
+
         margin_req = sec_profile['margin_req']
         multiplier = sec_profile['multiplier']
+
     elif sectype == 'STK':
         multiplier = 1
 
     # Read backtest data
     save_path = generate_filepath(para_combination=para_combination, folder=folder)
 
     if file_format == 'parquet':
```

### Comparing `plotguy-1.2.4/plotguy/aggregate.py` & `plotguy-1.2.5/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.4/plotguy/components.py` & `plotguy-1.2.5/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.4/plotguy/equity_curves.py` & `plotguy-1.2.5/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.4/plotguy/signals.py` & `plotguy-1.2.5/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.4/setup.py` & `plotguy-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.2.4",
+    version="1.2.5",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas==1.5.3',
```

