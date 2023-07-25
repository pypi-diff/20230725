# Comparing `tmp/benimang-0.4.8.tar.gz` & `tmp/benimang-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.8.tar", last modified: Tue Jul 25 08:34:07 2023, max compression
+gzip compressed data, was "benimang-0.4.9.tar", last modified: Tue Jul 25 09:20:43 2023, max compression
```

## Comparing `benimang-0.4.8.tar` & `benimang-0.4.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.046455 benimang-0.4.8/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-25 08:34:07.046455 benimang-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.041453 benimang-0.4.8/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.8/beni/__init__.py
--rw-rw-rw-   0        0        0     6556 2023-07-25 07:39:02.000000 benimang-0.4.8/beni/bbyte.py
--rw-rw-rw-   0        0        0     1866 2023-07-25 06:18:05.000000 benimang-0.4.8/beni/bcache.py
--rw-rw-rw-   0        0        0     1816 2023-07-25 06:21:32.000000 benimang-0.4.8/beni/bcolor.py
--rw-rw-rw-   0        0        0      436 2023-07-25 06:23:25.000000 benimang-0.4.8/beni/bdefine.py
--rw-rw-rw-   0        0        0     1600 2023-07-25 07:11:17.000000 benimang-0.4.8/beni/bexecute.py
--rw-rw-rw-   0        0        0     2661 2023-07-25 06:34:46.000000 benimang-0.4.8/beni/bfile.py
--rw-rw-rw-   0        0        0     5090 2023-07-25 07:47:04.000000 benimang-0.4.8/beni/bfunc.py
--rw-rw-rw-   0        0        0     5752 2023-07-25 07:01:09.000000 benimang-0.4.8/beni/bhttp.py
--rw-rw-rw-   0        0        0     2242 2023-07-25 06:54:08.000000 benimang-0.4.8/beni/binput.py
--rw-rw-rw-   0        0        0     5672 2023-07-25 07:25:27.000000 benimang-0.4.8/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.8/beni/blog.py
--rw-rw-rw-   0        0        0     5413 2023-07-25 07:16:01.000000 benimang-0.4.8/beni/bpath.py
--rw-rw-rw-   0        0        0     2415 2023-07-25 07:11:21.000000 benimang-0.4.8/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1083 2023-07-25 07:01:09.000000 benimang-0.4.8/beni/bprogress.py
--rw-rw-rw-   0        0        0     3813 2023-07-25 07:15:16.000000 benimang-0.4.8/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10447 2023-07-25 08:21:55.000000 benimang-0.4.8/beni/bsqlite.py
--rw-rw-rw-   0        0        0     3990 2023-07-25 08:13:07.000000 benimang-0.4.8/beni/bstore.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.8/beni/btable.py
--rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.8/beni/btask.py
--rw-rw-rw-   0        0        0     1380 2023-07-25 07:06:47.000000 benimang-0.4.8/beni/btime.py
--rw-rw-rw-   0        0        0      436 2023-07-25 02:06:35.000000 benimang-0.4.8/beni/btype.py
--rw-rw-rw-   0        0        0     2366 2023-07-25 02:09:39.000000 benimang-0.4.8/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.044454 benimang-0.4.8/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-25 08:33:37.000000 benimang-0.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 08:34:07.047455 benimang-0.4.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.045454 benimang-0.4.8/test/
--rw-rw-rw-   0        0        0      398 2023-07-25 07:46:56.000000 benimang-0.4.8/test/test_bbyte.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:20:43.661022 benimang-0.4.9/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-25 09:20:43.661022 benimang-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 09:20:43.655020 benimang-0.4.9/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.9/beni/__init__.py
+-rw-rw-rw-   0        0        0     6556 2023-07-25 07:39:02.000000 benimang-0.4.9/beni/bbyte.py
+-rw-rw-rw-   0        0        0     1866 2023-07-25 06:18:05.000000 benimang-0.4.9/beni/bcache.py
+-rw-rw-rw-   0        0        0     1816 2023-07-25 06:21:32.000000 benimang-0.4.9/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 06:23:25.000000 benimang-0.4.9/beni/bdefine.py
+-rw-rw-rw-   0        0        0     1600 2023-07-25 07:11:17.000000 benimang-0.4.9/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2617 2023-07-25 08:54:22.000000 benimang-0.4.9/beni/bfile.py
+-rw-rw-rw-   0        0        0     5090 2023-07-25 07:47:04.000000 benimang-0.4.9/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5752 2023-07-25 07:01:09.000000 benimang-0.4.9/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2242 2023-07-25 06:54:08.000000 benimang-0.4.9/beni/binput.py
+-rw-rw-rw-   0        0        0     5672 2023-07-25 07:25:27.000000 benimang-0.4.9/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.9/beni/blog.py
+-rw-rw-rw-   0        0        0     5413 2023-07-25 07:16:01.000000 benimang-0.4.9/beni/bpath.py
+-rw-rw-rw-   0        0        0     2415 2023-07-25 07:11:21.000000 benimang-0.4.9/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1083 2023-07-25 07:01:09.000000 benimang-0.4.9/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3813 2023-07-25 07:15:16.000000 benimang-0.4.9/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10447 2023-07-25 08:21:55.000000 benimang-0.4.9/beni/bsqlite.py
+-rw-rw-rw-   0        0        0     3990 2023-07-25 08:13:07.000000 benimang-0.4.9/beni/bstore.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.9/beni/btable.py
+-rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.9/beni/btask.py
+-rw-rw-rw-   0        0        0     1380 2023-07-25 07:06:47.000000 benimang-0.4.9/beni/btime.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 02:06:35.000000 benimang-0.4.9/beni/btype.py
+-rw-rw-rw-   0        0        0     2366 2023-07-25 02:09:39.000000 benimang-0.4.9/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:20:43.659022 benimang-0.4.9/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-25 09:20:43.000000 benimang-0.4.9/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-07-25 09:20:43.000000 benimang-0.4.9/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:20:43.000000 benimang-0.4.9/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 09:20:43.000000 benimang-0.4.9/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-25 09:19:08.000000 benimang-0.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:20:43.661022 benimang-0.4.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 09:20:43.660022 benimang-0.4.9/test/
+-rw-rw-rw-   0        0        0      398 2023-07-25 07:46:56.000000 benimang-0.4.9/test/test_bbyte.py
```

### Comparing `benimang-0.4.8/beni/bbyte.py` & `benimang-0.4.9/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bcache.py` & `benimang-0.4.9/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bcolor.py` & `benimang-0.4.9/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bexecute.py` & `benimang-0.4.9/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bfile.py` & `benimang-0.4.9/beni/bfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,13 @@
     ary = content.split('>>>')
     ary = [x.strip() for x in ary]
     ary = [x for x in ary if x]
     ary.sort()
     for substr in ary:
         subAry = substr.replace('\r\n', '\n').split('\n')
         fileName = subAry.pop(0)
-        if subAry:
-            file = output / fileName
-            bcolor.printYellow(file)
-            await bfile.writeText(
-                file,
-                '\n'.join(subAry).strip(),
-            )
+        file = output / fileName
+        bcolor.printYellow(file)
+        await bfile.writeText(
+            file,
+            '\n'.join(subAry).strip(),
+        )
```

### Comparing `benimang-0.4.8/beni/bfunc.py` & `benimang-0.4.9/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bhttp.py` & `benimang-0.4.9/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/binput.py` & `benimang-0.4.9/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/block.py` & `benimang-0.4.9/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/blog.py` & `benimang-0.4.9/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bpath.py` & `benimang-0.4.9/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bplaywright.py` & `benimang-0.4.9/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bprogress.py` & `benimang-0.4.9/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bqiniu.py` & `benimang-0.4.9/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bsqlite.py` & `benimang-0.4.9/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bstore.py` & `benimang-0.4.9/beni/bstore.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/btable.py` & `benimang-0.4.9/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/btask.py` & `benimang-0.4.9/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/btime.py` & `benimang-0.4.9/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/beni/bzip.py` & `benimang-0.4.9/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.8/benimang.egg-info/SOURCES.txt` & `benimang-0.4.9/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

