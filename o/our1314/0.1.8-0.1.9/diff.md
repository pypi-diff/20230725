# Comparing `tmp/our1314-0.1.8.tar.gz` & `tmp/our1314-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.1.8.tar", last modified: Tue Jul 25 06:47:32 2023, max compression
+gzip compressed data, was "our1314-0.1.9.tar", last modified: Tue Jul 25 06:52:37 2023, max compression
```

## Comparing `our1314-0.1.8.tar` & `our1314-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:47:32.689075 our1314-0.1.8/
--rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-25 06:47:32.689075 our1314-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:47:32.672076 our1314-0.1.8/our1314/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.8/our1314/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:47:32.685075 our1314-0.1.8/our1314/cv/
--rw-rw-rw-   0        0        0        0 2023-07-25 06:04:58.000000 our1314-0.1.8/our1314/cv/__init__.py
--rw-rw-rw-   0        0        0     1240 2023-07-25 05:55:44.000000 our1314-0.1.8/our1314/cv/mouseselect.py
--rw-rw-rw-   0        0        0     1407 2023-07-25 06:46:57.000000 our1314-0.1.8/our1314/cv/templatematch.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:47:32.688075 our1314-0.1.8/our1314/myutils/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.8/our1314/myutils/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.8/our1314/myutils/exportsd.py
--rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.8/our1314/myutils/importsd.py
--rw-rw-rw-   0        0        0     5732 2023-07-25 06:45:29.000000 our1314-0.1.8/our1314/myutils/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:47:32.684075 our1314-0.1.8/our1314.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-25 06:47:32.000000 our1314-0.1.8/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-07-25 06:47:32.000000 our1314-0.1.8/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:47:32.000000 our1314-0.1.8/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 06:47:32.000000 our1314-0.1.8/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:47:32.690076 our1314-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-07-25 06:47:29.000000 our1314-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:37.773675 our1314-0.1.9/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:52:37.773675 our1314-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:37.754675 our1314-0.1.9/our1314/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.9/our1314/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:37.767675 our1314-0.1.9/our1314/cv/
+-rw-rw-rw-   0        0        0        0 2023-07-25 06:04:58.000000 our1314-0.1.9/our1314/cv/__init__.py
+-rw-rw-rw-   0        0        0     1240 2023-07-25 05:55:44.000000 our1314-0.1.9/our1314/cv/mouseselect.py
+-rw-rw-rw-   0        0        0     1439 2023-07-25 06:48:34.000000 our1314-0.1.9/our1314/cv/templatematch.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:37.772676 our1314-0.1.9/our1314/myutils/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.9/our1314/myutils/__init__.py
+-rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.9/our1314/myutils/exportsd.py
+-rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.9/our1314/myutils/importsd.py
+-rw-rw-rw-   0        0        0     5734 2023-07-25 06:52:19.000000 our1314-0.1.9/our1314/myutils/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:37.762676 our1314-0.1.9/our1314.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:52:37.000000 our1314-0.1.9/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-25 06:52:37.000000 our1314-0.1.9/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:52:37.000000 our1314-0.1.9/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 06:52:37.000000 our1314-0.1.9/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:52:37.773675 our1314-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-07-25 06:52:33.000000 our1314-0.1.9/setup.py
```

### Comparing `our1314-0.1.8/LICENSE` & `our1314-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `our1314-0.1.8/our1314/cv/mouseselect.py` & `our1314-0.1.9/our1314/cv/mouseselect.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.8/our1314/cv/templatematch.py` & `our1314-0.1.9/our1314/cv/templatematch.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.model_id = halcon.create_scaled_shape_model(temp, 5, -rad(10.0), rad(20.0), rad(0.3657), 0.8, 1/0.8, 0.01, ['none', 'no_pregeneration'], 'use_polarity', [10,30,30], 10)
         
         _, r1, c1 = halcon.area_center(model_region)
         r2, c2, phi, len1, len2 = halcon.smallest_rectangle2(model_region)
 
         halcon.set_shape_model_origin(self.model_id, r2[0]-r1[0], c2[0]-c1[0])
         self.select_rect = halcon.get_shape_model_contours(self.model_id, 1)
-        select_pts = 
+        select_pts = contours2coord(self.select_rect)
 
         pass
 
 
     def aa(self):
         halcon.find_scaled_shape_model()
         pass
```

### Comparing `our1314-0.1.8/our1314/myutils/exportsd.py` & `our1314-0.1.9/our1314/myutils/exportsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.8/our1314/myutils/importsd.py` & `our1314-0.1.9/our1314/myutils/importsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.8/our1314/myutils/myutils.py` & `our1314-0.1.9/our1314/myutils/myutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
 def rad(deg):
     return deg*pi/180
 
 def contours2coord(contours):
     coord=[]
     for i in range(halcon.count_obj(contours)):
-        objectseleted = halcon.select_obj(contours, i)
+        objectseleted = halcon.select_obj(contours, i+1)
         row, col = halcon.get_contour_xld(objectseleted)
 
         for r,c in zip(row, col):
             coord.append([c,r])
     return np.array(coord)
 
 if __name__ == '__main__':
```

