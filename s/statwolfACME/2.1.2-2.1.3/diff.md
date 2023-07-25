# Comparing `tmp/statwolfACME-2.1.2-py2.py3-none-any.whl.zip` & `tmp/statwolfACME-2.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13669 bytes, number of entries: 10
+Zip file size: 13667 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    18082 b- defN 23-May-31 14:59 ACME/ACME.py
--rw-r--r--  2.0 unx     3993 b- defN 23-Feb-02 14:51 ACME/ACME_anomaly_detection.py
+-rw-r--r--  2.0 unx     3899 b- defN 23-Jul-05 13:20 ACME/ACME_anomaly_detection.py
 -rw-r--r--  2.0 unx    15589 b- defN 23-Feb-06 08:58 ACME/ACME_function.py
--rw-r--r--  2.0 unx     8172 b- defN 23-May-31 14:36 ACME/ACME_plot.py
+-rw-r--r--  2.0 unx     8177 b- defN 23-Jul-05 13:44 ACME/ACME_plot.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 08:44 ACME/__init__.py
 -rw-r--r--  2.0 unx      596 b- defN 23-Jan-31 08:44 ACME/utils.py
--rw-r--r--  2.0 unx      765 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-May-31 15:02 statwolfACME-2.1.2.dist-info/RECORD
-10 files, 48078 bytes uncompressed, 12373 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx      765 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-Jul-25 08:40 statwolfACME-2.1.3.dist-info/RECORD
+10 files, 47989 bytes uncompressed, 12371 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: ACME/__init__.py
 Comment: 
 
 Filename: ACME/utils.py
 Comment: 
 
-Filename: statwolfACME-2.1.2.dist-info/METADATA
+Filename: statwolfACME-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: statwolfACME-2.1.2.dist-info/WHEEL
+Filename: statwolfACME-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: statwolfACME-2.1.2.dist-info/top_level.txt
+Filename: statwolfACME-2.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: statwolfACME-2.1.2.dist-info/RECORD
+Filename: statwolfACME-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ACME/ACME_anomaly_detection.py

```diff
@@ -14,16 +14,16 @@
     Returns:
     --------
     - feature_table : pd.DataFrame
     '''
     # calculate the effect 
     feature_table = local_table.loc[feature].copy()
     feature_table['direction'] = 'normal'
-    feature_table.loc[feature_table['predict'] > 0,'direction'] = 'anomalies'
-    feature_table['effect'] = np.abs(feature_table['baseline_prediction'] - feature_table['predict']) * np.sign(-2*(feature_table['baseline_prediction']>feature_table['predict']).astype(int)+1)
+    feature_table.loc[feature_table['predict'] > 0.5,'direction'] = 'anomalies'
+    feature_table['effect'] = feature_table['predict'] - feature_table['baseline_prediction']
 
     return feature_table
 
 def computeAnomalyDetectionImportance(local_table, weights={}):
     '''
     Compute the anomaly detection importance.
 
@@ -63,15 +63,16 @@
     for feature in local_table.index.unique():
         
         importance[feature] = {}
 
         tmp = local_table.loc[feature]
 
         # search when the sign changes
-        tmp['sign_change'] = (np.sign(tmp['baseline_prediction']) != np.sign(tmp['predict'])).astype(int)
+        tmp['state_pred_change'] = (np.sign(tmp['baseline_prediction']*2-1) != np.sign(tmp['predict']*2-1)).astype(int)
+
         tmp = tmp.reset_index(drop=True)
         # calculate quantile distance
         tmp['quantile_distance'] = np.abs(tmp['quantile']-tmp['baseline_quantile'])
 
         # local actual score
         local_score = tmp['baseline_prediction'].values[0]
 
@@ -79,25 +80,25 @@
         min_score = min(tmp['predict'].min(),local_score)
         max_score = max(tmp['predict'].max(),local_score)
 
         #delta of the score
         delta = np.abs( max_score - min_score )
 
         #ratio 
-        ratio = (local_score - min_score)/delta
+        ratio = local_score - min_score
         
         # change
-        if np.sign(min_score) !=  np.sign(max_score):
+        if min_score<0.5 and max_score>=0.5:
             change=1
         else:
             change=0
         
         # number of quantile required to change the state 
         if change == 1:
-            distance = tmp.loc[tmp['sign_change']==1,'quantile_distance'].min() 
+            distance = tmp.loc[tmp['state_pred_change']==1,'quantile_distance'].min() 
         else:
             distance = 1
 
         importance[feature]['ratio'] = ratio
         importance[feature]['delta'] = delta
         importance[feature]['change'] = change
         importance[feature]['distance_to_change'] = distance
```

