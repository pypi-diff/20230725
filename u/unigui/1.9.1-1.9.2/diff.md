# Comparing `tmp/unigui-1.9.1.tar.gz` & `tmp/unigui-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.1.tar", last modified: Sat Jul 22 23:32:35 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.2.tar", last modified: Tue Jul 25 17:54:52 2023, max compression
```

## Comparing `unigui-1.9.1.tar` & `unigui-1.9.2.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     8640 2023-07-21 16:29:57.000000 unigui-1.9.1/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     2700 2023-07-21 15:52:14.000000 unigui-1.9.1/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      108 2023-07-21 04:22:38.000000 unigui-1.9.1/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     4772 2023-07-21 16:20:46.000000 unigui-1.9.1/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2490 2023-07-21 10:20:58.000000 unigui-1.9.1/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5587 2023-07-19 22:23:17.000000 unigui-1.9.1/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8110 2023-07-21 04:21:24.000000 unigui-1.9.1/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/css/9.44b298e4.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/css/vendor.191faa77.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)    37826 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/css/vendor.191faa77.css.gz
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)  1434158 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/vendor.18cce91f.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5860 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/app.c7c500ce.js
--rw-rw-r--   0 george    (1000) george    (1000)    14595 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/9.100130f6.js.gz
--rw-rw-r--   0 george    (1000) george    (1000)   469773 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/vendor.18cce91f.js.gz
--rw-rw-r--   0 george    (1000) george    (1000)    47791 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/9.100130f6.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-22 22:58:02.000000 unigui-1.9.1/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.1/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      630 2023-07-22 23:30:56.000000 unigui-1.9.1/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-22 23:32:35.000000 unigui-1.9.1/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-22 23:32:35.000000 unigui-1.9.1/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.1/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.1/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       54 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.1/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1342 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-22 23:32:35.000000 unigui-1.9.1/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5365 2023-07-25 04:13:41.000000 unigui-1.9.2/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3583 2023-07-25 06:24:07.000000 unigui-1.9.2/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.2/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.2/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7226 2023-07-25 05:54:26.000000 unigui-1.9.2/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.2/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.2/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8678 2023-07-24 17:31:39.000000 unigui-1.9.2/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/344.ca964e27.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/vendor.f747ec02.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/vendor.5659ce27.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    48615 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/344.037a8712.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/app.1711f3eb.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      630 2023-07-25 17:54:11.000000 unigui-1.9.2/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-25 17:54:52.000000 unigui-1.9.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-25 17:54:52.000000 unigui-1.9.2/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.2/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       54 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.2/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.1/unigui/guielements.py` & `unigui-1.9.2/unigui/users.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,253 +1,242 @@
-from . import utils
-
-class Gui:
-    def __init__(self, *args, **kwargs):
-        self.name = args[0]
-        la = len(args)
-        if la > 1:
-            self.value = args[1]
-        if la > 2:
-            self.changed = args[2]
-        for key in kwargs.keys():            
-            self.add(key, kwargs[key]) 
+import importlib
+from .utils import *
+from .guielements import *
+import sys
+import asyncio
+from threading import Thread
+import logging
+
+class User:      
+    def __init__(self):          
+        self.screens = []        
+        self.active_dialog = None
+        self.screen_module = None    
+        self.__handlers__ = {}                    
+        User.last_user = self     
+
+    def sync_send(self, obj):
+        asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
+
+    def progress(self, str, *updates):
+        """open or update progress window if str != null else close it  """             
+        return self.sync_send(TextMessage('progress', str, *updates, user = self))
+                   
+    def load_screen(self, file):
+        screen_vars = {
+            'icon' : None,
+            'prepare' : None,            
+            'blocks' : [],
+            'header' : config.appname,                        
+            'toolbar' : [], 
+            'order' : 0
+        }             
+        name = file[:-3]        
+        path = f'{screens_dir}/{file}'                
+        spec = importlib.util.spec_from_file_location(name,path)
+        module = importlib.util.module_from_spec(spec)        
+                
+        module.user = self                               
         
