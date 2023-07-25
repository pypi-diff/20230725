# Comparing `tmp/sphinx_apitree-1.4.1.tar.gz` & `tmp/sphinx_apitree-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.4.1.tar` & `sphinx_apitree-1.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/LICENSE
--rw-r--r--   0        0        0     2858 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/README.md
--rw-r--r--   0        0        0      105 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/__init__.py
--rw-r--r--   0        0        0     6603 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/ast_utils.py
--rw-r--r--   0        0        0     4938 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/conf_util.py
--rw-r--r--   0        0        0     1058 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/context.py
--rw-r--r--   0        0        0      179 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/debug_utils.py
--rw-r--r--   0        0        0     1801 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/ext/auto_ref.py
--rw-r--r--   0        0        0      885 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/ext/docstring.py
--rw-r--r--   0        0        0     3688 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/ext/github_link.py
--rw-r--r--   0        0        0     1691 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/html_helper.py
--rw-r--r--   0        0        0     1324 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/import_utils.py
--rw-r--r--   0        0        0       30 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/structs.py
--rw-r--r--   0        0        0    10966 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/symbol_match.py
--rw-r--r--   0        0        0      212 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/api.md
--rw-r--r--   0        0        0       84 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/function.md
--rw-r--r--   0        0        0      183 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/module.md
--rw-r--r--   0        0        0       84 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1728 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/tree_extractor.py
--rw-r--r--   0        0        0      738 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/apitree/writer.py
--rw-r--r--   0        0        0     1556 2023-07-25 12:50:39.406801 sphinx_apitree-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/LICENSE
+-rw-r--r--   0        0        0     2858 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/README.md
+-rw-r--r--   0        0        0      105 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/__init__.py
+-rw-r--r--   0        0        0     6613 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ast_utils.py
+-rw-r--r--   0        0        0     4938 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/context.py
+-rw-r--r--   0        0        0      179 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/debug_utils.py
+-rw-r--r--   0        0        0     1801 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      885 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     3688 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/html_helper.py
+-rw-r--r--   0        0        0     1324 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/import_utils.py
+-rw-r--r--   0        0        0       30 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/structs.py
+-rw-r--r--   0        0        0    10966 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/symbol_match.py
+-rw-r--r--   0        0        0      212 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/api.md
+-rw-r--r--   0        0        0       84 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/function.md
+-rw-r--r--   0        0        0      183 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/module.md
+-rw-r--r--   0        0        0       84 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.2/PKG-INFO
```

### Comparing `sphinx_apitree-1.4.1/LICENSE` & `sphinx_apitree-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/README.md` & `sphinx_apitree-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/ast_utils.py` & `sphinx_apitree-1.4.2/apitree/ast_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     docstring_lines = []
     for lines_no in range(self.start - 2, 0, -1):
       line = lines[lines_no].strip()
       if not line.startswith('# '):
         break
       line = line.removeprefix('# ')
       docstring_lines.append(line)
-    return '\n'.join(docstring_lines)
+    return '\n'.join(reversed(docstring_lines))
 
   @property
   def code(self) -> str:
     lines = import_utils.module_lines(self.module_name)
     lines = lines[self.start - 1 : self.end]
     return '\n'.join(lines)
```

### Comparing `sphinx_apitree-1.4.1/apitree/conf_util.py` & `sphinx_apitree-1.4.2/apitree/conf_util.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/context.py` & `sphinx_apitree-1.4.2/apitree/context.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/ext/auto_ref.py` & `sphinx_apitree-1.4.2/apitree/ext/auto_ref.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/ext/docstring.py` & `sphinx_apitree-1.4.2/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/ext/github_link.py` & `sphinx_apitree-1.4.2/apitree/ext/github_link.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/html_helper.py` & `sphinx_apitree-1.4.2/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/import_utils.py` & `sphinx_apitree-1.4.2/apitree/import_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/symbol_match.py` & `sphinx_apitree-1.4.2/apitree/symbol_match.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/tree_extractor.py` & `sphinx_apitree-1.4.2/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/apitree/writer.py` & `sphinx_apitree-1.4.2/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/pyproject.toml` & `sphinx_apitree-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.1/PKG-INFO` & `sphinx_apitree-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.4.1
+Version: 1.4.2
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

