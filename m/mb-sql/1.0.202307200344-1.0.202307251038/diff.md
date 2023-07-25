# Comparing `tmp/mb_sql-1.0.202307200344-py3-none-any.whl.zip` & `tmp/mb_sql-1.0.202307251038-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 12074 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       43 b- defN 23-May-25 03:43 mb_sql/__init__.py
--rw-rw-r--  2.0 unx     3148 b- defN 23-May-23 16:18 mb_sql/conn.py
--rw-rw-r--  2.0 unx     1080 b- defN 23-Jul-20 03:44 mb_sql/slack.py
--rw-rw-r--  2.0 unx     3667 b- defN 23-May-16 14:53 mb_sql/sql.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-May-16 14:28 mb_sql/tables.py
--rw-rw-r--  2.0 unx    26722 b- defN 23-Jul-20 03:44 mb_sql/update.py
--rw-rw-r--  2.0 unx     5268 b- defN 23-Jul-20 00:46 mb_sql/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-20 03:44 mb_sql/version.py
--rw-rw-r--  2.0 unx      239 b- defN 23-Jul-20 03:44 mb_sql-1.0.202307200344.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 03:44 mb_sql-1.0.202307200344.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-20 03:44 mb_sql-1.0.202307200344.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      914 b- defN 23-Jul-20 03:44 mb_sql-1.0.202307200344.dist-info/RECORD
-12 files, 43245 bytes uncompressed, 10556 bytes compressed:  75.6%
+Zip file size: 13446 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       43 b- defN 23-May-30 16:26 mb_sql/__init__.py
+-rw-rw-r--  2.0 unx     3148 b- defN 23-May-30 16:26 mb_sql/conn.py
+-rw-rw-r--  2.0 unx     1080 b- defN 23-Jul-25 10:38 mb_sql/slack.py
+-rw-rw-r--  2.0 unx     4383 b- defN 23-Jun-27 15:46 mb_sql/snapshot.py
+-rw-rw-r--  2.0 unx     3667 b- defN 23-May-30 16:26 mb_sql/sql.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-May-30 16:26 mb_sql/tables.py
+-rw-rw-r--  2.0 unx    26722 b- defN 23-Jul-25 10:38 mb_sql/update.py
+-rw-rw-r--  2.0 unx     5268 b- defN 23-Jul-25 10:38 mb_sql/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-25 10:38 mb_sql/version.py
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jul-25 10:38 mb_sql-1.0.202307251038.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 10:38 mb_sql-1.0.202307251038.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-25 10:38 mb_sql-1.0.202307251038.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      989 b- defN 23-Jul-25 10:38 mb_sql-1.0.202307251038.dist-info/RECORD
+13 files, 47703 bytes uncompressed, 11816 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: mb_sql/conn.py
 Comment: 
 
 Filename: mb_sql/slack.py
 Comment: 
 
+Filename: mb_sql/snapshot.py
+Comment: 
+
 Filename: mb_sql/sql.py
 Comment: 
 
 Filename: mb_sql/tables.py
 Comment: 
 
 Filename: mb_sql/update.py
@@ -18,20 +21,20 @@
 
 Filename: mb_sql/utils.py
 Comment: 
 
 Filename: mb_sql/version.py
 Comment: 
 
-Filename: mb_sql-1.0.202307200344.dist-info/METADATA
+Filename: mb_sql-1.0.202307251038.dist-info/METADATA
 Comment: 
 
-Filename: mb_sql-1.0.202307200344.dist-info/WHEEL
+Filename: mb_sql-1.0.202307251038.dist-info/WHEEL
 Comment: 
 
-Filename: mb_sql-1.0.202307200344.dist-info/top_level.txt
+Filename: mb_sql-1.0.202307251038.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_sql-1.0.202307200344.dist-info/RECORD
+Filename: mb_sql-1.0.202307251038.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
-VERSION_DAY = int('20')
-VERSION_HOUR = int('03')
-VERSION_MINUTE = int('44')
+VERSION_DAY = int('25')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('38')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307200344
-version_date = '2023/07/20 03:44'
+PATCH_VERSION = 202307251038
+version_date = '2023/07/25 10:38'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_sql-1.0.202307200344.dist-info/RECORD` & `mb_sql-1.0.202307251038.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 mb_sql/__init__.py,sha256=16ZetnIdcpfU3bmRa_MNC07b0I9bZWeJLSvN4UvCEHk,43
 mb_sql/conn.py,sha256=xL8QqVKd96tsXOdtXR7wVOWrmsRdffFFr3Tf2SFltU0,3148
 mb_sql/slack.py,sha256=tr4qfaLrANs5T4tNseW-OGoQD2UcM215TLsh9bF39d8,1080
+mb_sql/snapshot.py,sha256=69xPPF71PLFwxMqr2jM4bRq-TyPFAiZyw1Extaw_1BY,4383
 mb_sql/sql.py,sha256=hiSImhnoNGJvAkIAJYA5Vfjqkz-i0yHEXcIQel7JDK4,3667
 mb_sql/tables.py,sha256=xECYrXJKvdGvCPZo9vT1o7-HO0LoFjaD8602BQo4oO4,1669
 mb_sql/update.py,sha256=eaqHxCDG2R4rKixlb9up_V1RexvpmL6OyaoNYzUVgKg,26722
 mb_sql/utils.py,sha256=kW2BsLx3eZ3d94z5VF1upQh7_lC_Vb5Nj_94-iNualw,5268
-mb_sql/version.py,sha256=ou2V07jWgINoCrquI1_rwzGNgC3FRFFHmh43fGVpGCo,396
-mb_sql-1.0.202307200344.dist-info/METADATA,sha256=9MSIyuKvL9ZTtiFzL7bIDf-XB5bdkBR2CP5RRZQssME,239
-mb_sql-1.0.202307200344.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_sql-1.0.202307200344.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
-mb_sql-1.0.202307200344.dist-info/RECORD,,
+mb_sql/version.py,sha256=hkOwjNyHDpxoAcIvRmNMzx0x9_fqTbGCP96ItGXr61w,396
+mb_sql-1.0.202307251038.dist-info/METADATA,sha256=at7AVMJ2zQ5hPHlk7-DrJe01QgPSPirczc92c77XTVI,239
+mb_sql-1.0.202307251038.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_sql-1.0.202307251038.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
+mb_sql-1.0.202307251038.dist-info/RECORD,,
```

