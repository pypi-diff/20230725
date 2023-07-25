# Comparing `tmp/passwordP-0.0.1.1-py3-none-any.whl.zip` & `tmp/passwordP-1.0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2712 bytes, number of entries: 7
+Zip file size: 2704 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       37 b- defN 23-Jul-25 11:04 passwordP/__init__.py
--rw-rw-r--  2.0 unx      762 b- defN 23-Jul-25 11:02 passwordP/passwordPP.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-25 11:05 passwordP-0.0.1.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      347 b- defN 23-Jul-25 11:05 passwordP-0.0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 11:05 passwordP-0.0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       22 b- defN 23-Jul-25 11:05 passwordP-0.0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      564 b- defN 23-Jul-25 11:05 passwordP-0.0.1.1.dist-info/RECORD
-7 files, 2890 bytes uncompressed, 1704 bytes compressed:  41.0%
+-rw-rw-r--  2.0 unx      721 b- defN 23-Jul-25 11:09 passwordP/passwordPP.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-25 11:10 passwordP-1.0.1.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      347 b- defN 23-Jul-25 11:10 passwordP-1.0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 11:10 passwordP-1.0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       22 b- defN 23-Jul-25 11:10 passwordP-1.0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      564 b- defN 23-Jul-25 11:10 passwordP-1.0.1.1.dist-info/RECORD
+7 files, 2849 bytes uncompressed, 1696 bytes compressed:  40.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: passwordP/__init__.py
 Comment: 
 
 Filename: passwordP/passwordPP.py
 Comment: 
 
-Filename: passwordP-0.0.1.1.dist-info/LICENSE.txt
+Filename: passwordP-1.0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: passwordP-0.0.1.1.dist-info/METADATA
+Filename: passwordP-1.0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: passwordP-0.0.1.1.dist-info/WHEEL
+Filename: passwordP-1.0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: passwordP-0.0.1.1.dist-info/top_level.txt
+Filename: passwordP-1.0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: passwordP-0.0.1.1.dist-info/RECORD
+Filename: passwordP-1.0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## passwordP/passwordPP.py

```diff
@@ -25,16 +25,14 @@
 
     # shuffling the password by creating a list
     password_list=list(password)
     random.shuffle(password_list)
     password=''.join(password_list)
     return password
 
-password=generate_pass()
-print(password)
 
 
 # In[ ]:
```

## Comparing `passwordP-0.0.1.1.dist-info/LICENSE.txt` & `passwordP-1.0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

