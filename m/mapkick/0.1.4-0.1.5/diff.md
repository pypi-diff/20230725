# Comparing `tmp/mapkick-0.1.4-py2.py3-none-any.whl.zip` & `tmp/mapkick-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 219876 bytes, number of entries: 10
+Zip file size: 219982 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-08 11:35 mapkick/__init__.py
 -rw-r--r--  2.0 unx     2636 b- defN 23-Feb-09 07:35 mapkick/django/__init__.py
--rw-r--r--  2.0 unx   834429 b- defN 23-Mar-11 20:06 mapkick/django/static/mapkick.bundle.js
+-rw-r--r--  2.0 unx   834630 b- defN 23-Jul-25 03:18 mapkick/django/static/mapkick.bundle.js
 -rw-r--r--  2.0 unx     2764 b- defN 23-Feb-15 19:55 mapkick/flask/__init__.py
--rw-r--r--  2.0 unx    53042 b- defN 23-Mar-11 20:06 mapkick/licenses/LICENSE-mapkick-bundle.txt
--rw-r--r--  2.0 unx     1068 b- defN 23-Mar-11 20:11 mapkick-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4241 b- defN 23-Mar-11 20:11 mapkick-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-11 20:11 mapkick-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-11 20:11 mapkick-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Mar-11 20:11 mapkick-0.1.4.dist-info/RECORD
-10 files, 899125 bytes uncompressed, 218464 bytes compressed:  75.7%
+-rw-r--r--  2.0 unx    53042 b- defN 23-Jul-25 03:18 mapkick/licenses/LICENSE-mapkick-bundle.txt
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-25 03:23 mapkick-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4424 b- defN 23-Jul-25 03:23 mapkick-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 03:23 mapkick-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-25 03:23 mapkick-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      827 b- defN 23-Jul-25 03:23 mapkick-0.1.5.dist-info/RECORD
+10 files, 899509 bytes uncompressed, 218570 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mapkick/flask/__init__.py
 Comment: 
 
 Filename: mapkick/licenses/LICENSE-mapkick-bundle.txt
 Comment: 
 
-Filename: mapkick-0.1.4.dist-info/LICENSE.txt
+Filename: mapkick-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mapkick-0.1.4.dist-info/METADATA
+Filename: mapkick-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: mapkick-0.1.4.dist-info/WHEEL
+Filename: mapkick-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: mapkick-0.1.4.dist-info/top_level.txt
+Filename: mapkick-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mapkick-0.1.4.dist-info/RECORD
+Filename: mapkick-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mapkick/django/static/mapkick.bundle.js

### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /*
  * This bundle includes:
  *
- * Mapkick.js v0.2.5
+ * Mapkick.js v0.2.6
  * https://github.com/ankane/mapkick.js
  * MIT License
  *
  * @mapbox/geojson-rewind v0.5.0
  * https://github.com/mapbox/geojson-rewind
  * ISC License
  *
@@ -26652,44 +26652,51 @@
                 } else {
                     center = [0, 0];
                     if (!zoom) {
                         zoom = 1;
                     }
                 }
             }
+            if (!zoom) {
+                zoom = 15;
+            }
 
             var mapOptions = {
                 container: element,
                 style: style,
                 dragRotate: false,
                 touchZoomRotate: false,
                 center: center,
-                zoom: zoom || 15
+                zoom: zoom
             };
             if (!options.style) {
                 mapOptions.projection = "mercator";
             }
             if (options.accessToken) {
                 mapOptions.accessToken = options.accessToken;
             }
+            if (options.library) {
+                Object.assign(mapOptions, options.library);
+            }
             map = new library.Map(mapOptions);
 
             if (options.controls) {
                 map.addControl(new library.NavigationControl({
                     showCompass: false
                 }));
             }
 
             if (!options.zoom) {
                 // hack to prevent error
                 if (!map.style.stylesheet) {
                     map.style.stylesheet = {};
                 }
 
-                if (!bounds.isEmpty()) {
+                // check zoom for hash library option
+                if (!bounds.isEmpty() && map.getZoom() === zoom) {
                     map.fitBounds(bounds, {
                         padding: 40,
                         animate: false,
                         maxZoom: 15
                     });
                 }
             }
```

## mapkick/licenses/LICENSE-mapkick-bundle.txt

```diff
@@ -1,9 +1,9 @@
 ================================================================================
-Mapkick.js 0.2.5
+Mapkick.js 0.2.6
 ================================================================================
 
 Copyright (c) 2017-2023 Andrew Kane
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining
```

## Comparing `mapkick-0.1.4.dist-info/LICENSE.txt` & `mapkick-0.1.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `mapkick-0.1.4.dist-info/METADATA` & `mapkick-0.1.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapkick
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create beautiful JavaScript maps with one line of Python
 Home-page: https://github.com/ankane/mapkick.py
 Author: Andrew Kane
 Author-email: andrew@ankane.org
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -106,15 +106,15 @@
 
 Point map
 
 ```python
 Map([{'latitude': 37.7829, 'longitude': -122.4190}])
 ```
 
-Area map (experimental)
+Area map
 
 ```python
 AreaMap([{'geometry': {'type': 'Polygon', 'coordinates': ...}}])
 ```
 
 ## Data
 
@@ -201,14 +201,22 @@
 
 Refresh data from a remote source every `n` seconds
 
 ```python
 Map(url, refresh=60)
 ```
 
+Pass options directly to the mapping library
+
+```python
+Map(data, library={'hash': True})
+```
+
+See the documentation for [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/api/map/) for more info
+
 ## History
 
 View the [changelog](https://github.com/ankane/mapkick.py/blob/master/CHANGELOG.md)
 
 ## Contributing
 
 Everyone is encouraged to help improve this project. Here are a few ways you can help:
```

