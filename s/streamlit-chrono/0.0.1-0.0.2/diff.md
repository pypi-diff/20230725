# Comparing `tmp/streamlit-chrono-0.0.1.tar.gz` & `tmp/streamlit-chrono-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chrono-0.0.1.tar", last modified: Tue Jul 25 18:53:37 2023, max compression
+gzip compressed data, was "streamlit-chrono-0.0.2.tar", last modified: Tue Jul 25 18:57:02 2023, max compression
```

## Comparing `streamlit-chrono-0.0.1.tar` & `streamlit-chrono-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.989576 streamlit-chrono-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-07-25 14:11:06.000000 streamlit-chrono-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       53 2023-07-25 18:47:11.000000 streamlit-chrono-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1123 2023-07-25 18:53:36.987581 streamlit-chrono-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-25 18:52:15.000000 streamlit-chrono-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 18:53:36.990577 streamlit-chrono-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-07-25 18:25:57.000000 streamlit-chrono-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.887715 streamlit-chrono-0.0.1/streamlit_chrono/
--rw-rw-rw-   0        0        0     9602 2023-07-25 18:20:58.000000 streamlit-chrono-0.0.1/streamlit_chrono/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.851450 streamlit-chrono-0.0.1/streamlit_chrono/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.946929 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/
--rw-rw-rw-   0        0        0      221 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-25 14:11:06.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.859445 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.975586 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/
--rw-rw-rw-   0        0        0   509474 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js
--rw-rw-rw-   0        0        0     1664 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1656103 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.map
-drwxrwxrwx   0        0        0        0 2023-07-25 18:53:36.924516 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/
--rw-rw-rw-   0        0        0     1123 2023-07-25 18:53:10.000000 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-07-25 18:53:36.000000 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:53:10.000000 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-25 18:53:10.000000 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-25 18:53:10.000000 streamlit-chrono-0.0.1/streamlit_chrono.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.363209 streamlit-chrono-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 14:11:06.000000 streamlit-chrono-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-25 18:47:11.000000 streamlit-chrono-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1156 2023-07-25 18:57:02.360200 streamlit-chrono-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-07-25 18:54:34.000000 streamlit-chrono-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:57:02.364210 streamlit-chrono-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-25 18:55:50.000000 streamlit-chrono-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.260202 streamlit-chrono-0.0.2/streamlit_chrono/
+-rw-rw-rw-   0        0        0     9602 2023-07-25 18:20:58.000000 streamlit-chrono-0.0.2/streamlit_chrono/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.219462 streamlit-chrono-0.0.2/streamlit_chrono/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.321203 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/
+-rw-rw-rw-   0        0        0      221 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-25 14:11:06.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.227471 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.348496 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   509474 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js
+-rw-rw-rw-   0        0        0     1664 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1656103 2023-07-25 18:19:38.000000 streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.map
+drwxrwxrwx   0        0        0        0 2023-07-25 18:57:02.300203 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-07-25 18:56:34.000000 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2023-07-25 18:57:01.000000 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:56:34.000000 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 18:56:34.000000 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-25 18:56:34.000000 streamlit-chrono-0.0.2/streamlit_chrono.egg-info/top_level.txt
```

### Comparing `streamlit-chrono-0.0.1/LICENSE` & `streamlit-chrono-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/PKG-INFO` & `streamlit-chrono-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: streamlit-chrono
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to add Chrono Timeline
-Home-page: 
+Home-page: https://github.com/keshavd/streamlit-chrono
 Author: Keshav Dial
 Author-email: keshav.dial@sanofi.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# streamlit-custom-component
+# streamlit-chrono
 
 Streamlit port of the react-chrono library. Allows for the rendering of timelines with cards.
 
 ## Installation instructions
 
 ```sh
 pip install streamlit-chrono
```

### Comparing `streamlit-chrono-0.0.1/README.md` & `streamlit-chrono-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# streamlit-custom-component
+# streamlit-chrono
 
 Streamlit port of the react-chrono library. Allows for the rendering of timelines with cards.
 
 ## Installation instructions
 
 ```sh
 pip install streamlit-chrono
```

### Comparing `streamlit-chrono-0.0.1/setup.py` & `streamlit-chrono-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-chrono",
-    version="0.0.1",
+    version="0.0.2",
     author="Keshav Dial",
     author_email="keshav.dial@sanofi.com",
     description="Streamlit component that allows you to add Chrono Timeline",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="",
+    url="https://github.com/keshavd/streamlit-chrono",
     packages=setuptools.find_namespace_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.7",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
```

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono/__init__.py` & `streamlit-chrono-0.0.2/streamlit_chrono/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/bootstrap.min.css` & `streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js` & `streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.LICENSE.txt` & `streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.map` & `streamlit-chrono-0.0.2/streamlit_chrono/frontend/build/static/js/main.7714f0cc.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono.egg-info/PKG-INFO` & `streamlit-chrono-0.0.2/streamlit_chrono.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: streamlit-chrono
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to add Chrono Timeline
-Home-page: 
+Home-page: https://github.com/keshavd/streamlit-chrono
 Author: Keshav Dial
 Author-email: keshav.dial@sanofi.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# streamlit-custom-component
+# streamlit-chrono
 
 Streamlit port of the react-chrono library. Allows for the rendering of timelines with cards.
 
 ## Installation instructions
 
 ```sh
 pip install streamlit-chrono
```

### Comparing `streamlit-chrono-0.0.1/streamlit_chrono.egg-info/SOURCES.txt` & `streamlit-chrono-0.0.2/streamlit_chrono.egg-info/SOURCES.txt`

 * *Files identical despite different names*

