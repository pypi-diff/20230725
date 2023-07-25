# Comparing `tmp/collagen-0.1.4.tar.gz` & `tmp/collagen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collagen-0.1.4.tar", last modified: Sun Jul 23 16:00:12 2023, max compression
+gzip compressed data, was "collagen-0.2.0.tar", last modified: Tue Jul 25 20:21:07 2023, max compression
```

## Comparing `collagen-0.1.4.tar` & `collagen-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-23 16:00:03.000000 collagen-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-23 16:00:12.105856 collagen-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-23 16:00:03.000000 collagen-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/collagen/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-23 16:00:03.000000 collagen-0.1.4/collagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-23 16:00:12.105856 collagen-0.1.4/collagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-23 16:00:03.000000 collagen-0.1.4/collagen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-07-23 16:00:03.000000 collagen-0.1.4/collagen/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/collagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-23 16:00:12.000000 collagen-0.1.4/collagen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.101856 collagen-0.1.4/mkdocstrings_handlers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/mkdocstrings_handlers/collagen/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-23 16:00:03.000000 collagen-0.1.4/mkdocstrings_handlers/collagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-23 16:00:03.000000 collagen-0.1.4/mkdocstrings_handlers/collagen/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.101856 collagen-0.1.4/mkdocstrings_handlers/collagen/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/mkdocstrings_handlers/collagen/templates/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-23 16:00:03.000000 collagen-0.1.4/mkdocstrings_handlers/collagen/templates/terminal/hints.html
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-23 16:00:03.000000 collagen-0.1.4/mkdocstrings_handlers/collagen/templates/terminal/ops.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-23 16:00:12.105856 collagen-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 16:00:03.000000 collagen-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:00:12.105856 collagen-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-23 16:00:03.000000 collagen-0.1.4/tests/test_zvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    86677 2023-07-23 16:00:03.000000 collagen-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.685014 collagen-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 20:20:56.000000 collagen-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 20:21:07.685014 collagen-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-25 20:20:56.000000 collagen-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.681014 collagen-0.2.0/collagen/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 20:21:07.685014 collagen-0.2.0/collagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.681014 collagen-0.2.0/collagen/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/branching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/other.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.681014 collagen-0.2.0/collagen/standard/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/hson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/json5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/resources/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/stack_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/standard/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-25 20:20:56.000000 collagen-0.2.0/collagen/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.681014 collagen-0.2.0/collagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 20:21:07.000000 collagen-0.2.0/collagen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.677014 collagen-0.2.0/mkdocstrings_handlers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.681014 collagen-0.2.0/mkdocstrings_handlers/collagen/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 20:20:56.000000 collagen-0.2.0/mkdocstrings_handlers/collagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-07-25 20:20:56.000000 collagen-0.2.0/mkdocstrings_handlers/collagen/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.677014 collagen-0.2.0/mkdocstrings_handlers/collagen/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.685014 collagen-0.2.0/mkdocstrings_handlers/collagen/templates/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-25 20:20:56.000000 collagen-0.2.0/mkdocstrings_handlers/collagen/templates/terminal/metadata.html
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 20:20:56.000000 collagen-0.2.0/mkdocstrings_handlers/collagen/templates/terminal/ops.html
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 20:21:07.685014 collagen-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 20:20:56.000000 collagen-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:21:07.685014 collagen-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 20:20:56.000000 collagen-0.2.0/tests/test_zvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86677 2023-07-25 20:20:56.000000 collagen-0.2.0/versioneer.py
```

### Comparing `collagen-0.1.4/LICENSE` & `collagen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collagen-0.1.4/collagen/vm.py` & `collagen-0.2.0/collagen/vm.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,46 +34,46 @@
         return self._stack.pop()
 
     def popn(self, n: int) -> List[Any]:
         if n > len(self._stack):
             raise RuntimeError("Cannot pop from empty stack")
         return [self._stack.pop() for _ in range(n)][::-1]
 
-    def set(self, key: str, value: Any):
-        self._set[key] = value
-
-    def has(self, key) -> bool:
-        return key in self._set
+    def set(self, key: str, value: Any, global_var: bool = False):
+        if global_var:
+            self._vm._globals[key] = value
+        else:
+            self._set[key] = value
 
