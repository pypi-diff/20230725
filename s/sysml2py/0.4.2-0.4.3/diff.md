# Comparing `tmp/sysml2py-0.4.2.tar.gz` & `tmp/sysml2py-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.4.2.tar", max compression
+gzip compressed data, was "sysml2py-0.4.3.tar", max compression
```

## Comparing `sysml2py-0.4.2.tar` & `sysml2py-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-07-24 16:53:35.802486 sysml2py-0.4.2/LICENSE
--rw-r--r--   0        0        0     3757 2023-07-24 16:53:35.806486 sysml2py-0.4.2/README.md
--rw-r--r--   0        0        0     1576 2023-07-24 16:53:36.630487 sysml2py-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3297 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/__init__.py
--rw-r--r--   0        0        0     8299 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/definition.py
--rw-r--r--   0        0        0     2297 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/formatting.py
--rw-r--r--   0        0        0    22296 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0        0        0    10762 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0        0        0    48820 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0        0        0   105604 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/grammar/classes.py
--rw-r--r--   0        0        0    28524 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/KerML.xtext
--rw-r--r--   0        0        0    14284 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/KerMLExpressions.xtext
--rw-r--r--   0        0        0    60663 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/SysML.xtext
--rw-r--r--   0        0        0     6279 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0        0        0    22976 2023-07-24 16:53:35.806486 sysml2py-0.4.2/src/sysml2py/usage.py
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 02:52:20.556001 sysml2py-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-25 02:52:20.556001 sysml2py-0.4.3/README.md
+-rw-r--r--   0        0        0     1576 2023-07-25 02:52:21.436050 sysml2py-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3297 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/__init__.py
+-rw-r--r--   0        0        0     8299 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/definition.py
+-rw-r--r--   0        0        0     2297 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/formatting.py
+-rw-r--r--   0        0        0    22296 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0        0        0    10762 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0        0        0    48820 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0        0        0   105339 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/grammar/classes.py
+-rw-r--r--   0        0        0    28524 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/KerML.xtext
+-rw-r--r--   0        0        0    14284 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/KerMLExpressions.xtext
+-rw-r--r--   0        0        0    60663 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/SysML.xtext
+-rw-r--r--   0        0        0     6279 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0        0        0    23886 2023-07-25 02:52:20.556001 sysml2py-0.4.3/src/sysml2py/usage.py
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.4.3/PKG-INFO
```

### Comparing `sysml2py-0.4.2/LICENSE` & `sysml2py-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/README.md` & `sysml2py-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/pyproject.toml` & `sysml2py-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #requires = ["setuptools>=61.0"]
 #build-backend = "setuptools.build_meta"
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "sysml2py"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -47,15 +47,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
 
 [tool.poetry]
 name = "sysml2py"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Christopher Cox <chris.cox@westfall.io>"]
 readme = "README.md"
 packages = [{ include = "sysml2py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sysml2py-0.4.2/src/sysml2py/__init__.py` & `sysml2py-0.4.3/src/sysml2py/__init__.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/definition.py` & `sysml2py-0.4.3/src/sysml2py/definition.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/formatting.py` & `sysml2py-0.4.3/src/sysml2py/formatting.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.4.3/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.4.3/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.4.3/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/grammar/classes.py` & `sysml2py-0.4.3/src/sysml2py/grammar/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,44 +100,47 @@
 class DefinitionElement:
     def __init__(self, definition):
         self.children = []
         if valid_definition(definition, "DefinitionElement"):
             # This is a SysML Element
             if isinstance(definition["ownedRelatedElement"], str):
                 raise NotImplementedError
-            if definition["ownedRelatedElement"]["name"] == "Package":
+
+            de = definition["ownedRelatedElement"]["name"]
+            if de == "Package":
                 self.children.append(Package(definition["ownedRelatedElement"]))
-            elif definition["ownedRelatedElement"]["name"] == "PartDefinition":
+            elif de == "PartDefinition":
                 self.children.append(PartDefinition(definition["ownedRelatedElement"]))
-            elif definition["ownedRelatedElement"]["name"] == "AttributeDefinition":
+            elif de == "AttributeDefinition":
                 self.children.append(
                     AttributeDefinition(definition["ownedRelatedElement"])
                 )
-            elif definition["ownedRelatedElement"]["name"] == "AnnotatingElement":
+            elif de == "AnnotatingElement":
                 self.children.append(
                     AnnotatingElement(definition["ownedRelatedElement"])
                 )
 
-            elif definition["ownedRelatedElement"]["name"] == "EnumerationDefinition":
+            elif de == "EnumerationDefinition":
                 self.children.append(
                     EnumerationDefinition(definition["ownedRelatedElement"])
                 )
-            elif definition["ownedRelatedElement"]["name"] == "ItemDefinition":
+            elif de == "ItemDefinition":
                 self.children.append(ItemDefinition(definition["ownedRelatedElement"]))
-            elif definition["ownedRelatedElement"]["name"] == "ConnectionDefinition":
+            elif de == "ConnectionDefinition":
                 self.children.append(
                     ConnectionDefinition(definition["ownedRelatedElement"])
                 )
-            elif definition["ownedRelatedElement"]["name"] == "PortDefinition":
+            elif de == "PortDefinition":
                 self.children.append(PortDefinition(definition["ownedRelatedElement"]))
-            elif definition["ownedRelatedElement"]["name"] == "InterfaceDefinition":
+            elif de == "InterfaceDefinition":
                 self.children.append(
                     InterfaceDefinition(definition["ownedRelatedElement"])
                 )
             else:
+                print(de)
                 raise NotImplementedError
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
```

### Comparing `sysml2py-0.4.2/src/sysml2py/textx/KerML.xtext` & `sysml2py-0.4.3/src/sysml2py/textx/KerML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/textx/KerMLExpressions.xtext` & `sysml2py-0.4.3/src/sysml2py/textx/KerMLExpressions.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/textx/SysML.xtext` & `sysml2py-0.4.3/src/sysml2py/textx/SysML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.4.3/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.4.2/src/sysml2py/usage.py` & `sysml2py-0.4.3/src/sysml2py/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         return self
 
     def _ensure_body(self, subgrammar="usage"):
         # Add children
         body = []
         for abc in self.children:
             body.append(
-                DefinitionBodyItem(abc.dump(child="DefinitionBody")).get_definition()
+                DefinitionBodyItem(
+                    abc._get_definition(child="DefinitionBody")
+                ).get_definition()
             )
 
         if len(body) > 0:
             getattr(self.grammar, subgrammar).completion.body.body = DefinitionBody(
                 {"name": "DefinitionBody", "ownedRelatedElement": body}
             )
         return self
@@ -144,16 +146,16 @@
             else:
                 package["ownedRelationship"].insert(
                     0, self.typedby._get_definition(child=child)["ownedRelationship"][0]
                 )
 
         return package
 
-    def dump(self, child=None):
-        return classtree(self._get_definition(child)).dump()
+    def dump(self):
+        return classtree(self._get_definition()).dump()
 
     def _set_name(self, name, short=False):
         if hasattr(self.grammar, "usage"):
             path = self.grammar.usage.declaration.declaration
         elif hasattr(self.grammar, "definition"):
             path = self.grammar.definition.declaration
         else:
@@ -679,14 +681,39 @@
                 "name": "PackageMember",
                 "ownedRelatedElement": package,
                 "prefix": None,
             }
 
         return package
 
+    def _get_definition(self, child=None):
+        package = self.usage_dump(child)
+
+        if child is None:
+            package = {
+                "name": "PackageBodyElement",
+                "ownedRelationship": [package],
+                "prefix": None,
+            }
+
+        # Add the typed by definition to the package output
+        if self.typedby is not None:
+            if child is None:
+                package["ownedRelationship"].insert(
+                    0, self.typedby._get_definition(child="PackageBody")
+                )
+            elif child == "PackageBody":
+                package = [self.typedby._get_definition(child="PackageBody"), package]
+            else:
+                package["ownedRelationship"].insert(
+                    0, self.typedby._get_definition(child=child)["ownedRelationship"][0]
+                )
+
+        return package
+
     def dump(self, child=None):
         package = self.usage_dump(child)
 
         if child is None:
             package = {
                 "name": "PackageBodyElement",
                 "ownedRelationship": [package],
```

### Comparing `sysml2py-0.4.2/PKG-INFO` & `sysml2py-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Christopher Cox
 Author-email: chris.cox@westfall.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

