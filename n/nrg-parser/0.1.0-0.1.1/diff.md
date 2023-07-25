# Comparing `tmp/nrg_parser-0.1.0-py3-none-any.whl.zip` & `tmp/nrg_parser-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,24 @@
-Zip file size: 14733 bytes, number of entries: 17
+Zip file size: 15971 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 common/__init__.py
 -rw-r--r--  2.0 unx      978 b- defN 80-Jan-01 00:00 common/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 common/utilities/__init__.py
 -rw-r--r--  2.0 unx     1461 b- defN 80-Jan-01 00:00 common/utilities/function_helper.py
 -rw-r--r--  2.0 unx      119 b- defN 80-Jan-01 00:00 nrg_parser/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/constants/__init__.py
 -rw-r--r--  2.0 unx     1171 b- defN 80-Jan-01 00:00 nrg_parser/mast/constants/iea_mapping_config.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/logger_model/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/logger_model/nrg/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/logger_model/nrg/reader/__init__.py
--rw-r--r--  2.0 unx    18053 b- defN 80-Jan-01 00:00 nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py
+-rw-r--r--  2.0 unx    18215 b- defN 80-Jan-01 00:00 nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/iea_json/__init__.py
 -rw-r--r--  2.0 unx    11929 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/iea_json/convert_to_iea_json.py
 -rw-r--r--  2.0 unx     4643 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/iea_json/create_iea_json_nrg.py
 -rw-r--r--  2.0 unx     3235 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/iea_json/iea_models.py
 -rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 nrg_parser/mast/utilities/iea_json/nrg_config.py
--rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 nrg_parser-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1032 b- defN 80-Jan-01 00:00 nrg_parser-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nrg_parser-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1570 b- defN 16-Jan-01 00:00 nrg_parser-0.1.0.dist-info/RECORD
-17 files, 45457 bytes uncompressed, 12079 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 nrg_parser-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2114 b- defN 80-Jan-01 00:00 nrg_parser-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 nrg_parser-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2028 b- defN 16-Jan-01 00:00 nrg_parser-0.1.1.dist-info/RECORD
+22 files, 47159 bytes uncompressed, 12561 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -1,52 +1,67 @@
 Filename: common/__init__.py
 Comment: 
 
 Filename: common/logger.py
 Comment: 
 
+Filename: common/utilities/__init__.py
+Comment: 
+
 Filename: common/utilities/function_helper.py
 Comment: 
 
 Filename: nrg_parser/__init__.py
 Comment: 
 
 Filename: nrg_parser/mast/__init__.py
 Comment: 
 
+Filename: nrg_parser/mast/constants/__init__.py
+Comment: 
+
 Filename: nrg_parser/mast/constants/iea_mapping_config.py
 Comment: 
 
+Filename: nrg_parser/mast/logger_model/__init__.py
+Comment: 
+
 Filename: nrg_parser/mast/logger_model/nrg/__init__.py
 Comment: 
 
 Filename: nrg_parser/mast/logger_model/nrg/reader/__init__.py
 Comment: 
 
 Filename: nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py
 Comment: 
 
+Filename: nrg_parser/mast/utilities/__init__.py
+Comment: 
+
+Filename: nrg_parser/mast/utilities/iea_json/__init__.py
+Comment: 
+
 Filename: nrg_parser/mast/utilities/iea_json/convert_to_iea_json.py
 Comment: 
 
 Filename: nrg_parser/mast/utilities/iea_json/create_iea_json_nrg.py
 Comment: 
 
 Filename: nrg_parser/mast/utilities/iea_json/iea_models.py
 Comment: 
 
 Filename: nrg_parser/mast/utilities/iea_json/nrg_config.py
 Comment: 
 
-Filename: nrg_parser-0.1.0.dist-info/LICENSE
+Filename: nrg_parser-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: nrg_parser-0.1.0.dist-info/METADATA
+Filename: nrg_parser-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: nrg_parser-0.1.0.dist-info/WHEEL
+Filename: nrg_parser-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: nrg_parser-0.1.0.dist-info/RECORD
+Filename: nrg_parser-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py