-    def get(self, key: str) -> Any:
-        if key not in self._set:
-            raise RuntimeError(f"Global variable has not been set: {key}")
-        return self._set[key]
+    def has(self, key, global_var: bool = False) -> bool:
+        if global_var:
+            return key in self._vm._globals
+        else:
+            return key in self._set
 
-    def delete(self, key):
-        del self._set[key]
+    def get(self, key: str, global_var: bool = False) -> Any:
+        if global_var:
+            if key not in self._vm._globals:
+                raise RuntimeError(f"Global variable has not been set: {key}")
+            return self._vm._globals[key]
+        else:
+            if key not in self._set:
+                raise RuntimeError(f"Global variable has not been set: {key}")
+            return self._set[key]
+
+    def delete(self, key, global_var: bool = False):
+        if global_var:
+            del self._vm._globals[key]
+        else:
+            del self._set[key]
 
     @staticmethod
     def op(name) -> Union[dict, Callable]:
         return _static_ops[name]
 
-    def set_global(self, key: str, value: Any):
-        self._vm._globals[key] = value
-
-    def has_global(self, key) -> bool:
-        return key in self._vm._globals
-
-    def get_global(self, key: str) -> Any:
-        if key not in self._vm._globals:
-            raise RuntimeError(f"Global variable has not been set: {key}")
-        return self._vm._globals[key]
-
-    def delete_global(self, key):
-        del self._vm._globals[key]
-
 
 def calc_depth(state: State) -> int:
     depth = 0
     frame = state._op_frame
     parent = frame._parent
     while parent is not None:
         parent = parent._parent
@@ -248,16 +248,15 @@
             for i, check in enumerate(test["checks"]):
                 if "answer" in check:
                     assert vm.stack == check['answer'], f"check {i} of test '{test_name}' failed"
                     checks_passed += 1
     return checks_passed
 
 
-def op(name):
-    # todo: add hints for pop order + type
+def method(name):
     global _static_ops
     def inner(func: Callable):
         global _static_ops
         if func.__code__.co_argcount != 1:
             raise RuntimeError("function must take exactly one position argument (state: cvm.State)")
         _static_ops[name] = func
         return func
```

### Comparing `collagen-0.1.4/mkdocstrings_handlers/collagen/handler.py` & `collagen-0.2.0/mkdocstrings_handlers/collagen/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,92 +5,92 @@
 
 import urllib.parse
 import importlib
 import collagen.vm
 import re
 
 
-def add_hyperlinks_to_descriptions(hints):
-    if 'description' in hints and 'references' in hints:
-        for i, ref in enumerate(hints['references']):
+def add_hyperlinks_to_descriptions(metadata):
+    if 'description' in metadata and 'references' in metadata:
+        for i, ref in enumerate(metadata['references']):
             if 'url' not in ref:
                 continue
-            hints['description'] = hints['description'].replace(f"[{i+1}]", f'<a href="{ref["url"]}" target="_blank">[{i+1}]</a>')
-    return hints
+            metadata['description'] = metadata['description'].replace(f"[{i+1}]", f'<a href="{ref["url"]}" target="_blank">[{i+1}]</a>')
+    return metadata
 
 
-def parse_docstring(docstring: str, hints: dict = None) -> dict:
-    if hints is None:
-        hints = {}
+def parse_docstring(docstring: str, metadata: dict = None) -> dict:
+    if metadata is None:
+        metadata = {}
 
     def _docstring_description_regex(headers: list):
         return rf"\A(?P<base>[\s\S]+?)(?:\n\n|\Z)(?:{'|'.join(headers)})?"
 
     def _docstring_section_regex(header: str, name: str):
         return rf"(?:^{header}[ \t]*\n-{{{len(header)}}}[ \t]*\n(?P<{name}>[\s\S]*?)(?:\n\n|\Z))"
 
     def _docstrings_parse_args(text: str, optional_key: str):
         pattern = r"(?P<name>^\S[^:\n]*)(?P<type>:[^\(\n]*)?(?P<default>\(default:[ \t]*[^\)]*\))?[ \t]*(?P<description>(?:\n[  \t]+[\S \t]+)+)?"
