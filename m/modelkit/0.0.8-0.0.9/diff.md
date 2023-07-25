# Comparing `tmp/modelkit-0.0.8-py3-none-any.whl.zip` & `tmp/modelkit-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 62174 bytes, number of entries: 58
--rw-r--r--  2.0 unx      304 b- defN 21-Jun-21 12:06 modelkit/__init__.py
+Zip file size: 61919 bytes, number of entries: 58
+-rw-r--r--  2.0 unx      304 b- defN 21-Jun-21 13:01 modelkit/__init__.py
 -rw-r--r--  2.0 unx     5815 b- defN 21-Jun-18 08:16 modelkit/api.py
 -rw-r--r--  2.0 unx     8654 b- defN 21-Jun-18 08:16 modelkit/cli.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-14 12:12 modelkit/py.typed
 -rw-r--r--  2.0 unx      334 b- defN 21-May-14 12:12 modelkit/assets/__init__.py
 -rw-r--r--  2.0 unx     8849 b- defN 21-Jun-14 19:25 modelkit/assets/cli.py
 -rw-r--r--  2.0 unx     2167 b- defN 21-Jun-10 18:33 modelkit/assets/errors.py
 -rw-r--r--  2.0 unx     6258 b- defN 21-Jun-21 12:06 modelkit/assets/manager.py
 -rw-r--r--  2.0 unx    11539 b- defN 21-Jun-21 10:40 modelkit/assets/remote.py
 -rw-r--r--  2.0 unx     4332 b- defN 21-Jun-20 18:19 modelkit/assets/settings.py
 -rw-r--r--  2.0 unx     1967 b- defN 21-May-14 12:12 modelkit/assets/versioning.py
 -rw-r--r--  2.0 unx      542 b- defN 21-Jun-10 09:20 modelkit/assets/drivers/__init__.py
 -rw-r--r--  2.0 unx     2815 b- defN 21-Jun-14 19:25 modelkit/assets/drivers/gcs.py
 -rw-r--r--  2.0 unx     2614 b- defN 21-Jun-14 19:25 modelkit/assets/drivers/local.py
 -rw-r--r--  2.0 unx      926 b- defN 21-Jun-10 18:33 modelkit/assets/drivers/retry.py
--rw-r--r--  2.0 unx     3259 b- defN 21-Jun-21 12:06 modelkit/assets/drivers/s3.py
+-rw-r--r--  2.0 unx     3056 b- defN 21-Jun-21 12:58 modelkit/assets/drivers/s3.py
 -rw-r--r--  2.0 unx       81 b- defN 21-May-24 08:16 modelkit/core/__init__.py
 -rw-r--r--  2.0 unx     5606 b- defN 21-Jun-20 18:19 modelkit/core/errors.py
 -rw-r--r--  2.0 unx    15873 b- defN 21-Jun-20 18:19 modelkit/core/library.py
 -rw-r--r--  2.0 unx    25778 b- defN 21-Jun-21 10:37 modelkit/core/model.py
 -rw-r--r--  2.0 unx     4352 b- defN 21-Jun-18 08:16 modelkit/core/model_configuration.py
 -rw-r--r--  2.0 unx     2291 b- defN 21-Jun-14 19:25 modelkit/core/settings.py
 -rw-r--r--  2.0 unx      650 b- defN 21-Jun-20 18:19 modelkit/core/types.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jun-10 18:33 modelkit/core/models/__init__.py
 -rw-r--r--  2.0 unx     3108 b- defN 21-Jun-21 10:37 modelkit/core/models/distant_model.py
--rw-r--r--  2.0 unx    13040 b- defN 21-Jun-21 10:37 modelkit/core/models/tensorflow_model.py
+-rw-r--r--  2.0 unx    13040 b- defN 21-Jun-21 12:40 modelkit/core/models/tensorflow_model.py
 -rw-r--r--  2.0 unx      523 b- defN 21-Jun-18 08:16 modelkit/testing/__init__.py
 -rw-r--r--  2.0 unx     3470 b- defN 21-Jun-18 08:16 modelkit/testing/fixtures.py
 -rw-r--r--  2.0 unx     3441 b- defN 21-May-24 08:16 modelkit/testing/reference.py
 -rw-r--r--  2.0 unx     1991 b- defN 21-Jun-18 08:16 modelkit/testing/tf_serving.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jun-16 14:16 modelkit/utils/__init__.py
 -rw-r--r--  2.0 unx     2794 b- defN 21-Jun-14 19:25 modelkit/utils/cache.py
 -rw-r--r--  2.0 unx      550 b- defN 21-Jun-10 18:33 modelkit/utils/logging.py
