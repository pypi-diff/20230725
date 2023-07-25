# Comparing `tmp/davis_rig_parser-0.1.8.tar.gz` & `tmp/davis_rig_parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davis_rig_parser-0.1.8.tar", last modified: Mon Jul 10 17:53:11 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.1.9.tar", last modified: Tue Jul 25 18:51:01 2023, max compression
```

## Comparing `davis_rig_parser-0.1.8.tar` & `davis_rig_parser-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.1.8/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.848085 davis_rig_parser-0.1.8/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.8/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18431 2023-07-10 17:32:59.000000 davis_rig_parser-0.1.8/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-10 17:53:11.000000 davis_rig_parser-0.1.8/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-10 17:51:34.000000 davis_rig_parser-0.1.8/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-10 17:53:11.852085 davis_rig_parser-0.1.8/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.8/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 18:51:01.245059 davis_rig_parser-0.1.9/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-25 18:51:01.245059 davis_rig_parser-0.1.9/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.1.9/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 18:51:01.217058 davis_rig_parser-0.1.9/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.9/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18703 2023-07-11 17:05:28.000000 davis_rig_parser-0.1.9/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 18:51:01.221058 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-25 18:51:01.000000 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-25 18:51:01.000000 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-25 18:51:01.000000 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-25 18:51:01.000000 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-25 18:51:01.000000 davis_rig_parser-0.1.9/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-25 18:51:01.245059 davis_rig_parser-0.1.9/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-25 18:43:36.000000 davis_rig_parser-0.1.9/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 18:51:01.221058 davis_rig_parser-0.1.9/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.9/tests/test.py
```

### Comparing `davis_rig_parser-0.1.8/README.md` & `davis_rig_parser-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `davis_rig_parser-0.1.8/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.1.9/davis_rig_parser/davis_rig_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,7 +406,14 @@
     
     #Save dataframe for later use/plotting/analyses
     #timestamped with date
     if save_df==True:
         df.to_pickle(dir_name+'/%s_grouped_dframe.df' %(date.today().strftime("%d_%m_%Y")))
 
     return df
+
+#Work in progress below ---- No documentation yet
+def assign_day(df):
+    #uses a date column to assign a day column
+    for name, group in df.groupby(['Animal']):
+        mindate = min(df['Date'])
+        group['Day'] = [(x).days + 1 for x in (group['Date'] - mindate)]
```

