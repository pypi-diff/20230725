# Comparing `tmp/sphinx_apitree-1.4.2.tar.gz` & `tmp/sphinx_apitree-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.4.2.tar` & `sphinx_apitree-1.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/LICENSE
--rw-r--r--   0        0        0     2858 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/README.md
--rw-r--r--   0        0        0      105 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/__init__.py
--rw-r--r--   0        0        0     6613 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ast_utils.py
--rw-r--r--   0        0        0     4938 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/conf_util.py
--rw-r--r--   0        0        0     1058 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/context.py
--rw-r--r--   0        0        0      179 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/debug_utils.py
--rw-r--r--   0        0        0     1801 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/auto_ref.py
--rw-r--r--   0        0        0      885 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/docstring.py
--rw-r--r--   0        0        0     3688 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/ext/github_link.py
--rw-r--r--   0        0        0     1691 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/html_helper.py
--rw-r--r--   0        0        0     1324 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/import_utils.py
--rw-r--r--   0        0        0       30 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/structs.py
--rw-r--r--   0        0        0    10966 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/symbol_match.py
--rw-r--r--   0        0        0      212 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/api.md
--rw-r--r--   0        0        0       84 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/function.md
--rw-r--r--   0        0        0      183 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/module.md
--rw-r--r--   0        0        0       84 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1728 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/tree_extractor.py
--rw-r--r--   0        0        0      738 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/apitree/writer.py
--rw-r--r--   0        0        0     1556 2023-07-25 13:02:23.655329 sphinx_apitree-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 14:19:22.038716 sphinx_apitree-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2858 2023-07-25 14:19:22.038716 sphinx_apitree-1.4.3/README.md
+-rw-r--r--   0        0        0      105 2023-07-25 14:19:22.038716 sphinx_apitree-1.4.3/apitree/__init__.py
+-rw-r--r--   0        0        0     6613 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/ast_utils.py
+-rw-r--r--   0        0        0     5533 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/context.py
+-rw-r--r--   0        0        0      179 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/debug_utils.py
+-rw-r--r--   0        0        0     1801 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      885 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     3688 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/html_helper.py
+-rw-r--r--   0        0        0     1324 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/import_utils.py
+-rw-r--r--   0        0        0       30 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/structs.py
+-rw-r--r--   0        0        0    11763 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/symbol_match.py
+-rw-r--r--   0        0        0      212 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/api.md
+-rw-r--r--   0        0        0       84 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/function.md
+-rw-r--r--   0        0        0      183 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/module.md
+-rw-r--r--   0        0        0       84 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-25 14:19:22.042716 sphinx_apitree-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 sphinx_apitree-1.4.3/PKG-INFO
```

### Comparing `sphinx_apitree-1.4.2/LICENSE` & `sphinx_apitree-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/README.md` & `sphinx_apitree-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/ast_utils.py` & `sphinx_apitree-1.4.3/apitree/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/conf_util.py` & `sphinx_apitree-1.4.3/apitree/conf_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,40 +28,61 @@
   Args:
     modules: Top module names to document.
     includes_paths: Mapping to external files to `docs/` path (e.g.
       `my_module/submodule/README.md` to `submodule.md`). By default, only
       files inside `docs/...` can be read
     globals: The `conf.py` `globals()` dict. Will be mutated.
   """
+  _clear_etils()
 
   docs_dir = epath.Path(globals['__file__']).parent  # <repo>/docs/
   repo_dir = docs_dir.parent
   # TODO(epot): Fragile if one of the module is already imported.
   # If so, should check that imported modules are
   # `import_utils.belong_to_project`
   sys.path.insert(0, os.fspath(repo_dir))
 
   project_name = _get_project_name(repo_dir=repo_dir)
 
+  # API generator
+  api_ext = 'sphinx.ext.autodoc'
+  api_ext_config = dict(
+      autodoc_typehints_format='fully-qualified',  # `x.y.MyClass`
+      autodoc_default_options={
+          'members': True,
+          'show-inheritance': True,
+          'member-order': 'bysource',
+          'undoc-members': True,
+      },
+  )
+
+  # Uncomment to try autoapi
+  # api_ext = 'autoapi.extension'
+  # api_ext_config = dict(
+  #     autoapi_dirs=[f'../{project_name}'],
+  #     autoapi_ignore=['*migrations*', '*_test.py'],
+  #     autoapi_keep_files=True,
+  #     autoapi_python_use_implicit_namespaces=True,
+  # )
+
   globals.update(
       # Project information
       project=project_name,
       copyright=f'2023, {project_name} authors',
       author=f'{project_name} authors',
       # General configuration
       extensions=[
+          api_ext,  # API Doc generator
           'myst_nb',  # Notebook support
           'sphinx.ext.napoleon',  # Numpy-style docstrings
-          'sphinx.ext.autodoc',  # API Doc generator
-          'sphinx.ext.linkcode',  # Links to GitHub
+          # 'sphinx.ext.linkcode',  # Links to GitHub
           # Others:
           # 'sphinx_autodoc_typehints',
           # 'sphinx.ext.linkcode',
           # 'sphinx.ext.inheritance_diagram',
-          # 'autoapi.extension',
           # 'myst_parser',
           # API Tree
           'apitree.ext.docstring',  # Fix bad ```python md formatting
           'apitree.ext.auto_ref',  # Add cross ref for inline code
       ],
       exclude_patterns=[
           '_build',
@@ -79,22 +100,16 @@
       # TODO(epot): Instead should have a self-reference TOC
       html_theme_options={'home_page_in_toc': True},
       # -- Extensions ---------------------------------------------------
       # ---- myst -------------------------------------------------
       myst_heading_anchors=3,
       # ---- myst_nb -------------------------------------------------
       nb_execution_mode='off',
-      # ---- autodoc -------------------------------------------------
-      autodoc_typehints_format='fully-qualified',  # `x.y.MyClass`
-      autodoc_default_options={
-          'members': True,
-          'show-inheritance': True,
-          'member-order': 'bysource',
-          'undoc-members': True,
-      },
+      # ---- api extension -------------------------------------------------
+      **api_ext_config,
       # Register hooks
       setup=functools.partial(
           setup,
           callbacks=[
               functools.partial(
                   _write_api_doc, docs_dir=docs_dir, modules=modules
               ),
@@ -159,7 +174,15 @@
 
 
 def _get_project_name(repo_dir):
   # TODO(epot): This hardcode too much assumption on the program
   path = repo_dir / 'pyproject.toml'
   info = tomllib.loads(path.read_text())
   return info['project']['name']
+
+
+def _clear_etils():
+  # For re-triggering etils import (as it is used both for documentation
+  # and in apitree
+  for module_name in list(sys.modules):
+    if module_name.startswith('etils'):
+      del sys.modules[module_name]
```

### Comparing `sphinx_apitree-1.4.2/apitree/context.py` & `sphinx_apitree-1.4.3/apitree/context.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/ext/auto_ref.py` & `sphinx_apitree-1.4.3/apitree/ext/auto_ref.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/ext/docstring.py` & `sphinx_apitree-1.4.3/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/ext/github_link.py` & `sphinx_apitree-1.4.3/apitree/ext/github_link.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/html_helper.py` & `sphinx_apitree-1.4.3/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/import_utils.py` & `sphinx_apitree-1.4.3/apitree/import_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/symbol_match.py` & `sphinx_apitree-1.4.3/apitree/symbol_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import dataclasses
+import enum
 import functools
 import os
 import pathlib
 import types
 import typing
 from collections.abc import Callable, Iterator
 from typing import Any
@@ -20,14 +21,23 @@
 @dataclasses.dataclass
 class Context:
   module_name: str
   alias: str
   # visited: dict[str, _RefNode] = dataclasses.field(default_factory=dict)
 
 
+class SymbolType(enum.StrEnum):
+  MODULE = enum.auto()
+  CLASS = enum.auto()
+  FUNCTION = enum.auto()
+  ATTRIBUTE = enum.auto()
+  TYPING = enum.auto()
+  UNKNOWN = enum.auto()
+
+
 @edc.dataclass
 @dataclasses.dataclass
 class Symbol:
   name: str
   value: Any
 
   parent: types.ModuleType
@@ -80,15 +90,15 @@
 class Match:
   symbol: Symbol
 
   recurse: bool = False
   documented = True
   template_name: str | None = None
   docstring_1line: str = ''
-  icon: str = ''
+  icon: SymbolType = SymbolType.UNKNOWN
 
   extra_template_kwargs = {}
 
   SUBCLASSES: list[Match] = []
   SKIP_REGISTRATION = False
 
   def __init__(self, symbol):
@@ -152,29 +162,44 @@
     return self.template.format(
         qualname=self.symbol.qualname,
         qualname_no_alias=self.symbol.qualname_no_alias,
         **self.extra_template_kwargs,
     )
 
   def make_symbols_table(self, nodes: Iterator[tree_extractor.Node]):
-    table = md_utils.Table(header=['', '', ''])
+    table = md_utils.Table(header=['', ''])
 
     for n in nodes:
       filename = n.match.filename
       filename = filename.relative_to(self.filename.parent)
       filename = os.fspath(filename)
       filename = filename.removesuffix('.md')
       table.add_row(
-          f'*{n.match.icon}*',
+          # f'*{n.match.icon}*',
           f'[{n.symbol.qualname}]({filename})',
           f'{n.match.docstring_1line}',
       )
 
     return table.make()
 
+  def make_symbols_tables(self, nodes: tree_extractor.Node) -> str:
+    type_to_childs = epy.groupby(nodes, key=lambda n: n.match.icon)
+    lines = []
+    for type_ in SymbolType:
+      if type_ not in type_to_childs:
+        continue
+      lines.append('')
+      lines.append(f'### {type_.capitalize()}')
+      lines.append('')
+
+      childs = type_to_childs[type_]
+      childs = sorted(childs, key=lambda n: n.symbol.qualname)
+      lines.append(self.make_symbols_table(childs))
+    return '\n'.join(lines)
+
 
 def _not(cls: type[Match]) -> Callable[[Match], bool]:
   def match(self):
     return not cls.match(self)
 
   return match
 
@@ -193,15 +218,15 @@
     if not getattr(self.symbol.value, '__doc__', None):
       return ''
     else:
       return self.symbol.value.__doc__.split('\n', 1)[0]
 
 
 class _IsModule(_WithDocstring, Match):
-  icon = 'm'
+  icon = SymbolType.MODULE
   template_name = 'module'
 
   def match(self) -> bool:
     return isinstance(self.symbol.value, types.ModuleType)
 
   @property
   def filename(self) -> pathlib.Path:
@@ -211,15 +236,15 @@
         / 'index.md'
     )
 
   @property
   def extra_template_kwargs(self):
     return dict(
         toctree=self.toctree,
-        symbols_table=self.make_symbols_table(
+        symbols_table=self.make_symbols_tables(
             self.symbol.node.documented_childs
         ),
         source_link=github_link.get_module_link(self.symbol.value.__name__),
         **super().extra_template_kwargs,
     )
 
   @property
@@ -246,15 +271,15 @@
     return pathlib.Path(self.symbol.ctx.alias) / 'index.md'
 
   @property
   def extra_template_kwargs(self):
     return dict(
         **super().extra_template_kwargs,
         import_statement=self.import_statement,
-        all_symbols_table=self.make_symbols_table(
+        all_symbols_table=self.make_symbols_tables(
             self.symbol.node.iter_documented_nodes()
         ),
     )
 
   @property
   def import_statement(self) -> str:
     module_name = self.symbol.ctx.module_name
@@ -398,36 +423,36 @@
         source_code=self._ast_symbol.code,
         docstring=self._ast_symbol.docstring,
         **super().extra_template_kwargs,
     )
 
 
 class _TypeAliasValue(_DocumentedValue, _WithSourceLink):
-  icon = 't'
+  icon = SymbolType.TYPING
   template_name = 'type_alias'
 
   def match(self):
     # TODO(epot): How to detect `Any`,...
 
     return (
         isinstance(self.symbol.value, typing.TypeVar)
         or typing_extensions.get_origin(self.symbol.value) is not None
     )
 
 
 class _ClassValue(_WithDocstring, _DocumentedValue):
-  icon = 'c'
+  icon = SymbolType.CLASS
   template_name = 'class'
 
   def match(self):
     return isinstance(self.symbol.value, type)
 
 
 class _FunctionValue(_WithDocstring, _DocumentedValue):
-  icon = 'f'
+  icon = SymbolType.FUNCTION
   template_name = 'function'
 
   def match(self):
     return isinstance(
         self.symbol.value,
         (
             types.FunctionType,
@@ -437,15 +462,15 @@
             types.MethodWrapperType,
             functools._lru_cache_wrapper,  # `@functools.wraps`
         ),
     )
 
 
 class _AttributeValue(_DocumentedValue, _WithSourceLink):
-  icon = 'a'
+  icon = SymbolType.ATTRIBUTE
   template_name = 'attribute'
 
 
 def _is_package(module: types.ModuleType) -> bool:
   # Have custom attribute so standard module can behave like package.
   if hasattr(module, '__apitree__'):
     return module.__apitree__['is_package']
```

### Comparing `sphinx_apitree-1.4.2/apitree/tree_extractor.py` & `sphinx_apitree-1.4.3/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/apitree/writer.py` & `sphinx_apitree-1.4.3/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/pyproject.toml` & `sphinx_apitree-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.4.2/PKG-INFO` & `sphinx_apitree-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.4.2
+Version: 1.4.3
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