-        hints = []
+        metadata = []
         for match in re.findall(pattern, text, re.MULTILINE):
             arg = {}
             name = match[0]
             optional = bool(re.match(r"^\[\S+\]", name))
             arg['name'] = name.strip(" []")
             arg['type'] = match[1].strip(" :")
             arg['default'] = match[2].removeprefix("(default:").removesuffix(")").strip()
             arg['description'] = match[3].strip()
             arg[optional_key] = optional or arg['default'] != ''
             arg = {k: v for k, v in arg.items() if v != ''}
-            hints.append(arg)
-        return hints
+            metadata.append(arg)
+        return metadata
 
     def _docstring_reference():
         return r"^\d+\.[ \t]*((?:(?:\n[ \t]+)?[^\n\(]+)+)(\([^\)]+\))?(?!\d)"
 
     SECTIONS = ['Inputs', 'Parameters', 'Outputs', 'References']
     if matches := re.match(_docstring_description_regex(SECTIONS), docstring):
-        hints['description'] = matches.group(1)
+        metadata['description'] = matches.group(1)
 
     if matches := re.search(_docstring_section_regex('Inputs', 'inputs'), docstring, re.MULTILINE):
         text = matches.group('inputs')
         inputs = _docstrings_parse_args(text, 'conditional')
         if inputs:
-            hints['inputs'] = inputs
+            metadata['inputs'] = inputs
 
     if matches := re.search(_docstring_section_regex('Parameters', 'params'), docstring, re.MULTILINE):
         text = matches.group('params')
         params = _docstrings_parse_args(text, 'optional')
         params_dict = {}
         for param in params:
             params_dict[param.pop("name")] = param
-        if 'parameters' not in hints:
-            hints['parameters'] = {}
-        hints['parameters'].update(params_dict)
+        if 'parameters' not in metadata:
+            metadata['parameters'] = {}
+        metadata['parameters'].update(params_dict)
 
     if matches := re.search(_docstring_section_regex('Outputs', 'outputs'), docstring, re.MULTILINE):
         text = matches.group('outputs')
         outputs = _docstrings_parse_args(text, 'conditional')
         if outputs:
-            hints['outputs'] = outputs
+            metadata['outputs'] = outputs
 
     if matches := re.search(_docstring_section_regex('References', 'references'), docstring, re.MULTILINE):
         text = matches.group('references')
         references = re.findall(_docstring_reference(), text, re.MULTILINE)
         refs = []
         for ref in references:
             ref = {
                 'text': ref[0].strip(),
                 'url': ref[1].strip(" \t()")
             }
             ref = {k: v for k, v in ref.items() if v != ''}
             refs.append(ref)
         if len(refs):
-            hints['references'] = refs
-    return hints
+            metadata['references'] = refs
+    return metadata
 
 
 class CollagenHandler(BaseHandler):
     def __init__(self, *args, **kwargs) -> None:
         self.fallback_theme = 'terminal'
         super().__init__(*args, **kwargs)
 
@@ -102,31 +102,31 @@
             importlib.import_module(module)
         vm = collagen.vm.VirtualMachine()
         for routine, url in includes.items():
             vm._include(routine, url)
 
         docs: dict = {
             'op_names': [],
-            'op_hints': []
+            'op_metadata': []
         }
         for op_name in config.get('ops', []):
             op = collagen.vm._static_ops[op_name]
             if callable(op):
                 docstring = inspect.getdoc(op)
-                hints = parse_docstring(docstring)
+                metadata = parse_docstring(docstring)
             else:
-                hints: dict = op.get('hints', {})
-            hints = add_hyperlinks_to_descriptions(hints)
+                metadata: dict = op.get('metadata', {})
+            metadata = add_hyperlinks_to_descriptions(metadata)
             docs['op_names'].append(op_name)
-            docs['op_hints'].append(hints)
+            docs['op_metadata'].append(metadata)
 
         docs['extdata_op'] = []
         docs['extdata_scheme'] = []
         docs['extdata_media_type'] = []
-        docs['extdata_hints'] = []
+        docs['extdata_metadata'] = []
         for data_spec in config.get("data", []):
             if ":" in data_spec:
                 scheme, media_type = data_spec.split(":")
             else:
                 scheme = data_spec
                 media_type = None
 
@@ -134,64 +134,64 @@
             putter = collagen.vm._static_putters.get(scheme, {}).get(media_type, None)
             deleter = collagen.vm._static_deleters.get(scheme, {}).get(media_type, None)
 
             if getter is not None:
                 docs['extdata_op'].append("get")
                 docs['extdata_scheme'].append(scheme)
                 docs['extdata_media_type'].append(media_type)
