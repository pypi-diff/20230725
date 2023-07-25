# Comparing `tmp/foundation-model-package-0.0.8.tar.gz` & `tmp/foundation-model-package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-package-0.0.8.tar", last modified: Tue Jul 25 19:41:55 2023, max compression
+gzip compressed data, was "foundation-model-package-0.0.9.tar", last modified: Tue Jul 25 20:02:21 2023, max compression
```

## Comparing `foundation-model-package-0.0.8.tar` & `foundation-model-package-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      446 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-package-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.383670 foundation-model-package-0.0.8/foundation_model_package.egg-info/
--rw-rw-rw-   0        0        0      446 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.462906 foundation-model-package-0.0.8/foundation_model_pkg/
--rw-rw-rw-   0        0        0       46 2023-07-07 21:33:54.000000 foundation-model-package-0.0.8/foundation_model_pkg/__init__.py
--rw-rw-rw-   0        0        0    16381 2023-07-25 19:40:29.000000 foundation-model-package-0.0.8/foundation_model_pkg/foundation_model.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.541298 foundation-model-package-0.0.8/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0     5676 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.556931 foundation-model-package-0.0.8/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      762 2023-07-25 16:57:42.000000 foundation-model-package-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml
--rw-rw-rw-   0        0        0       42 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      577 2023-07-25 19:41:30.000000 foundation-model-package-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:21.116131 foundation-model-package-0.0.9/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      446 2023-07-25 20:02:21.100503 foundation-model-package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-package-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:20.833774 foundation-model-package-0.0.9/foundation_model_package.egg-info/
+-rw-rw-rw-   0        0        0      446 2023-07-25 20:02:20.000000 foundation-model-package-0.0.9/foundation_model_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-25 20:02:20.000000 foundation-model-package-0.0.9/foundation_model_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 20:02:20.000000 foundation-model-package-0.0.9/foundation_model_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-25 20:02:20.000000 foundation-model-package-0.0.9/foundation_model_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:20.880766 foundation-model-package-0.0.9/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       46 2023-07-07 21:33:54.000000 foundation-model-package-0.0.9/foundation_model_pkg/__init__.py
+-rw-rw-rw-   0        0        0    16381 2023-07-25 19:40:29.000000 foundation-model-package-0.0.9/foundation_model_pkg/foundation_model.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:20.990496 foundation-model-package-0.0.9/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0     5676 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:21.052999 foundation-model-package-0.0.9/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      591 2023-07-25 20:01:24.000000 foundation-model-package-0.0.9/foundation_model_pkg/yamls/foundation_model.yaml
+-rw-rw-rw-   0        0        0       42 2023-07-25 20:02:21.116131 foundation-model-package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      577 2023-07-25 20:02:12.000000 foundation-model-package-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:02:21.100503 foundation-model-package-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-package-0.0.9/tests/test_my_tool_1.py
```

### Comparing `foundation-model-package-0.0.8/foundation_model_pkg/foundation_model.py` & `foundation-model-package-0.0.9/foundation_model_pkg/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.8/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-package-0.0.9/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.8/foundation_model_pkg/tools/utils.py` & `foundation-model-package-0.0.9/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-package-0.0.9/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-foundation_model_pkg.tools.foundation_model.foundation_model:
-  function: foundation_model
+foundation_model_pkg.tools.FoundationModel.foundation_model:
   inputs:
     prompt:
       type:
         - PromptTemplate
     connection:
       type:
         - CustomConnection
     api:
       enum:
         - chat
         - completion
       type:
         - string
-    model_family:
-      enum:
-        - LLaMa
-        - Dolly
-        - GPT-2
-        - Falcon
-      type:
-        - string
-    chat_history:
-      default: "[]"
-      type:
-        - list
     model_kwargs:
       default: "{}"
       type:
         - object
-  is_builtin: true
-  module: foundation_model_pkg.tools.foundation_model
   name: Foundation Model
+  module: foundation_model_pkg.tools.foundation_model
+  class_name: FoundationModel
+  function: foundation_model
   description: Tool to use Azure Foundation Models
   stage: test
   type: python
+  is_builtin: true
```

### Comparing `foundation-model-package-0.0.8/setup.py` & `foundation-model-package-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-package",
-    version="0.0.8",
+    version="0.0.9",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `foundation-model-package-0.0.8/tests/test_my_tool_1.py` & `foundation-model-package-0.0.9/tests/test_my_tool_1.py`

 * *Files identical despite different names*

