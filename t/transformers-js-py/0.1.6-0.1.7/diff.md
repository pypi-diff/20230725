# Comparing `tmp/transformers_js_py-0.1.6.tar.gz` & `tmp/transformers_js_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.1.6.tar", max compression
+gzip compressed data, was "transformers_js_py-0.1.7.tar", max compression
```

## Comparing `transformers_js_py-0.1.6.tar` & `transformers_js_py-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-25 12:46:01.630470 transformers_js_py-0.1.6/LICENSE
--rw-r--r--   0        0        0     3879 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/README.md
--rw-r--r--   0        0        0      579 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2755 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/transformers_js/__init__.py
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 transformers_js_py-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3982 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/README.md
+-rw-r--r--   0        0        0      579 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/transformers_js/__init__.py
+-rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 transformers_js_py-0.1.7/PKG-INFO
```

### Comparing `transformers_js_py-0.1.6/LICENSE` & `transformers_js_py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.6/README.md` & `transformers_js_py-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 # [{'label': 'POSITIVE', 'score': 0.999817686}]
 ```
 
 </td>
 </tr>
 </table>
 
+See the [Transformers.js document](https://github.com/xenova/transformers.js/) for available features.
 
 ## Examples
 
 ### stlite
 
 [🎈Online Demo](https://edit.share.stlite.net/#!ChBzdHJlYW1saXRfYXBwLnB5EvwDChBzdHJlYW1saXRfYXBwLnB5EucDCuQDaW1wb3J0IHN0cmVhbWxpdCBhcyBzdAoKZnJvbSB0cmFuc2Zvcm1lcnNfanMgaW1wb3J0IGltcG9ydF90cmFuc2Zvcm1lcnNfanMKCnN0LnRpdGxlKCJTZW50aW1lbnQgYW5hbHlzaXMiKQoKdGV4dCA9IHN0LnRleHRfaW5wdXQoIklucHV0IHNvbWUgdGV4dCIpCgppZiB0ZXh0OgogICAgd2l0aCBzdC5zcGlubmVyKCk6CiAgICAgICAgdHJhbnNmb3JtZXJzID0gYXdhaXQgaW1wb3J0X3RyYW5zZm9ybWVyc19qcygpCiAgICAgICAgcGlwZWxpbmUgPSB0cmFuc2Zvcm1lcnMucGlwZWxpbmUKICAgICAgICBpZiAicGlwZSIgbm90IGluIHN0LnNlc3Npb25fc3RhdGU6CiAgICAgICAgICAgIHN0LnNlc3Npb25fc3RhdGVbInBpcGUiXSA9IGF3YWl0IHBpcGVsaW5lKCdzZW50aW1lbnQtYW5hbHlzaXMnKQogICAgICAgIHBpcGUgPSBzdC5zZXNzaW9uX3N0YXRlWyJwaXBlIl0KICAgICAgICBvdXQgPSBhd2FpdCBwaXBlKHRleHQpCiAgICBzdC53cml0ZShvdXQpChoSdHJhbnNmb3JtZXJzX2pzX3B5)
```

### Comparing `transformers_js_py-0.1.6/pyproject.toml` & `transformers_js_py-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "transformers_js"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformers_js_py-0.1.6/transformers_js/__init__.py` & `transformers_js_py-0.1.7/transformers_js/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,17 @@
     return obj
 
 
 async def import_transformers_js():
     pyodide.code.run_js(
         """
     async function loadTransformersJs() {
-        const isBrowser = typeof window !== 'undefined';
+        const isBrowserMainThread = typeof window !== 'undefined';
+        const isWorker = typeof self !== 'undefined' && typeof self.postMessage === 'function' && typeof self.importScripts === 'function';
+        const isBrowser = isBrowserMainThread || isWorker;
         const transformers = await import(isBrowser ? 'https://cdn.jsdelivr.net/npm/@xenova/transformers@2.4.2' : '@xenova/transformers');
 
         transformers.env.allowLocalModels = false;
 
         globalThis._transformers = {  // Convert a module to an object.
             ...transformers,
         };
```

### Comparing `transformers_js_py-0.1.6/PKG-INFO` & `transformers_js_py-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-js-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: Apache-2.0
 Author: Yuichiro Tachibana (Tsuchiya)
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -56,14 +56,15 @@
 # [{'label': 'POSITIVE', 'score': 0.999817686}]
 ```
 
 </td>
 </tr>
 </table>
 
+See the [Transformers.js document](https://github.com/xenova/transformers.js/) for available features.
 
 ## Examples
 
 ### stlite
 
 [🎈Online Demo](https://edit.share.stlite.net/#!ChBzdHJlYW1saXRfYXBwLnB5EvwDChBzdHJlYW1saXRfYXBwLnB5EucDCuQDaW1wb3J0IHN0cmVhbWxpdCBhcyBzdAoKZnJvbSB0cmFuc2Zvcm1lcnNfanMgaW1wb3J0IGltcG9ydF90cmFuc2Zvcm1lcnNfanMKCnN0LnRpdGxlKCJTZW50aW1lbnQgYW5hbHlzaXMiKQoKdGV4dCA9IHN0LnRleHRfaW5wdXQoIklucHV0IHNvbWUgdGV4dCIpCgppZiB0ZXh0OgogICAgd2l0aCBzdC5zcGlubmVyKCk6CiAgICAgICAgdHJhbnNmb3JtZXJzID0gYXdhaXQgaW1wb3J0X3RyYW5zZm9ybWVyc19qcygpCiAgICAgICAgcGlwZWxpbmUgPSB0cmFuc2Zvcm1lcnMucGlwZWxpbmUKICAgICAgICBpZiAicGlwZSIgbm90IGluIHN0LnNlc3Npb25fc3RhdGU6CiAgICAgICAgICAgIHN0LnNlc3Npb25fc3RhdGVbInBpcGUiXSA9IGF3YWl0IHBpcGVsaW5lKCdzZW50aW1lbnQtYW5hbHlzaXMnKQogICAgICAgIHBpcGUgPSBzdC5zZXNzaW9uX3N0YXRlWyJwaXBlIl0KICAgICAgICBvdXQgPSBhd2FpdCBwaXBlKHRleHQpCiAgICBzdC53cml0ZShvdXQpChoSdHJhbnNmb3JtZXJzX2pzX3B5)
```