@@ -37,24 +37,24 @@
 -rw-r--r--  2.0 unx     1338 b- defN 21-Jun-10 18:33 modelkit/utils/pydantic.py
 -rw-r--r--  2.0 unx     1152 b- defN 21-Jun-14 19:25 modelkit/utils/redis.py
 -rw-r--r--  2.0 unx      257 b- defN 21-Jun-18 08:16 modelkit/utils/serialization.py
 -rw-r--r--  2.0 unx     2834 b- defN 21-Jun-18 08:16 modelkit/utils/tensorflow.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-14 12:12 tests/assets/__init__.py
 -rw-r--r--  2.0 unx     4416 b- defN 21-Jun-21 12:06 tests/assets/conftest.py
 -rw-r--r--  2.0 unx     4454 b- defN 21-Jun-14 19:25 tests/assets/test_asset_specification.py
--rw-r--r--  2.0 unx     5717 b- defN 21-Jun-21 12:06 tests/assets/test_assetsmanager.py
+-rw-r--r--  2.0 unx     4872 b- defN 21-Jun-21 13:00 tests/assets/test_assetsmanager.py
 -rw-r--r--  2.0 unx     2298 b- defN 21-Jun-10 18:33 tests/assets/test_assetsmanager_subpart.py
 -rw-r--r--  2.0 unx     3585 b- defN 21-Jun-10 18:33 tests/assets/test_assetsmanager_versioning.py
 -rw-r--r--  2.0 unx      883 b- defN 21-May-21 09:00 tests/assets/test_driver_errors.py
 -rw-r--r--  2.0 unx     1323 b- defN 21-May-28 13:08 tests/assets/test_drivers.py
 -rw-r--r--  2.0 unx     4741 b- defN 21-Jun-14 19:25 tests/assets/test_local_manager.py
 -rw-r--r--  2.0 unx     3254 b- defN 21-Jun-10 18:33 tests/assets/test_lock.py
 -rw-r--r--  2.0 unx     1272 b- defN 21-May-14 12:12 tests/assets/test_retry.py
 -rw-r--r--  2.0 unx     6376 b- defN 21-Jun-14 19:25 tests/assets/test_settings.py
 -rw-r--r--  2.0 unx     3323 b- defN 21-May-14 12:12 tests/assets/test_versioning.py
--rw-r--r--  2.0 unx     1065 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3754 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4884 b- defN 21-Jun-21 12:06 modelkit-0.0.8.dist-info/RECORD
-58 files, 204251 bytes uncompressed, 54428 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx     1065 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3754 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4884 b- defN 21-Jun-21 13:02 modelkit-0.0.9.dist-info/RECORD
+58 files, 203203 bytes uncompressed, 54173 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -150,26 +150,26 @@
 
 Filename: tests/assets/test_settings.py
 Comment: 
 
 Filename: tests/assets/test_versioning.py
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/LICENSE
+Filename: modelkit-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/METADATA
+Filename: modelkit-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/WHEEL
+Filename: modelkit-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/entry_points.txt
+Filename: modelkit-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/top_level.txt
+Filename: modelkit-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: modelkit-0.0.8.dist-info/RECORD
+Filename: modelkit-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## modelkit/__init__.py

```diff
@@ -4,8 +4,8 @@
 from modelkit.core.model import Model  # NOQA
 
 # Silence Tensorflow warnings
 # https://github.com/tensorflow/tensorflow/issues/30427
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## modelkit/assets/drivers/s3.py

```diff
@@ -39,19 +39,14 @@
             endpoint_url=settings.s3_endpoint,
             aws_access_key_id=settings.aws_access_key_id,
             aws_secret_access_key=settings.aws_secret_access_key,
             aws_session_token=settings.aws_session_token,
             region_name=settings.aws_default_region,
         )
         self.bucket = settings.bucket
-        try:
-            self.client.head_bucket(Bucket=self.bucket)
-        except self.client.exceptions.ClientError:
-            logger.error(f"Bucket {self.bucket} does not exist")
-            raise
 
     @retry(**RETRY_POLICY)
     def iterate_objects(self, prefix=None):
         paginator = self.client.get_paginator("list_objects_v2")
         pages = paginator.paginate(Bucket=self.bucket, Prefix=prefix or "")
         for page in pages:
             for obj in page.get("Contents", []):
```

## tests/assets/test_assetsmanager.py

```diff
@@ -134,28 +134,7 @@
                 asset_path=(
                     f"gs://{gcs_assetsmanager.remote_assets_store.bucket}/"
                     f"{gcs_assetsmanager.remote_assets_store.prefix}/"
                     "category-test"
                 ),
                 destination_dir=tmp_dir,
             )
