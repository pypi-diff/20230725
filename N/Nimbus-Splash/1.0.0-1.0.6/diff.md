# Comparing `tmp/Nimbus_Splash-1.0.0-py3-none-any.whl.zip` & `tmp/Nimbus_Splash-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 22200 bytes, number of entries: 11
--rw-r--r--  2.0 unx      108 b- defN 23-Feb-13 11:25 nimbus_splash/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-25 11:19 nimbus_splash/__version__.py
--rw-r--r--  2.0 unx     8493 b- defN 23-Jul-24 16:58 nimbus_splash/cli.py
--rw-r--r--  2.0 unx    12717 b- defN 23-Jul-24 16:54 nimbus_splash/job.py
--rw-r--r--  2.0 unx     4686 b- defN 23-May-23 11:33 nimbus_splash/utils.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      556 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      915 b- defN 23-Jul-25 11:19 Nimbus_Splash-1.0.0.dist-info/RECORD
-11 files, 62850 bytes uncompressed, 20642 bytes compressed:  67.2%
+Zip file size: 22293 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-25 14:05 nimbus_splash/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-25 14:05 nimbus_splash/__version__.py
+-rw-r--r--  2.0 unx     8493 b- defN 23-Jul-25 14:05 nimbus_splash/cli.py
+-rw-r--r--  2.0 unx    12717 b- defN 23-Jul-25 14:05 nimbus_splash/job.py
+-rw-r--r--  2.0 unx     4686 b- defN 23-Jul-25 14:05 nimbus_splash/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      752 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      916 b- defN 23-Jul-25 14:05 Nimbus_Splash-1.0.6.dist-info/RECORD
+11 files, 63091 bytes uncompressed, 20735 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: nimbus_splash/job.py
 Comment: 
 
 Filename: nimbus_splash/utils.py
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/LICENSE
+Filename: Nimbus_Splash-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/METADATA
+Filename: Nimbus_Splash-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/WHEEL
+Filename: Nimbus_Splash-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/entry_points.txt
+Filename: Nimbus_Splash-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/top_level.txt
+Filename: Nimbus_Splash-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: Nimbus_Splash-1.0.0.dist-info/RECORD
+Filename: Nimbus_Splash-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nimbus_splash/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.0'
+__version__ = '1.0.6'
```

## Comparing `Nimbus_Splash-1.0.0.dist-info/LICENSE` & `Nimbus_Splash-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Nimbus_Splash-1.0.0.dist-info/METADATA` & `Nimbus_Splash-1.0.6.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: Nimbus-Splash
-Version: 1.0.0
+Version: 1.0.6
 Summary: A package to make life easier when using the University of         Bath's cloud computing suite for Orca calculations.
 Home-page: https://github.com/jonkragskow/nimbus_splash
 Author: Jon Kragskow
 Author-email: jgck20@bath.ac.uk
+Project-URL: Bug Tracker, https://github.com/JonKragskow/nimbus_splash/issues
+Project-URL: Documentation, https://www.kragskow.dev/nimbus_splash/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xyz-py
```

## Comparing `Nimbus_Splash-1.0.0.dist-info/RECORD` & `Nimbus_Splash-1.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 nimbus_splash/__init__.py,sha256=xtSEgJBmqB5nA53MiApdwAo6z4xubTj82TMpwZZFBog,108
-nimbus_splash/__version__.py,sha256=RsZjRjMprNcDm97wqRRSk6rTLgTX8N0GyicZyZ8OsBQ,22
+nimbus_splash/__version__.py,sha256=iNeZ6LZ9iCV_ugsqAh5K1fFqbKkfU8o3NbLYBWI3m1I,22
 nimbus_splash/cli.py,sha256=531SEOIimtnZuvq6HZEvhFxdUC28M94ihdFdQX0pJcA,8493
 nimbus_splash/job.py,sha256=zefji9Ed9R7uYeicR9jV0o4S6j77o00jEMVGEbY_6g0,12717
 nimbus_splash/utils.py,sha256=JKnYpGt2hn5cKYnRD2gaxOd_2J1ZqjjOELilYc2EWP4,4686
-Nimbus_Splash-1.0.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-Nimbus_Splash-1.0.0.dist-info/METADATA,sha256=sJsooTowIgGpotjh7Xym7CRghUTGC6J2NUiWykDyv-Y,556
-Nimbus_Splash-1.0.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-Nimbus_Splash-1.0.0.dist-info/entry_points.txt,sha256=PMEo296Yijri8rEPo6ioeowhr51zH8NyjnyPNQcR7Bc,98
-Nimbus_Splash-1.0.0.dist-info/top_level.txt,sha256=HRWeSbDMz1EJYlFD63QBlmw17cX-8q5tuckILfUeFhE,14
-Nimbus_Splash-1.0.0.dist-info/RECORD,,
+Nimbus_Splash-1.0.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+Nimbus_Splash-1.0.6.dist-info/METADATA,sha256=KKTfNJS0-O_uR_64hWSQlvcal42-_dNfc1fNP0EaXkQ,752
+Nimbus_Splash-1.0.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+Nimbus_Splash-1.0.6.dist-info/entry_points.txt,sha256=7wINZw_3mt7fQows6TNXUcWOWwgrqBSivGSYfdkY_qc,142
+Nimbus_Splash-1.0.6.dist-info/top_level.txt,sha256=HRWeSbDMz1EJYlFD63QBlmw17cX-8q5tuckILfUeFhE,14
+Nimbus_Splash-1.0.6.dist-info/RECORD,,
```

