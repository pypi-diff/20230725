# Comparing `tmp/metabengine-0.0.3.tar.gz` & `tmp/metabengine-0.0.4.tar.gz`

## Comparing `metabengine-0.0.3.tar` & `metabengine-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/__init__.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/alignment.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/ann_feat_quality.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/calculate_mass.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/feat_extract.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/feature_grouping.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/msms.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/params.py
--rw-r--r--   0        0        0    13616 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/peak_detect.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/raw_data_utils.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/targeted_search.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.3/src/metabengine/visual.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.3/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.3/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/alignment.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/ann_feat_quality.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/calculate_mass.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/feat_extract.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/feature_grouping.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/msms.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/params.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/peak_detect.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/raw_data_utils.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/targeted_search.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.4/src/metabengine/visual.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.4/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.4/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.4/PKG-INFO
```

### Comparing `metabengine-0.0.3/src/metabengine/__init__.py` & `metabengine-0.0.4/src/metabengine/feat_extract.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
     cross_file_params = Cross_file_params()
 
     for file_name in file_names:
         d = feat_detection(file_name)
         alignement(feature_list, d, cross_file_params)
     
-    return feature_list
+    return feature_list
```

### Comparing `metabengine-0.0.3/src/metabengine/alignment.py` & `metabengine-0.0.4/src/metabengine/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,27 @@
         self.mz_seq = np.concatenate((np.full(file_count, np.nan), self.mz_seq))
         self.rt_seq = np.concatenate((np.full(file_count, np.nan), self.rt_seq))
         self.height_seq = np.concatenate((np.full(file_count, 0.0), self.height_seq))
         self.area_seq = np.concatenate((np.full(file_count, 0.0), self.area_seq))
         self.average_height_seq = np.concatenate((np.full(file_count, 0.0), self.average_height_seq))
         self.ms2_seq = [None] * file_count + self.ms2_seq
 
+    
+    def choose_best_ms2(self):
+        """
+        A function to choose the best MS2 for the feature. 
+        The best MS2 is the one with the highest summed intensity.
+        """
+
+        if len(self.ms2_seq) > 1:
+            total_ints = [np.sum(ms2.prod_int_seq) for ms2 in self.ms2_seq]
+            self.best_ms2 = self.ms2_seq[np.argmax(total_ints)]
+        else:
+            self.best_ms2 = self.ms2_seq[0]
+
 
 def find_roi_from_data(feat, d, cross_file_params):
     """
     A function to find the feature from the MS data.
 
     Parameters
     ----------------------------------------------------------
```

### Comparing `metabengine-0.0.3/src/metabengine/ann_feat_quality.py` & `metabengine-0.0.4/src/metabengine/ann_feat_quality.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/calculate_mass.py` & `metabengine-0.0.4/src/metabengine/calculate_mass.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/feat_extract.py` & `metabengine-0.0.4/src/metabengine/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 def feat_detection(file_name, pred_quality_NN=False, annotate_isotope=False, output_single_file=False, path=None):
 
     d = raw.MSData()
     params = Params()
     d.read_raw_data(file_name, params)
     params.estimate_params(d)
-    print(params.int_tol)
     d.drop_ion_by_int(params)
     d.find_rois(params)
     d.cut_rois(params)
     d.process_rois(params)
 
     if pred_quality_NN:
         predict_quality(d)
@@ -36,10 +35,15 @@
 
     feature_list = []
 
     cross_file_params = Cross_file_params()
 
     for file_name in file_names:
         d = feat_detection(file_name)
+        print('Running alignment on: ', file_name)
         alignement(feature_list, d, cross_file_params)
     
-    return feature_list
+    # choose the best MS2 for each feature
+    for feat in feature_list:
+        feat.choose_best_ms2()
+    
+    return feature_list
```

### Comparing `metabengine-0.0.3/src/metabengine/feature_grouping.py` & `metabengine-0.0.4/src/metabengine/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/msms.py` & `metabengine-0.0.4/src/metabengine/msms.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/params.py` & `metabengine-0.0.4/src/metabengine/params.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/peak_detect.py` & `metabengine-0.0.4/src/metabengine/peak_detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,8 +412,10 @@
     def find_best_ms2(self):
         """
         Function to find the best MS2 spectrum of the ROI.
         """
 
         if len(self.ms2_seq) > 1:
             total_ints = [np.sum(ms2.prod_int_seq) for ms2 in self.ms2_seq]
-            self.best_ms2 = self.ms2_seq[np.argmax(total_ints)]
+            self.best_ms2 = self.ms2_seq[np.argmax(total_ints)]
+        else:
+            self.best_ms2 = self.ms2_seq[0]
```

### Comparing `metabengine-0.0.3/src/metabengine/raw_data_utils.py` & `metabengine-0.0.4/src/metabengine/raw_data_utils.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/src/metabengine/targeted_search.py` & `metabengine-0.0.4/src/metabengine/targeted_search.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/LICENSE` & `metabengine-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.3/pyproject.toml` & `metabengine-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metabengine"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Data preprocessing for mass spectrometry-based metabolomics data"
```

### Comparing `metabengine-0.0.3/PKG-INFO` & `metabengine-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabengine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data preprocessing for mass spectrometry-based metabolomics data
 Project-URL: Homepage, https://github.com/Waddlessss/metabengine
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

