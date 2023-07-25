# Comparing `tmp/our1314-0.1.6.tar.gz` & `tmp/our1314-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.1.6.tar", last modified: Tue Jul 25 06:20:36 2023, max compression
+gzip compressed data, was "our1314-0.1.7.tar", last modified: Tue Jul 25 06:22:40 2023, max compression
```

## Comparing `our1314-0.1.6.tar` & `our1314-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:20:36.886486 our1314-0.1.6/
--rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-25 06:20:36.885482 our1314-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:20:36.864479 our1314-0.1.6/our1314/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.6/our1314/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:20:36.880480 our1314-0.1.6/our1314/cv/
--rw-rw-rw-   0        0        0        0 2023-07-25 06:04:58.000000 our1314-0.1.6/our1314/cv/__init__.py
--rw-rw-rw-   0        0        0     1240 2023-07-25 05:55:44.000000 our1314-0.1.6/our1314/cv/mouseselect.py
--rw-rw-rw-   0        0        0      966 2023-07-25 06:17:55.000000 our1314-0.1.6/our1314/cv/templatematch.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:20:36.884481 our1314-0.1.6/our1314/myutils/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.6/our1314/myutils/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.6/our1314/myutils/exportsd.py
--rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.6/our1314/myutils/importsd.py
--rw-rw-rw-   0        0        0     5426 2023-07-25 05:56:11.000000 our1314-0.1.6/our1314/myutils/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:20:36.877479 our1314-0.1.6/our1314.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-25 06:20:36.000000 our1314-0.1.6/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-07-25 06:20:36.000000 our1314-0.1.6/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:20:36.000000 our1314-0.1.6/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 06:20:36.000000 our1314-0.1.6/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:20:36.887480 our1314-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-07-25 06:19:39.000000 our1314-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:22:40.672670 our1314-0.1.7/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:22:40.671671 our1314-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:22:40.655669 our1314-0.1.7/our1314/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.7/our1314/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:22:40.666670 our1314-0.1.7/our1314/cv/
+-rw-rw-rw-   0        0        0        0 2023-07-25 06:04:58.000000 our1314-0.1.7/our1314/cv/__init__.py
+-rw-rw-rw-   0        0        0     1240 2023-07-25 05:55:44.000000 our1314-0.1.7/our1314/cv/mouseselect.py
+-rw-rw-rw-   0        0        0      966 2023-07-25 06:17:55.000000 our1314-0.1.7/our1314/cv/templatematch.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:22:40.671671 our1314-0.1.7/our1314/myutils/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.7/our1314/myutils/__init__.py
+-rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.7/our1314/myutils/exportsd.py
+-rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.7/our1314/myutils/importsd.py
+-rw-rw-rw-   0        0        0     5426 2023-07-25 06:22:12.000000 our1314-0.1.7/our1314/myutils/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:22:40.664671 our1314-0.1.7/our1314.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:22:40.000000 our1314-0.1.7/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-25 06:22:40.000000 our1314-0.1.7/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:22:40.000000 our1314-0.1.7/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 06:22:40.000000 our1314-0.1.7/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:22:40.672670 our1314-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-07-25 06:22:24.000000 our1314-0.1.7/setup.py
```

### Comparing `our1314-0.1.6/LICENSE` & `our1314-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `our1314-0.1.6/our1314/cv/mouseselect.py` & `our1314-0.1.7/our1314/cv/mouseselect.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.6/our1314/cv/templatematch.py` & `our1314-0.1.7/our1314/cv/templatematch.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.6/our1314/myutils/exportsd.py` & `our1314-0.1.7/our1314/myutils/exportsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.6/our1314/myutils/importsd.py` & `our1314-0.1.7/our1314/myutils/importsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.6/our1314/myutils/myutils.py` & `our1314-0.1.7/our1314/myutils/myutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 def hobject2ndarray(hobj):
     return himage_as_numpy_array(hobj)
 
 def deg(rad):
     return rad*180/pi
 
 def rad(deg):
-    return deg*180/pi
+    return deg*pi/180
 
 
 if __name__ == '__main__':
     # a = getlastfile('D:/work/proj/xray/test_learn_python/image_classification/cnn_imgcls/run/train/oqa_agl/weights', '.pth')
     # x = torch.rand((1, 3, 110, 310))
     # x = Resize3(330)(x)
     # x = PadSquare()(x)
```

