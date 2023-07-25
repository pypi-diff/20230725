# Comparing `tmp/gcgen-0.1.0.tar.gz` & `tmp/gcgen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcgen-0.1.0.tar", last modified: Wed Feb  8 21:48:09 2023, max compression
+gzip compressed data, was "gcgen-0.1.2.tar", last modified: Tue Jul 25 09:03:46 2023, max compression
```

## Comparing `gcgen-0.1.0.tar` & `gcgen-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:48:09.434999 gcgen-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-08 21:48:09.434999 gcgen-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-08 21:47:58.000000 gcgen-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:48:09.430999 gcgen-0.1.0/gcgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:48:09.434999 gcgen-0.1.0/gcgen/api/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/api/snippets_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/api/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/api/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:48:09.434999 gcgen-0.1.0/gcgen/emitter/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/emitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/emitter/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/emitter/section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/emitter/special_chars.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/excbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    18981 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/log.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-08 21:47:58.000000 gcgen-0.1.0/gcgen/snippetparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:48:09.430999 gcgen-0.1.0/gcgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-08 21:48:09.000000 gcgen-0.1.0/gcgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-08 21:48:09.000000 gcgen-0.1.0/gcgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:48:09.000000 gcgen-0.1.0/gcgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-08 21:48:09.000000 gcgen-0.1.0/gcgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-08 21:48:09.000000 gcgen-0.1.0/gcgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-08 21:47:58.000000 gcgen-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:48:09.434999 gcgen-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-08 21:47:58.000000 gcgen-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:46.342964 gcgen-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-25 09:03:46.342964 gcgen-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 09:03:37.000000 gcgen-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:46.338964 gcgen-0.1.2/gcgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:46.342964 gcgen-0.1.2/gcgen/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/api/snippets_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/api/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/api/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:46.342964 gcgen-0.1.2/gcgen/emitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/emitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/emitter/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/emitter/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/emitter/special_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/excbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-07-25 09:03:37.000000 gcgen-0.1.2/gcgen/snippetparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:46.338964 gcgen-0.1.2/gcgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-25 09:03:46.000000 gcgen-0.1.2/gcgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 09:03:46.000000 gcgen-0.1.2/gcgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:03:46.000000 gcgen-0.1.2/gcgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 09:03:46.000000 gcgen-0.1.2/gcgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 09:03:46.000000 gcgen-0.1.2/gcgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 09:03:37.000000 gcgen-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:03:46.342964 gcgen-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 09:03:37.000000 gcgen-0.1.2/setup.py
```

### Comparing `gcgen-0.1.0/PKG-INFO` & `gcgen-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: gcgen
-Version: 0.1.0
+Version: 0.1.2
 Summary: generate code in any language or format
 Home-page: https://jwdevantier.github.io/gcgen/
 Author: Jesper Wendel Devantier
 Author-email: jwd@defmacro.it
 License: MIT
-Classifier: Framework :: Pytest
 Description-Content-Type: text/markdown
 
