# Comparing `tmp/aksharify-0.1.6.tar.gz` & `tmp/aksharify-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.6.tar", max compression
+gzip compressed data, was "aksharify-0.1.7.tar", max compression
```

## Comparing `aksharify-0.1.6.tar` & `aksharify-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.6/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-24 12:10:44.889223 aksharify-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.6/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.6/src/aksharify/__init__.py
--rw-r--r--   0        0        0     5546 2023-07-24 11:46:55.981672 aksharify-0.1.6/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5327 2023-07-24 12:06:38.063502 aksharify-0.1.6/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1565 2023-07-23 09:44:07.082682 aksharify-0.1.6/src/aksharify/image.py
--rw-r--r--   0        0        0     4946 2023-07-23 04:22:55.602321 aksharify-0.1.6/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-25 06:50:23.423792 aksharify-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.7/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.7/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     5546 2023-07-24 11:46:55.981672 aksharify-0.1.7/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.7/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.7/src/aksharify/image.py
+-rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.7/src/aksharify/interactive.py
+-rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.7/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.7/PKG-INFO
```

### Comparing `aksharify-0.1.6/LICENSE.md` & `aksharify-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.6/pyproject.toml` & `aksharify-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.6"
+version = "0.1.7"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
```

### Comparing `aksharify-0.1.6/README.md` & `aksharify-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.6/src/aksharify/aksharify.py` & `aksharify-0.1.7/src/aksharify/aksharify.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.6/src/aksharify/distributions.py` & `aksharify-0.1.7/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.6/src/aksharify/image.py` & `aksharify-0.1.7/src/aksharify/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
             raise ValueError("Provide image or link to the Image")
         elif path:
             self.obj = ski.io.imread(path)
         else:
             response = requests.get(url)
             image_data = response.content
             self.obj = ski.io.imread(BytesIO(image_data))
+        self.refresh()
+
+    def refresh(self):
         self.image = self.obj
         self.bwimg = ski.color.rgb2gray(self.obj[:,:,:3])
         self.w, self.h = self.obj.shape[1], self.obj.shape[0]
         
     def show(self, grayscale=False):
         plt.axis('off')
         if not grayscale:
```

### Comparing `aksharify-0.1.6/src/aksharify/outputs.py` & `aksharify-0.1.7/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.6/PKG-INFO` & `aksharify-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
```

