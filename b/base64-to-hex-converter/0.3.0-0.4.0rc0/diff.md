# Comparing `tmp/base64-to-hex-converter-0.3.0.tar.gz` & `tmp/base64-to-hex-converter-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base64-to-hex-converter-0.3.0.tar", last modified: Wed Jul 20 16:54:32 2022, max compression
+gzip compressed data, was "base64-to-hex-converter-0.4.0rc0.tar", last modified: Tue Jul 25 18:27:32 2023, max compression
```

## Comparing `base64-to-hex-converter-0.3.0.tar` & `base64-to-hex-converter-0.4.0rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    35149 2022-07-12 12:30:10.000000 base64-to-hex-converter-0.3.0/LICENSE
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      976 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/PKG-INFO
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      150 2022-07-12 13:20:00.000000 base64-to-hex-converter-0.3.0/README.md
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       84 2022-07-12 12:30:10.000000 base64-to-hex-converter-0.3.0/pyproject.toml
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      917 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/setup.cfg
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/src/
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/src/b64to16/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       74 2022-07-13 14:02:48.000000 base64-to-hex-converter-0.3.0/src/b64to16/__init__.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      971 2022-07-20 16:46:01.000000 base64-to-hex-converter-0.3.0/src/b64to16/__main__.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     2901 2022-07-20 16:52:25.000000 base64-to-hex-converter-0.3.0/src/b64to16/b64to16.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       22 2022-07-20 16:53:42.000000 base64-to-hex-converter-0.3.0/src/b64to16/version.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-20 16:54:32.959898 base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      976 2022-07-20 16:54:32.000000 base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/PKG-INFO
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      340 2022-07-20 16:54:32.000000 base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2022-07-20 16:54:32.000000 base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        8 2022-07-20 16:54:32.000000 base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/top_level.txt
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    35149 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/LICENSE
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      979 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      150 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/README.md
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       84 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/pyproject.toml
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      917 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/setup.cfg
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/b64to16/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       74 2023-07-25 18:04:15.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/__init__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1111 2023-07-25 18:19:24.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/__main__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     3807 2023-07-25 18:14:27.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/b64to16.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       26 2023-07-25 18:25:08.000000 base64-to-hex-converter-0.4.0rc0/src/b64to16/version.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-25 18:27:32.241430 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      979 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      340 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        8 2023-07-25 18:27:32.000000 base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/top_level.txt
```

### Comparing `base64-to-hex-converter-0.3.0/LICENSE` & `base64-to-hex-converter-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.3.0/PKG-INFO` & `base64-to-hex-converter-0.4.0rc0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base64-to-hex-converter
-Version: 0.3.0
+Version: 0.4.0rc0
 Summary: Base64 to Hexadecimal Converter
 Home-page: https://github.com/guidanoli/base64-to-hex-converter
 Author: Guilherme Dantas
 Author-email: guidanoli@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/guidanoli/base64-to-hex-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `base64-to-hex-converter-0.3.0/setup.cfg` & `base64-to-hex-converter-0.4.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `base64-to-hex-converter-0.3.0/src/b64to16/__main__.py` & `base64-to-hex-converter-0.4.0rc0/src/b64to16/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import sys
 
 from .version import __version__
 from .b64to16 import Base64to16Converter
 
 
 if __name__ == '__main__':
     about = 'Converts data in Base64 to Hexadecimal'
@@ -12,24 +13,31 @@
         '-v',
         '--version',
         action='version',
         version=__version__)
     parser.add_argument(
         'json_file',
         type=str,
+        nargs='?',
         help='path to a JSON file')
     parser.add_argument(
         '-x',
         action='store_true',
         help="do not prefix hexadecimal strings with '0x'")
     parser.add_argument(
         '-k',
         action='store_true',
         help=("convert dictionary keys to hexadecimal strings too" +
               " (might cause conflicts)"))
+
     args = parser.parse_args()
     cvt = Base64to16Converter(
         hexprefix=(not args.x),
         cvtkeys=args.k,
     )
-    json_data = cvt.convert_json(args.json_file)
+
+    if args.json_file:
+        json_data = cvt.convert_json_from_filename(args.json_file)
+    else:
+        json_data = cvt.convert_json_from_fp(sys.stdin)
+
     print(json_data)
```

### Comparing `base64-to-hex-converter-0.3.0/src/b64to16/b64to16.py` & `base64-to-hex-converter-0.4.0rc0/src/b64to16/b64to16.py`

 * *Files 15% similar despite different names*

```diff
@@ -70,22 +70,49 @@
             try:
                 return self.convert_string(data)
             except binascii.Error:
                 return data
         else:
             return data
 
-    def convert_json(self, json_file):
+    def convert_json_from_fp(self, fp):
+        """Processes JSON input, converting all string values in Base64 format
+        into hexadecimal strings. Assumes input is in JSON format.
+        If not, raises a json.JSONDecodeError.
+
+        Arguments:
+            json_file - path to the JSON file
+
+        Returns:
+            transformed JSON string
+        """
+        json_data = json.load(fp)
+        data = self.convert_data(json_data)
+        return json.dumps(data)
+
+    def convert_json_from_filename(self, json_file):
         """Processes a JSON file, converting all string values in Base64 format
         into hexadecimal strings. Assumes file is in JSON format.
         If not, raises a json.JSONDecodeError.
 
         Arguments:
             json_file - path to the JSON file
 
         Returns:
             transformed JSON string
         """
         with open(json_file) as fp:
-            json_data = json.load(fp)
-            data = self.convert_data(json_data)
-            return json.dumps(data)
+            return self.convert_json_from_fp(fp)
+
+    def convert_json(self, json_filename):
+        """Processes a JSON file, converting all string values in Base64 format
+        into hexadecimal strings. Assumes file is in JSON format.
+        If not, raises a json.JSONDecodeError.
+        Deprecated. Use `convert_json_from_filename`.
+
+        Arguments:
+            json_filename - path to the JSON file
+
+        Returns:
+            transformed JSON string
+        """
+        return self.convert_json_from_filename(json_filename)
```

### Comparing `base64-to-hex-converter-0.3.0/src/base64_to_hex_converter.egg-info/PKG-INFO` & `base64-to-hex-converter-0.4.0rc0/src/base64_to_hex_converter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base64-to-hex-converter
-Version: 0.3.0
+Version: 0.4.0rc0
 Summary: Base64 to Hexadecimal Converter
 Home-page: https://github.com/guidanoli/base64-to-hex-converter
 Author: Guilherme Dantas
 Author-email: guidanoli@hotmail.com
 License: GNU General Public License v3.0
 Project-URL: Bug Tracker, https://github.com/guidanoli/base64-to-hex-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
```