-# Readme
+# GCGEN: General Code Generator
+- PyPI Package: [![PYPI](https://img.shields.io/pypi/v/gcgen.svg)](https://pypi.org/project/gcgen/).
+- Documentation: https://jwdevantier.github.io/gcgen/
 
-`gcgen`, or general code generator, is a tool which enables straight-forward
-code generation in between hand-written code in your source files.
+A tool which permits straight-forward code generation driven by plain Python.
+Gcgen lets you insert generated code into existing files, surrounded by
+hand-written code or create new files from scratch. It also helps you build
+and share context, providing ways to load in data which is used when processing
+your code-generation code.
 
-Please see site: https://jwdevantier.github.io/gcgen/ for details
+Please see site: https://jwdevantier.github.io/gcgen/ for details.
```

### Comparing `gcgen-0.1.0/gcgen/__main__.py` & `gcgen-0.1.2/gcgen/__main__.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/api/__init__.py` & `gcgen-0.1.2/gcgen/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/api/snippets_helpers.py` & `gcgen-0.1.2/gcgen/api/snippets_helpers.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/api/tree.py` & `gcgen-0.1.2/gcgen/api/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,52 +209,14 @@
             self.visit_default(node)
             return
         # pass `self` explicitly as 'methods' are not bound
         m(self, node)
 
 
 class NodeTransformerMeta(type):
-    """Base class with which to implement a transformer.
-
-    Implement a transformer, a type of class capable of traversing a tree and
-    to replace some/all of the traversed nodes as it does so.
-    Transformers are especially useful for implementing rewrite operations where
-    specific nodes are replaced/modified to make subsequent parsing and eventually
-    code generation easier.
-
-    To start traversal, pass the tree to the `transform` method.
-    Traversal works by defining a `transform` method on the transformer for each
-    type of node, which in turn calls `transform` on each of its child nodes
-    to continue traversing down the tree. The return value of each transform
-    handler should be the transformed sub-tree.
-    In this way, parts or all of the tree may be transformed as part of the
-    operation.
-
-    Note:
-        For every node for which there is no specific handler, `visit_default`
-        is called. The default behavior of `visit_default` is to raise a
-        `NotImplementedError`.
-        To install a visit handler, write a method taking 1 argument, `node`,
-        and decorate it using the `on_visit()` decorator, passing the decorator
-        one or more `Type` objects (~classes), marking the types of nodes to
-        handle using the method.
-
-    Note:
-        * inheritance works (unlike functools.singledispatchmethod)
-            * handlers are inherited, and can be overridden
-        * method names of handlers MUST remain unique. If defining several
-          handlers using the same method name, only the last handler is retained.
-        * handlers must be decorated with `on_visit` as the _last_ decorator,
-          wrapping handlers in other decorators breaks the ability to identify
-          a method as a handler.
-        * a single handler can handle multiple types of nodes, either by:
-            * decorating the handler multiple times using `@on_visit(...)`
-            * passing multiple arguments to `@on_visit(...)`
-    """
-
     def __new__(cls, name, bases, dct):
         typ = super().__new__(cls, name, bases, dct)
 
         base_handlers = (getattr(b, "__transformers", {}) for b in bases)
         transformers = {}
 
         for bh in base_handlers:
@@ -279,14 +241,51 @@
             if isinstance(val, OnTransform):
                 setattr(obj, ident, val.method.__get__(obj))
 
         return obj
 
 
 class NodeTransformer(metaclass=NodeTransformerMeta):
+    """Base class with which to implement a transformer.
+
+    Implement a transformer, a type of class capable of traversing a tree and
+    to replace some/all of the traversed nodes as it does so.
+    Transformers are especially useful for implementing rewrite operations where
+    specific nodes are replaced/modified to make subsequent parsing and eventually
+    code generation easier.
+
+    To start traversal, pass the tree to the `transform` method.
+    Traversal works by defining a `transform` method on the transformer for each
+    type of node, which in turn calls `transform` on each of its child nodes
+    to continue traversing down the tree. The return value of each transform
+    handler should be the transformed sub-tree.
+    In this way, parts or all of the tree may be transformed as part of the
+    operation.
+
+    Note:
+        For every node for which there is no specific handler, `transform_default` is called.
+        The default behavior of `transform_default` is to raise a `NotImplementedError`.
+        To install a transform handler, write a method taking 1 argument, `node`,
+        and decorate it using the `on_transform()` decorator, passing the decorator
+        one or more `Type` objects (~classes), marking the types of nodes to
+        handle using the method.
+
+    Note:
+        * inheritance works (unlike functools.singledispatchmethod)
+            * handlers are inherited, and can be overridden
+        * method names of handlers MUST remain unique. If defining several
+          handlers using the same method name, only the last handler is retained.
+        * handlers must be decorated with `on_transform` as the _last_ decorator,
+          wrapping handlers in other decorators breaks the ability to identify
+          a method as a handler.
+        * a single handler can handle multiple types of nodes, either by:
+            * decorating the handler multiple times using `@on_visit(...)`
+            * passing multiple arguments to `@on_visit(...)`
+    """
+
     def transform_default(self, node: Any) -> Any:
         """Default transform function for nodes of types for which there is no specific transform function.
 
         This method defines the default action when calling `transform` on a node for
         which handler has been defined for the node's exact type.
         The default behavior is to raise an error, but this method may be overridden
         by a deriving class to e.g. return back the same object.
```

### Comparing `gcgen-0.1.0/gcgen/api/write_file.py` & `gcgen-0.1.2/gcgen/api/write_file.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/decorators.py` & `gcgen-0.1.2/gcgen/decorators.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/emitter/section.py` & `gcgen-0.1.2/gcgen/emitter/section.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Union, NewType, Iterator
-from gcgen.emitter.special_chars import *
+from gcgen.emitter.special_chars import CtrlChr, Padding
 
 
 class SectionError(Exception):
     pass
 
 
 class SectionDedentError(SectionError):
     msg = "dedent called too many times - trying to dedent out of minimum indentation"
 
 
-SectionElem = Union[str, "Section", "SpecialChar"]
+SectionElem = Union[str, "Section", CtrlChr, Padding]
 SectionBuf = NewType("SectionBuf", List[SectionElem])
 
 
 class Section:
     """A class for storing (buffered) text/code output.
 
     A section is an abstraction of text writing which provides 2 capabilities:
@@ -28,33 +28,34 @@
 
     (2) By allowing a section to contain other sections, it becomes possible to
     define 'placeholders' which can be filled out at a later time. Effectively
     making it possible to define the final output out of order, e.g. adding
     more variable definitions to the start of a function as it becomes
     necessary.
     """
+    __slots__ = "_buf", "_indent_level"
 
     def __init__(self) -> None:
         self._buf: SectionBuf = SectionBuf([])
         # to ensure indent/dedent is balanced within a section
         self._indent_level = 0
 
     def newline(self) -> "Section":
         """add a newline."""
-        self._buf.append(NL)
+        self._buf.append(CtrlChr.Newline)
         return self
 
     def nl(self) -> "Section":
         return self.newline()
 
     def freshline(self) -> "Section":
         """emit newline iff. not currently at the beginning of a line."""
-        if self._buf and self._buf[-1] in (FL, NL):
+        if self._buf and self._buf[-1] in (CtrlChr.Freshline, CtrlChr.Newline):
             return self
-        self._buf.append(FL)
+        self._buf.append(CtrlChr.Freshline)
         return self
 
     def fl(self) -> "Section":
         """emit newline iff. not currently at the beginning of a line."""
         return self.freshline()
 
     def add_section(self, s: "Section") -> "Section":
@@ -72,27 +73,27 @@
         """Indent subsequent lines.
 
         Causes all future lines to be indented one level more.
 
         Note: this function will cause a newline if the current line has any
         contents already written to it (using `emit`).
         """
-        self._buf.append(I)
+        self._buf.append(CtrlChr.Indent)
         self._indent_level += 1
         return self
 
     def dedent(self) -> "Section":
         """Dedent lines by one.
 
         Causes all future lines to be indented one level less.
 
         Note: this function will cause a newline if the current line has any
         contents already written to it (using `emit`).
         """
-        self._buf.append(D)
+        self._buf.append(CtrlChr.Dedent)
         self._indent_level -= 1
         if self._indent_level < 0:
             raise SectionDedentError
         return self
 
     def ensure_padding_lines(self, nlines: int) -> "Section":
         """Ensure (at least) `n` empty lines of padding between two sections
@@ -110,15 +111,15 @@
                 raise TypeError(f"got {type(elem)}, expected str (val: {repr(elem)})")
             bappend(elem.replace("\n", "\\n"))
         return self
 
     def emitln(self, *elems: str) -> "Section":
         """Emit one or more string elements followed by a newline."""
         self.emit(*elems)
-        self._buf.append(NL)
+        self._buf.append(CtrlChr.Newline)
         return self
 
     def emitln_r(self, *elems: str) -> "Section":
         """Write line, then indent.
 
         NOTE: deprecated, use `sec.emitln(...).indent()` instead
         """
```

### Comparing `gcgen-0.1.0/gcgen/generate.py` & `gcgen-0.1.2/gcgen/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,15 @@
 
 def fmt_module_name(root: Path, modpath: Path) -> str:
     modname = modpath.relative_to(root)
     modname = modname.parent / modname.name[: -len(modname.suffix)]
     return ".".join(e.replace(" ", "_") for e in modname.parts)
 
 
-def import_from_path(root: Path, modpath: Path):
+def import_from_path(root: Path, modpath: Path) -> ModuleType:
     modname = fmt_module_name(root, modpath)
     spec = importlib.util.spec_from_file_location(modname, modpath)
     if spec is None:
         raise RuntimeError("spec not loaded, should be impossible")
     mod = importlib.util.module_from_spec(spec)
     sys.modules[modname] = mod
     assert spec.loader is not None
@@ -385,121 +385,128 @@
     }
 
 
 def get_mod_snippet_fns(mod: ModuleType) -> Dict[str, Callable]:
     return {name: fn for name, fn in mod.__dict__.items() if decorators.is_snippet(fn)}
 
 
-def compile(root: Path, tag_start: str = "<<?", tag_end: str = "?>>"):
-    # in case `root` is a relative path like '.', resolve to absolute path
-    # for later use, where cwd changes.
-    root = root.resolve()
-
-    def _compile(
-        path: Path, parent_scope: Scope, snippets_scope: Scope, indent_by: Scope
-    ):
-        gcgen_mod = None
-        gcgen_conf_path = path / "gcgen_conf.py"
-        if gcgen_conf_path.exists():
-            gcgen_mod = import_from_path(root, gcgen_conf_path)
-        scope = parent_scope.derive()
-
-        exclude_dirs = []
-        if gcgen_mod is not None:
-            if hasattr(gcgen_mod, "gcgen_exclude_dirs"):
-                try:
-                    exclude_dirs = gcgen_mod.gcgen_exclude_dirs()
-                except Exception as e:
-                    logger.critical(
-                        f"error during execution of `gcgen_exclude_dirs` in {gcgen_conf_path!s}",
-                        exc_info=True,
-                    )
-                    raise CompileExcludeFilesError(gcgen_conf_path)
-
-            if hasattr(gcgen_mod, "gcgen_indent_by"):
-                indent_by = indent_by.derive()
-                mod_indent_by = gcgen_mod.gcgen_indent_by
-                if not isinstance(mod_indent_by, dict):
-                    raise IndentByValueError(mod_indent_by, gcgen_conf_path)
-                indent_by.update(mod_indent_by)
-            # if fn to extend local scope exists, run it
-            if hasattr(gcgen_mod, "gcgen_scope_extend"):
-                try:
-                    gcgen_mod.gcgen_scope_extend(scope)
-                except Exception as e:
-                    logger.critical(
-                        f"error during execution of `gcgen_scope_extend` in {gcgen_conf_path!s}",
-                        exc_info=True,
-                    )
-                    raise CompileScopeExtendError(gcgen_conf_path) from e
-            # if one or more snippets are defined, extend scope
-            snippet_fns = list(get_mod_snippet_fns(gcgen_mod).values())
-            if snippet_fns:
-                snippets_scope = snippets_scope.derive()
-                for snippet_fn in snippet_fns:
-                    for name in decorators.snippet_names(snippet_fn):
-                        snippets_scope[name] = snippet_fn
-
-        # traverse and compile in depth-first order, passing initialized scope
-        for p in path.iterdir():
-            if p.is_dir() and p.name not in exclude_dirs:
-                _compile(p, scope, snippets_scope, indent_by)
-
-        if gcgen_mod is None:
-            return
-
-        # operate from within the path containing the gcgen_conf.py we are currently processing
-        os.chdir(path)
-        # parse snippets in any files explicitly listed as having them
-        if hasattr(gcgen_mod, "gcgen_parse_files"):
+def _compile(
+        root: Path,
+        tag_start: str,
+        tag_end: str,
+        path: Path,
+        parent_scope: Scope,
+        snippets_scope: Scope,
+        indent_by: Scope
+) -> None:
+    gcgen_mod = None
+    gcgen_conf_path = path / "gcgen_conf.py"
+    if gcgen_conf_path.exists():
+        gcgen_mod = import_from_path(root, gcgen_conf_path)
+    scope = parent_scope.derive()
+
+    exclude_dirs = []
+    if gcgen_mod is not None:
+        if hasattr(gcgen_mod, "gcgen_exclude_dirs"):
             try:
-                files = gcgen_mod.gcgen_parse_files()
+                exclude_dirs = gcgen_mod.gcgen_exclude_dirs()
             except Exception as e:
                 logger.critical(
-                    f"error during execution of `gcgen_parse_files` in {gcgen_conf_path!s}",
+                    f"error during execution of `gcgen_exclude_dirs` in {gcgen_conf_path!s}",
                     exc_info=True,
                 )
-                raise CompileParseFilesError(gcgen_conf_path) from e
-            parser = Parser(tag_start, tag_end, scope, snippets_scope, indent_by, root)
-            for file in files:
-                logger.info(f"Parsing {file!s}")
-                file = Path(file)
-                if str(file) != file.name:
-                    logger.error(
-                        f"{file!s} - entries in `gcgen_parse_files` must be plain filenames, not paths!",
-                    )
-                    raise ParseFilesInvalidValue(file, gcgen_conf_path)
-
-                # compute absolute path to file (needed by compiler)
-                file = (path / file).resolve()
-                if not file.exists():
-                    logger.error(
-                        f"{file!s} - Could not find file!",
-                    )
-                    raise ParseFileNotFoundError(file, gcgen_conf_path)
-                elif not file.is_file():
-                    logger.error(
-                        f"{file!s} - expected a file, got something else!",
-                        extra={"file": str(file), "gcgen file": gcgen_conf_path},
-                    )
-                    raise ParseFileNotFileError(file, gcgen_conf_path)
-                file_scope = scope.derive()
-                parser.scope = file_scope
-                logger.debug(f"Input:\n{file.read_text()}")
-                parser.parse(file, file)
-                logger.debug(f"Output{file.read_text()}")
-
-        # parse generators (functions which may create arbitrarily many files)
-        for name, fn in get_mod_generator_fns(gcgen_mod).items():
-            local_scope = scope.derive()
+                raise CompileExcludeFilesError(gcgen_conf_path)
+
+        if hasattr(gcgen_mod, "gcgen_indent_by"):
+            indent_by = indent_by.derive()
+            mod_indent_by = gcgen_mod.gcgen_indent_by
+            if not isinstance(mod_indent_by, dict):
+                raise IndentByValueError(mod_indent_by, gcgen_conf_path)
+            indent_by.update(mod_indent_by)
+        # if fn to extend local scope exists, run it
+        if hasattr(gcgen_mod, "gcgen_scope_extend"):
             try:
-                fn(local_scope)
+                gcgen_mod.gcgen_scope_extend(scope)
             except Exception as e:
-                logger.error(
-                    f"error executing generator function {name!s} in {gcgen_conf_path!s}",
+                logger.critical(
+                    f"error during execution of `gcgen_scope_extend` in {gcgen_conf_path!s}",
                     exc_info=True,
                 )
-                raise CompileGeneratorFunctionError(name, gcgen_conf_path) from e
+                raise CompileScopeExtendError(gcgen_conf_path) from e
+        # if one or more snippets are defined, extend scope
+        snippet_fns = list(get_mod_snippet_fns(gcgen_mod).values())
+        if snippet_fns:
+            snippets_scope = snippets_scope.derive()
+            for snippet_fn in snippet_fns:
+                for name in decorators.snippet_names(snippet_fn):
+                    snippets_scope[name] = snippet_fn
+
+    # traverse and compile in depth-first order, passing initialized scope
+    for p in path.iterdir():
+        if p.is_dir() and p.name not in exclude_dirs:
+            _compile(root, tag_start, tag_end, p, scope, snippets_scope, indent_by)
+
+    if gcgen_mod is None:
+        return
+
+    # operate from within the path containing the gcgen_conf.py we are currently processing
+    os.chdir(path)
+    # parse snippets in any files explicitly listed as having them
+    if hasattr(gcgen_mod, "gcgen_parse_files"):
+        try:
+            files = gcgen_mod.gcgen_parse_files()
+        except Exception as e:
+            logger.critical(
+                f"error during execution of `gcgen_parse_files` in {gcgen_conf_path!s}",
+                exc_info=True,
+            )
+            raise CompileParseFilesError(gcgen_conf_path) from e
+        parser = Parser(tag_start, tag_end, scope, snippets_scope, indent_by, root)
+        for file in files:
+            logger.info(f"Parsing {file!s}")
+            file = Path(file)
+            if str(file) != file.name:
+                logger.error(
+                    f"{file!s} - entries in `gcgen_parse_files` must be plain filenames, not paths!",
+                )
+                raise ParseFilesInvalidValue(file, gcgen_conf_path)
+
+            file = (path / file)
+            if file.is_symlink():
+                # symlinks need to be resolved, otherwise the atomic
+                # file replace at the end of the parse step will fail
+                file = file.resolve()
+            if not file.exists():
+                logger.error(
+                    f"{file!s} - Could not find file!",
+                )
+                raise ParseFileNotFoundError(file, gcgen_conf_path)
+            elif not file.is_file():
+                logger.error(
+                    f"{file!s} - expected a file, got something else!",
+                    extra={"file": str(file), "gcgen file": gcgen_conf_path},
+                )
+                raise ParseFileNotFileError(file, gcgen_conf_path)
+            file_scope = scope.derive()
+            parser.scope = file_scope
+            parser.parse(file, file)
+
+    # parse generators (functions which may create arbitrarily many files)
+    for name, fn in get_mod_generator_fns(gcgen_mod).items():
+        local_scope = scope.derive()
+        try:
+            fn(local_scope)
+        except Exception as e:
+            logger.error(
+                f"error executing generator function {name!s} in {gcgen_conf_path!s}",
+                exc_info=True,
+            )
+            raise CompileGeneratorFunctionError(name, gcgen_conf_path) from e
+
+def compile(root: Path, tag_start: str = "<<?", tag_end: str = "?>>") -> None:
+    # in case `root` is a relative path like '.', resolve to absolute path
+    # for later use, where cwd changes.
+    root = root.resolve()
 
     indent_by = Scope()
     indent_by[""] = "   "
-    _compile(root, Scope(), Scope(), indent_by)
+    _compile(root, tag_start, tag_end, root, Scope(), Scope(), indent_by)
```

### Comparing `gcgen-0.1.0/gcgen/log.py` & `gcgen-0.1.2/gcgen/log.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen/scope.py` & `gcgen-0.1.2/gcgen/scope.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class Scope:
     """
     A scope is a form of layered dictionary, where derived/child scopes
     indirectly inherit all entries visible from the parent scope, with the
     ability to add new entries, override entries and delete entries, all
     without changing any of the parent scopes.
     """
+    __slots__ = "_dict", "_outer"
 
     def __init__(self):
         self._dict = {}
         self._outer = None
 
     def derive(self) -> "Scope":
         """Create a child scope with this scope as its parent.
```

### Comparing `gcgen-0.1.0/gcgen/snippetparser.py` & `gcgen-0.1.2/gcgen/snippetparser.py`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/gcgen.egg-info/PKG-INFO` & `gcgen-0.1.2/gcgen.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: gcgen
-Version: 0.1.0
+Version: 0.1.2
 Summary: generate code in any language or format
 Home-page: https://jwdevantier.github.io/gcgen/
 Author: Jesper Wendel Devantier
 Author-email: jwd@defmacro.it
 License: MIT
-Classifier: Framework :: Pytest
 Description-Content-Type: text/markdown
 
-# Readme
+# GCGEN: General Code Generator
+- PyPI Package: [![PYPI](https://img.shields.io/pypi/v/gcgen.svg)](https://pypi.org/project/gcgen/).
+- Documentation: https://jwdevantier.github.io/gcgen/
 
-`gcgen`, or general code generator, is a tool which enables straight-forward
-code generation in between hand-written code in your source files.
+A tool which permits straight-forward code generation driven by plain Python.
+Gcgen lets you insert generated code into existing files, surrounded by
+hand-written code or create new files from scratch. It also helps you build
+and share context, providing ways to load in data which is used when processing
+your code-generation code.
 
-Please see site: https://jwdevantier.github.io/gcgen/ for details
+Please see site: https://jwdevantier.github.io/gcgen/ for details.
```

### Comparing `gcgen-0.1.0/gcgen.egg-info/SOURCES.txt` & `gcgen-0.1.2/gcgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcgen-0.1.0/setup.py` & `gcgen-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 print(f"Building version: {version}")
 
 setup(
     name="gcgen",
     description="generate code in any language or format",
     long_description=README,
     long_description_content_type="text/markdown",
-    classifiers=["Framework :: Pytest"],
+    classifiers=[],
     version=version,
     author="Jesper Wendel Devantier",
     author_email="jwd@defmacro.it",
     url="https://jwdevantier.github.io/gcgen/",
     packages=find_packages(exclude=["tests"]),
     install_requires=[],
     entry_points={"console_scripts": ["gcgen = gcgen.__main__:main"]},
     license="MIT",
     options={"bdist_wheel": {"universal": True}},
-    package_data = {
-        'gcgen': ['py.typed'],
+    package_data={
+        "gcgen": ["py.typed"],
     },
 )
```