-
-
-@skip_unless("ENABLE_S3_TEST", "True")
-def test_s3_assetsmanager_fail_on_init(s3_assetsmanager):
-    with tempfile.TemporaryDirectory() as tmp_d:
-        with pytest.raises(botocore.exceptions.ClientError):
-            AssetsManager(
-                assets_dir=tmp_d,
-                remote_store={
-                    "driver": {
-                        "storage_provider": "s3",
-                        "aws_default_region": "us-east-1",
-                        "bucket": "DOESNOTEXIST",
-                        "aws_access_key_id": "minioadmin",
-                        "aws_secret_access_key": "minioadmin",
-                        "aws_session_token": None,
-                        "s3_endpoint": "http://127.0.0.1:9000",
-                    },
-                    "storage_prefix": "test-assets-prefix",
-                },
-            )
```

## Comparing `modelkit-0.0.8.dist-info/LICENSE` & `modelkit-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `modelkit-0.0.8.dist-info/METADATA` & `modelkit-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine learning lib.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `modelkit-0.0.8.dist-info/RECORD` & `modelkit-0.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-modelkit/__init__.py,sha256=Fc0Nu5e0N2j6fELzEIJ_h56ejuD7e2-_1aIAJHXMzeY,304
+modelkit/__init__.py,sha256=V8NHTRMruFWyuq7BmHAzqRRnKMhnqUYmYktLvlKEYYA,304
 modelkit/api.py,sha256=OaaO8CKXeYe2AOshvkuj7zIo7dMcHVJCf4L1Q3Pbc_E,5815
 modelkit/cli.py,sha256=kJC85O8ae6jNTxlaz0CVlDAhqoeYR4IOzg99Em4-ZDY,8654
 modelkit/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modelkit/assets/__init__.py,sha256=QX9hlzrDXyGNtRWZiIF8xrHB8x5w8e-xnt8i9x65nVw,334
 modelkit/assets/cli.py,sha256=2Yd_L3aIzkbggZGYpNSkF8Zws4ChsmDexwluqmKGqQY,8849
 modelkit/assets/errors.py,sha256=OtdaKj7V4MFI9Qr9FkhtCDfvfEekbooyGA8nzX2dK4I,2167
 modelkit/assets/manager.py,sha256=tDd-Vk70_JUR-0w3UtuihH7ZTvmtkbKAWGqepLl9Iao,6258
 modelkit/assets/remote.py,sha256=3A_rIcvFg0R7FW9zM3iUfwX-HC5WekWwNhTCMijjLvk,11539
 modelkit/assets/settings.py,sha256=wLgjjYBSCw2uFf9t45up0a29YKoNuLrofhYD3lUi7Ro,4332
 modelkit/assets/versioning.py,sha256=avBMhJiRgar83UQUKiKDHDJ8P3jtRMx4YviG6m3P_b8,1967
 modelkit/assets/drivers/__init__.py,sha256=O5X2xuLmaJt7Hj0QAEBe9iF-sSw72-nxtoXBkes668s,542
 modelkit/assets/drivers/gcs.py,sha256=MBVrhP4mnM68FzioN7RVAl4OpZk780ATHj5zgjB2XvA,2815
 modelkit/assets/drivers/local.py,sha256=dGmC9XODP3YKgyz32JYkyab6tgz7I5zIbzU01CNWSOA,2614
 modelkit/assets/drivers/retry.py,sha256=Gs9-AKKMvg2YigD7cJoGHpxdbG1PZGZ3JmhpEaWl9WU,926
-modelkit/assets/drivers/s3.py,sha256=I98mM4wfYW7Mk1IawblVuEmNDPkZZgtgYVOyclSXsRo,3259
+modelkit/assets/drivers/s3.py,sha256=-GinIKsFRvjC1upbj-_pzWn-qBb6gBddD5uEAQj9vtc,3056
 modelkit/core/__init__.py,sha256=yktiL7RTNZwQF7YgGDmMt1ANP2MvM6GyEzTTnAQAhV8,81
 modelkit/core/errors.py,sha256=3Mb7peAMPYM50-mZ92TkOI9t9pTMLCSMrxT4ciS4VyA,5606
 modelkit/core/library.py,sha256=hsvTUdciZK_ozbGngJOKFDZcaju3J4IvTeMmAz0UKEE,15873
 modelkit/core/model.py,sha256=MD8dL8LDsHlWh3WZTU3V9SlxrkkRPxJXyVRwK5-MvQI,25778
 modelkit/core/model_configuration.py,sha256=6V7vRDbPhxiGojNCH2a7vV1fJOnhZcWvWSqPcUkhIGM,4352
 modelkit/core/settings.py,sha256=G7EWomCLE4ChRx-I20iydONhUdw-oUQVXCbMHJQd6mc,2291
 modelkit/core/types.py,sha256=DfF3drZbkTQLrmGPAprqqhTsmQwWxCufotUVUHRfPoE,650
