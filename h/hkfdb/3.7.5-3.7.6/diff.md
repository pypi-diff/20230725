# Comparing `tmp/hkfdb-3.7.5.tar.gz` & `tmp/hkfdb-3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.7.5.tar", last modified: Mon Jul 17 10:10:42 2023, max compression
+gzip compressed data, was "hkfdb-3.7.6.tar", last modified: Mon Jul 24 23:15:30 2023, max compression
```

## Comparing `hkfdb-3.7.5.tar` & `hkfdb-3.7.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-17 10:10:42.812902 hkfdb-3.7.5/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.5/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-17 10:10:42.812757 hkfdb-3.7.5/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.5/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-17 10:10:42.811709 hkfdb-3.7.5/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   109629 2023-07-17 10:09:22.000000 hkfdb-3.7.5/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.5/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-17 10:10:42.812578 hkfdb-3.7.5/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-17 10:10:42.000000 hkfdb-3.7.5/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-17 10:10:42.000000 hkfdb-3.7.5/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-17 10:10:42.000000 hkfdb-3.7.5/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-17 10:10:42.000000 hkfdb-3.7.5/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-17 10:10:42.000000 hkfdb-3.7.5/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-17 10:10:42.812950 hkfdb-3.7.5/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-17 10:09:58.000000 hkfdb-3.7.5/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.201116 hkfdb-3.7.6/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.6/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-24 23:15:30.200772 hkfdb-3.7.6/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.6/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.199352 hkfdb-3.7.6/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   109716 2023-07-24 23:12:08.000000 hkfdb-3.7.6/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.6/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-24 23:15:30.200484 hkfdb-3.7.6/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-24 23:15:29.000000 hkfdb-3.7.6/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-24 23:15:30.201187 hkfdb-3.7.6/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-24 23:14:24.000000 hkfdb-3.7.6/setup.py
```

### Comparing `hkfdb-3.7.5/LICENSE` & `hkfdb-3.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.5/PKG-INFO` & `hkfdb-3.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.5
+Version: 3.7.6
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.5/README.md` & `hkfdb-3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.5/hkfdb/Database.py` & `hkfdb-3.7.6/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,14 +427,15 @@
                     expiry_dates = list(df['expiry_date'].unique())
                     expiry_dates.sort()
                     # print(expiry_dates)
 
                     # Calculate roll diff
                     roll_diff_dict = {}
 
+
                     for expiry_date in expiry_dates:
 
                         try:
                             exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
                                                     (df['current_month_expiry_date_diff'] == rolling_day) &
                                                     (df['current_month'] == True)].sort_values(by=['datetime'],
                                                                                                ascending=False).reset_index(
@@ -468,23 +469,25 @@
                                 # print(df_roll)
                                 roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
                                 roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
                                 roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
                                 roll_diff_dict[expiry_date]['rolling_time'] = df_roll.at[0, 'time']
 
                         except Exception as e:
-                            roll_diff_dict = {}
+                            try:
+                                roll_diff_dict.pop(expiry_date)
+                            except:
+                                pass
                             pass
 
 
                     df = df.reset_index(drop=True)
                     df['roll_diff'] = 0
 
                     for expiry_date in roll_diff_dict.keys():
-                        print('Hi')
                         d = roll_diff_dict[expiry_date]['rolling_day']
                         t = roll_diff_dict[expiry_date]['rolling_time']
                         diff = roll_diff_dict[expiry_date]['roll_diff']
 
                         condition = (df['date'] == d) & (df['time'] == t) & (df['current_month'] == False)
                         indices = df[condition].index[0]
                         df.at[indices, 'roll_diff'] = diff
```

### Comparing `hkfdb-3.7.5/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.7.6/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.5
+Version: 3.7.6
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.5/setup.py` & `hkfdb-3.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.7.5",
+    version="3.7.6",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

