# Comparing `tmp/armada_airflow-0.5.0-py3-none-any.whl.zip` & `tmp/armada_airflow-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20367 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:08 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:10 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Jul-21 22:10 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jul-21 22:10 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:08 armada/operators/__init__.py
--rw-r--r--  2.0 unx     6081 b- defN 23-Jul-21 22:08 armada/operators/armada.py
--rw-r--r--  2.0 unx     9671 b- defN 23-Jul-21 22:08 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     3080 b- defN 23-Jul-21 22:08 armada/operators/grpc.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Jul-21 22:08 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     2613 b- defN 23-Jul-21 22:08 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx    10090 b- defN 23-Jul-21 22:08 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3916 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/RECORD
-16 files, 58334 bytes uncompressed, 18081 bytes compressed:  69.0%
+Zip file size: 20377 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 14:59 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 15:05 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Jul-25 15:05 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jul-25 15:05 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 14:59 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     6170 b- defN 23-Jul-25 14:59 armada/operators/armada.py
+-rw-r--r--  2.0 unx     9671 b- defN 23-Jul-25 14:59 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     3080 b- defN 23-Jul-25 14:59 armada/operators/grpc.py
+-rw-r--r--  2.0 unx     3044 b- defN 23-Jul-25 14:59 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     2613 b- defN 23-Jul-25 14:59 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Jul-25 14:59 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3916 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/RECORD
+16 files, 58423 bytes uncompressed, 18091 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.5.0.dist-info/LICENSE
+Filename: armada_airflow-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.5.0.dist-info/METADATA
+Filename: armada_airflow-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.5.0.dist-info/WHEEL
+Filename: armada_airflow-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.5.0.dist-info/top_level.txt
+Filename: armada_airflow-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.5.0.dist-info/RECORD
+Filename: armada_airflow-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/armada.py

```diff
@@ -84,14 +84,15 @@
         super().__init__(**kwargs)
         self.name = name
         self.armada_channel_args = GrpcChannelArguments(**armada_channel_args)
 
         if "options" not in job_service_channel_args:
             job_service_channel_args["options"] = default_jobservice_channel_options
 
+        self.job_service_channel_args = GrpcChannelArguments(**job_service_channel_args)
         self.armada_queue = armada_queue
         self.job_request_items = job_request_items
         self.lookout_url_template = lookout_url_template
         self.poll_interval = poll_interval
 
     def execute(self, context) -> None:
         """
```

## Comparing `armada_airflow-0.5.0.dist-info/LICENSE` & `armada_airflow-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.5.0.dist-info/METADATA` & `armada_airflow-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
```

## Comparing `armada_airflow-0.5.0.dist-info/RECORD` & `armada_airflow-0.5.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=idcVXwvH0EeYCcyBcloshRhh_JQhCpLn5a2-LPqkxIU,2891
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-armada/operators/armada.py,sha256=b_0OVumrM9wkKP7g27INyoJUIS1itmBbsm_KsY7DNjM,6081
+armada/operators/armada.py,sha256=U5VzsgXre5drhjU7Zzsd-p1liM6S2BlNUSKI1Jf481I,6170
 armada/operators/armada_deferrable.py,sha256=ggadgIswvrd2tA0D3aT86_jSEPvnRxRfDyg_fSppYtI,9671
 armada/operators/grpc.py,sha256=o9X4HhUdjVJIjhsLZNtjLRGubr7bYQRFCkUH7LD2lXw,3080
 armada/operators/jobservice.py,sha256=_Rrrmz6NqbEeATWegdabjMv7y7dEGUzWy5hgKS23-8o,3044
 armada/operators/jobservice_asyncio.py,sha256=DmtzNfSroAheBj-pAOeUZ6lZcx4UItUNt08DFvH3cIA,2613
 armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
-armada_airflow-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.5.0.dist-info/METADATA,sha256=K_8M-DkTXpo5qbCAz6XO3-NM2UrsGFFzDTlC1Dhwmf8,3916
-armada_airflow-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-armada_airflow-0.5.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.5.0.dist-info/RECORD,,
+armada_airflow-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.5.1.dist-info/METADATA,sha256=OvMtR60m1Gv3XRYliBz9azQZzwlAqnRXjF-dr1ir2nA,3916
+armada_airflow-0.5.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+armada_airflow-0.5.1.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.5.1.dist-info/RECORD,,
```

