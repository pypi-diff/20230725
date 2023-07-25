# Comparing `tmp/finterion_investing_algorithm_framework-0.2-py3-none-any.whl.zip` & `tmp/finterion_investing_algorithm_framework-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10404 bytes, number of entries: 13
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/__init__.py
--rw-r--r--  2.0 unx     1388 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/create_app.py
--rw-r--r--  2.0 unx      197 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/exceptions.py
--rw-r--r--  2.0 unx     1813 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/market_service.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/configuration/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/configuration/constants.py
--rw-r--r--  2.0 unx      176 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/models/__init__.py
--rw-r--r--  2.0 unx      515 b- defN 23-Jul-25 09:59 finterion_investing_algorithm_framework/models/portfolio_configuration.py
--rw-r--r--  2.0 unx    11343 b- defN 23-Jul-25 10:00 finterion_investing_algorithm_framework-0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3287 b- defN 23-Jul-25 10:00 finterion_investing_algorithm_framework-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 10:00 finterion_investing_algorithm_framework-0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Jul-25 10:00 finterion_investing_algorithm_framework-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1462 b- defN 23-Jul-25 10:00 finterion_investing_algorithm_framework-0.2.dist-info/RECORD
-13 files, 20615 bytes uncompressed, 7824 bytes compressed:  62.0%
+Zip file size: 10393 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/create_app.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/exceptions.py
+-rw-r--r--  2.0 unx     1813 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/market_service.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/configuration/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/configuration/constants.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/models/__init__.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Jul-25 16:07 finterion_investing_algorithm_framework/models/portfolio_configuration.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-Jul-25 16:08 finterion_investing_algorithm_framework-0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3287 b- defN 23-Jul-25 16:08 finterion_investing_algorithm_framework-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 16:08 finterion_investing_algorithm_framework-0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-25 16:08 finterion_investing_algorithm_framework-0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1462 b- defN 23-Jul-25 16:08 finterion_investing_algorithm_framework-0.4.dist-info/RECORD
+13 files, 20571 bytes uncompressed, 7813 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: finterion_investing_algorithm_framework/models/__init__.py
 Comment: 
 
 Filename: finterion_investing_algorithm_framework/models/portfolio_configuration.py
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.2.dist-info/LICENSE
+Filename: finterion_investing_algorithm_framework-0.4.dist-info/LICENSE
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.2.dist-info/METADATA
+Filename: finterion_investing_algorithm_framework-0.4.dist-info/METADATA
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.2.dist-info/WHEEL
+Filename: finterion_investing_algorithm_framework-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.2.dist-info/top_level.txt
+Filename: finterion_investing_algorithm_framework-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.2.dist-info/RECORD
+Filename: finterion_investing_algorithm_framework-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## finterion_investing_algorithm_framework/create_app.py

```diff
@@ -25,27 +25,24 @@
     logger.info(
         f"Running algorithm {model['name']} in "
         f"environment {model['environment']}"
     )
     portfolio_configuration = LogicfundsPortfolioConfiguration(
         api_key=api_key, trading_symbol=model['profile']['trading_symbol']
     )
-
     app = framework_create_app(
         config=config, web=web, stateless=stateless, initialize=initialize
     )
     app.container.market_service.override(
         FinterionMarketService(api_key=api_key)
     )
     app.add_portfolio_configuration(portfolio_configuration)
 
-    if not stateless:
-        class PingTask(Task):
-            interval = 1
-            time_unit = TimeUnit.HOUR
-
-            def run(self, algorithm):
-                client.ping()
+    class PingTask(Task):
+        interval = 30
+        time_unit = TimeUnit.MINUTES
 
-        app.add_task(PingTask)
+        def run(self, algorithm):
+            client.ping()
 
+    app.add_task(PingTask)
     return app
```

## Comparing `finterion_investing_algorithm_framework-0.2.dist-info/LICENSE` & `finterion_investing_algorithm_framework-0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `finterion_investing_algorithm_framework-0.2.dist-info/METADATA` & `finterion_investing_algorithm_framework-0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion-investing-algorithm-framework
-Version: 0.2
+Version: 0.4
 Summary: Official Finterion plugin for the investing algorithm framework
 Home-page: https://github.com/finterion/finterion-investing-algorithm-framework.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,investing-algorithm-framework,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

## Comparing `finterion_investing_algorithm_framework-0.2.dist-info/RECORD` & `finterion_investing_algorithm_framework-0.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 finterion_investing_algorithm_framework/__init__.py,sha256=u-srn87VlLUPUJHWR5hgMAHqw2BWtb1v0eH0tQ8M16w,107
-finterion_investing_algorithm_framework/create_app.py,sha256=zPwITKndkPwkN5C0oTxZm4SJzPVlc-UkLySnCkRm0Sg,1388
+finterion_investing_algorithm_framework/create_app.py,sha256=T_W0JfiYSc-rueWz_oJeRx0HzJvU_Fpin3DPU_4M-nk,1344
 finterion_investing_algorithm_framework/exceptions.py,sha256=KOaDjHQC7vNpKwYYNxJ2nuaJYceMmvExW3BLSzPSWJk,197
 finterion_investing_algorithm_framework/market_service.py,sha256=RPCBJi3L5S7rhmn5XCB3K4PHQxsjTGFyWvxAw4b-O3Y,1813
 finterion_investing_algorithm_framework/configuration/__init__.py,sha256=370OXcHya0GtGhrA59sIuznTYSn8xJy-dciCOSTsfl8,102
 finterion_investing_algorithm_framework/configuration/constants.py,sha256=bhabsdZ8omPvAZlQmdPGM70vHQHS2pcJm2olpkSEciU,93
 finterion_investing_algorithm_framework/models/__init__.py,sha256=96Cq_doBIVXfK9OJW3SnMTiXx9WPnd9LITlpT5vEFzw,176
 finterion_investing_algorithm_framework/models/portfolio_configuration.py,sha256=1QesgEDUDoPk50ZFsDZFpFNldP_PExoUgdhKHp3w908,515
-finterion_investing_algorithm_framework-0.2.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
-finterion_investing_algorithm_framework-0.2.dist-info/METADATA,sha256=8M46rR3f7_07evNWpdPfYx1cCpCbTXQH836BqsZ-0z4,3287
-finterion_investing_algorithm_framework-0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-finterion_investing_algorithm_framework-0.2.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
-finterion_investing_algorithm_framework-0.2.dist-info/RECORD,,
+finterion_investing_algorithm_framework-0.4.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
+finterion_investing_algorithm_framework-0.4.dist-info/METADATA,sha256=whjtPG8xSgCDhHrW74ooGZEzPJV9ZJYKOKhIcWL2M8A,3287
+finterion_investing_algorithm_framework-0.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+finterion_investing_algorithm_framework-0.4.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
+finterion_investing_algorithm_framework-0.4.dist-info/RECORD,,
```

