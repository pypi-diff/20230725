# Comparing `tmp/statwolfACME-2.1.3-py2.py3-none-any.whl.zip` & `tmp/statwolfACME-2.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13667 bytes, number of entries: 10
--rw-r--r--  2.0 unx    18082 b- defN 23-May-31 14:59 ACME/ACME.py
+Zip file size: 13785 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    19035 b- defN 23-Jul-25 09:48 ACME/ACME.py
 -rw-r--r--  2.0 unx     3899 b- defN 23-Jul-05 13:20 ACME/ACME_anomaly_detection.py
 -rw-r--r--  2.0 unx    15589 b- defN 23-Feb-06 08:58 ACME/ACME_function.py
--rw-r--r--  2.0 unx     8177 b- defN 23-Jul-05 13:44 ACME/ACME_plot.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Jul-25 10:21 ACME/ACME_plot.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 08:44 ACME/__init__.py
 -rw-r--r--  2.0 unx      596 b- defN 23-Jan-31 08:44 ACME/utils.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/RECORD
-10 files, 47989 bytes uncompressed, 12371 bytes compressed:  74.2%
+-rw-r--r--  2.0 unx      765 b- defN 23-Jul-25 10:37 statwolfACME-2.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 10:37 statwolfACME-2.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-25 10:37 statwolfACME-2.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-Jul-25 10:37 statwolfACME-2.1.4.dist-info/RECORD
+10 files, 48946 bytes uncompressed, 12489 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: ACME/__init__.py
 Comment: 
 
 Filename: ACME/utils.py
 Comment: 
 
-Filename: statwolfACME-2.1.3.dist-info/METADATA
+Filename: statwolfACME-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: statwolfACME-2.1.3.dist-info/WHEEL
+Filename: statwolfACME-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: statwolfACME-2.1.3.dist-info/top_level.txt
+Filename: statwolfACME-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: statwolfACME-2.1.3.dist-info/RECORD
+Filename: statwolfACME-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ACME/ACME.py

```diff
@@ -295,22 +295,32 @@
         # if plot return plot, else return the table
         if plot:
             fig = feature_exploration_plot(feature_table, feature, self._task)
             return fig
         else:
             return feature_table
 
-    def summary_plot(self, local=False):
+    def summary_plot(self, local=False, weights = {}):
         '''
         Generate the recap plot
 
         Params: 
         -------
         - local : bool
             if local or global plot 
+        - weights : dict
+            Dictionary with the importance for each element used in AD. Sum must be 1
+                * ratio : float
+                    importance of local score position
+                * distance : float
+                    importance of inter-quantile distance necessary to change
+                * change : float
+                    importance of the possibility to change prediction
+                * delta : float
+                    importance of the score delta
         
         Returns:
         --------
         - plotly figure
         '''
 
         # if desired explainability is global, task is classification and there are multi label: produce the bar plot
@@ -328,20 +338,27 @@
                 meta['local'] = False
                 
             if local:
                 table = self._local_explain['meta']
                 meta['local'] = True
                 meta['index'] = self._local_explain['local_name']
                 meta['baseline'] = self._local_explain['baseline_pred']
+
+                if self._task in ['ad','anomaly detection']:
+                    local_table = self._local_explain['meta'].drop(columns='size').copy()
+                    importance_df = computeAnomalyDetectionImportance(local_table, weights = weights)
+                    table = table.drop(columns=['importance'])
+                    table = table.merge(importance_df[['importance']],left_index=True,right_index=True)
+                    
             else:
                 table = self._global_explain['meta']
                 meta['local'] = False
 
             # prepare for the plotting
-            plot_df = table.sort_values(['importance','original']).reset_index().rename(columns={'index':'feature'}).copy()
+            plot_df = table.sort_values(['importance','quantile']).reset_index().rename(columns={'index':'feature'}).copy()
 
             # if local set the refering x to the local values observation
             # for the global set to 0
             if local:
                 meta['x'] = table['baseline_prediction'].values[0]
             else: 
                 meta['x'] = 0
```

## ACME/ACME_plot.py

```diff
@@ -67,15 +67,15 @@
             title = title + ' : regression ' 
         elif meta['task'] in ['ad','anomaly detection']:
             title = title + ' : anomaly detection '
         else:
             title = title + ' : classification. Label_class : ' + str(meta['label_class'])       
 
     #set the color for the local score line
-    if (meta['local'] is not None) and (meta['task'] in ['ad','anomaly detection']):
+    if meta['local'] and (meta['task'] in ['ad','anomaly detection']):
         color_local = 'red' if meta['x'] > 0 else 'blue' 
     else:
         color_local = 'black'
     
     # draw plot
     fig = px.scatter(round(plot_df,3), 
                         x = 'predict' if meta['local'] else 'effect', 
@@ -91,15 +91,15 @@
                     x0 = meta['x'], y0 = y_bottom, 
                     x1 = meta['x'], y1 = y_top, 
                     line = dict(color = color_local, 
                                 width = 2,
                                 dash = 'dash')
                     )]
     # if anomaly detection add a line that marks the thresholds for state changing
-    if meta['task'] in meta['task'] in ['ad','anomaly detection']:
+    if meta['task'] in meta['task'] in ['ad','anomaly detection'] and meta['local']:
         shapes = shapes + [dict( 
                                     type='line', 
                                     x0 = 0.5, y0 = y_bottom, 
                                     x1 = 0.5, y1 = y_top, 
                                     line = dict(color = 'black', 
                                                 width = 2,
                                                 dash = 'solid')
```

## Comparing `statwolfACME-2.1.3.dist-info/METADATA` & `statwolfACME-2.1.4.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statwolfACME
-Version: 2.1.3
+Version: 2.1.4
 Summary: ACME - Accelerated Model Explainability
 Home-page: https://github.com/dandolodavid/ACME
 Author: Dandolo David
 Author-email: dandolodavid@gmail.com
 License: BSD 4-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