## ACME/ACME_plot.py

```diff
@@ -94,16 +94,16 @@
                                 width = 2,
                                 dash = 'dash')
                     )]
     # if anomaly detection add a line that marks the thresholds for state changing
     if meta['task'] in meta['task'] in ['ad','anomaly detection']:
         shapes = shapes + [dict( 
                                     type='line', 
-                                    x0 = 0, y0 = y_bottom, 
-                                    x1 = 0, y1 = y_top, 
+                                    x0 = 0.5, y0 = y_bottom, 
+                                    x1 = 0.5, y1 = y_top, 
                                     line = dict(color = 'black', 
                                                 width = 2,
                                                 dash = 'solid')
                                     )]
 
     fig.update_layout(shapes=shapes)
     
@@ -135,61 +135,61 @@
     fig = go.Figure()
     # score and values of the baseline prediction (if local the baseline is the local observation)
     actual_score = table['baseline_prediction'].values[0]
     actual_values = table.loc[table['quantile'] == table['baseline_quantile'].values[0], 'original'].values[0]
 
     # set colors based on task
     if task in ['ad','anomaly detection']:
-        color = 'red' if actual_score > 0 else 'blue'
+        color = 'red' if actual_score >= 0.5 else 'blue'
     else: 
         color = 'black'
 
     # set the dictionary with the names to use in the plot
     plot_meta = {}
     if task in ['ad','anomaly detection']:
         plot_meta['lower_trace'] = {'name' : 'normal', 'value':'normal'}
         plot_meta['upper_trace'] = {'name' : 'anomalies', 'value':'anomalies'}
     else:
         plot_meta['lower_trace'] = {'name' : 'lower', 'value':'lower'}
         plot_meta['upper_trace'] = {'name' : 'upper', 'value':'upper'}
 
     # add effects that pushes the score to anomaly state
-    fig.add_bar(x = table.loc[table.direction ==  plot_meta['lower_trace']['value'],'effect'], 
-                y = table.loc[table.direction ==  plot_meta['lower_trace']['value'],'original'].values, 
+    fig.add_bar(x = table.loc[table['direction'] ==  plot_meta['upper_trace']['value'],'effect'], 
+                y = table.loc[table['direction'] ==  plot_meta['upper_trace']['value'],'original'].values, 
                 base = table['baseline_prediction'].values[0], 
-                marker = dict(color = 'blue'), 
+                marker = dict(color = 'red'), 
                 hovertemplate = 'Prediction: %{x}<br>Feature value: %{y}',
-                name =  plot_meta['lower_trace']['name'], orientation='h')
+                name =  plot_meta['upper_trace']['name'], orientation='h')
 
     # add effects that pushes the score to normal state
-    fig.add_bar(x = table.loc[table.direction == plot_meta['upper_trace']['value'],'effect'], 
-                y = table.loc[table.direction == plot_meta['upper_trace']['value'],'original'].values, 
+    fig.add_bar(x = table.loc[table['direction'] == plot_meta['lower_trace']['value'],'effect'], 
+                y = table.loc[table['direction'] == plot_meta['lower_trace']['value'],'original'].values, 
                 base = table['baseline_prediction'].values[0],
-                marker = dict(color = 'red'),
+                marker = dict(color = 'blue'),
                 hovertemplate = 'Prediction: %{x}<br>Feature value: %{y}',
-                name =  plot_meta['upper_trace']['name'], orientation='h')
+                name =  plot_meta['lower_trace']['name'], orientation='h')
 
     # add a line that marks the actual state
-    fig.add_scatter(y = [ table['original'].values[0]*0.9 ,table['original'].values[-1]*1.05 ],
+    fig.add_scatter(y = [ table['original'].min()*0.9 ,table['original'].max()*1.05 ],
                     x = [ actual_score,actual_score ], 
                     mode ='lines', 
                     hovertemplate = 'Actual '+ 'score' if task in ['ad','anomaly detection'] else 'prediction',
                     name = 'actual score', line = dict(color = color ,width=2,dash="dash") )
 
     # add a great point corrisponding to the the actual score
     fig.add_scatter( x = [actual_score],
                     y = [actual_values], mode='markers',
                     
                     hovertemplate = 'Actual feature value<br> '+ 'Prediction: %{x}<br>Value: %{y}',
                     marker = dict(size=20,color=color),  name = 'current value')
     
     # add a line that marks the thresholds for state changing
     if task in ['ad','anomaly detection']:
-        fig.add_scatter( y = [ table['original'].values[0]*0.9, table['original'].values[-1]*1.05 ],
-                         x = [ 0,0 ], 
+        fig.add_scatter( y = [ table['original'].min()*0.9, table['original'].max()*1.05 ],
+                         x = [ 0.5,0.5 ], 
                          mode='lines',
                          
                          hovertemplate = 'Changepoint',
                          line=dict(color="black",width=2),  name = 'change point')
 
     fig.update_layout(  title='Feature ' + str(feature), 
                         yaxis_title = 'feature values',
```