-    def add(self, attr, value):
-        setattr(self, attr, value) 
-
-    def mutate(self, obj):
-        self.__dict__ = obj.__dict__    
-
-    def accept(self, value):
-        if hasattr(self, 'changed'):
-            self.changed(self, value)
-        else:
-            self.value = value
-
-Line = Gui("Line", type = 'line')
-
-def smart_complete(lst, min_input_length = 1, max_output_length = 10):
-    di = {it: it.lower() for it in lst}
-    def complete(gui, ustr):
-        if len(ustr) < min_input_length:
-            return []
-        ustr = ustr.lower()
-        arr = [(itlow.find(ustr), it) for it, itlow in di.items() if itlow.find(ustr) != -1]
-        arr.sort(key=lambda e: e[0])
-        if len(arr) > max_output_length:
-            arr = arr[: max_output_length]
-        return [e[1] for e in arr]
-    return complete
-
-class Edit(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)        
-        if 'type' not in kwargs:
-            self.type =  'autoedit' if 'complete' in kwargs else 'edit'
-        if not hasattr(self,'value'):
-            self.value = '' if self.type != 'number' else 0
-
-class Text(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.value = ''
-        self.edit = False
-
-class Button(Gui):
-    def __init__(self, *args, **kwargs):
-        self.name = args[0]
-        if len(args) > 1:
-            self.changed = args[1]        
-        for key in kwargs.keys():            
-            self.add(key, kwargs[key])
-
-def CameraButton(name, *args):    
-    return Button(name, *args, type = 'camera')
+        spec.loader.exec_module(module)            
+        screen = Screen(module.name)
+        #set system vars
+        for var in screen_vars:                                            
+            setattr(screen, var, getattr(module,var,screen_vars[var]))         
         
-def UploadImageButton(name, handler,**kwargs):    
-    kwargs['type'] = 'image_uploader'
-    if 'width' not in kwargs:
-        kwargs['width'] = 250.0              
-    if 'height' not in kwargs:
-        kwargs['height'] = 300.0         
-    return Button(name, handler, **kwargs)
-
-UploadButton = UploadImageButton
-
-class Image(Gui):
-    '''has to contain file parameter as name'''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.type='image'
-        if not hasattr(self,'width'):
-            self.width = 500.0              
-        if not hasattr(self,'image'):
-            self.image = self.value if hasattr(self, 'value') else None
-
-class Video(Gui):
-    '''has to contain src parameter'''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.type='video'
-        if not hasattr(self,'width'):
-            self.width = 500.0              
-        if not hasattr(self,'src'):
-            raise "No video src reference!"
-        if not hasattr(self,'ratio'):
-            self.ratio = "9/9"
-
-graph_default_value = {'nodes' : [], 'edges' : []}
-
-class Graph(Gui):
-    '''has to contain nodes, edges, see Readme'''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.type='graph'
-        if not hasattr(self,'value'):
-            self.value = graph_default_value
-        if not hasattr(self,'minwidth'):
-            self.minwidth = 600.0              
-        if not hasattr(self,'minheight'):
-            self.minheight = 600.0              
-        if not hasattr(self, 'nodes'):
-            self.nodes = []
-        if not hasattr(self, 'edges'):
-            self.edges = []
-
-class Switch(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if not hasattr(self,'value'):
-            self.value = False
-
-list_types = ['toggles','list','dropdown']
-
-class Select(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if not hasattr(self,'options'):             
-            self.options = []
-        if not hasattr(self,'value'):
-            self.value = None
-
-class Tree(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)         
-        self.type = 'tree' 
-        if not hasattr(self,'options'):
-            self.options = {}        
-        if not hasattr(self,'value'):
-            self.value = None        
-
-def accept_cell_value(table, val):    
-    value, position = val
-    if not isinstance(value, bool):
-        try:
-            value = float(value)        
-        except ValueError:
-            pass
-        table.rows[position[0]][position[1]] = value    
-
-def delete_table_row(table, value):
-    if table.rows:        
-        keyed = len(table.headers) < len(table.rows[0])
-        table.value = value   
-        if isinstance(value, list):        
-            if keyed:
-                table.rows = [row for row in table.rows if row[-1] not in value]
+        if screen.toolbar:
+            screen.toolbar += User.toolbar
+        else: 
+            screen.toolbar = User.toolbar  
+                                
+        module.screen = screen        
+        return module
+
+    def set_clean(self):
+        #remove user modules from sys 
+        if os.path.exists(blocks_dir):
+            for file in os.listdir(blocks_dir):
+                if file.endswith(".py") and file != '__init__.py':
+                    name = f'{blocks_dir}.{file[0:-3]}'
+                    if name in sys.modules:
+                        sys.modules[name].user = self
+                        del sys.modules[name]                          
+    def load(self):              
+        if os.path.exists(screens_dir):
+            for file in os.listdir(screens_dir):
+                if file.endswith(".py") and file != '__init__.py':
+                    module = self.load_screen(file)                
+                    self.screens.append(module)                
+            
+        if self.screens:
+            self.screens.sort(key=lambda s: s.screen.order)            
+            main = self.screens[0]
+            if 'prepare' in dir(main):
+                main.prepare()
+            self.screen_module = main
+            self.update_menu()
+            self.set_clean()       
+            return True                 
+
+    def update_menu(self):
+        menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
+        for s in self.screens:
+            s.screen.menu = menu
+
+    @property
+    def screen(self):        
+        return  self.screen_module.screen 
+
+    def set_screen(self,name):
+        return self.process(['root', name])
+
+    def result4message(self, data):
+        result = None
+        dialog = self.active_dialog
+        if dialog:            
+            if len(data) == 2: #button pressed
+                self.active_dialog = None
+                #data[1] is returned value                                
+                result = dialog.callback(dialog, data[1]) 
             else:
-                value.sort(reverse=True)
-                for v in value:            
-                    del table.rows[v]
-            table.value = []
+                el = self.find_element(data)
+                if el:
+                    result = self.process_element(el, data)                
+        elif len(data) == 2 and not data[1]: #dialog closed            
+            return    
         else:
-            if keyed:            
-                table.rows = [row for row in table.rows if row[-1] != value]
-            else:
-                del table.rows[value]  
-            table.value = None    
-
-def append_table_row(table, value):
-    ''' append has to return new row or error string, val is search string in the table'''
-    new_id_row, search = value #new_id_row == rows count
-    new_row = [''] * len(table.headers)
-    if search:
-        new_row[0] = search
-    table.rows.append(new_row)
-    return new_row
-
-class Table(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)             
-        if not hasattr(self,'headers'):
-            self.headers = []
-        if not hasattr(self,'type'):
-            self.type = 'table'
-        if not hasattr(self,'value'):
-            self.value = None
-        if not hasattr(self,'rows'):
-            self.rows = []
-        if not hasattr(self,'value'):
-            self.value = None
-        if not hasattr(self,'dense'):
-            self.dense = True
-
-        if getattr(self,'edit', True):
-            edit_setting = hasattr(self,'modify') or hasattr(self,'delete') or hasattr(self,'append')
-            if not edit_setting:                             
-                self.delete = delete_table_row             
-                self.append = append_table_row             
-                self.modify = accept_cell_value             
+            result = self.process(data)           
+        if result and isinstance(result, Dialog):
+            self.active_dialog = result
+        return result
+
+    @property
+    def blocks(self):
+        return [self.active_dialog.content] if self.active_dialog and \
+            self.active_dialog.content else self.screen.blocks
+
+    def find_element(self, path):               
+        for bl in flatten(self.blocks):
+            if bl.name == path[0]:
+                for c in bl.value:
+                    if isinstance(c, list):
+                        for sub in c:
+                            if sub.name == path[1]:
+                                return sub
+                    elif c.name == path[1]:
+                        return c
+        if path[0] == 'toolbar':
+            for e in self.screen.toolbar:
+                if e.name == path[1]:                
+                    return e
+
+    def find_path(self, elem):        
+        for bl in flatten(self.blocks):        
+            if bl == elem:
+                return [bl.name]
+            for c in bl.value:
+                if isinstance(c, list):
+                    for sub in c:
+                        if sub == elem:
+                            return [bl.name, sub.name]
+                elif c == elem:
+                    return [bl.name, c.name]
+        for e in self.screen.toolbar:
+            if e == elem:                
+                return ['toolbar', e.name]
+
+    def prepare_result(self, raw):
+        if raw == UpdateScreen:
+            raw = self.screen                        
+        else:
+            if isinstance(raw, Message):
+                raw.fill_paths4(self)                
+            elif isinstance(raw,Gui):
+                raw = Message(raw, user = self)                 
+            elif isinstance(raw, (list, tuple)) and all(isinstance(e,Gui) for e in raw):
+                raw = Message(*raw, user = self)
+        return raw
+
+    def process(self,arr):
+        self.last_input = arr        
+        if arr[0] == 'root':
+            for s in self.screens:
+                if s.name == arr[1]:
+                    self.screen_module = s
+                    if getattr(s.screen,'prepare', False):
+                        s.screen.prepare()
+                    return True            
+            self.log(f'Unknown screen name: {s.name}')
+        else:
+            elem = self.find_element(arr)                        
+            return self.process_element(elem, arr)        
         
-    def selected_list(self):                            
-        return [self.value] if self.value != None else [] if type(self.value) == int else self.value   
-
-    def clean(self):
-        self.rows = []
-        self.value = [] if isinstance(self.value,(tuple, list)) else None
-        return self
+    def process_element(self, elem, arr):        
+        id = arr.pop() if len(arr) == 5 else 0
+        action = arr[-2]        
+        val = arr[-1]
         
-class Block(Gui):
-    def __init__(self, *args, **kwargs):        
-        self.name = args[0]        
-        self.type = 'block'
-        self.value = list(args[1:])
-        for key in kwargs.keys():            
-            self.add(key, kwargs[key])        
-
-    def check(self):
-        ch_names = set()        
-        for child in utils.flatten(self.value):            
-            if child.name in ch_names:                        
-                return f'The block {self.name} contains a duplicated element name "{child.name}"!'                        
-            ch_names.add(child.name)                
-
-class Dialog:  
-    def __init__(self, name, callback, *content, buttons = ['Ok', 'Cancel'], icon = 'not_listed_location'):
-        self.name = name
-        self.callback = callback  
-        self.type = 'dialog'         
-        self.buttons = buttons
+        handler = self.__handlers__.get((elem, action), None)
+        if handler:
+            result = handler(elem, val)                
+            return result
         
-        self.content = Block(name,[], *content, dialog = True, icon = icon) 
+        handler = getattr(elem, action, False)                                
+        if handler:                
+            res = handler(elem, val)  
+            if id:                        
+                res = Answer(res, None, id)                
+            return res
+        elif action == 'changed':
+            if hasattr(elem,'value'): #exlude Buttons and others without 'value'
+                elem.value = val                                        
+            return   
+        self.log(f'{elem} does not contain method for {action} event type!')                     
+        return Error('Internal server error.')
+
+    def reflect(self):        
+        user = User.UserType()
+        user.screens = self.screens
+        if self.screens:
+            user.screen_module = self.screens[0]     
+        user.__handlers__ =  self.__handlers__        
+        return user
+
+    def log(self, str, type = 'error'):        
+        scr = self.screen.name if self.screens else 'omitted'
+        str = f"session: {self.session}, screen: {scr}, message: {self.last_input} \n  {str}"
+        if type == 'error':
+            logging.error(str)
+        else:
+            logging.warning(str)    
 
-class TextViewer(Gui):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.type = 'docviewer' 
-                     
-class Screen(Gui):
-    def __init__(self, *args, **kwargs):
-        self.name = args[0]        
-        for key in kwargs.keys():            
-            self.add(key, kwargs[key])   
-        self.type = 'screen'
-
-    def check(self):
-        bl_names = set()        
-        for bl in utils.flatten(self.blocks):                                    
-            if bl.name in bl_names:
-                return (f'The screen {self.name} contains a duplicated block name {bl.name}!')                
-            bl_names.add(bl.name)
-            errstr = bl.check()    
-            if errstr:
-                return errstr
+def make_user():
+    if config.mirror and User.last_user:
+        user = User.last_user.reflect()
+        ok = user.screens
+    else:
+        user = User.UserType()
+        ok = user.load()
+    if config.mirror:
+        User.reflections.append(user)         
+    return user, ok
+
+#loop and thread is for progress window and sync interactions
+loop = asyncio.new_event_loop()
+
+def f(loop):
+    asyncio.set_event_loop(loop)
+    loop.run_forever() 
+
+async_thread = Thread(target=f, args=(loop,))
+async_thread.start()
+
+def handle(elem, event):
+    def h(fn):
+        User.last_user.__handlers__[elem, event] = fn
+    return h
+
+User.extra_loop = loop
+User.UserType = User
+User.last_user = None
+User.toolbar = []
+User.reflections = []
```

### Comparing `unigui-1.9.1/unigui/server.py` & `unigui-1.9.2/unigui/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,59 +27,74 @@
     file_path  = Path(f"{webpath}{file_path}" )
     if request.path == '/':
         file_path /= 'index.html' 
     
     answer = web.HTTPNotFound() if not file_path.exists() else web.FileResponse(file_path)          
     return answer
 
+def broadcast(message, message_user):
+    screen = message_user.screen_module
+    for user in User.reflections:
+        if user is not message_user and screen is user.screen_module:
+            user.sync_send(message)
+
+def screen_switch_message(message):
+    return len(message) == 2 and message[0] == 'root'
+
 async def websocket_handler(request):
     ws = web.WebSocketResponse()
     await ws.prepare(request)
-    user = User.UserType()
+    user, ok = make_user()
 
     async def send(res):
         res = jsonString(user.prepare_result(res))
         await ws.send_str(res)   
 
     user.send = send     
-    user.session__ = request.remote
-    ok = user.load()    
+    user.session = request.remote    
     await ws.send_str(jsonString(user.screen if ok else empty_app)) 
-
     try:
         async for msg in ws:
             if msg.type == WSMsgType.TEXT:
                 if msg.data == 'close':
                     await ws.close()
                 else:
-                    data = json.loads(msg.data)            
-                    result = user.result4message(data)
+                    input = json.loads(msg.data)            
+                    result = user.result4message(input)
                     if result:            
                         result = user.prepare_result(result)
                         await ws.send_str(jsonString(result))
-                    recorder(data, result)
-
+                    if recorder.record_file:
+                        recorder.accept(input, result)
+                    if config.mirror and not screen_switch_message(input):                        
+                        if result:
+                            broadcast(result, user)                            
+                        msg_object = user.find_element(input)                         
+                        if not isinstance(result, Message) or not result.contains(msg_object):                                                        
+                            broadcast(msg_object, user)
             elif msg.type == WSMsgType.ERROR:
-                print('ws connection closed with exception %s' % ws.exception())
+                user.log('ws connection closed with exception %s' % ws.exception())
     except:        
         user.log(traceback.format_exc())
+
+    if User.reflections:
+        User.reflections.remove(user)
     return ws       
 
 def start(appname = '', user_type = User, http_handlers = []):
     if appname:
         config.appname = appname
 
     User.UserType = user_type    
 
     if config.autotest:
         run_tests()
 
     http_handlers.insert(0, web.get('/ws', websocket_handler))        
-    for h in [web.static(f'/{config.upload_dir}', f"/{app_dir}/{upload_dir}"), 
-        web.get('/{tail:.*}', static_serve), web.post('/', post_handler)]:
-        http_handlers.append(h)
+    http_handlers += [web.static(f'/{config.upload_dir}', f"/{app_dir}/{upload_dir}"), 
+        web.get('/{tail:.*}', static_serve), web.post('/', post_handler)]
 
-    print(f'Start {appname} server on {port} port..')    
+    print(f'Start {appname} web server..')    
     app = web.Application()
     app.add_routes(http_handlers)    
     web.run_app(app,  port=port)
```

### Comparing `unigui-1.9.1/unigui/utils.py` & `unigui-1.9.2/unigui/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,25 +57,29 @@
         return None
     file = open(fname, "wb")
     file.write(response.content)
     file.close() 
     return fname
 
 class Message:
-    def __init__(self, *gui_objects, user = None):
-        if gui_objects:
-            self.updates = [{'data': gui} for gui in gui_objects]
-            if user:
-                self.fill_paths4(user)
+    def __init__(self, *gui_objects, user = None):        
+        self.updates = [{'data': gui} for gui in gui_objects] if gui_objects else []
+        if user:
+            self.fill_paths4(user)
 
     def fill_paths4(self, user):
         if hasattr(self, 'updates'):
             for update in self.updates:
                 update['path'] = user.find_path(update['data'])
 
+    def contains(self, guiobj):
+        for update in self.updates:
+            if guiobj is update['data']:
+                return True
+
 def TextMessage(type, text, *data, user = None):
     message = Message(*data, user=user)
     message.type = type
     message.value = text    
     return message    
 
 def Warning(text, *data):
```

### Comparing `unigui-1.9.1/unigui/reloader.py` & `unigui-1.9.2/unigui/reloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             user.sync_send(True)
 
             free()  
             return module  
 
     class ScreenEventHandler(PatternMatchingEventHandler):    
         def on_modified(self, event):
-            if not event.is_directory and hasattr(User,'last_user'):                            
+            if not event.is_directory and User.last_user:                            
                 short_path = event.src_path[len(cwd) + 1:]
                 arr = short_path.split(divpath) 
                 name = arr[-1]
                 dir = arr[0] if len(arr) > 1 else '' 
                                 
                 if name.endswith('.py'):
                     user = User.last_user
@@ -93,15 +93,15 @@
                             module = user.screen_module
                             if module:
                                 current = module.__file__
                                 if not fresh_module or current != fresh_module.__file__:
                                     reload(current.split(divpath)[-1]) 
                                                     
         def on_deleted(self, event):            
-            if not event.is_directory and hasattr(User,'last_user'):
+            if not event.is_directory and User.last_user:
                 user = User.last_user            
                 arr = event.src_path.split(divpath) 
                 name = arr[-1]
                 dir = arr[-2]  
                 if name.endswith('.py') and dir == 'screens':
                     delfile = f'{dir}/{name}'
                     for i, s in enumerate(user.screens):
```

### Comparing `unigui-1.9.1/unigui/web/favicon.ico` & `unigui-1.9.2/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/css/9.44b298e4.css` & `unigui-1.9.2/unigui/web/css/344.ca964e27.css`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}body[data-v-591efd84]{display:flex;justify-content:center}.custom-caption[data-v-591efd84]{padding:5px!important}.web-camera-container[data-v-591efd84]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-591efd84]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-591efd84]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-591efd84]{opacity:1}.web-camera-container .camera-shoot[data-v-591efd84]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-591efd84]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-591efd84]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-591efd84]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-591efd84]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-591efd84]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-591efd84]{animation:preload-591efd84 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-591efd84]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-591efd84]:nth-child(3){animation-delay:.4s}@keyframes preload-591efd84{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-12be25e8]{height:400px;width:400px}body[data-v-5682537f]{display:flex;justify-content:center}.custom-caption[data-v-5682537f]{padding:5px!important}.web-camera-container[data-v-5682537f]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-5682537f]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-5682537f]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-5682537f]{opacity:1}.web-camera-container .camera-shoot[data-v-5682537f]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-5682537f]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-5682537f]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-5682537f]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-5682537f]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-5682537f]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]{animation:preload-5682537f 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]:nth-child(3){animation-delay:.4s}@keyframes preload-5682537f{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
```

### Comparing `unigui-1.9.1/unigui/web/css/vendor.191faa77.css` & `unigui-1.9.2/unigui/web/css/vendor.f747ec02.css`

 * *Files 0% similar despite different names*

```diff
@@ -1406,15 +1406,15 @@
 000057d0: 736c 6174 6533 6428 302c 2d32 3030 3070  slate3d(0,-2000p
 000057e0: 782c 3029 7d7d 2e7a 6f6f 6d4f 7574 5570  x,0)}}.zoomOutUp
 000057f0: 7b61 6e69 6d61 7469 6f6e 2d6e 616d 653a  {animation-name:
 00005800: 7a6f 6f6d 4f75 7455 703b 7472 616e 7366  zoomOutUp;transf
 00005810: 6f72 6d2d 6f72 6967 696e 3a63 656e 7465  orm-origin:cente
 00005820: 7220 626f 7474 6f6d 7d0a 2f2a 210a 202a  r bottom}./*!. *
 00005830: 202a 2051 7561 7361 7220 4672 616d 6577   * Quasar Framew
-00005840: 6f72 6b20 7632 2e31 322e 320a 202a 202a  ork v2.12.2. * *
+00005840: 6f72 6b20 7632 2e31 322e 330a 202a 202a  ork v2.12.3. * *
 00005850: 2028 6329 2032 3031 352d 7072 6573 656e   (c) 2015-presen
 00005860: 7420 5261 7a76 616e 2053 746f 656e 6573  t Razvan Stoenes
 00005870: 6375 0a20 2a20 2a20 5265 6c65 6173 6564  cu. * * Released
 00005880: 2075 6e64 6572 2074 6865 204d 4954 204c   under the MIT L
 00005890: 6963 656e 7365 2e0a 202a 202a 2f2a 2c3a  icense.. * */*,:
 000058a0: 6166 7465 722c 3a62 6566 6f72 657b 2d77  after,:before{-w
 000058b0: 6562 6b69 742d 7461 702d 6869 6768 6c69  ebkit-tap-highli
```

### Comparing `unigui-1.9.1/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.2/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.2/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.2/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.2/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/js/vendor.18cce91f.js` & `unigui-1.9.2/unigui/web/js/vendor.5659ce27.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -14380,15 +14380,15 @@
                     n.onSSRHydrated.forEach((e => {
                         e()
                     })), n.$q.onSSRHydrated = () => {}
                 })
             }
             const E = function(e, t = {}) {
                 const n = {
-                    version: "2.12.2"
+                    version: "2.12.3"
                 };
                 !1 === S.Uf ? (void 0 !== t.config && Object.assign(S.w6, t.config), n.config = {
                     ...S.w6
                 }, (0, S.tP)()) : n.config = t.config || {}, D(e, t, {
                     parentApp: e,
                     $q: n,
                     lang: t.lang,
@@ -15086,14 +15086,32 @@
                     $q: e,
                     parentApp: t
                 }) {
                     e.dialog = B(A, !0, t), !0 !== this.__installed && (this.create = e.dialog)
                 }
             }
         },
