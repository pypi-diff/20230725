# Comparing `tmp/botiverse-0.4.8-py3-none-any.whl.zip` & `tmp/botiverse-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1059422 bytes, number of entries: 91
+Zip file size: 1059415 bytes, number of entries: 91
 -rw-rw-rw-  2.0 fat       86 b- defN 23-Jul-24 21:38 botiverse/__init__.py
 -rw-rw-rw-  2.0 fat      416 b- defN 23-Jul-25 18:44 botiverse/bots/__init__.py
 -rw-rw-rw-  2.0 fat     7954 b- defN 23-Jul-24 21:38 botiverse/bots/BasicBot/BasicBot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-24 21:38 botiverse/bots/BasicBot/__init__.py
 -rw-rw-rw-  2.0 fat     4783 b- defN 23-Jul-25 17:11 botiverse/bots/BasicTaskBot/BasicTaskBot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 09:37 botiverse/bots/BasicTaskBot/__init__.py
 -rw-rw-rw-  2.0 fat     7588 b- defN 23-Jul-24 22:25 botiverse/bots/BasicTaskBot/utils.py
@@ -82,12 +82,12 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 09:37 botiverse/preprocessors/TF_IDF/__init__.py
 -rw-rw-rw-  2.0 fat     2831 b- defN 23-Jul-08 04:13 botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 09:37 botiverse/preprocessors/TF_IDF_GLOVE/__init__.py
 -rw-rw-rw-  2.0 fat     5580 b- defN 23-Jul-25 18:44 botiverse/preprocessors/Vocalize/Vocalize.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 09:37 botiverse/preprocessors/Vocalize/__init__.py
 -rw-rw-rw-  2.0 fat     7054 b- defN 23-Jul-25 18:44 botiverse/preprocessors/Wav2Vec/Wav2Vec.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 09:37 botiverse/preprocessors/Wav2Vec/__init__.py
--rw-rw-rw-  2.0 fat     1246 b- defN 23-Jul-25 18:56 botiverse-0.4.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 18:56 botiverse-0.4.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-25 18:56 botiverse-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     8608 b- defN 23-Jul-25 18:56 botiverse-0.4.8.dist-info/RECORD
-91 files, 1425919 bytes uncompressed, 1045394 bytes compressed:  26.7%
+-rw-rw-rw-  2.0 fat     1242 b- defN 23-Jul-25 18:58 botiverse-0.4.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 18:58 botiverse-0.4.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-25 18:58 botiverse-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     8608 b- defN 23-Jul-25 18:58 botiverse-0.4.9.dist-info/RECORD
+91 files, 1425915 bytes uncompressed, 1045387 bytes compressed:  26.7%
```

## zipnote {}

```diff
@@ -255,20 +255,20 @@
 
 Filename: botiverse/preprocessors/Wav2Vec/Wav2Vec.py
 Comment: 
 
 Filename: botiverse/preprocessors/Wav2Vec/__init__.py
 Comment: 
 
-Filename: botiverse-0.4.8.dist-info/METADATA
+Filename: botiverse-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: botiverse-0.4.8.dist-info/WHEEL
+Filename: botiverse-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: botiverse-0.4.8.dist-info/top_level.txt
+Filename: botiverse-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: botiverse-0.4.8.dist-info/RECORD
+Filename: botiverse-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `botiverse-0.4.8.dist-info/METADATA` & `botiverse-0.4.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.4.8
-Summary: botiverse is a chatbot library that offers a high-level API to     access a diverse set of chatbot models
+Version: 0.4.9
+Summary: botiverse is a chatbot library that offers a high-level API to access a diverse set of chatbot models
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Requires-Dist: benepar
 Requires-Dist: cvxopt
 Requires-Dist: Flask
```

## Comparing `botiverse-0.4.8.dist-info/RECORD` & `botiverse-0.4.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -81,11 +81,11 @@
 botiverse/preprocessors/TF_IDF/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 botiverse/preprocessors/TF_IDF_GLOVE/TF_IDF_GLOVE.py,sha256=_scS7M12OkfntLSmaI_oB7x-JifGLaDmwgYkUIq82ec,2831
 botiverse/preprocessors/TF_IDF_GLOVE/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 botiverse/preprocessors/Vocalize/Vocalize.py,sha256=pAuLidRwBbPgJ3nFMCO7fnn2SgvAsq8aCaBDnGxNmNI,5580
 botiverse/preprocessors/Vocalize/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 botiverse/preprocessors/Wav2Vec/Wav2Vec.py,sha256=VrRH2iKLw8gYypEZuIYfq0EIVdNEM_xYf1-Hbph86Us,7054
 botiverse/preprocessors/Wav2Vec/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-botiverse-0.4.8.dist-info/METADATA,sha256=wIYCWiR07Eh1BMr5W_X3Q2YcamTVkf7DRmk1IyKdk2w,1246
-botiverse-0.4.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-botiverse-0.4.8.dist-info/top_level.txt,sha256=BC8sEKu6yqp_io2SmYi7PEt6vkOkL4UIXccg-yq8UmA,10
-botiverse-0.4.8.dist-info/RECORD,,
+botiverse-0.4.9.dist-info/METADATA,sha256=XuBbp-SeSNjDur7IfEslMimPh0xuE-UMW70C73wNMvw,1242
+botiverse-0.4.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+botiverse-0.4.9.dist-info/top_level.txt,sha256=BC8sEKu6yqp_io2SmYi7PEt6vkOkL4UIXccg-yq8UmA,10
+botiverse-0.4.9.dist-info/RECORD,,
```

