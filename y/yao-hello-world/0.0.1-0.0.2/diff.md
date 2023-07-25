# Comparing `tmp/yao_hello_world-0.0.1.tar.gz` & `tmp/yao_hello_world-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao_hello_world-0.0.1.tar", last modified: Mon Jul 24 15:00:34 2023, max compression
+gzip compressed data, was "yao_hello_world-0.0.2.tar", last modified: Tue Jul 25 07:10:59 2023, max compression
```

## Comparing `yao_hello_world-0.0.1.tar` & `yao_hello_world-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.419034 yao_hello_world-0.0.1/
--rw-rw-rw-   0        0        0       36 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0       97 2023-07-24 15:00:34.419034 yao_hello_world-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-24 15:00:34.420044 yao_hello_world-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      436 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.365709 yao_hello_world-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      735 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/tests/test_hello_world_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.367713 yao_hello_world-0.0.1/yao_hello_world/
--rw-rw-rw-   0        0        0       82 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/yao_hello_world/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.409253 yao_hello_world-0.0.1/yao_hello_world/tools/
--rw-rw-rw-   0        0        0       82 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/yao_hello_world/tools/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/yao_hello_world/tools/hello_world_tool.py
--rw-rw-rw-   0        0        0      522 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/yao_hello_world/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.417248 yao_hello_world-0.0.1/yao_hello_world/yamls/
--rw-rw-rw-   0        0        0      332 2023-07-24 14:59:36.000000 yao_hello_world-0.0.1/yao_hello_world/yamls/hello_world_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-07-24 15:00:34.404245 yao_hello_world-0.0.1/yao_hello_world.egg-info/
--rw-rw-rw-   0        0        0       97 2023-07-24 15:00:34.000000 yao_hello_world-0.0.1/yao_hello_world.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-24 15:00:34.000000 yao_hello_world-0.0.1/yao_hello_world.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:00:34.000000 yao_hello_world-0.0.1/yao_hello_world.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-24 15:00:34.000000 yao_hello_world-0.0.1/yao_hello_world.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 15:00:34.000000 yao_hello_world-0.0.1/yao_hello_world.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.054965 yao_hello_world-0.0.2/
+-rw-rw-rw-   0        0        0       32 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       97 2023-07-25 07:10:59.053967 yao_hello_world-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.020957 yao_hello_world-0.0.2/hello_world/
+-rw-rw-rw-   0        0        0       82 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/hello_world/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.028961 yao_hello_world-0.0.2/hello_world/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/hello_world/tools/__init__.py
+-rw-rw-rw-   0        0        0      487 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/hello_world/tools/hello_world_tool.py
+-rw-rw-rw-   0        0        0      490 2023-07-25 07:07:39.000000 yao_hello_world-0.0.2/hello_world/tools/hello_world_tool_2.py
+-rw-rw-rw-   0        0        0      522 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/hello_world/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.032955 yao_hello_world-0.0.2/hello_world/yamls/
+-rw-rw-rw-   0        0        0      352 2023-07-25 07:02:46.000000 yao_hello_world-0.0.2/hello_world/yamls/hello_world_tool.yaml
+-rw-rw-rw-   0        0        0      354 2023-07-25 07:08:38.000000 yao_hello_world-0.0.2/hello_world/yamls/hello_world_tool2.yaml
+-rw-rw-rw-   0        0        0       42 2023-07-25 07:10:59.054965 yao_hello_world-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      432 2023-07-25 07:10:42.000000 yao_hello_world-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.036955 yao_hello_world-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-07-25 07:02:06.000000 yao_hello_world-0.0.2/tests/test_hello_world_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:10:59.052967 yao_hello_world-0.0.2/yao_hello_world.egg-info/
+-rw-rw-rw-   0        0        0       97 2023-07-25 07:10:58.000000 yao_hello_world-0.0.2/yao_hello_world.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-07-25 07:10:58.000000 yao_hello_world-0.0.2/yao_hello_world.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:10:58.000000 yao_hello_world-0.0.2/yao_hello_world.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-25 07:10:58.000000 yao_hello_world-0.0.2/yao_hello_world.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-07-25 07:10:58.000000 yao_hello_world-0.0.2/yao_hello_world.egg-info/top_level.txt
```

### Comparing `yao_hello_world-0.0.1/tests/test_hello_world_tool.py` & `yao_hello_world-0.0.2/tests/test_hello_world_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import unittest
 
 from promptflow.connections import CustomConnection
-from yao_hello_world.tools.hello_world_tool import hello_world_tool
+from hello_world.tools.hello_world_tool import get_greeting_message
 
 
 @pytest.fixture
 def my_custom_connection() -> CustomConnection:
     my_custom_connection = CustomConnection(
         {
             "api-key" : "my-api-key",
@@ -14,15 +14,15 @@
             "api-url" : "my-api-url"
         }
     )
     return my_custom_connection
 
 
 class TestTool:
-    def test_hello_world_tool(self, my_custom_connection):
-        result = hello_world_tool(my_custom_connection, input_text="Microsoft")
+    def test_get_greeting_message(self, my_custom_connection):
+        result = get_greeting_message(my_custom_connection, input_text="Microsoft")
         assert result == "Hello Microsoft"
 
 
 # Run the unit tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `yao_hello_world-0.0.1/yao_hello_world/tools/utils.py` & `yao_hello_world-0.0.2/hello_world/tools/utils.py`

 * *Files identical despite different names*