+        589: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                Z: () => s
+            });
+            var r = n(4688),
+                i = n(7506);
+            const o = !1 === r.Lp.has.webStorage ? (0, i.I)() : (0, i.c)("local"),
+                a = {
+                    install({
+                        $q: e
+                    }) {
+                        e.localStorage = o
+                    }
+                };
+            Object.assign(a, o);
+            const s = a
+        },
         6417: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => P
             });
             var r = n(1959),
                 i = n(3673),
@@ -15483,14 +15501,32 @@
                         if (window.localStorage) return e = !0, !0
                     } catch (t) {}
                     return e = !1, !1
                 })), s = !0 === v.is.ios && -1 === window.navigator.vendor.toLowerCase().indexOf("apple"), !0 === o.value ? Object.assign(g, v, a, p) : Object.assign(g, v)
             }
             const m = g
         },
+        7153: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                Z: () => s
+            });
+            var r = n(4688),
+                i = n(7506);
+            const o = !1 === r.Lp.has.webStorage ? (0, i.I)() : (0, i.c)("session"),
+                a = {
+                    install({
+                        $q: e
+                    }) {
+                        e.sessionStorage = o
+                    }
+                };
+            Object.assign(a, o);
+            const s = a
+        },
         9405: (e, t, n) => {
             "use strict";
 
             function r(e, t = 250, n) {
                 let r = null;
 
                 function i() {
@@ -15674,15 +15710,16 @@
         },
         2162: (e, t, n) => {
             "use strict";
             n.d(t, {
                 xb: () => r,
                 Kn: () => i,
                 J_: () => o,
-                hj: () => a
+                Gf: () => a,
+                hj: () => s
             });
             n(71);
 
             function r(e, t) {
                 if (e === t) return !0;
                 if (null !== e && null !== t && "object" === typeof e && "object" === typeof t) {
                     if (e.constructor !== t.constructor) return !1;
@@ -15743,14 +15780,18 @@
             }
 
             function o(e) {
                 return "[object Date]" === Object.prototype.toString.call(e)
             }
 
             function a(e) {
+                return "[object RegExp]" === Object.prototype.toString.call(e)
+            }
+
+            function s(e) {
                 return "number" === typeof e && isFinite(e)
             }
         },
         9916: (e, t, n) => {
             "use strict";
             n.d(t, {
                 m: () => u,
@@ -16331,14 +16372,105 @@
                 return void 0 !== e.appContext.config.globalProperties.$router
             }
 
             function o(e) {
                 return !0 === e.isUnmounted || !0 === e.isDeactivated
             }
         },
+        7506: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                I: () => s,
+                c: () => l
+            });
+            var r = n(4716),
+                i = n(2162);
+
+            function o(e) {
+                return !0 === (0, i.J_)(e) ? "__q_date|" + e.toUTCString() : !0 === (0, i.Gf)(e) ? "__q_expr|" + e.source : "number" === typeof e ? "__q_numb|" + e : "boolean" === typeof e ? "__q_bool|" + (e ? "1" : "0") : "string" === typeof e ? "__q_strn|" + e : "function" === typeof e ? "__q_strn|" + e.toString() : e === Object(e) ? "__q_objt|" + JSON.stringify(e) : e
+            }
+
+            function a(e) {
+                const t = e.length;
+                if (t < 9) return e;
+                const n = e.substring(0, 8),
+                    r = e.substring(9);
+                switch (n) {
+                    case "__q_date":
+                        return new Date(r);
+                    case "__q_expr":
+                        return new RegExp(r);
+                    case "__q_numb":
+                        return Number(r);
+                    case "__q_bool":
+                        return Boolean("1" === r);
+                    case "__q_strn":
+                        return "" + r;
+                    case "__q_objt":
+                        return JSON.parse(r);
+                    default:
+                        return e
+                }
+            }
+
+            function s() {
+                const e = () => null;
+                return {
+                    has: () => !1,
+                    getLength: () => 0,
+                    getItem: e,
+                    getIndex: e,
+                    getKey: e,
+                    getAll: () => {},
+                    getAllKeys: () => [],
+                    set: r.ZT,
+                    remove: r.ZT,
+                    clear: r.ZT,
+                    isEmpty: () => !0
+                }
+            }
+
+            function l(e) {
+                const t = window[e + "Storage"],
+                    n = e => {
+                        const n = t.getItem(e);
+                        return n ? a(n) : null
+                    };
+                return {
+                    has: e => null !== t.getItem(e),
+                    getLength: () => t.length,
+                    getItem: n,
+                    getIndex: e => e < t.length ? n(t.key(e)) : null,
+                    getKey: e => e < t.length ? t.key(e) : null,
+                    getAll: () => {
+                        let e;
+                        const r = {},
+                            i = t.length;
+                        for (let o = 0; o < i; o++) e = t.key(o), r[e] = n(e);
+                        return r
+                    },
+                    getAllKeys: () => {
+                        const e = [],
+                            n = t.length;
+                        for (let r = 0; r < n; r++) e.push(t.key(r));
+                        return e
+                    },
+                    set: (e, n) => {
+                        t.setItem(e, o(n))
+                    },
+                    remove: e => {
+                        t.removeItem(e)
+                    },
+                    clear: () => {
+                        t.clear()
+                    },
+                    isEmpty: () => 0 === t.length
+                }
+            }
+        },
         8400: (e, t, n) => {
             "use strict";
             n.d(t, {
                 b0: () => o,
                 u3: () => a,
                 OI: () => s,
                 f3: () => h,
@@ -16466,15 +16598,15 @@
             n.d(t, {
                 Z: () => a
             });
             var r = n(112),
                 i = n(9111),
                 o = n(9409);
             const a = {
-                version: "2.12.2",
+                version: "2.12.3",
                 install: r.Z,
                 lang: i.Z,
                 iconSet: o.Z
             }
         },
         8231: e => {
             e.exports = function(e) {
```

### Comparing `unigui-1.9.1/unigui/web/js/430.591e9a73.js` & `unigui-1.9.2/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/js/app.c7c500ce.js` & `unigui-1.9.2/unigui/web/js/app.1711f3eb.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 (() => {
     "use strict";
     var e = {
             653: (e, t, r) => {
                 r(5363), r(71);
-                var n = r(8880),
-                    o = r(9592),
+                var o = r(8880),
+                    n = r(9592),
                     a = r(3673);
                 const i = {
                     id: "q-app"
                 };
 
-                function l(e, t, r, n, o, l) {
+                function l(e, t, r, o, n, l) {
                     const s = (0, a.up)("router-view");
                     return (0, a.wg)(), (0, a.iD)("div", i, [(0, a.Wm)(s)])
                 }
                 const s = (0, a.aZ)({
                     name: "App"
                 });
                 var u = r(4260);
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(9)]).then(r.bind(r, 6009)),
+                        component: () => Promise.all([r.e(736), r.e(344)]).then(r.bind(r, 8344)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -46,138 +46,142 @@
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
                 async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
-                        n = e(d);
-                    return n.use(o.Z, t), {
-                        app: n,
+                        o = e(d);
+                    return o.use(n.Z, t), {
+                        app: o,
                         router: r
                     }
                 }
                 var b = r(6417),
-                    y = r(5597);
-                const w = {
+                    y = r(5597),
+                    w = r(589),
+                    O = r(7153);
+                const k = {
                         config: {
                             notify: {}
                         },
                         plugins: {
                             Notify: b.Z,
-                            Dialog: y.Z
+                            Dialog: y.Z,
+                            LocalStorage: w.Z,
+                            SessionStorage: O.Z
                         }
                     },
-                    O = "";
-                async function k({
+                    C = "";
+                async function P({
                     app: e,
                     router: t
                 }, r) {
-                    let n = !1;
-                    const o = e => {
+                    let o = !1;
+                    const n = e => {
                             try {
                                 return t.resolve(e).href
                             } catch (r) {}
                             return Object(e) === e ? null : e
                         },
                         a = e => {
-                            if (n = !0, "string" === typeof e && /^https?:\/\//.test(e)) return void(window.location.href = e);
-                            const t = o(e);
+                            if (o = !0, "string" === typeof e && /^https?:\/\//.test(e)) return void(window.location.href = e);
+                            const t = n(e);
                             null !== t && (window.location.href = t, window.location.reload())
                         },
                         i = window.location.href.replace(window.location.origin, "");
-                    for (let s = 0; !1 === n && s < r.length; s++) try {
+                    for (let s = 0; !1 === o && s < r.length; s++) try {
                         await r[s]({
                             app: e,
                             router: t,
                             ssrContext: null,
                             redirect: a,
                             urlPath: i,
-                            publicPath: O
+                            publicPath: C
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
-                    }!0 !== n && (e.use(t), e.mount("#q-app"))
+                    }!0 !== o && (e.use(t), e.mount("#q-app"))
                 }
-                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                g(o.ri, k).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
-                    k(e, r)
+                    P(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
-                    default: () => o
+                    default: () => n
                 });
-                var n = r(3340);
-                const o = (0, n.xr)((async ({
+                var o = r(3340);
+                const n = (0, o.xr)((async ({
                     app: e
                 }) => {}))
             }
         },
         t = {};
 
-    function r(n) {
-        var o = t[n];
-        if (void 0 !== o) return o.exports;
-        var a = t[n] = {
-            id: n,
+    function r(o) {
+        var n = t[o];
+        if (void 0 !== n) return n.exports;
+        var a = t[o] = {
+            id: o,
             loaded: !1,
             exports: {}
         };
-        return e[n].call(a.exports, a, a.exports, r), a.loaded = !0, a.exports
+        return e[o].call(a.exports, a, a.exports, r), a.loaded = !0, a.exports
     }
     r.m = e, (() => {
         var e = [];
-        r.O = (t, n, o, a) => {
-            if (!n) {
+        r.O = (t, o, n, a) => {
+            if (!o) {
                 var i = 1 / 0;
                 for (c = 0; c < e.length; c++) {
-                    for (var [n, o, a] = e[c], l = !0, s = 0; s < n.length; s++)(!1 & a || i >= a) && Object.keys(r.O).every((e => r.O[e](n[s]))) ? n.splice(s--, 1) : (l = !1, a < i && (i = a));
+                    for (var [o, n, a] = e[c], l = !0, s = 0; s < o.length; s++)(!1 & a || i >= a) && Object.keys(r.O).every((e => r.O[e](o[s]))) ? o.splice(s--, 1) : (l = !1, a < i && (i = a));
                     if (l) {
                         e.splice(c--, 1);
-                        var u = o();
+                        var u = n();
                         void 0 !== u && (t = u)
                     }
                 }
                 return t
             }
             a = a || 0;
             for (var c = e.length; c > 0 && e[c - 1][2] > a; c--) e[c] = e[c - 1];
-            e[c] = [n, o, a]
+            e[c] = [o, n, a]
         }
     })(), (() => {
         r.n = e => {
             var t = e && e.__esModule ? () => e["default"] : () => e;
             return r.d(t, {
                 a: t
             }), t
         }
     })(), (() => {
         r.d = (e, t) => {
-            for (var n in t) r.o(t, n) && !r.o(e, n) && Object.defineProperty(e, n, {
+            for (var o in t) r.o(t, o) && !r.o(e, o) && Object.defineProperty(e, o, {
                 enumerable: !0,
-                get: t[n]
+                get: t[o]
             })
         }
     })(), (() => {
-        r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
+        r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
-            9: "100130f6",
             193: "283445be",
+            344: "037a8712",
             430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
-            9: "44b298e4",
             143: "31d6cfe0",
-            736: "191faa77"
+            344: "ca964e27",
+            736: "f747ec02"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -185,31 +189,31 @@
             }
         }()
     })(), (() => {
         r.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t)
     })(), (() => {
         var e = {},
             t = "uniqua:";
-        r.l = (n, o, a, i) => {
-            if (e[n]) e[n].push(o);
+        r.l = (o, n, a, i) => {
+            if (e[o]) e[o].push(n);
             else {
                 var l, s;
                 if (void 0 !== a)
                     for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
                         var d = u[c];
-                        if (d.getAttribute("src") == n || d.getAttribute("data-webpack") == t + a) {
+                        if (d.getAttribute("src") == o || d.getAttribute("data-webpack") == t + a) {
                             l = d;
                             break
                         }
                     }
-                l || (s = !0, l = document.createElement("script"), l.charset = "utf-8", l.timeout = 120, r.nc && l.setAttribute("nonce", r.nc), l.setAttribute("data-webpack", t + a), l.src = n), e[n] = [o];
+                l || (s = !0, l = document.createElement("script"), l.charset = "utf-8", l.timeout = 120, r.nc && l.setAttribute("nonce", r.nc), l.setAttribute("data-webpack", t + a), l.src = o), e[o] = [n];
                 var p = (t, r) => {
                         l.onerror = l.onload = null, clearTimeout(f);
-                        var o = e[n];
-                        if (delete e[n], l.parentNode && l.parentNode.removeChild(l), o && o.forEach((e => e(r))), t) return t(r)
+                        var n = e[o];
+                        if (delete e[o], l.parentNode && l.parentNode.removeChild(l), n && n.forEach((e => e(r))), t) return t(r)
                     },
                     f = setTimeout(p.bind(null, void 0, {
                         type: "timeout",
                         target: l
                     }), 12e4);
                 l.onerror = p.bind(null, l.onerror), l.onload = p.bind(null, l.onload), s && document.head.appendChild(l)
             }
@@ -223,91 +227,91 @@
             })
         }
     })(), (() => {
         r.nmd = e => (e.paths = [], e.children || (e.children = []), e)
     })(), (() => {
         r.p = ""
     })(), (() => {
-        var e = (e, t, r, n) => {
-                var o = document.createElement("link");
-                o.rel = "stylesheet", o.type = "text/css";
+        var e = (e, t, r, o) => {
+                var n = document.createElement("link");
+                n.rel = "stylesheet", n.type = "text/css";
                 var a = a => {
-                    if (o.onerror = o.onload = null, "load" === a.type) r();
+                    if (n.onerror = n.onload = null, "load" === a.type) r();
                     else {
                         var i = a && ("load" === a.type ? "missing" : a.type),
                             l = a && a.target && a.target.href || t,
                             s = new Error("Loading CSS chunk " + e + " failed.\n(" + l + ")");
-                        s.code = "CSS_CHUNK_LOAD_FAILED", s.type = i, s.request = l, o.parentNode.removeChild(o), n(s)
+                        s.code = "CSS_CHUNK_LOAD_FAILED", s.type = i, s.request = l, n.parentNode.removeChild(n), o(s)
                     }
                 };
-                return o.onerror = o.onload = a, o.href = t, document.head.appendChild(o), o
+                return n.onerror = n.onload = a, n.href = t, document.head.appendChild(n), n
             },
             t = (e, t) => {
-                for (var r = document.getElementsByTagName("link"), n = 0; n < r.length; n++) {
-                    var o = r[n],
-                        a = o.getAttribute("data-href") || o.getAttribute("href");
-                    if ("stylesheet" === o.rel && (a === e || a === t)) return o
+                for (var r = document.getElementsByTagName("link"), o = 0; o < r.length; o++) {
+                    var n = r[o],
+                        a = n.getAttribute("data-href") || n.getAttribute("href");
+                    if ("stylesheet" === n.rel && (a === e || a === t)) return n
                 }
                 var i = document.getElementsByTagName("style");
-                for (n = 0; n < i.length; n++) {
-                    o = i[n], a = o.getAttribute("data-href");
-                    if (a === e || a === t) return o
+                for (o = 0; o < i.length; o++) {
+                    n = i[o], a = n.getAttribute("data-href");
+                    if (a === e || a === t) return n
                 }
             },
-            n = n => new Promise(((o, a) => {
-                var i = r.miniCssF(n),
+            o = o => new Promise(((n, a) => {
+                var i = r.miniCssF(o),
                     l = r.p + i;
-                if (t(i, l)) return o();
-                e(n, l, o, a)
+                if (t(i, l)) return n();
+                e(o, l, n, a)
             })),
-            o = {
+            n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                9: 1
+                344: 1
             };
-            o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
-                o[e] = 0
+            n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
+                n[e] = 0
             }), (t => {
-                throw delete o[e], t
+                throw delete n[e], t
             })))
         }
     })(), (() => {
         var e = {
             143: 0
         };
-        r.f.j = (t, n) => {
-            var o = r.o(e, t) ? e[t] : void 0;
-            if (0 !== o)
-                if (o) n.push(o[2]);
+        r.f.j = (t, o) => {
+            var n = r.o(e, t) ? e[t] : void 0;
+            if (0 !== n)
+                if (n) o.push(n[2]);
                 else {
-                    var a = new Promise(((r, n) => o = e[t] = [r, n]));
-                    n.push(o[2] = a);
+                    var a = new Promise(((r, o) => n = e[t] = [r, o]));
+                    o.push(n[2] = a);
                     var i = r.p + r.u(t),
                         l = new Error,
-                        s = n => {
-                            if (r.o(e, t) && (o = e[t], 0 !== o && (e[t] = void 0), o)) {
-                                var a = n && ("load" === n.type ? "missing" : n.type),
-                                    i = n && n.target && n.target.src;
-                                l.message = "Loading chunk " + t + " failed.\n(" + a + ": " + i + ")", l.name = "ChunkLoadError", l.type = a, l.request = i, o[1](l)
+                        s = o => {
+                            if (r.o(e, t) && (n = e[t], 0 !== n && (e[t] = void 0), n)) {
+                                var a = o && ("load" === o.type ? "missing" : o.type),
+                                    i = o && o.target && o.target.src;
+                                l.message = "Loading chunk " + t + " failed.\n(" + a + ": " + i + ")", l.name = "ChunkLoadError", l.type = a, l.request = i, n[1](l)
                             }
                         };
                     r.l(i, s, "chunk-" + t, t)
                 }
         }, r.O.j = t => 0 === e[t];
-        var t = (t, n) => {
-                var o, a, [i, l, s] = n,
+        var t = (t, o) => {
+                var n, a, [i, l, s] = o,
                     u = 0;
                 if (i.some((t => 0 !== e[t]))) {
-                    for (o in l) r.o(l, o) && (r.m[o] = l[o]);
+                    for (n in l) r.o(l, n) && (r.m[n] = l[n]);
                     if (s) var c = s(r)
                 }
-                for (t && t(n); u < i.length; u++) a = i[u], r.o(e, a) && e[a] && e[a][0](), e[i[u]] = 0;
+                for (t && t(o); u < i.length; u++) a = i[u], r.o(e, a) && e[a] && e[a][0](), e[i[u]] = 0;
                 return r.O(c)
             },
-            n = globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || [];
-        n.forEach(t.bind(null, 0)), n.push = t.bind(null, n.push.bind(n))
+            o = globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || [];
+        o.forEach(t.bind(null, 0)), o.push = t.bind(null, o.push.bind(o))
     })();
-    var n = r.O(void 0, [736], (() => r(653)));
-    n = r.O(n)
+    var o = r.O(void 0, [736], (() => r(653)));
+    o = r.O(o)
 })();
```

### Comparing `unigui-1.9.1/unigui/web/js/9.100130f6.js` & `unigui-1.9.2/unigui/web/js/344.037a8712.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [9], {
-        6009: (e, t, a) => {
+    [344], {
+        8344: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => la
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
@@ -79,24 +79,24 @@
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
                             }, 8, ["modelValue"]), (0, s.Wm)(g), (0, s.Wm)(f, {
                                 "no-caps": "",
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
-                                onClick: t[1] || (t[1] = t => e.Dark.set(!e.Dark.isActive))
+                                onClick: e.switchTheme
                             }, {
                                 default: (0, s.w5)((() => [(0, s.Wm)(m, {
                                     class: "text-body2"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Uk)("Dark/Light mode")])),
                                     _: 1
                                 })])),
                                 _: 1
-                            }, 8, ["icon"])])),
+                            }, 8, ["icon", "onClick"])])),
                             _: 1
                         })])),
                         _: 1
                     }, 8, ["class"]), (0, s.Wm)(v, {
                         class: "content"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Wm)(k, {
@@ -145,166 +145,164 @@
             a(71);
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
             let g = !0;
-            const m = 136,
-                f = 400,
-                y = `height: ${m}px; width: ${f}px`;
-
-            function w(e) {
-                let t = e.minheight ? e.minheight : m,
-                    a = e.minwidth ? e.minwidth : f;
-                return `height: ${t}px; width: ${a}px`
-            }
-            const b = window.location.host,
-                k = `${window.location.protocol}//${b}`;
-            console.log(k);
-            const v = !1;
-            let C = {},
-                _ = {},
-                q = {};
+            const m = ["graph", "docviewer", "linechart", "block"];
+            const f = window.location.host,
+                y = `${window.location.protocol}//${f}`,
+                w = !1;
+            let b = {},
+                k = {},
+                v = {};
 
-            function A(e) {
-                p = new WebSocket(v ? "ws://localhost:8000/ws" : `ws://${b}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+            function C(e) {
+                p = new WebSocket(w ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
                     g && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
-            function D(e) {
+            function _(e) {
                 console.log("sended", e), p.send(JSON.stringify(e))
             }
-            let S, j = 0,
-                z = !0;
+            let q, A = 0,
+                D = !0;
 
-            function Z(e) {
-                z = e, e || (q = {})
+            function S(e) {
+                D = e, e || (v = {})
             }
 
-            function $(e) {
-                if (z) {
-                    let t = e.pdata ? `${e.data.name}@${e.pdata.name}` : `_scroll@${e.data.name}`,
-                        a = q[t];
-                    if (a) return a.styleSize;
-                    z = !1
+            function j(e) {
+                if (D) {
+                    let t = v[e.fullname];
+                    if (t) return t.styleSize;
+                    D = !1
                 }
-                return w(e.data)
+                return ""
             }
 
-            function M(e, t, a, s = "complete") {
-                let l = ++j,
+            function z(e, t, a, s = "complete") {
+                let l = ++A,
                     i = [e.pdata.name, e.data.name, s, t, l];
-                D(i), u[l] = a
+                _(i), u[l] = a
             }
 
-            function V() {
-                C = {}, q = _, z = !0, _ = {}
+            function Z() {
+                b = {}, v = k, D = !0, k = {}
             }
 
-            function E(e, t) {
+            function M(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function W(e) {
+            function $(e) {
                 for (let t of e) {
                     let e = t.path;
                     if (e.length > 1) {
                         e.reverse();
                         let a = e.join("@"),
-                            s = _[a];
-                        E(s, t.data)
+                            s = k[a];
+                        M(s, t.data)
                     } else {
-                        let a = C[e[0]];
+                        let a = b[e[0]];
                         Object.assign(a.data, t.data)
                     }
                 }
             }
 
-            function K(e) {
+            function V(e) {
                 "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
-            function Q(e) {
+            function E(e) {
                 let t = [];
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function O() {
-                for (let [e, t] of Object.entries(_)) t.expanding && (t.styleSize = w(t.data));
+            function W(e = !1) {
+                for (let [t, a] of Object.entries(k)) !a.expanding || e && !m.includes(a.type) || (a.styleSize = "");
                 (0, s.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            U()
+                            Q()
                         }))
                     }))
                 }))
             }
-            let H = (0, c.debounce)(O, 200);
+            let K = (0, c.debounce)(W, 200);
 
-            function U(e) {
-                Array.isArray(e) && (e = null), S && (S.disconnect(), S = null), g && console.log("------------------recalc design");
-                const t = N(e),
-                    a = F(e);
+            function Q(e) {
+                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
+                const t = H(e),
+                    a = O(e);
                 for (let [s, l] of Object.entries(t)) {
-                    let e = _[s];
-                    const [t, i] = a[s];
-                    let n, o = e.geom().el,
-                        d = e.pdata ? e.pdata.name : e.name,
-                        r = C[d];
-                    for (let a of r.data.value.slice(1))
+                    let e = k[s],
+                        t = a[s];
+                    const [i, n] = t || [0, 1];
+                    let o, d = e.geom(),
+                        r = d.el,
+                        c = e.pdata ? e.pdata.name : e.name,
+                        h = b[c];
+                    for (let a of h.data.value.slice(1))
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
-                                    t = `${e.name}@${d}`;
-                                n = _[t];
+                                    t = `${e.name}@${c}`;
+                                o = k[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
-                        n = e;
+                        o = e;
                         break
                     }
-                    let c = r.data.width ? r.data.width - o.clientWidth - t : r.$el.getBoundingClientRect().right - (n ? n.geom().right : e.geom().right);
-                    c /= i;
-                    let h = s.startsWith("_scroll@") ? e.geom().inner.clientHeight : o.clientHeight;
-                    e.styleSize = `height: ${h+l}px; width: ${o.clientWidth+c+t}px;`
+                    let u = i;
+                    u /= n;
+                    let p = m.includes(e.type) ? `width:${Math.ceil(r.clientWidth+u)}px` : "",
+                        g = s.startsWith("_scroll@") ? d.inner.clientHeight : r.clientHeight;
+                    e.styleSize = `height: ${g+l}px; ${p}`
                 }
             }
 
-            function N(e) {
+            function H(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a += 14;
                 let s = {},
                     l = new Map,
                     i = {};
-                for (let [d, r] of Object.entries(C)) i[r.name] = r.$el.getBoundingClientRect().height;
+                for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let n = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        o = t ? Q(d) : [
+                        o = t ? E(d) : [
                             [d]
                         ];
                     for (let a of o) {
-                        let e = 0;
-                        for (let t of a) e += i[t.name] + 12;
+                        let e = 0,
+                            t = !0;
+                        for (let s of a) e += i[s.name] + 12, b[s.name].only_fixed_elems || (t = !1);
+                        if (t) {
+                            let e = b[a.slice(-1)[0].name];
+                            k[e.fullname] = e
+                        }
                         n.push([e, a])
                     }
                     n.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
                     for (let s of n) {
                         let t = s[1];
                         (0, r.hu)(Array.isArray(t));
                         const i = [];
-                        for (let [e, a] of Object.entries(_))
+                        for (let [e, a] of Object.entries(k))
                             if (a.expanding_height) {
                                 let [s, n] = e.split("@");
                                 if (t.find((e => e.name == n))) {
                                     let e = !0;
                                     const t = a.geom();
                                     for (let [s, n] of i.entries()) {
                                         let o = n.geom();
@@ -337,15 +335,15 @@
                 }
                 let o = Array.from(l.entries());
                 o.sort(((e, t) => e[0] in s || e[1] in s ? -1 : 1));
                 for (let [d, r] of o) r in s ? s[d] = s[r] : s[r] = s[d];
                 return s
             }
 
-            function F(e) {
+            function O(e) {
                 e = null;
                 const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 15,
                     s = [],
                     l = {};
                 for (let o of t)
                     if (0 == s.length)
@@ -364,21 +362,21 @@
                     s = e
                 }
                 s.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
                 let n = new Map;
                 for (let o of s) {
                     let e = Array.isArray(o) ? o[o.length - 1] : o,
-                        t = C[e.name].$el.getBoundingClientRect().right;
+                        t = b[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(o) ? o[0] : o;
-                    let s = C[e.name].$el.getBoundingClientRect().left,
+                    let s = b[e.name].$el.getBoundingClientRect().left,
                         l = a - t + s - 10;
                     const d = [];
-                    for (let [a, i] of Object.entries(_))
-                        if (i.expanding_width) {
+                    for (let [a, i] of Object.entries(k))
+                        if (i.expanding_width && (i.fullname.startsWith("_scroll@") || m.includes(i.type))) {
                             let e = a.split("@")[1];
                             if (o.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
                                 for (let [a, s] of d.entries())
                                     if (s !== i && s.geom().left == t) {
                                         s.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, n.set(s.fullname, i.fullname)) : n.set(i.fullname, s.fullname), e = !1;
@@ -392,15 +390,15 @@
                     let e = d.length,
                         t = {};
                     for (let a = 0; a < d.length; a++) {
                         let s = d[a],
                             i = s.parent_name,
                             n = i || s.name;
                         if (t[n] ? t[n]++ : t[n] = 1, n = s.parent_name, n) {
-                            let e = C[n];
+                            let e = b[n];
                             if (e.data.width) {
                                 let t = a + 1,
                                     i = d[t];
                                 if (i && i.parent_name != n) {
                                     let t = s.geom().right - s.geom().left,
                                         a = e.data.width - t;
                                     l[s.fullname] = [a, 1]
@@ -417,98 +415,99 @@
                             l[a.fullname] = [Math.floor(o / e), t[s]]
                         }
                     }
                 }
                 for (let [o, d] of n.entries()) d in l ? l[o] = l[d] : l[d] = l[o];
                 return l
             }
-            const T = (0, s.aZ)({
+            const U = (0, s.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        D(["root", this.name])
+                        _(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var P = a(4260),
-                R = a(3414),
-                I = a(2035),
-                L = a(4554),
-                B = a(2350),
-                Y = a(7518),
-                X = a.n(Y);
-            const G = (0, P.Z)(T, [
+            var N = a(4260),
+                T = a(3414),
+                F = a(2035),
+                P = a(4554),
+                I = a(2350),
+                R = a(7518),
+                L = a.n(R);
+            const B = (0, N.Z)(U, [
                     ["render", d]
                 ]),
-                J = G;
-            X()(T, "components", {
-                QItem: R.Z,
-                QItemSection: I.Z,
-                QIcon: L.Z,
-                QItemLabel: B.Z
+                Y = B;
+            L()(U, "components", {
+                QItem: T.Z,
+                QItemSection: F.Z,
+                QIcon: P.Z,
+                QItemLabel: I.Z
             });
-            const ee = {
+            const X = {
                     key: 0,
                     class: "row q-col-gutter-xs q-py-xs"
                 },
-                te = {
+                G = {
                     class: "q-col-gutter-xs"
                 },
-                ae = {
+                J = {
                     key: 0,
                     class: "column q-col-gutter-xs"
                 };
 
-            function se(e, t, a, l, i, n) {
+            function ee(e, t, a, l, i, n) {
                 const o = (0, s.up)("zone", !0),
                     d = (0, s.up)("block");
-                return e.data instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ee, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data, (e => ((0, s.wg)(), (0, s.iD)("div", te, [e instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ae, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e, (e => ((0, s.wg)(), (0, s.j4)(o, {
+                return e.data instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", X, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data, (e => ((0, s.wg)(), (0, s.iD)("div", G, [e instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", J, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e, (e => ((0, s.wg)(), (0, s.j4)(o, {
                     class: "q-col-gutter-xs q-py-xs",
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const le = {
+            const te = {
                     class: "row"
                 },
-                ie = ["data", "pdata"],
-                ne = {
+                ae = ["data", "pdata"],
+                se = {
                     key: 0,
                     class: "row"
                 },
-                oe = ["data", "pdata"],
-                de = {
+                le = ["data", "pdata"],
+                ie = {
                     key: 0,
                     class: "row"
                 };
 
-            function re(e, t, a, i, n, o) {
+            function ne(e, t, a, i, n, o) {
                 const d = (0, s.up)("element"),
                     r = (0, s.up)("q-icon"),
                     c = (0, s.up)("q-scroll-area"),
                     h = (0, s.up)("q-card");
                 return (0, s.wg)(), (0, s.j4)(h, {
-                    class: "my-card q-ma-xs"
+                    class: "my-card q-ma-xs",
+                    style: (0, l.j5)(e.only_fixed_elems ? e.styleSize : "")
                 }, {
-                    default: (0, s.w5)((() => [(0, s._)("div", le, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
+                    default: (0, s.w5)((() => [(0, s._)("div", te, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 0,
                         class: "q-ma-sm",
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, s.wg)(), (0, s.j4)(r, {
                         key: 1,
                         class: "q-mt-sm",
@@ -533,88 +532,88 @@
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data.value.slice(1), (t => ((0, s.wg)(), (0, s.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ne, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
+                        }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", se, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, ie)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, s.wg)(!0), (0, s.iD)(s.HY, {
                         key: 1
                     }, (0, s.Ko)(e.data.value.slice(1), (t => ((0, s.wg)(), (0, s.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", de, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
+                    }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ie, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, oe)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
-                })
+                }, 8, ["style"])
             }
-            var ce = a(8880);
-            const he = e => ((0, s.dD)("data-v-591efd84"), e = e(), (0, s.Cn)(), e),
-                ue = {
+            var oe = a(8880);
+            const de = e => ((0, s.dD)("data-v-5682537f"), e = e(), (0, s.Cn)(), e),
+                re = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
-                pe = ["width", "height"],
-                ge = ["src"],
-                me = {
+                ce = ["width", "height"],
+                he = ["src"],
+                ue = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                fe = {
+                pe = {
                     class: "camera-button"
                 },
-                ye = {
+                ge = {
                     key: 0
                 },
-                we = {
+                me = {
                     key: 1
                 },
-                be = {
+                fe = {
                     class: "camera-loading"
                 },
-                ke = he((() => (0, s._)("ul", {
+                ye = de((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
-                ve = [ke],
-                xe = ["height"],
-                Ce = ["height"],
-                _e = {
+                we = [ye],
+                be = ["height"],
+                ke = ["height"],
+                ve = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                qe = he((() => (0, s._)("img", {
+                xe = de((() => (0, s._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                Ae = [qe],
-                De = {
+                Ce = [xe],
+                _e = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function Se(e, t, a, i, n, o) {
+            function qe(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-img"),
                     c = (0, s.up)("q-badge"),
                     h = (0, s.up)("q-select"),
                     u = (0, s.up)("q-checkbox"),
                     p = (0, s.up)("q-toggle"),
                     g = (0, s.up)("q-btn"),
@@ -629,22 +628,22 @@
                     C = (0, s.up)("cgraph"),
                     _ = (0, s.up)("q-tooltip"),
                     q = (0, s.up)("q-spinner-puff");
                 return "image" == e.type ? ((0, s.wg)(), (0, s.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, ce.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, oe.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, l.j5)(e.elemSize)
                 }, {
                     default: (0, s.w5)((() => [e.data.header ? ((0, s.wg)(), (0, s.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, ce.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, oe.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, l.zw)(e.data.header), 1)) : (0, s.kq)("", !0), e.value ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "light-blue-2",
                         style: {
@@ -684,30 +683,33 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", ue, [e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", re, [e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 0,
                     ripple: !1,
                     color: "indigo-10",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
                 }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(m, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
+                    class: (0, l.C_)({
+                        "bg-blue-grey-9": e.Dark.isActive
+                    }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
-                }, null, 8, ["modelValue", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
+                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
                     key: 6,
                     data: e.data,
@@ -717,27 +719,27 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, ce.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
-                    onKeyup: (0, ce.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
                     key: 9,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
@@ -747,57 +749,57 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, ce.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, s.wg)(), (0, s.j4)(k, {
                     key: 10,
                     style: (0, l.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(b, {
                         nodes: e.treeNodes,
+                        "selected-color": e.Dark.isActive ? "cyan-12" : "cyan-10",
                         dense: e.data.dense,
                         selected: e.value,
                         "onUpdate:selected": t[8] || (t[8] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[9] || (t[9] = t => e.expandedKeys = t),
                         "node-key": "label",
-                        "default-expand-all": "",
-                        "selected-color": "blue-10"
-                    }, null, 8, ["nodes", "dense", "selected", "expanded"])])),
+                        "default-expand-all": ""
+                    }, null, 8, ["nodes", "selected-color", "dense", "selected", "expanded"])])),
                     _: 1
                 }, 8, ["style", "thumb-style", "bar-style"])) : "docviewer" == e.type ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("textarea", {
                     key: 11,
                     class: (0, l.C_)(["textarea", {
                         "bg-grey-10": e.Dark.isActive,
                         "text-white": e.Dark.isActive
                     }]),
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, l.j5)(e.elemSize)
                 }, null, 6)), [
-                    [ce.nr, e.value]
+                    [oe.nr, e.value]
                 ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, s._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, ge)], 8, pe)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
+                }, null, 8, he)], 8, ce)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -822,53 +824,53 @@
                     }),
                     color: e.Dark.isActive ? "purple-10" : "blue"
                 }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", me, [(0, s._)("div", fe, [(0, s._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", ue, [(0, s._)("div", pe, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", we, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", ye, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", be, ve, 512), [
-                    [ce.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", me, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", ge, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", fe, we, 512), [
+                    [oe.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
                     class: (0, l.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, s.wy)((0, s._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, xe), [
-                    [ce.F8, !e.isPhotoTaken]
+                }, null, 8, be), [
+                    [oe.F8, !e.isPhotoTaken]
                 ]), (0, s.wy)((0, s._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, Ce), [
-                    [ce.F8, e.isPhotoTaken]
+                }, null, 8, ke), [
+                    [oe.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [ce.F8, !e.isLoading]
-                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s._)("button", {
+                    [oe.F8, !e.isLoading]
+                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ve, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, Ae)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", De, [(0, s.Wm)(g, {
+                }, Ce)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
@@ -922,23 +924,23 @@
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["class", "icon", "onClick"]))
             }
-            const je = {
+            const Ae = {
                     key: 0
                 },
-                ze = {
+                De = {
                     class: "row"
                 },
-                Ze = ["onClick"];
+                Se = ["onClick"];
 
-            function $e(e, t, a, i, n, o) {
+            function je(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
                     g = (0, s.up)("q-checkbox"),
@@ -948,26 +950,26 @@
                 return (0, s.wg)(), (0, s.j4)(y, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
                     style: (0, l.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
-                    virtualScrollSliceSize: "60",
+                    virtualScrollSliceSize: "100",
                     "rows-per-page-options": [0],
                     "virtual-scroll-sticky-size-start": 48,
                     "row-key": "iiid",
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", je, [(0, s._)("div", ze, [(0, s.Wm)(c, {
+                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", Ae, [(0, s._)("div", De, [(0, s.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, s.Nv)({
                         append: (0, s.w5)((() => ["" != e.search ? ((0, s.wg)(), (0, s.j4)(d, {
@@ -1172,35 +1174,35 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, s.wg)(), (0, s.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, l.zw)(t.row[a.name]), 9, Ze))])),
+                            }, (0, l.zw)(t.row[a.name]), 9, Se))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["dense", "style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var Me = a(1959),
-                Ve = a(9058);
+            var ze = a(1959),
+                Ze = a(9058);
 
-            function Ee(e, t) {
-                return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
+            function Me(e, t) {
+                return e.length === t.length && e.every(((e, a) => t[a] && e.iiid == t[a].iiid))
             }
-            const We = (0, s.aZ)({
+            const $e = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, Me.BK)(e);
+                    } = (0, ze.BK)(e);
                     let l = (0, s.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const s = a.headers,
                                 l = s.length,
                                 i = a.rows,
                                 n = i.length;
@@ -1214,19 +1216,19 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == l.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => l.value[e])) : [l.value[e.value]];
                             return a
                         },
                         n = i(),
-                        o = (0, Me.iH)(n),
-                        d = (0, Me.iH)(n),
-                        r = (0, Me.iH)(!Array.isArray(t.value.value)),
+                        o = (0, ze.iH)(n),
+                        d = (0, ze.iH)(n),
+                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
                         c = (e, s) => {
-                            D([a.value.name, t.value.name, e, s])
+                            _([a.value.name, t.value.name, e, s])
                         },
                         h = (0, s.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, s.Fl)((() => t.value.value));
                     return (0, s.YP)(l, ((e, t) => {
                         d.value = i(), o.value = d.value
                     })), (0, s.YP)(t, ((e, a) => {
                         g && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
@@ -1238,15 +1240,15 @@
                         sendMessage: c,
                         datavalue: u,
                         updated: o
                     }
                 },
                 data() {
                     return {
-                        Dark: Ve.Z,
+                        Dark: Ze.Z,
                         search: "",
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
@@ -1316,23 +1318,23 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        M(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        z(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        M(this, [t, this.search], (function(s) {
+                        z(this, [t, this.search], (function(s) {
                             if (!Array.isArray(s)) return h.error(s);
                             g && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
@@ -1367,15 +1369,15 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Ee(this.updated, this.selected)) {
+                        if (!Me(this.updated, this.selected)) {
                             let e = this.selected.length;
                             this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
@@ -1400,52 +1402,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Ke = a(9267),
-                Qe = a(4842),
-                Oe = a(8870),
-                He = a(2165),
-                Ue = a(8186),
-                Ne = a(2414),
-                Fe = a(3884),
-                Te = a(5735),
-                Pe = a(7208);
-            const Re = (0, P.Z)(We, [
-                    ["render", $e]
+            var Ve = a(9267),
+                Ee = a(4842),
+                We = a(8870),
+                Ke = a(2165),
+                Qe = a(8186),
+                He = a(2414),
+                Oe = a(3884),
+                Ue = a(5735),
+                Ne = a(7208);
+            const Te = (0, N.Z)($e, [
+                    ["render", je]
                 ]),
-                Ie = Re;
-            X()(We, "components", {
-                QTable: Ke.Z,
-                QInput: Qe.Z,
-                QIcon: L.Z,
-                QTooltip: Oe.Z,
-                QBtn: He.Z,
-                QTr: Ue.Z,
-                QTh: Ne.Z,
-                QTd: Fe.Z,
-                QCheckbox: Te.Z,
-                QSelect: Pe.Z
+                Fe = Te;
+            L()($e, "components", {
+                QTable: Ve.Z,
+                QInput: Ee.Z,
+                QIcon: P.Z,
+                QTooltip: We.Z,
+                QBtn: Ke.Z,
+                QTr: Qe.Z,
+                QTh: He.Z,
+                QTd: Oe.Z,
+                QCheckbox: Ue.Z,
+                QSelect: Ne.Z
             });
-            const Le = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Be(e, t, a, i, n, o) {
+            function Ie(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Le)
+                }, null, 12, Pe)
             }
-            var Ye = a(2393),
-                Xe = a.n(Ye);
-            const Ge = Xe().stylesheet().selector("node").css({
+            var Re = a(2393),
+                Le = a.n(Re);
+            const Be = Le().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1471,50 +1473,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Je = {
+                Ye = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function et(e, t) {
+            function Xe(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const tt = (0, s.aZ)({
+            const Ge = (0, s.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Ge,
-                            layoutOptions: Je,
+                            style: Be,
+                            layoutOptions: Ye,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Xe()({
+                        let e = Le()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1564,15 +1566,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            D([this.pdata["name"], this.data["name"], e, t])
+                            _([this.pdata["name"], this.data["name"], e, t])
                         },
                         handleKeyDown(e) {
                             "Shift" == e.key && (this.shiftKey = !0)
                         },
                         handleKeyUp(e) {
                             "Shift" == e.key && (this.shiftKey = !1)
                         },
@@ -1636,15 +1638,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     s = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), et(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), et(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Xe(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Xe(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1661,53 +1663,53 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                at = (0, P.Z)(tt, [
-                    ["render", Be]
+                Je = (0, N.Z)(Ge, [
+                    ["render", Ie]
                 ]),
-                st = at;
+                et = Je;
 
-            function lt(e, t, a, i, n, o) {
+            function tt(e, t, a, i, n, o) {
                 const d = (0, s.up)("v-chart");
                 return (0, s.wg)(), (0, s.j4)(d, {
                     ref: "chart",
                     option: n.options,
-                    style: (0, l.j5)(a.styleSize),
+                    style: (0, l.j5)(a.styleSize ? a.styleSize : "width: 300px; height: 200px"),
                     autoresize: !0
                 }, null, 8, ["option", "style"])
             }
-            var it = a(7559),
-                nt = a(4447),
-                ot = a(1006),
-                dt = a(3526),
-                rt = a(763),
-                ct = a(546),
-                ht = a(6902),
-                ut = a(2826),
-                pt = a(5256),
-                gt = a(3825),
-                mt = a(8825);
-            (0, rt.D)([nt.N, ot.N, dt.N]), (0, rt.D)([ct.N, ht.N, ut.N, pt.N, gt.N]);
-            let ft = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const yt = {
+            var at = a(7559),
+                st = a(4447),
+                lt = a(1006),
+                it = a(3526),
+                nt = a(763),
+                ot = a(546),
+                dt = a(6902),
+                rt = a(2826),
+                ct = a(5256),
+                ht = a(3825),
+                ut = a(8825);
+            (0, nt.D)([st.N, lt.N, it.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
+            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const gt = {
                     name: "linechart",
                     components: {
-                        VChart: it.ZP
+                        VChart: at.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, mt.Z)();
+                        const e = (0, ut.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: {
                                 responsive: !0,
                                 maintainAspectRatio: !1,
                                 legend: {
@@ -1751,14 +1753,15 @@
                                     start: 0,
                                     end: 10
                                 }],
                                 series: []
                             }
                         }
                     },
+                    computed: {},
                     methods: {
                         clicked(e) {
                             alert("!");
                             var t = [e.offsetX, e.offsetY],
                                 a = myChart.convertFromPixel("grid", t),
                                 s = myChart.getModel().get("xAxis")[0].data[a[0]];
                             console.log(s)
@@ -1782,58 +1785,59 @@
                             let l = [];
                             for (let n = 0; n < s.length; n++) s[n] = "i" == s[n] ? -1 : parseInt(s[n]), l.push([]), n && (this.options.series.push({
                                 name: t[s[n]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ft[n]
+                                    color: pt[n]
                                 },
                                 data: l[n]
                             }), this.options.legend.data.push(t[s[n]]));
                             this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? n : i[n][s[e]]);
                             this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
-                wt = (0, P.Z)(yt, [
-                    ["render", lt]
+                mt = (0, N.Z)(gt, [
+                    ["render", tt],
+                    ["__scopeId", "data-v-12be25e8"]
                 ]),
-                bt = wt;
+                ft = mt;
 
-            function kt(e) {
+            function yt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
-                a.open("POST", k, !0), a.onload = function() {
+                a.open("POST", y, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const vt = (0, s.aZ)({
+            const wt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Ie,
-                    cgraph: st,
-                    linechart: bt
+                    utable: Fe,
+                    cgraph: et,
+                    linechart: ft
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        D([this.pdata["name"], this.data["name"], e, t])
+                        _([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
                         t && this.sendMessage("changed", e.xhr.responseText)
@@ -1844,15 +1848,15 @@
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         this.value = e
                     },
                     complete(e, t, a) {
-                        "" != e && M(this, e, (e => t((() => {
+                        "" != e && z(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1885,15 +1889,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(kt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
                     },
                     rect() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         return e.getBoundingClientRect()
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
@@ -1909,25 +1913,25 @@
                             top: s.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 updated() {
-                    _[this.fullname] = this
+                    k[this.fullname] = this
                 },
                 mounted() {
-                    _[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
+                    k[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
                 },
                 data() {
                     return {
-                        Dark: Ve.Z,
+                        Dark: Ze.Z,
                         value: this.data.value,
-                        styleSize: $(this),
-                        host_path: k,
+                        styleSize: h.visibility ? j(this) : "",
+                        host_path: y,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -2036,58 +2040,63 @@
                         Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        this.styleSize || (this.styleSize = finitStyle(this.data)), this.value = this.data.value, this.updated = this.value, _[this.fullname] = this
+                        this.styleSize || (this.styleSize = ""), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var xt = a(4027),
-                Ct = a(9721),
-                _t = a(8886),
-                qt = a(8761),
-                At = a(1232),
-                Dt = a(5551),
-                St = a(5869),
-                jt = a(1745),
-                zt = a(8430);
-            const Zt = (0, P.Z)(vt, [
-                    ["render", Se],
-                    ["__scopeId", "data-v-591efd84"]
+            var bt = a(4027),
+                kt = a(9721),
+                vt = a(8886),
+                xt = a(8761),
+                Ct = a(1232),
+                _t = a(5551),
+                qt = a(5869),
+                At = a(1745),
+                Dt = a(8430);
+            const St = (0, N.Z)(wt, [
+                    ["render", qe],
+                    ["__scopeId", "data-v-5682537f"]
                 ]),
-                $t = Zt;
-            X()(vt, "components", {
-                QImg: xt.Z,
-                QIcon: L.Z,
-                QSelect: Pe.Z,
-                QBadge: Ct.Z,
-                QCheckbox: Te.Z,
-                QToggle: _t.Z,
-                QBtn: He.Z,
-                QBtnToggle: qt.Z,
-                QInput: Qe.Z,
-                QScrollArea: At.Z,
-                QTree: Dt.Z,
-                QSeparator: St.Z,
-                QUploader: jt.Z,
-                QTooltip: Oe.Z,
-                QSpinnerPuff: zt.Z
+                jt = St;
+
+            function zt(e) {
+                let t = e.type;
+                return "tree" == t || "table" == t || "list" == t || "docviewer" == t || "graph" == t || "linechart" == t
+            }
+            L()(wt, "components", {
+                QImg: bt.Z,
+                QIcon: P.Z,
+                QSelect: Ne.Z,
+                QBadge: kt.Z,
+                QCheckbox: Ue.Z,
+                QToggle: vt.Z,
+                QBtn: Ke.Z,
+                QBtnToggle: xt.Z,
+                QInput: Ee.Z,
+                QScrollArea: Ct.Z,
+                QTree: _t.Z,
+                QSeparator: qt.Z,
+                QUploader: At.Z,
+                QTooltip: We.Z,
+                QSpinnerPuff: Dt.Z
             });
-            const Mt = (0, s.aZ)({
+            const Zt = (0, s.aZ)({
                 name: "block",
                 components: {
-                    element: $t
+                    element: jt
                 },
                 data() {
                     return {
-                        Dark: Ve.Z,
-                        styleSize: y,
+                        Dark: Ze.Z,
+                        styleSize: "",
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
                         },
@@ -2098,171 +2107,184 @@
                             width: "8px",
                             opacity: .2
                         }
                     }
                 },
                 methods: {
                     log() {
-                        console.log(Object.keys(C).length, this.name, this.$el.getBoundingClientRect())
+                        console.log(Object.keys(b).length, this.name, this.$el.getBoundingClientRect())
                     },
                     geom() {
-                        let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
-                        const t = e.querySelector(".q-scrollarea"),
-                            a = e.getBoundingClientRect();
+                        let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling,
+                            t = e.querySelector(".q-scrollarea");
+                        t || (t = e);
+                        const a = e.getBoundingClientRect();
                         return {
                             el: e,
                             inner: t,
                             left: a.left,
                             right: a.right,
                             top: a.top,
                             scrollHeight: window.innerHeight,
                             scrollWidth: window.innerWidth
                         }
                     }
                 },
                 mounted() {
-                    C[this.name] = this, this.expanding && (_[this.fullname] = this)
+                    b[this.name] = this, this.expanding && (k[this.fullname] = this)
                 },
                 computed: {
                     name() {
                         return this.data.name
                     },
                     fullname() {
-                        return `_scroll@${this.name}`
+                        return `${this.data.scroll?"_scroll":"_space"}@${this.name}`
                     },
                     icon() {
                         return this.data.icon
                     },
+                    type() {
+                        return this.data.type
+                    },
                     expanding() {
                         return this.data.scroll
                     },
                     expanding_width() {
                         return this.expanding
                     },
+                    only_fixed_elems() {
+                        if (this.data.scroll) return !1;
+                        for (let e of this.data.value)
+                            if (Array.isArray(e)) {
+                                for (let t of e)
+                                    if (zt(t)) return !1
+                            } else if (zt(e)) return !1;
+                        return !0
+                    },
                     expanding_height() {
-                        return !this.data.height && this.expanding
+                        return !this.data.height && (this.expanding || this.only_fixed_elems)
                     },
                     tops() {
                         let e = this.data.value;
                         return e.length ? Array.isArray(e[0]) ? e[0] : [e[0]] : []
                     }
                 },
                 props: {
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), C[this.name] = this, this.expanding && (this.styleSize = $(this), _[this.fullname] = this)
+                        g && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? j(this) : "", k[this.fullname] = this)
                     }
                 }
             });
-            var Vt = a(151);
-            const Et = (0, P.Z)(Mt, [
-                    ["render", re]
+            var Mt = a(151);
+            const $t = (0, N.Z)(Zt, [
+                    ["render", ne]
                 ]),
-                Wt = Et;
+                Vt = $t;
 
-            function Kt() {
-                let e = z && _.size == q.size;
+            function Et() {
+                let e = D && k.size == v.size;
                 if (e)
-                    for (let [t, a] of Object.entries(_))
-                        if (!q[t]) {
+                    for (let [t, a] of Object.entries(k))
+                        if (!v[t]) {
                             e = !1;
                             break
-                        } e || (U(), (0, s.Y3)((() => {
+                        } e || (Q(), (0, s.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             h.visible(!0)
                         }))
                     }))
                 })))
             }
-            X()(Mt, "components", {
-                QCard: Vt.Z,
-                QIcon: L.Z,
-                QScrollArea: At.Z
+            L()(Zt, "components", {
+                QCard: Mt.Z,
+                QIcon: P.Z,
+                QScrollArea: Ct.Z
             });
-            const Qt = (0, s.aZ)({
+            const Wt = (0, s.aZ)({
                     name: "zone",
                     components: {
-                        block: Wt
+                        block: Vt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, s.Y3)((() => {
                             requestAnimationFrame((() => {
-                                requestAnimationFrame(Kt)
+                                requestAnimationFrame(Et)
                             }))
                         }))
                     }
                 }),
-                Ot = (0, P.Z)(Qt, [
-                    ["render", se]
+                Kt = (0, N.Z)(Wt, [
+                    ["render", ee]
                 ]),
-                Ht = Ot,
-                Ut = {
+                Qt = Kt,
+                Ht = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Nt(e, t, a, i, n, o) {
+            function Ot(e, t, a, i, n, o) {
                 const d = (0, s.up)("block"),
                     r = (0, s.up)("q-item-label"),
                     c = (0, s.up)("q-space"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-card"),
                     p = (0, s.up)("q-dialog");
                 return (0, s.wg)(), (0, s.j4)(p, {
                     ref: "dialog",
                     onHide: o.onDialogHide,
-                    onKeyup: (0, ce.D2)(o.pressedEnter, ["enter"])
+                    onKeyup: (0, oe.D2)(o.pressedEnter, ["enter"])
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(u, {
                         class: "q-dialog-plugin q-pa-md items-start q-gutter-md",
                         bordered: "",
                         style: (0, l.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
                     }, {
                         default: (0, s.w5)((() => [a.data ? ((0, s.wg)(), (0, s.j4)(d, {
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, s.kq)("", !0), (0, s.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, s._)("div", Ut, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
+                        }), (0, s._)("div", Ht, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide", "onKeyup"])
             }
-            const Ft = {
+            const Ut = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Wt
+                    block: Vt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || D([this.data["name"], e]), this.hide()
+                        this.data.internal || _([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -2273,78 +2295,86 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Tt = a(5926),
-                Pt = a(2025);
-            const Rt = (0, P.Z)(Ft, [
-                    ["render", Nt]
+            var Nt = a(5926),
+                Tt = a(2025);
+            const Ft = (0, N.Z)(Ut, [
+                    ["render", Ot]
                 ]),
-                It = Rt;
-            X()(Ft, "components", {
-                QDialog: Tt.Z,
-                QCard: Vt.Z,
-                QItemLabel: B.Z,
-                QSpace: Pt.Z,
-                QBtn: He.Z
+                Pt = Ft;
+            L()(Ut, "components", {
+                QDialog: Nt.Z,
+                QCard: Mt.Z,
+                QItemLabel: I.Z,
+                QSpace: Tt.Z,
+                QBtn: Ke.Z
             });
+            var It = a(589);
+            let Rt = "theme";
+            try {
+                Ze.Z.set(It.Z.getItem(Rt))
+            } catch (ia) {}
             let Lt = null;
             const Bt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
-                        Dark: Ve.Z,
+                        Dark: Ze.Z,
                         menu: [],
                         tab: "",
                         tooldata: {
                             name: "toolbar"
                         },
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         },
                         visibility: !1
                     }
                 },
                 components: {
-                    menubar: J,
-                    zone: Ht,
-                    element: $t
+                    menubar: Y,
+                    zone: Qt,
+                    element: jt
                 },
                 created() {
-                    A(this)
+                    C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
+                    switchTheme() {
+                        Ze.Z.set(!Ze.Z.isActive), It.Z.set(Rt, Ze.Z.isActive)
+                    },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        D(["root", e])
+                        _(["root", e])
                     },
                     visible(e) {
                         this.$refs.page.$el.style.visibility = e ? "" : "hidden", this.visibility = e
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), H()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), K()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: It
+                                component: Pt
                             },
                             {
                                 height: a,
                                 ...s
                             } = e;
                         s.width = 750;
                         let l = {
@@ -2382,63 +2412,70 @@
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) V(), this.screen.name != e.name && (Z(!1), this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) Z(), this.screen.name != e.name && (S(!1), this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = It, t.componentProps = {
+                            t.component = Pt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if ("answer" == e.type) K(e);
+                        } else if ("answer" == e.type) V(e);
                         else {
-                            e.updates && W(e.updates);
-                            let t = !1;
-                            ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.updates || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
+                            let t = e.updates && e.updates.length;
+                            t && $(e.updates);
+                            let a = !1;
+                            ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), a = !0), a || t || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
                         Lt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
-                    window.addEventListener("resize", this.onResize)
+                    window.addEventListener("resize", this.onResize);
+                    const e = new ResizeObserver((e => {
+                        let t = document.documentElement.scrollHeight > window.innerHeight;
+                        t && W(!0)
+                    }));
+                    let t = this.$refs.page.$el;
+                    e.observe(t)
                 }
             });
             var Yt = a(9214),
                 Xt = a(3812),
                 Gt = a(9570),
                 Jt = a(7547),
                 ea = a(3269),
                 ta = a(2652),
                 aa = a(4379);
-            const sa = (0, P.Z)(Bt, [
+            const sa = (0, N.Z)(Bt, [
                     ["render", o]
                 ]),
                 la = sa;
-            X()(Bt, "components", {
+            L()(Bt, "components", {
                 QLayout: Yt.Z,
                 QHeader: Xt.Z,
                 QToolbar: Gt.Z,
-                QBtn: He.Z,
-                QItemLabel: B.Z,
+                QBtn: Ke.Z,
+                QItemLabel: I.Z,
                 QTabs: Jt.Z,
                 QTab: ea.Z,
-                QSpace: Pt.Z,
-                QTooltip: Oe.Z,
+                QSpace: Tt.Z,
+                QTooltip: We.Z,
                 QPageContainer: ta.Z,
                 QPage: aa.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.9.1/unigui/web/js/193.283445be.js` & `unigui-1.9.2/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui/web/index.html` & `unigui-1.9.2/unigui/web/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.18cce91f.js></script><script defer src=js/app.c7c500ce.js></script><link href=css/vendor.191faa77.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.1711f3eb.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.1/LICENSE` & `unigui-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/setup.py` & `unigui-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.1',      
+      version='1.9.2',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.1/PKG-INFO` & `unigui-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.1
+Version: 1.9.2
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.1/README.md` & `unigui-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.9.1/unigui.egg-info/PKG-INFO` & `unigui-1.9.2/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.1
+Version: 1.9.2
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

