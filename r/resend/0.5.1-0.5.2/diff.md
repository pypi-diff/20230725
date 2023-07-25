# Comparing `tmp/resend-0.5.1-py2.py3-none-any.whl.zip` & `tmp/resend-0.5.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7260 bytes, number of entries: 13
--rw-r--r--  2.0 unx      373 b- defN 23-Jun-14 10:28 resend/__init__.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Jun-14 10:28 resend/api.py
--rw-r--r--  2.0 unx      796 b- defN 23-Jun-14 10:28 resend/api_keys.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Jun-14 10:28 resend/domains.py
--rw-r--r--  2.0 unx      588 b- defN 23-Jun-14 10:28 resend/emails.py
--rw-r--r--  2.0 unx     4152 b- defN 23-Jun-14 10:28 resend/exceptions.py
--rw-r--r--  2.0 unx     1694 b- defN 23-Jun-14 10:28 resend/request.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jun-14 10:37 resend/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Jun-14 10:37 resend-0.5.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2255 b- defN 23-Jun-14 10:37 resend-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-14 10:37 resend-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 10:37 resend-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      972 b- defN 23-Jun-14 10:37 resend-0.5.1.dist-info/RECORD
-13 files, 14507 bytes uncompressed, 5664 bytes compressed:  61.0%
+Zip file size: 7279 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      373 b- defN 23-Jul-25 21:02 resend/__init__.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-25 21:02 resend/api.py
+-rw-r--r--  2.0 unx      796 b- defN 23-Jul-25 21:02 resend/api_keys.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jul-25 21:02 resend/domains.py
+-rw-r--r--  2.0 unx      588 b- defN 23-Jul-25 21:02 resend/emails.py
+-rw-r--r--  2.0 unx     4152 b- defN 23-Jul-25 21:02 resend/exceptions.py
+-rw-r--r--  2.0 unx     1701 b- defN 23-Jul-25 21:02 resend/request.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Jul-25 21:02 resend/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jul-25 21:07 resend-0.5.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2280 b- defN 23-Jul-25 21:07 resend-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 21:07 resend-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-25 21:07 resend-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      972 b- defN 23-Jul-25 21:07 resend-0.5.2.dist-info/RECORD
+13 files, 14539 bytes uncompressed, 5683 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: resend/request.py
 Comment: 
 
 Filename: resend/version.py
 Comment: 
 
-Filename: resend-0.5.1.dist-info/LICENSE.md
+Filename: resend-0.5.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: resend-0.5.1.dist-info/METADATA
+Filename: resend-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: resend-0.5.1.dist-info/WHEEL
+Filename: resend-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: resend-0.5.1.dist-info/top_level.txt
+Filename: resend-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: resend-0.5.1.dist-info/RECORD
+Filename: resend-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## resend/request.py

```diff
@@ -41,15 +41,15 @@
 
         Returns:
             Dict: configured HTTP Headers
         """
         return {
             "Accept": "application/json",
             "Authorization": f"Bearer {resend.api_key}",
-            "User-Agent": f"python:{get_version()}",
+            "User-Agent": f"resend-python:{get_version()}",
         }
 
     def make_request(self, url: str):
         headers = self.__get_headers()
         params = self.params
         verb = self.verb
```

## resend/version.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 def get_version():
     """Returns the current version of this lib
 
     Returns:
         str: version number
```

## Comparing `resend-0.5.1.dist-info/LICENSE.md` & `resend-0.5.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `resend-0.5.1.dist-info/METADATA` & `resend-0.5.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.5.1
+Version: 0.5.2
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Keywords: email,email platform
 Platform: UNKNOWN
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: requests (==2.31.0)
 
 # Resend Python SDK
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
```

## Comparing `resend-0.5.1.dist-info/RECORD` & `resend-0.5.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 resend/__init__.py,sha256=UIDNarnLyDjjkkXg3W7hwm1tjZ4KeLD0A6BiCsk6m0w,373
 resend/api.py,sha256=63kPeE8oW32KRZUWz7fA3TfSgUxboHl35-z3r-oKO-k,1059
 resend/api_keys.py,sha256=LI0y1A_FYVjmPerdqTKuF-D6tLLCgE65p_BFPaL9DZE,796
 resend/domains.py,sha256=fdgTsWzL7eGz3CusnbhzU95sW--QQogJgJrr6oVv9pU,1268
 resend/emails.py,sha256=8iCUoVDAWm6jWVux1vtJsblaAS0zPBZ4oVCmAkX7jpc,588
 resend/exceptions.py,sha256=UG4t5KTlsHYXxaLYs44KGGcdgORZ61JCO3XZa1IbhRw,4152
-resend/request.py,sha256=pDTYiY5V4YDdO4cBh6HWKTdOR9xImk-7mHR9r8DyXm0,1694
-resend/version.py,sha256=CSguLUDHPb6FY0IiCl7qZSx3bft0Aw9ev12D6QPe-mI,163
-resend-0.5.1.dist-info/LICENSE.md,sha256=osumSw2owqnD5qoaVWZ-txW8uPCkoIEhqf9O10DWrzA,1070
-resend-0.5.1.dist-info/METADATA,sha256=eQiFPPdNiBGt9VPv-6MnIxRsWc885JWqcBeameemLzE,2255
-resend-0.5.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-resend-0.5.1.dist-info/top_level.txt,sha256=sSzgEO0yVPRNWY_L1GO_SXzz3dOzps41bTW_UtyQ0p4,7
-resend-0.5.1.dist-info/RECORD,,
+resend/request.py,sha256=cQyAcm0CdlP8vJ__U607l28tKVyxi83xEeuFPC4akwA,1701
+resend/version.py,sha256=62Tx1SZ7zF3nbTov5yMho4pcnO-uu5udvAzp0FmpdKE,163
+resend-0.5.2.dist-info/LICENSE.md,sha256=osumSw2owqnD5qoaVWZ-txW8uPCkoIEhqf9O10DWrzA,1070
+resend-0.5.2.dist-info/METADATA,sha256=2-lf1y63Dc_Rxopa7yinYSk60II3t_eE53Q85_uJzdM,2280
+resend-0.5.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+resend-0.5.2.dist-info/top_level.txt,sha256=sSzgEO0yVPRNWY_L1GO_SXzz3dOzps41bTW_UtyQ0p4,7
+resend-0.5.2.dist-info/RECORD,,
```

