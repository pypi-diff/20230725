# Comparing `tmp/sphinx_apitree-1.3.1.tar.gz` & `tmp/sphinx_apitree-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.3.1.tar` & `sphinx_apitree-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/LICENSE
--rw-r--r--   0        0        0     1980 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/README.md
--rw-r--r--   0        0        0      105 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/__init__.py
--rw-r--r--   0        0        0     2631 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/ast_utils.py
--rw-r--r--   0        0        0     4707 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/conf_util.py
--rw-r--r--   0        0        0     1058 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/context.py
--rw-r--r--   0        0        0     1761 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/auto_ref.py
--rw-r--r--   0        0        0      808 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/docstring.py
--rw-r--r--   0        0        0     2908 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/github_link.py
--rw-r--r--   0        0        0     1691 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/html_helper.py
--rw-r--r--   0        0        0       30 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/structs.py
--rw-r--r--   0        0        0    10880 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/symbol_match.py
--rw-r--r--   0        0        0      183 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/api.md
--rw-r--r--   0        0        0       42 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/function.md
--rw-r--r--   0        0        0      154 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/module.md
--rw-r--r--   0        0        0      121 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1728 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/tree_extractor.py
--rw-r--r--   0        0        0      738 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/writer.py
--rw-r--r--   0        0        0     1556 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 sphinx_apitree-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2858 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/README.md
+-rw-r--r--   0        0        0      105 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/__init__.py
+-rw-r--r--   0        0        0     6603 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/ast_utils.py
+-rw-r--r--   0        0        0     4707 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/context.py
+-rw-r--r--   0        0        0      179 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/debug_utils.py
+-rw-r--r--   0        0        0     1801 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      885 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     3688 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/html_helper.py
+-rw-r--r--   0        0        0     1324 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/import_utils.py
+-rw-r--r--   0        0        0       30 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/structs.py
+-rw-r--r--   0        0        0    10966 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/symbol_match.py
+-rw-r--r--   0        0        0      212 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/api.md
+-rw-r--r--   0        0        0       84 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/function.md
+-rw-r--r--   0        0        0      183 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/module.md
+-rw-r--r--   0        0        0       84 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-25 10:25:16.625658 sphinx_apitree-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.0/PKG-INFO
```

### Comparing `sphinx_apitree-1.3.1/LICENSE` & `sphinx_apitree-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/apitree/conf_util.py` & `sphinx_apitree-1.4.0/apitree/conf_util.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/apitree/context.py` & `sphinx_apitree-1.4.0/apitree/context.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/apitree/ext/auto_ref.py` & `sphinx_apitree-1.4.0/apitree/ext/auto_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import pathlib
 import typing
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
-from apitree import context
+from apitree import context, debug_utils
 
 
 def _is_inside_link(node: nodes.Node):
     while node.parent:
         if isinstance(node.parent, nodes.reference):
             return True
         node = node.parent
@@ -63,8 +63,8 @@
 
   new_p = pathlib.Path(*(['..'] * num_parents)).joinpath(*p0.parts[num_common_parts:])
   return new_p
 
 
 
 def setup(app: Sphinx):
-    app.connect('doctree-resolved', _add_refs)
+    app.connect('doctree-resolved', debug_utils.print_error()(_add_refs))
```

### Comparing `sphinx_apitree-1.3.1/apitree/ext/docstring.py` & `sphinx_apitree-1.4.0/apitree/ext/docstring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Fix bad ```python md formatting."""
 
 from sphinx.application import Sphinx
 
+from apitree import debug_utils
+
 
 def _preprocess_docstring(app, what, name, obj, options, lines):
   # Modify each line of the docstring
   is_block = False
   new_lines = []
   for line in lines:
     if line == '```python':
@@ -25,8 +27,11 @@
         line = f'  {line}'
       new_lines.append(line)
   lines[:] = new_lines
 
 
 def setup(app: Sphinx):
   # Fix bad ```python md formatting
-  app.connect('autodoc-process-docstring', _preprocess_docstring)
+  app.connect(
+      'autodoc-process-docstring',
+      debug_utils.print_error()(_preprocess_docstring),
+  )
```

### Comparing `sphinx_apitree-1.3.1/apitree/html_helper.py` & `sphinx_apitree-1.4.0/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/apitree/symbol_match.py` & `sphinx_apitree-1.4.0/apitree/symbol_match.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,14 +214,15 @@
   @property
   def extra_template_kwargs(self):
     return dict(
         toctree=self.toctree,
         symbols_table=self.make_symbols_table(
             self.symbol.node.documented_childs
         ),
+        source_link=github_link.get_module_link(self.symbol.value.__name__),
         **super().extra_template_kwargs,
     )
 
   @property
   def toctree(self) -> str:
     items = []
     for n in self.symbol.node.documented_childs:
@@ -366,21 +367,40 @@
 
 
 # TODO(epot): How to duplicate this with _ImportedValue ?
 
 
 class _WithSourceLink(Match):
 
+  @functools.cached_property
+  def _ast_symbol(self):
+    module_name = self.symbol.parent.__name__
+    name = self.symbol.name
+
+    return ast_utils.extract_last_symbol(module_name, name)
+
+  @property
+  def docstring_1line(self) -> str:
+    doc = ' '.join(self._ast_symbol.docstring.split('\n'))
+    if len(doc) > 83:  # Truncate
+      return doc[:80] + '...'
+    else:
+      return doc
+
   @property
   def extra_template_kwargs(self):
     module_name = self.symbol.parent.__name__
