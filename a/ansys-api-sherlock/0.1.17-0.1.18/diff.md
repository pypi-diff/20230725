# Comparing `tmp/ansys-api-sherlock-0.1.17.tar.gz` & `tmp/ansys-api-sherlock-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.17.tar", last modified: Fri Jul 14 17:40:06 2023, max compression
+gzip compressed data, was "ansys-api-sherlock-0.1.18.tar", last modified: Tue Jul 25 14:03:54 2023, max compression
```

## Comparing `ansys-api-sherlock-0.1.17.tar` & `ansys-api-sherlock-0.1.18.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.956967 ansys-api-sherlock-0.1.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.956967 ansys-api-sherlock-0.1.18/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.956967 ansys-api-sherlock-0.1.18/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-25 14:03:39.000000 ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:03:54.960967 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 14:03:54.000000 ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.17/LICENSE` & `ansys-api-sherlock-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/PKG-INFO` & `ansys-api-sherlock-0.1.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.17
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 17:40:06 on 14 July 2023
+Version: 0.1.18
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:03:54 on 25 July 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.17/README.md` & `ansys-api-sherlock-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/setup.py` & `ansys-api-sherlock-0.1.18/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files 26% similar despite different names*

```diff
@@ -245,16 +245,81 @@
  * Contains the status of the update as well as all the update error messages.
  */
 message UpdateTestPointsResponse {
   ReturnCode returnCode 		= 1;	// Status code of response.
   repeated string updateError	= 2;	// Test Points update error messages.
 }
 
+message PolygonalShape {
+    
+  message Point {
+    double x = 1;					// The x coordinate of the point
+    double y = 2;					// The y coordinate of the point
+  }
+    
+  repeated Point points = 1;		// The points used to define the polygonal shape, must be >= 3
+  optional double rotation = 2;		// The rotation of the shape
+}
+  
+message RectangularShape {
+  optional double length = 1;		// The length of the rectangle
+  optional double width = 2;		// The width of the rectangle
+  optional double centerX = 3;		// The x coordinate of the center of the rectangle
+  optional double centerY = 4;		// The y coordinate of the center of the rectangle
+  optional double rotation = 5;		// The rotation of the rectangle
+}
+  
+message SlotShape {
+  optional double length = 1;		// The length of the slot shape
+  optional double width = 2;		// The width of the slot shape
+  optional uint32 nodeCount = 3;	// The number of nodes
+  optional double centerX = 4;		// The x coordinate of the center of the slot shape
+  optional double centerY = 5;		// The x coordinate of the center of the slot shape
+  optional double rotation = 6;		// The rotation of the shape
+}
+  
+message CircularShape {
+  optional double diameter = 1;		// The diameter of the circle
+  optional uint32 nodeCount = 2;	// The number of nodes
+  optional double centerX = 3;		// The x coordinate of the center of the circle
+  optional double centerY = 4;		// The x coordinate of the center of the circle
+  optional double rotation = 5;		// The rotation of the shape
+}
+  
+message PCBShape {
+}
+
+message AddPottingRegionRequest {
+  
+  message PottingRegion {
+    string ccaName = 1;							// The name of the CCA
+    optional string pottingID = 2;				// The potting ID, must be unique
+    optional string pottingSide = 3;			// The potting side, options are "TOP", "BOT", or "BOTTOM"
+    optional string pottingMaterial = 4;		// The potting material
+    optional string pottingUnits = 5;			// The units to use for the potting region
+    optional double pottingThickness = 6;		// The potting thickness
+    optional double pottingStandoff = 7;		// The potting standoff
+  
+    oneof Shape {
+      PolygonalShape polygonalShape = 8;		// Used to add a region with a polygonal shape
+  	  RectangularShape rectangularShape = 9;	// Used to add a region with a rectangular shape
+  	  SlotShape slotShape = 10;					// Used to add a region with a slot shape
+  	  CircularShape circularShape = 11;			// Used to add a region with a circular shape
+  	  PCBShape pCBShape = 12;					// Used to add a region with a PCB shape
+    }
+  }
+  
+  string project = 1;							// The name of the Sherlock project to add the potting regions to
+  repeated PottingRegion pottingRegions = 2;	// The potting regions to add
+}
 
 service SherlockLayerService {
+  // Add a potting region with the specified shape and properties
+  rpc addPottingRegion(AddPottingRegionRequest) returns (ReturnCode);
+
   // Delete all ICT fixtures in specific cca of specific project.
   rpc deleteAllICTFixtures(DeleteAllICTFixturesRequest) returns (ReturnCode);
 
   // Delete all mount points in specific cca of specific project.
   rpc deleteAllMountPoints(DeleteAllMountPointsRequest) returns (ReturnCode);
   
   // Delete all test points in specific cca of specific project.
```

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys-api-sherlock-0.1.18/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.17
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 17:40:06 on 14 July 2023
+Version: 0.1.18
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:03:54 on 25 July 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys-api-sherlock-0.1.18/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