```diff
@@ -34,26 +34,30 @@
 
 class SymphonieProTxtReader:
     """
     Symphonie Text File Reader
     This class takes Symphonie Desktop Pro rld -> txt converted file.
     """
 
-    def __init__(self, txt_filepath):
+    def __init__(self, txt_filepath: str):
         """
         Initializes SymphonieProTxt by reading/parsing its file content,
         both headers and timeseries data.
 
         Parameters:
         -----------
             txt_filepath: symphonie pro txt data file path
 
         Attributes:
         -----------
-        
+        first_timestamp: datetime
+        last_timestamp: datetime
+        header_sections_dict: dict
+        sensor_history_list: list
+        header_line_ctr: int 
         """
         # initialize
         self.header_sections_dict = {}
         self.sensor_history_list = []
         self.header_line_ctr = 0
         self.timeseries_data = pd.DataFrame()
         self.first_timestamp = None
```

## Comparing `nrg_parser-0.1.0.dist-info/LICENSE` & `nrg_parser-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nrg_parser-0.1.0.dist-info/RECORD` & `nrg_parser-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 common/logger.py,sha256=RAnykR1dcMQpmjfby6CKHSOa5iLMrPbYNScfEZMVe5Y,978
+common/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 common/utilities/function_helper.py,sha256=SGdVwQTANX3ipiDNr1HpEcGrxtrkUDHrg0EzT_UGrlM,1461
 nrg_parser/__init__.py,sha256=U-ViZJMTTbTyen7zuSYU6VcKkMyCG2IOEHPqTfF8IBk,119
 nrg_parser/mast/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nrg_parser/mast/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nrg_parser/mast/constants/iea_mapping_config.py,sha256=-1Ct4WgmC6_hr_TdTDmQ_dsUt6Y8BSug1hTr2ko4wFo,1171
+nrg_parser/mast/logger_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nrg_parser/mast/logger_model/nrg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nrg_parser/mast/logger_model/nrg/reader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py,sha256=kXpj6JPISA3sydseuHokpD2MsEN2O7af4jL6kXWlfwk,18053
+nrg_parser/mast/logger_model/nrg/reader/symphoniepro_txt_reader.py,sha256=BDGqdPEbK-FFoIOHgpMYbthlHJk4pUT2z3Aw04yei9Q,18215
+nrg_parser/mast/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nrg_parser/mast/utilities/iea_json/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nrg_parser/mast/utilities/iea_json/convert_to_iea_json.py,sha256=Km4_nfhjaFDhAXVZoA8G9n_fwjjQd6hMt-0obW4681w,11929
 nrg_parser/mast/utilities/iea_json/create_iea_json_nrg.py,sha256=D_GLBhPzyeGYbVJScK0tSO-ylwUk4u8NvmfsQYWr9Gs,4643
 nrg_parser/mast/utilities/iea_json/iea_models.py,sha256=BHAhfjWU-MYXmJZ27RTjCswwidJV9TRTfj-dy6BE1uI,3235
 nrg_parser/mast/utilities/iea_json/nrg_config.py,sha256=mxS4gGAbhjAQxJ1i9ugik7pBZGN634vNJAN312e-4S4,104
-nrg_parser-0.1.0.dist-info/LICENSE,sha256=ly4sLPpm5eooZ_HoEhx7Lu0YmLgr5Ppzr92YeDCExUI,1074
-nrg_parser-0.1.0.dist-info/METADATA,sha256=wULKShjhNHd-NRs8bDra0kofEq6aSbLYRGNTt0PGxSc,1032
-nrg_parser-0.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-nrg_parser-0.1.0.dist-info/RECORD,,
+nrg_parser-0.1.1.dist-info/LICENSE,sha256=ly4sLPpm5eooZ_HoEhx7Lu0YmLgr5Ppzr92YeDCExUI,1074
+nrg_parser-0.1.1.dist-info/METADATA,sha256=H7DjxqIBtAHoaohEry-qDf4c9ePLVSqNSke91RZFStM,2114
+nrg_parser-0.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+nrg_parser-0.1.1.dist-info/RECORD,,
```

