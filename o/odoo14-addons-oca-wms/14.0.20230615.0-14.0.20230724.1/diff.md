# Comparing `tmp/odoo14_addons_oca_wms-14.0.20230615.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_wms-14.0.20230724.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1784 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3559 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/RECORD
-4 files, 4045 bytes uncompressed, 1010 bytes compressed:  75.0%
+Zip file size: 1812 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3773 b- defN 23-Jul-25 05:53 odoo14_addons_oca_wms-14.0.20230724.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 05:53 odoo14_addons_oca_wms-14.0.20230724.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-25 05:53 odoo14_addons_oca_wms-14.0.20230724.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      393 b- defN 23-Jul-25 05:53 odoo14_addons_oca_wms-14.0.20230724.1.dist-info/RECORD
+4 files, 4259 bytes uncompressed, 1038 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA
+Filename: odoo14_addons_oca_wms-14.0.20230724.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_wms-14.0.20230724.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_wms-14.0.20230724.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/RECORD
+Filename: odoo14_addons_oca_wms-14.0.20230724.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA` & `odoo14_addons_oca_wms-14.0.20230724.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-wms
-Version: 14.0.20230615.0
+Version: 14.0.20230724.1
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -35,14 +35,15 @@
 Requires-Dist: odoo14-addon-shopfloor-packing-info
 Requires-Dist: odoo14-addon-shopfloor-reception
 Requires-Dist: odoo14-addon-shopfloor-reception-mobile
 Requires-Dist: odoo14-addon-shopfloor-rest-log
 Requires-Dist: odoo14-addon-shopfloor-single-product-transfer
 Requires-Dist: odoo14-addon-shopfloor-single-product-transfer-force-package
 Requires-Dist: odoo14-addon-shopfloor-single-product-transfer-mobile
+Requires-Dist: odoo14-addon-shopfloor-single-product-transfer-unique-order-at-location
 Requires-Dist: odoo14-addon-shopfloor-workstation
 Requires-Dist: odoo14-addon-shopfloor-workstation-label-printer
 Requires-Dist: odoo14-addon-shopfloor-workstation-mobile
 Requires-Dist: odoo14-addon-stock-available-to-promise-release
 Requires-Dist: odoo14-addon-stock-available-to-promise-release-dynamic-routing
 Requires-Dist: odoo14-addon-stock-checkout-sync
 Requires-Dist: odoo14-addon-stock-dynamic-routing
@@ -57,12 +58,14 @@
 Requires-Dist: odoo14-addon-stock-reception-screen
 Requires-Dist: odoo14-addon-stock-reception-screen-measuring-device
 Requires-Dist: odoo14-addon-stock-reception-screen-qty-by-packaging
 Requires-Dist: odoo14-addon-stock-release-channel
 Requires-Dist: odoo14-addon-stock-storage-type
 Requires-Dist: odoo14-addon-stock-storage-type-buffer
 Requires-Dist: odoo14-addon-stock-storage-type-putaway-abc
+Requires-Dist: odoo14-addon-stock-unique-order-per-location
 Requires-Dist: odoo14-addon-stock-warehouse-flow
+Requires-Dist: odoo14-addon-stock-warehouse-flow-product-packaging
 Requires-Dist: odoo14-addon-stock-warehouse-flow-release
 
 UNKNOWN
```

