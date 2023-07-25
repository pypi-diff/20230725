# Comparing `tmp/mass_analytics-1.0.6.tar.gz` & `tmp/mass_analytics-1.0.7.tar.gz`

## Comparing `mass_analytics-1.0.6.tar` & `mass_analytics-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/src/mass_analytics/date.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 mass_analytics-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/date.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/README.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/PKG-INFO
```

### Comparing `mass_analytics-1.0.6/src/mass_analytics/data_frame_util.py` & `mass_analytics-1.0.7/src/mass_analytics/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.6/src/mass_analytics/date.py` & `mass_analytics-1.0.7/src/mass_analytics/date.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.6/src/mass_analytics/reader.py` & `mass_analytics-1.0.7/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.6/LICENSE.txt` & `mass_analytics-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.6/README.md` & `mass_analytics-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.6/pyproject.toml` & `mass_analytics-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6d61 7373 5f61 6e61 6c79 7469 6373   "mass_analytics
 00000070: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000080: 302e 3622 0d0a 6175 7468 6f72 7320 3d20  0.6"..authors = 
+00000080: 302e 3722 0d0a 6175 7468 6f72 7320 3d20  0.7"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 7365 6c69  im", email="seli
 000000b0: 6d2e 616c 6f75 696e 6940 6d61 7373 2d61  m.alouini@mass-a
 000000c0: 6e61 6c79 7469 6373 2e63 6f6d 2220 7d2c  nalytics.com" },
 000000d0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 000000e0: 203d 2022 4120 736d 616c 6c20 6578 616d   = "A small exam
 000000f0: 706c 6520 7061 636b 6167 6520 666f 7220  ple package for
```

### Comparing `mass_analytics-1.0.6/PKG-INFO` & `mass_analytics-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.0.6
+Version: 1.0.7
 Summary: A small example package for mass-analytics
 Author-email: Selim <selim.alouini@mass-analytics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