-                hints = {
+                metadata = {
                     'outputs': [
                         {'name': 'data', 'description': 'The loaded resource', 'conditional': False}
                     ],
                     'parameters': {
                         'uri': {
                             'type': 'str',
                             'description': 'The URI of the resource to load',
                             'optional': False,
                         }
                     }
                 }
                 getter = inspect.getdoc(getter)
-                hints = parse_docstring(getter, hints)
-                docs['extdata_hints'].append(hints)
+                metadata = parse_docstring(getter, metadata)
+                docs['extdata_metadata'].append(metadata)
             if putter is not None:
                 docs['extdata_op'].append("put")
                 docs['extdata_scheme'].append(scheme)
                 docs['extdata_media_type'].append(media_type)
-                hints = {
+                metadata = {
                     'inputs': [
                         {'name': 'data', 'description': 'The resource to save', 'conditional': False}
                     ],
                     'parameters': {
                         'uri': {
                             'type': 'str',
                             'description': 'The URI of where the resource should be saved',
                             'optional': False,
                         }
                     }
                 }
                 putter = inspect.getdoc(putter)
-                hints = parse_docstring(putter, hints)
-                docs['extdata_hints'].append(hints)
+                metadata = parse_docstring(putter, metadata)
+                docs['extdata_metadata'].append(metadata)
             if deleter is not None:
                 docs['extdata_op'].append("del")
                 docs['extdata_scheme'].append(scheme)
                 docs['extdata_media_type'].append(media_type)
-                hints = {
+                metadata = {
                     'parameters': {
                         'uri': {
                             'type': 'str',
                             'description': 'The URI of the resource to delete',
                             'optional': False,
                         }
                     }
                 }
                 deleter = inspect.getdoc(deleter)
-                hints = parse_docstring(deleter, hints)
-                docs['extdata_hints'].append(hints)
+                metadata = parse_docstring(deleter, metadata)
+                docs['extdata_metadata'].append(metadata)
 
         return docs
 
     def render(self, data: CollectorItem, config: Mapping[str, Any]) -> str:
         self.env.filters['zip'] = zip
         template = self.env.get_template("ops.html")
         return template.render(**data)
```

### Comparing `collagen-0.1.4/mkdocstrings_handlers/collagen/templates/terminal/hints.html` & `collagen-0.2.0/mkdocstrings_handlers/collagen/templates/terminal/metadata.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-    {%- if hints.description -%}
-    <p>{{ hints.description|safe }}</p>
+    {%- if metadata.description -%}
+    <p>{{ metadata.description|safe }}</p>
     {%- endif -%}
 
-    {%- if hints.parameters -%}
+    {%- if metadata.parameters -%}
     <div>
         <h2 style="margin-bottom: 0.2em;">Parameters</h2>
-        {%- for param_name, param_hints in hints.parameters.items() if param_hints.optional == false  -%}
+        {%- for param_name, param_metadata in metadata.parameters.items() if param_metadata.optional == false  -%}
         <span style="float:left">
             {{ param_name }}*
-            {%- if 'type' in param_hints -%}
-            : <i>{{ param_hints.type }}</i>
+            {%- if 'type' in param_metadata -%}
+            : <i>{{ param_metadata.type }}</i>
             {%- endif -%}
         </span>
         <span style="float: right">(*required)</span>
         <br/>
-        {%- if 'description' in param_hints -%}
+        {%- if 'description' in param_metadata -%}
         <p style='margin-left:2em'>
-            {{ param_hints.description }}
+            {{ param_metadata.description }}
         </p>
         {%- endif -%}
         {%- endfor -%}
 
-        {%- for param_name, param_hints in hints.parameters.items() if (param_hints.optional == true) or (param_hints.optional is undefined) -%}
+        {%- for param_name, param_metadata in metadata.parameters.items() if (param_metadata.optional == true) or (param_metadata.optional is undefined) -%}
         <span style="float: left">
             {{ param_name }}
-            {%- if 'type' in param_hints -%}
-            : <i>{{ param_hints.type }}</i>
+            {%- if 'type' in param_metadata -%}
+            : <i>{{ param_metadata.type }}</i>
             {%- endif -%}
         </span>
-        {%- if 'default' in param_hints -%}
-        <span style="float: right">(default: {{ param_hints.default }})</span>
+        {%- if 'default' in param_metadata -%}
+        <span style="float: right">(default: {{ param_metadata.default }})</span>
         {%- endif -%}
         <br/>
-        {%- if 'description' in param_hints -%}
+        {%- if 'description' in param_metadata -%}
         <p style='margin-left:2em'>
-            {{ param_hints.description }}
+            {{ param_metadata.description }}
         </p>
         {%- endif -%}
         {%- endfor -%}
 
     </div>
     {%- endif -%}
 
-    {%- if hints.inputs -%}
+    {%- if metadata.inputs -%}
     <div>
         <h2 style="margin-bottom: 0.2em;">Inputs</h2>
-        {% for input in hints.inputs %}
+        {% for input in metadata.inputs %}
         <span style="float:left">
             {%- if input.conditional -%}
             [{{ input.name }}]
             {%- else -%}
             {{ input.name }}
             {%- endif -%}
             {%- if 'type' in input -%}
@@ -62,18 +62,18 @@
             {{ input.description }}
         </p>
         {%- endif -%}
         {%- endfor -%}
     </div>
     {%- endif -%}
 
-    {%- if hints.outputs -%}
+    {%- if metadata.outputs -%}
     <div>
         <h2 style="margin-bottom: 0.2em;">Outputs</h2>
-        {% for output in hints.outputs %}
+        {% for output in metadata.outputs %}
         <span style="float:left">
             {%- if output.conditional -%}
             [{{ output.name }}]
             {%- else -%}
             {{ output.name }}
             {%- endif -%}
             {%- if 'type' in output -%}
@@ -85,17 +85,17 @@
             {{ output.description }}
         </p>
         {%- endif -%}
         {%- endfor -%}
     </div>
     {%- endif -%}
 
-    {%- if hints.references -%}
+    {%- if metadata.references -%}
     <p><strong>References</strong><br>
-        {% for reference in hints.references %}
+        {% for reference in metadata.references %}
         <span>[{{ loop.index }}]</span>
         <span style="margin-left: 1em">
             {%- if reference is string -%}
             {{ reference }}
             {%- else -%}
             <a href="{{ reference.url }}">{{ reference.text }}</a>
             {%- endif -%}
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
- {%- if hints.description -%}
-{{ hints.description|safe }}
-{%- endif -%} {%- if hints.parameters -%}
+ {%- if metadata.description -%}
+{{ metadata.description|safe }}
+{%- endif -%} {%- if metadata.parameters -%}
 ***** Parameters *****
-{%- for param_name, param_hints in hints.parameters.items() if
-param_hints.optional == false -%}  {{ param_name }}* {%- if 'type' in
-param_hints -%} : {{ param_hints.type }} {%- endif -%}  (*required)
-{%- if 'description' in param_hints -%}
-{{ param_hints.description }}
-{%- endif -%} {%- endfor -%} {%- for param_name, param_hints in
-hints.parameters.items() if (param_hints.optional == true) or
-(param_hints.optional is undefined) -%}  {{ param_name }} {%- if 'type' in
-param_hints -%} : {{ param_hints.type }} {%- endif -%}  {%- if 'default' in
-param_hints -%} (default: {{ param_hints.default }}) {%- endif -%}
-{%- if 'description' in param_hints -%}
-{{ param_hints.description }}
+{%- for param_name, param_metadata in metadata.parameters.items() if
+param_metadata.optional == false -%}  {{ param_name }}* {%- if 'type' in
+param_metadata -%} : {{ param_metadata.type }} {%- endif -%}  (*required)
+{%- if 'description' in param_metadata -%}
+{{ param_metadata.description }}
+{%- endif -%} {%- endfor -%} {%- for param_name, param_metadata in
+metadata.parameters.items() if (param_metadata.optional == true) or
+(param_metadata.optional is undefined) -%}  {{ param_name }} {%- if 'type' in
+param_metadata -%} : {{ param_metadata.type }} {%- endif -%}  {%- if 'default'
+in param_metadata -%} (default: {{ param_metadata.default }}) {%- endif -%}
+{%- if 'description' in param_metadata -%}
+{{ param_metadata.description }}
 {%- endif -%} {%- endfor -%}
-{%- endif -%} {%- if hints.inputs -%}
+{%- endif -%} {%- if metadata.inputs -%}
 ***** Inputs *****
-{% for input in hints.inputs %}  {%- if input.conditional -%} [{{ input.name
+{% for input in metadata.inputs %}  {%- if input.conditional -%} [{{ input.name
 }}] {%- else -%} {{ input.name }} {%- endif -%} {%- if 'type' in input -%} : {
 { input.type }} {%- endif -%}
 {%- if input.description -%}
 {{ input.description }}
 {%- endif -%} {%- endfor -%}
-{%- endif -%} {%- if hints.outputs -%}
+{%- endif -%} {%- if metadata.outputs -%}
 ***** Outputs *****
-{% for output in hints.outputs %}  {%- if output.conditional -%} [{
+{% for output in metadata.outputs %}  {%- if output.conditional -%} [{
 { output.name }}] {%- else -%} {{ output.name }} {%- endif -%} {%- if 'type' in
 output -%} : {{ output.type }} {%- endif -%}
 {%- if output.description -%}
 {{ output.description }}
 {%- endif -%} {%- endfor -%}
-{%- endif -%} {%- if hints.references -%}
+{%- endif -%} {%- if metadata.references -%}
 References
-{% for reference in hints.references %} [{{ loop.index }}]  {%- if reference is
-string -%} {{ reference }} {%- else -%} {{_reference.text_}} {%- endif -%}
+{% for reference in metadata.references %} [{{ loop.index }}]  {%- if reference
+is string -%} {{ reference }} {%- else -%} {{_reference.text_}} {%- endif -%}
 {% endfor %}
 {%- endif -%}
```

### Comparing `collagen-0.1.4/mkdocstrings_handlers/collagen/templates/terminal/ops.html` & `collagen-0.2.0/mkdocstrings_handlers/collagen/templates/terminal/ops.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-{%- for op, hints in op_names|zip(op_hints) -%}
+{%- for op, metadata in op_names|zip(op_metadata) -%}
 <details>
-    <summary><code class="collagen-op-preview language-json">{ "op": "{{  op  }}"{{ ', ...' if hints.parameters|length != 0}} }</code></summary>
+    <summary><code class="collagen-op-preview language-json">{ "op": "{{  op  }}"{{ ', ...' if metadata.parameters|length != 0}} }</code></summary>
     <div style="padding: 1em;">
-        {% include 'hints.html' %}
+        {% include 'metadata.html' %}
     </div>
 </details>
 {%- endfor -%}
 
-{%- for op, hints, scheme, media_type in extdata_op|zip(extdata_hints,extdata_scheme,extdata_media_type) -%}
+{%- for op, metadata, scheme, media_type in extdata_op|zip(extdata_metadata,extdata_scheme,extdata_media_type) -%}
 <details>
     <summary><code class="collagen-op-preview language-json">{ "op": "{{  op  }}",
         {{'"media_type": "' + media_type + '",' if media_type}}
         "uri": "{{ scheme }}://..."
-        {{ ', ...' if hints.parameters|length > 1}}
+        {{ ', ...' if metadata.parameters|length > 1}}
     }</code></summary>
     <div style="padding: 1em;">
-        {% include 'hints.html' %}
+        {% include 'metadata.html' %}
     </div>
 </details>
 {%- endfor -%}
```

### Comparing `collagen-0.1.4/setup.cfg` & `collagen-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [metadata]
 name = collagen
 description = A virtual stack machine that executes Python code based on instructions provided in a JSON file.
-url = https://github.com/ieg-tech/collagen.git
+url = https://github.com/LiamBindle/collagen.git
 license = 
 install_requires = 
 	versioneer
 
 [options]
 packages = 
 	collagen
+	collagen.standard
+	collagen.standard.resources
 	mkdocstrings_handlers.collagen
 include_package_data = True
 
 [options.extras_require]
-develop = 
+dev = 
 	flake8
 	pytest
 docs = 
 	mkdocs
 	mkdocstrings[python]
 	mkdocs-terminal
 	pytkdocs[numpy-style]>=0.5.0
```

### Comparing `collagen-0.1.4/tests/test_zvm.py` & `collagen-0.2.0/tests/test_zvm.py`

 * *Files identical despite different names*

### Comparing `collagen-0.1.4/versioneer.py` & `collagen-0.2.0/versioneer.py`

 * *Files identical despite different names*

