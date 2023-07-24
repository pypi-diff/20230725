# Comparing `tmp/potassium-0.1.1.tar.gz` & `tmp/potassium-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potassium-0.1.1.tar", last modified: Thu Jun 29 05:38:32 2023, max compression
+gzip compressed data, was "potassium-0.1.2.tar", last modified: Mon Jul 24 22:00:46 2023, max compression
```

## Comparing `potassium-0.1.1.tar` & `potassium-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-29 05:38:32.079012 potassium-0.1.1/
--rw-r--r--   0 erik       (501) staff       (20)    11357 2023-04-24 01:09:41.000000 potassium-0.1.1/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)     7116 2023-06-29 05:38:32.078849 potassium-0.1.1/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     6450 2023-06-23 18:01:41.000000 potassium-0.1.1/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-29 05:38:32.077816 potassium-0.1.1/potassium/
--rw-r--r--   0 erik       (501) staff       (20)       83 2023-06-06 23:50:04.000000 potassium-0.1.1/potassium/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)      221 2023-04-24 01:09:41.000000 potassium-0.1.1/potassium/hooks.py
--rw-r--r--   0 erik       (501) staff       (20)     6373 2023-06-29 05:33:20.000000 potassium-0.1.1/potassium/potassium.py
--rw-r--r--   0 erik       (501) staff       (20)     5500 2023-06-23 18:01:41.000000 potassium-0.1.1/potassium/store.py
--rw-r--r--   0 erik       (501) staff       (20)     2397 2023-06-23 18:01:41.000000 potassium-0.1.1/potassium/store_test.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-29 05:38:32.078614 potassium-0.1.1/potassium.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     7116 2023-06-29 05:38:32.000000 potassium-0.1.1/potassium.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      297 2023-06-29 05:38:32.000000 potassium-0.1.1/potassium.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-29 05:38:32.000000 potassium-0.1.1/potassium.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       37 2023-06-29 05:38:32.000000 potassium-0.1.1/potassium.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       10 2023-06-29 05:38:32.000000 potassium-0.1.1/potassium.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       38 2023-06-29 05:38:32.079059 potassium-0.1.1/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1275 2023-06-29 05:29:34.000000 potassium-0.1.1/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-07-24 22:00:46.484933 potassium-0.1.2/
+-rw-r--r--   0 erik       (501) staff       (20)    11357 2023-04-24 01:09:41.000000 potassium-0.1.2/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)     7116 2023-07-24 22:00:46.484788 potassium-0.1.2/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     6450 2023-07-24 18:52:23.000000 potassium-0.1.2/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-07-24 22:00:46.484105 potassium-0.1.2/potassium/
+-rw-r--r--   0 erik       (501) staff       (20)       83 2023-06-06 23:50:04.000000 potassium-0.1.2/potassium/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)      221 2023-04-24 01:09:41.000000 potassium-0.1.2/potassium/hooks.py
+-rw-r--r--   0 erik       (501) staff       (20)     7406 2023-07-24 20:55:31.000000 potassium-0.1.2/potassium/potassium.py
+-rw-r--r--   0 erik       (501) staff       (20)     5500 2023-06-23 18:01:41.000000 potassium-0.1.2/potassium/store.py
+-rw-r--r--   0 erik       (501) staff       (20)     2397 2023-06-23 18:01:41.000000 potassium-0.1.2/potassium/store_test.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-07-24 22:00:46.484612 potassium-0.1.2/potassium.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     7116 2023-07-24 22:00:46.000000 potassium-0.1.2/potassium.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      297 2023-07-24 22:00:46.000000 potassium-0.1.2/potassium.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-07-24 22:00:46.000000 potassium-0.1.2/potassium.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       37 2023-07-24 22:00:46.000000 potassium-0.1.2/potassium.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       10 2023-07-24 22:00:46.000000 potassium-0.1.2/potassium.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       38 2023-07-24 22:00:46.484984 potassium-0.1.2/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1275 2023-07-24 21:56:55.000000 potassium-0.1.2/setup.py
```

### Comparing `potassium-0.1.1/LICENSE` & `potassium-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `potassium-0.1.1/PKG-INFO` & `potassium-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potassium
-Version: 0.1.1
+Version: 0.1.2
 Summary: The potassium package is a flask-like HTTP server for serving large AI models
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `potassium-0.1.1/README.md` & `potassium-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `potassium-0.1.1/potassium/potassium.py` & `potassium-0.1.2/potassium/potassium.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 
 class Potassium():
     "Potassium is a simple, stateful, GPU-enabled, and autoscaleable web framework for deploying machine learning models."
 
     def __init__(self, name):
         self.name = name
 
-        def default_func():
-            return
+        # default init function, if the user doesn't specify one
+        def empty_init():
+            return {}
 
         # semi-private vars, not intended for users to modify
-        self._init_func = default_func
+        self._init_func = empty_init
         self._endpoints = {}  # dictionary to store unlimited Endpoints, by unique route
         self._context = {}
         self._lock = Lock()
         self._event_chan = Queue(maxsize=1)
 
     #
     def init(self, func):
@@ -49,17 +50,33 @@
         Notes:
         - this function must return a dictionary
         - the context is not persisted to disk, and will be reloaded on server restart
         - the context is not shared between multiple replicas of the app
         """
 
         def wrapper():
+            print(colored("Running init()", 'yellow'))
             self._context = func()
+            if not isinstance(self._context, dict):
+                raise Exception("Potassium init() must return a dictionary")
+            
         self._init_func = wrapper
         return wrapper
+    
+    @staticmethod
+    def _standardize_route(route):
+        # handle empty or None case
+        if len(route) == 0 or route == None:
+            route = "/"
+
+        # prepend with "/" if not already, as router expects
+        if route[0] != "/":
+            route = "/" + route
+        
+        return route
 
     # handler is a blocking http POST handler
     def handler(self, route: str = "/"):
         "handler is a blocking http POST handler"
         def actual_decorator(func):
             @functools.wraps(func)
             def wrapper(request):
@@ -72,27 +89,37 @@
                 # check if out.json is a dict
                 if type(out.json) != dict:
                     raise Exception(
                         "Potassium Response object json must be a dict")
 
                 return out
 
+            nonlocal route # we need to modify the route variable in the outer scope
+            route = self._standardize_route(route)
+            if route in self._endpoints:
+                raise Exception("Route already in use")
+            
             self._endpoints[route] = Endpoint(type="handler", func=wrapper)
             return wrapper
         return actual_decorator
 
     # background is a non-blocking http POST handler
-    def background(self, route: str = "/"):
+    def background(self, route: str = "/"):    
         "background is a non-blocking http POST handler"
         def actual_decorator(func):
             @functools.wraps(func)
             def wrapper(request):
                 # send in app's stateful context if GPU, and the request
                 return func(self._context, request)
-
+            
+            nonlocal route # we need to modify the route variable in the outer scope
+            route = self._standardize_route(route)
+            if route in self._endpoints:
+                raise Exception("Route already in use")
+            
             self._endpoints[route] = Endpoint(
                 type="background", func=wrapper)
             return wrapper
         return actual_decorator
 
     # _handle_generic takes in a request and the endpoint it was routed to and handles it as expected by that endpoint
     def _handle_generic(self, route, endpoint, flask_request):
@@ -175,13 +202,12 @@
             return self._handle_generic(route, endpoint, request)
 
         return flask_app
 
     # serve runs the http server
     def serve(self, host="0.0.0.0", port=8000):
         print(colored("------\nStarting Potassium Server 🍌", 'yellow'))
-        print(colored("Running init()", 'yellow'))
         self._init_func()
         flask_app = self._create_flask_app()
         server = make_server(host, port, flask_app)
         print(colored(f"Serving at http://{host}:{port}\n------", 'green'))
         server.serve_forever()
```

### Comparing `potassium-0.1.1/potassium/store.py` & `potassium-0.1.2/potassium/store.py`

 * *Files identical despite different names*

### Comparing `potassium-0.1.1/potassium/store_test.py` & `potassium-0.1.2/potassium/store_test.py`

 * *Files identical despite different names*

### Comparing `potassium-0.1.1/potassium.egg-info/PKG-INFO` & `potassium-0.1.2/potassium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potassium
-Version: 0.1.1
+Version: 0.1.2
 Summary: The potassium package is a flask-like HTTP server for serving large AI models
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `potassium-0.1.1/setup.py` & `potassium-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='potassium',
     packages=['potassium'],
-    version='0.1.1',
+    version='0.1.2',
     license='Apache License 2.0',
     # Give a short description about your library
     description='The potassium package is a flask-like HTTP server for serving large AI models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
```

