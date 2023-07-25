# Comparing `tmp/concurrent_plugin-0.5.5-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 37647 bytes, number of entries: 19
+Zip file size: 37677 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx        2 b- defN 23-Jul-23 17:03 concurrent_plugin/__init__.py
 -rw-rw-r--  2.0 unx    42966 b- defN 23-Jul-23 17:21 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 23-Jul-23 17:21 concurrent_plugin/concurrent_core.py
--rw-rw-r--  2.0 unx    14403 b- defN 23-Jul-23 23:32 concurrent_plugin/concurrent_deployment.py
+-rw-rw-r--  2.0 unx    14530 b- defN 23-Jul-25 18:30 concurrent_plugin/concurrent_deployment.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Jul-23 17:21 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 23-Jul-23 17:21 concurrent_plugin/periodic_run.py
 -rw-rw-r--  2.0 unx     2091 b- defN 23-Jul-23 17:21 concurrent_plugin/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-23 17:03 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/mount_main.py
 -rw-rw-r--  2.0 unx    15974 b- defN 23-Jul-23 17:21 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      205 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx      268 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1750 b- defN 23-Jul-23 23:36 concurrent_plugin-0.5.5.dist-info/RECORD
-19 files, 133920 bytes uncompressed, 34725 bytes compressed:  74.1%
+-rw-rw-r--  2.0 unx      205 b- defN 23-Jul-25 18:31 concurrent_plugin-0.5.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 18:31 concurrent_plugin-0.5.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      268 b- defN 23-Jul-25 18:31 concurrent_plugin-0.5.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jul-25 18:31 concurrent_plugin-0.5.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1750 b- defN 23-Jul-25 18:31 concurrent_plugin-0.5.6.dist-info/RECORD
+19 files, 134047 bytes uncompressed, 34755 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.5.5.dist-info/METADATA
+Filename: concurrent_plugin-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.5.5.dist-info/WHEEL
+Filename: concurrent_plugin-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.5.5.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.5.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.5.dist-info/top_level.txt
+Filename: concurrent_plugin-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.5.dist-info/RECORD
+Filename: concurrent_plugin-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_deployment.py

```diff
@@ -129,14 +129,16 @@
                 body['resources.requests.hugepages'] = config['resources.requests.hugepages']
             if "resources.requests.nvidia.com/gpu" in config:
                 body['resources.requests.nvidia.com/gpu'] = config['resources.requests.nvidia.com/gpu']
             if 'kube-namespace' in config:
                 body['namespace'] = config['kube-namespace']
             else:
                 body['namespace'] = 'default'
+            if "optimizer-technology" in config:
+                body['optimizer-technology'] = config['optimizer-technology']
         kube_context = config.get('kube-context')
         if kube_context:
             body['kube_context'] = kube_context
 
         cognito_client_id, _, _, _, region = get_conf()
         token = get_token(cognito_client_id, region, True)
```

## Comparing `concurrent_plugin-0.5.5.dist-info/RECORD` & `concurrent_plugin-0.5.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
 concurrent_plugin/concurrent_backend.py,sha256=dASijwn_zQVckPJyqguBhqXyhZnReAUqUWXKKSGrqxo,42966
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
-concurrent_plugin/concurrent_deployment.py,sha256=57d9oLvzzDs1GWYNEfmfcyCGWEga-WLjW7oHiL4lA-8,14403
+concurrent_plugin/concurrent_deployment.py,sha256=nGxqLf3zb9i_Ou47v8MKKOqP3F81X2hGmRfKo6i4SLk,14530
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/utils.py,sha256=NpAWse8mKJkP_cyxLuCFizfVe2JjuyWkQWRGbBRjf9w,2091
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
 concurrent_plugin/infinfs/mount_service.py,sha256=G6jpVhFClkiwAoUyp4R35wTrhOzg23MA5-XZkyAWHX0,15974
-concurrent_plugin-0.5.5.dist-info/METADATA,sha256=zUnZ5E25g3bp33j6QrMPmH-FM_JFRBu0jNf8XQybHDw,205
-concurrent_plugin-0.5.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.5.5.dist-info/entry_points.txt,sha256=OOh9nvgYMGXymz5yNb-XEL0dM2cMrSIhh5HQNOOBFNY,268
-concurrent_plugin-0.5.5.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.5.5.dist-info/RECORD,,
+concurrent_plugin-0.5.6.dist-info/METADATA,sha256=dpsX8SLgPBjCcFfgbPrGNk1JLSoAyaMJfVUY3upfHvM,205
+concurrent_plugin-0.5.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.5.6.dist-info/entry_points.txt,sha256=OOh9nvgYMGXymz5yNb-XEL0dM2cMrSIhh5HQNOOBFNY,268
+concurrent_plugin-0.5.6.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.5.6.dist-info/RECORD,,
```