-    filepath = github_link._get_definition_line(module_name, self.symbol.name)
-    source_link = f'{github_link._get_github_url()}/tree/main/{filepath}'
+    name = self.symbol.name
+
+    source_link = github_link.get_assignement_link(module_name, name)
+
     return dict(
         source_link=source_link,
+        source_code=self._ast_symbol.code,
+        docstring=self._ast_symbol.docstring,
         **super().extra_template_kwargs,
     )
 
 
 class _TypeAliasValue(_DocumentedValue, _WithSourceLink):
   icon = 't'
   template_name = 'type_alias'
@@ -389,26 +409,14 @@
     # TODO(epot): How to detect `Any`,...
 
     return (
         isinstance(self.symbol.value, typing.TypeVar)
         or typing_extensions.get_origin(self.symbol.value) is not None
     )
 
-  @property
-  def extra_template_kwargs(self):
-    # TODO(epot): Extract the first and last line of the assignment
-    # module_name = self.symbol.parent.__name__
-    # filepath = github_link._get_definition_line(module_name, self.symbol.name)
-    # source_link = f'{github_link._get_github_url()}/tree/main/{filepath}'
-    source_code = ''
-    return dict(
-        source_code=source_code,
-        **super().extra_template_kwargs,
-    )
-
 
 class _ClassValue(_WithDocstring, _DocumentedValue):
   icon = 'c'
   template_name = 'class'
 
   def match(self):
     return isinstance(self.symbol.value, type)
@@ -423,23 +431,22 @@
         self.symbol.value,
         (
             types.FunctionType,
             types.BuiltinFunctionType,
             types.BuiltinMethodType,
             types.MethodType,
             types.MethodWrapperType,
+            functools._lru_cache_wrapper,  # `@functools.wraps`
         ),
     )
 
 
 class _AttributeValue(_DocumentedValue, _WithSourceLink):
   icon = 'a'
   template_name = 'attribute'
 
-  # TODO(epot): Extract doc from parent
-
 
 def _is_package(module: types.ModuleType) -> bool:
   # Have custom attribute so standard module can behave like package.
   if hasattr(module, '__apitree__'):
     return module.__apitree__['is_package']
   return module.__name__ == module.__package__
```

### Comparing `sphinx_apitree-1.3.1/apitree/tree_extractor.py` & `sphinx_apitree-1.4.0/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/apitree/writer.py` & `sphinx_apitree-1.4.0/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/pyproject.toml` & `sphinx_apitree-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.1/PKG-INFO` & `sphinx_apitree-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: sphinx-apitree
-Version: 1.3.1
-Summary: Sphinx extension to auto-generate API tree.
-Keywords: sphinx,doc
-Author-email: Conchylicultor <etiennefg.pot@mail.com>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Requires-Dist: etils[edc,enp,epath,epy,etree]
-Requires-Dist: typing_extensions
-Requires-Dist: pytest>=3.4 ; extra == "dev"
-Requires-Dist: pytest-xdist ; extra == "dev"
-Requires-Dist: pylint>=2.6.0 ; extra == "dev"
-Requires-Dist: pyink ; extra == "dev"
-Requires-Dist: sphinx-apitree[ext] ; extra == "dev"
-Requires-Dist: etils[ecolab] ; extra == "dev"
-Requires-Dist: sphinx ; extra == "ext"
-Requires-Dist: myst_nb ; extra == "ext"
-Requires-Dist: sphinx_book_theme ; extra == "ext"
-Project-URL: homepage, https://github.com/conchylicultor/sphinx-apitree
-Project-URL: repository, https://github.com/conchylicultor/sphinx-apitree
-Provides-Extra: dev
-Provides-Extra: ext
-
 # sphinx-apitree
 
 [![Unittests](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/conchylicultor/sphinx-apitree/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/sphinx-apitree.svg)](https://badge.fury.io/py/sphinx-apitree)
 
 
 `apitree` is a small library to generate a ready-to-use documentation with minimal friction!
@@ -96,14 +68,40 @@
     install:
         - method: pip
         path: .
         extra_requirements:
             - docs
     ```
 
+## Options
+
+By default, `apitree` tries to infer everything automatically. However there's sometimes
+times where the user want to overwrite the default choices.
+
+*   Package vs module: By default, all `__init__.py` define the public API (imports documented), while
+    the modules (`module.py`) define the implementation (imports not documented).
+    You can explicitly mark a module as package, so it's import are documented, by adding in the
+    module definition:
+
+    ```python
+    __apitree__ = dict(
+        is_package=True,
+    )
+    ```
+
 ## Examples of projects using apitree
 
 * https://github.com/google-research/visu3d (https://visu3d.readthedocs.io/)
 * https://github.com/google-research/dataclass_array (https://dataclass-array.readthedocs.io/)
 * https://github.com/google-research/etils (https://etils.readthedocs.io/)
 * https://github.com/google-research/kauldron (https://kauldron.readthedocs.io/)
 
+Generated with:
+
+```
+echo start \
+&& cd ../visu3d          && sphinx-build -b html docs/ docs/_build \
+&& cd ../dataclass_array && sphinx-build -b html docs/ docs/_build \
+&& cd ../etils           && sphinx-build -b html docs/ docs/_build \
+&& cd ../kauldron        && sphinx-build -b html docs/ docs/_build \
+&& echo finished
+```
```

