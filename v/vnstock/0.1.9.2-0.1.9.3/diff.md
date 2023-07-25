# Comparing `tmp/vnstock-0.1.9.2.tar.gz` & `tmp/vnstock-0.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock-0.1.9.2.tar", last modified: Tue Jul 25 14:03:49 2023, max compression
+gzip compressed data, was "vnstock-0.1.9.3.tar", last modified: Tue Jul 25 14:18:50 2023, max compression
```

## Comparing `vnstock-0.1.9.2.tar` & `vnstock-0.1.9.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:03:49.369386 vnstock-0.1.9.2/
--rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.9.2/LICENSE
--rw-rw-rw-   0        0        0    73061 2023-07-25 14:03:49.373380 vnstock-0.1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    72632 2023-07-25 13:50:06.000000 vnstock-0.1.9.2/README.md
--rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.9.2/pyproject.toml
--rw-rw-rw-   0        0        0      514 2023-07-25 14:03:49.384375 vnstock-0.1.9.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 14:03:49.368389 vnstock-0.1.9.2/vnstock.egg-info/
--rw-rw-rw-   0        0        0    73061 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:18:50.645149 vnstock-0.1.9.3/
+-rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.9.3/LICENSE
+-rw-rw-rw-   0        0        0    73061 2023-07-25 14:18:50.647143 vnstock-0.1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    72632 2023-07-25 13:50:06.000000 vnstock-0.1.9.3/README.md
+-rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-07-25 14:18:50.649138 vnstock-0.1.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 14:18:50.644152 vnstock-0.1.9.3/vnstock.egg-info/
+-rw-rw-rw-   0        0        0    73061 2023-07-25 14:18:50.000000 vnstock-0.1.9.3/vnstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-07-25 14:18:50.000000 vnstock-0.1.9.3/vnstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:18:50.000000 vnstock-0.1.9.3/vnstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:18:50.000000 vnstock-0.1.9.3/vnstock.egg-info/top_level.txt
```

### Comparing `vnstock-0.1.9.2/LICENSE` & `vnstock-0.1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.9.2/PKG-INFO` & `vnstock-0.1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vnstock-0.1.9.2/README.md` & `vnstock-0.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.9.2/setup.cfg` & `vnstock-0.1.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e73 746f 636b 0d0a 7665 7273   = vnstock..vers
-00000020: 696f 6e20 3d20 302e 312e 392e 320d 0a61  ion = 0.1.9.2..a
+00000020: 696f 6e20 3d20 302e 312e 392e 330d 0a61  ion = 0.1.9.3..a
 00000030: 7574 686f 7220 3d20 5468 696e 6820 5675  uthor = Thinh Vu
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206d 7274 6869 6e68 406c 6976 652e 636f   mrthinh@live.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2056 6965 746e 616d 2053 746f 636b 204d   Vietnam Stock M
 00000080: 6172 6b65 7420 4461 7461 0d0a 6c6f 6e67  arket Data..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `vnstock-0.1.9.2/vnstock.egg-info/PKG-INFO` & `vnstock-0.1.9.3/vnstock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