## Comparing `statwolfACME-2.1.2.dist-info/METADATA` & `statwolfACME-2.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statwolfACME
-Version: 2.1.2
+Version: 2.1.3
 Summary: ACME - Accelerated Model Explainability
 Home-page: https://github.com/dandolodavid/ACME
 Author: Dandolo David
 Author-email: dandolodavid@gmail.com
 License: BSD 4-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

## Comparing `statwolfACME-2.1.2.dist-info/RECORD` & `statwolfACME-2.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ACME/ACME.py,sha256=UccJd_hw_Qxs73Iehnky2htPLXCC2zSg8VC7QSzr7ZY,18082
-ACME/ACME_anomaly_detection.py,sha256=-OAT6JPmiI2UpSJpjjTrgrW0fPdGu7XDHLe_F_KNPM0,3993
+ACME/ACME_anomaly_detection.py,sha256=HIzIqfHZd-M1vC8Y-BprOIuWXmYzd0qp7DDpKHo48HQ,3899
 ACME/ACME_function.py,sha256=9EN-agizCTpyNKvRp0Ag-JY4YqN3jITU4iBESGRrTno,15589
-ACME/ACME_plot.py,sha256=5wGU9PzNREzgUvUGlIj0Om7ps0zJ0RVZu-xVJ-2EZKo,8172
+ACME/ACME_plot.py,sha256=q3Mtfz3C_-od_wE0JOpnlbFPv0T2UDpqiblNfim1w_c,8177
 ACME/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ACME/utils.py,sha256=lCpTKX1VOxRiOcujxQlzmzutuHp9DSoJMV1hFV-OKhc,596
-statwolfACME-2.1.2.dist-info/METADATA,sha256=6_kIL_BVRNm3_lxvPC_666lPw-FObMoc_p_yz6gy5aA,765
-statwolfACME-2.1.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-statwolfACME-2.1.2.dist-info/top_level.txt,sha256=Vmikm8I41738ZA9Dvu56w4VR3KLdVEkscgrMEyxUJfM,5
-statwolfACME-2.1.2.dist-info/RECORD,,
+statwolfACME-2.1.3.dist-info/METADATA,sha256=wM_ZrY-A2mSPZVIXXCuot_zUVVE3PpSe8yPHqCnVk0M,765
+statwolfACME-2.1.3.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+statwolfACME-2.1.3.dist-info/top_level.txt,sha256=Vmikm8I41738ZA9Dvu56w4VR3KLdVEkscgrMEyxUJfM,5
+statwolfACME-2.1.3.dist-info/RECORD,,
```