@@ -36,23 +36,23 @@
 modelkit/utils/pydantic.py,sha256=U1CWDKofAsFQq7EztL5Xlk5xzehAFnpoX-BLla3lbpI,1338
 modelkit/utils/redis.py,sha256=l24RiNutW1sM1k4LnVYtEsLOLKYJiIUYvPpdU54xseY,1152
 modelkit/utils/serialization.py,sha256=MOvlmtU92XQs8i9ljooxvOdQwzhGGdwQgBTpNxtN1NU,257
 modelkit/utils/tensorflow.py,sha256=o2Ne1XUfhR051rDHlVCIBUZeEn75wZWueM8HYCY7Yew,2834
 tests/assets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/assets/conftest.py,sha256=1-HDJp_Hr4FW2dm9gDoOL7QHtVYPFtz41Xd-UCy2Um8,4416
 tests/assets/test_asset_specification.py,sha256=iHIo-2mmDx82VRzjsNhpsiSYiZu7NxvtEBiGeGDkLI0,4454
-tests/assets/test_assetsmanager.py,sha256=Cd-svBy7XZs0jy69rsrzFkAd_6yVEfpa6x9dghH51oQ,5717
+tests/assets/test_assetsmanager.py,sha256=zum8_mUv2Okang5qSzZW1ZB8CGqnI-dMMz5Pi4F50GE,4872
 tests/assets/test_assetsmanager_subpart.py,sha256=oMXn_YacIGVkoVwKzrtnVz3rHa7A701Pple3CE-BIJc,2298
 tests/assets/test_assetsmanager_versioning.py,sha256=fJtcBW6KwW2VVC7kTQuDJlk0uEnGe7o222kI05nreeU,3585
 tests/assets/test_driver_errors.py,sha256=WUk_pzibvGTpzt7_MF3Zj2SsUKkVV6482tbr4AXFgJM,883
 tests/assets/test_drivers.py,sha256=qnO8g2Soqhw3K4lozYqAQRWKBvsoeAU1AfdMLjY2GZ0,1323
 tests/assets/test_local_manager.py,sha256=dxJpynTOeJ-nkSMwAnAMYTlc7WlXmJXEUCZYerDh6QU,4741
 tests/assets/test_lock.py,sha256=OeE3fRiJYCHPAmSYOHVLmRhd46ki-ewPmr-Nl1w3g6k,3254
 tests/assets/test_retry.py,sha256=c0F4QEoi8c9Hi2hLvZ8YC1o-Hc1YIvqzDDegvkmJQtE,1272
 tests/assets/test_settings.py,sha256=Yjh7-e5TcDh4SI0tEXNDYdlXe003LXy--IqQNpPyMqA,6376
 tests/assets/test_versioning.py,sha256=1CvhsCj23dFi305jyw-zexkkmLJdvbmSrGB5Q25L8WA,3323
-modelkit-0.0.8.dist-info/LICENSE,sha256=AY_YUNuHVERA4k5DwH2074qEPb9bBs-f8InmNaLPXms,1065
-modelkit-0.0.8.dist-info/METADATA,sha256=eb5ZhDBjDYhh898ccdRKG4AQE88Cmm0v7tMlFWu4ztw,3754
-modelkit-0.0.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-modelkit-0.0.8.dist-info/entry_points.txt,sha256=qRII1ILaPW_159MYfdjlVZPLlhvCQ1Mmm6YckWgq_O0,56
-modelkit-0.0.8.dist-info/top_level.txt,sha256=zzLGVKkEFho6pvj8zN7c55FKCOMtwYr5VP3BQboTo5c,15
-modelkit-0.0.8.dist-info/RECORD,,
+modelkit-0.0.9.dist-info/LICENSE,sha256=AY_YUNuHVERA4k5DwH2074qEPb9bBs-f8InmNaLPXms,1065
+modelkit-0.0.9.dist-info/METADATA,sha256=7PjZG3TGobR6BGuMiM6eR_qs9U1MvCuEqG9KuhXOJJk,3754
+modelkit-0.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+modelkit-0.0.9.dist-info/entry_points.txt,sha256=qRII1ILaPW_159MYfdjlVZPLlhvCQ1Mmm6YckWgq_O0,56
+modelkit-0.0.9.dist-info/top_level.txt,sha256=zzLGVKkEFho6pvj8zN7c55FKCOMtwYr5VP3BQboTo5c,15
+modelkit-0.0.9.dist-info/RECORD,,
```

