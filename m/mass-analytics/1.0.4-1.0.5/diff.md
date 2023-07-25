# Comparing `tmp/mass_analytics-1.0.4.tar.gz` & `tmp/mass_analytics-1.0.5.tar.gz`

## Comparing `mass_analytics-1.0.4.tar` & `mass_analytics-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/src/mass_analytics/date.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mass_analytics-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/src/mass_analytics/date.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/README.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 mass_analytics-1.0.5/PKG-INFO
```

### Comparing `mass_analytics-1.0.4/src/mass_analytics/date.py` & `mass_analytics-1.0.5/src/mass_analytics/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         ValueError: If no date columns are found in the DataFrame.
     """
          
     # Result list
     date_columns = []
     
     NUMBER_OF_ROWS = df.shape[0]
-    if NUMBER_OF_ROWS > 100:
-        NUMBER_ROW_TO_CHECK = int(NUMBER_OF_ROWS * 0.3) # Check only 30% of rows
+    if NUMBER_OF_ROWS > 1000:
+        NUMBER_ROW_TO_CHECK = 1000 # Check only 1000 rows
     else:
-        NUMBER_ROW_TO_CHECK = NUMBER_OF_ROWS # check all rows
+        NUMBER_ROW_TO_CHECK = NUMBER_OF_ROWS # Check all rows
                     
     for column in df.columns:
         if np.issubdtype(df[column].dtype, np.datetime64):
             date_columns.append(column)
             continue
         elif np.issubdtype(df[column].dtype, np.object_):
             counter = 0
@@ -65,26 +65,26 @@
                 elif type(value) is str:
                     if is_date(value):
                         counter += 1
                     elif value == 'nan':
                         counter_nan += 1
                         counter += 1
             
-            if counter > counter_nan and counter >= int(NUMBER_ROW_TO_CHECK * 0.75):
+            if counter > counter_nan and counter >= int(NUMBER_ROW_TO_CHECK * 0.50):
                 date_columns.append(column)
 
     if len(date_columns) == 0:
         raise ValueError("No date columns found in the DataFrame.")
     if len(date_columns) == 1:
         return date_columns[0]
     else:
         return date_columns
 
     
-def determine_periodicity(df, *columns):
+def get_periodicity(df, *columns):
     """
     Determine the periodicity of the given DataFrame or specified columns.
 
     The function analyzes the DataFrame or specified columns and attempts to identify
     the data's periodicity, such as daily ('D'), weekly on Monday ('W-MON') or Saturday ('W-SAT'),
     or monthly ('M'). The function calculates the time interval between consecutive
     data points in the specified columns and returns the most likely periodicity based
@@ -113,29 +113,31 @@
             columns = [columns]
 
     periodicity = {} # Result variable
 
     for col in columns:
         col_serie = df[col]
             
-        filter_dates_only = col_serie[col_serie.apply(lambda x: isinstance(x, datetime.datetime) or is_date(x))]
+        filter_dates_only = col_serie[col_serie.apply(lambda x: isinstance(x, datetime.datetime) or is_date(x))] 
+    
+        filter_dates_only = pd.Series(filter_dates_only.unique()).sort_values()
             
-        if filter_dates_only.size < 100:  
-            periodicity[col] = pd.infer_freq(filter_dates_only)
+        if filter_dates_only.size < 1000:
+            range_slice = int(filter_dates_only.size / 3)
         else:
-            periodicity_paterns = []
-            start = 0
-
-            len_to_check = int(df.shape[0] * 0.05) 
-
-            for index in range(8):
-                periodicity_paterns.append(pd.infer_freq(filter_dates_only[start:start + len_to_check]))
-                start += len_to_check
-                
-            periodicity[col] = max(set(periodicity_paterns), key = periodicity_paterns.count)
+            range_slice = 333 
+            
+        periodicity_paterns = []
+        start = 0
+        len_to_check = 3
+        for index in range(range_slice):
+            periodicity_paterns.append(pd.infer_freq(filter_dates_only[start:start + len_to_check]))
+            start += len_to_check
+        periodicity[col] = max(set(periodicity_paterns), key = periodicity_paterns.count)
 
     return periodicity
 
-
         
 
 
+
+
```

### Comparing `mass_analytics-1.0.4/src/mass_analytics/reader.py` & `mass_analytics-1.0.5/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.4/LICENSE.txt` & `mass_analytics-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.4/pyproject.toml` & `mass_analytics-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6d61 7373 5f61 6e61 6c79 7469 6373   "mass_analytics
 00000070: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000080: 302e 3422 0d0a 6175 7468 6f72 7320 3d20  0.4"..authors = 
+00000080: 302e 3522 0d0a 6175 7468 6f72 7320 3d20  0.5"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 7365 6c69  im", email="seli
 000000b0: 6d2e 616c 6f75 696e 6940 6d61 7373 2d61  m.alouini@mass-a
 000000c0: 6e61 6c79 7469 6373 2e63 6f6d 2220 7d2c  nalytics.com" },
 000000d0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 000000e0: 203d 2022 4120 736d 616c 6c20 6578 616d   = "A small exam
 000000f0: 706c 6520 7061 636b 6167 6520 666f 7220  ple package for
```

