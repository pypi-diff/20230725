# Comparing `tmp/sanic-routing-22.8.0.tar.gz` & `tmp/sanic-routing-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-routing-22.8.0.tar", last modified: Wed Aug 17 16:55:55 2022, max compression
+gzip compressed data, was "sanic-routing-23.6.0.tar", last modified: Tue Jul 25 09:36:41 2023, max compression
```

## Comparing `sanic-routing-22.8.0.tar` & `sanic-routing-23.6.0.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:55:55.250745 sanic-routing-22.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8184 2022-08-17 16:55:55.250745 sanic-routing-22.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7547 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:55:55.246745 sanic-routing-22.8.0/sanic_routing/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/group.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)    12520 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/route.py
--rw-r--r--   0 runner    (1001) docker     (121)    22525 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/router.py
--rw-r--r--   0 runner    (1001) docker     (121)    15519 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/sanic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:55:55.250745 sanic-routing-22.8.0/sanic_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8184 2022-08-17 16:55:55.000000 sanic-routing-22.8.0/sanic_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-17 16:55:55.000000 sanic-routing-22.8.0/sanic_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 16:55:55.000000 sanic-routing-22.8.0/sanic_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-17 16:55:55.000000 sanic-routing-22.8.0/sanic_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 16:55:55.250745 sanic-routing-22.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-17 16:55:30.000000 sanic-routing-22.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:36:41.522700 sanic-routing-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-25 09:36:41.522700 sanic-routing-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:36:41.518700 sanic-routing-23.6.0/sanic_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/sanic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:36:41.518700 sanic-routing-23.6.0/sanic_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-25 09:36:41.000000 sanic-routing-23.6.0/sanic_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 09:36:41.000000 sanic-routing-23.6.0/sanic_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:36:41.000000 sanic-routing-23.6.0/sanic_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 09:36:41.000000 sanic-routing-23.6.0/sanic_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:36:41.522700 sanic-routing-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:36:41.518700 sanic-routing-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_builtin_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_custom_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_router_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_routing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-25 09:36:32.000000 sanic-routing-23.6.0/tests/test_unquote.py
```

### Comparing `sanic-routing-22.8.0/LICENSE` & `sanic-routing-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/PKG-INFO` & `sanic-routing-23.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-routing
-Version: 22.8.0
+Version: 23.6.0
 Summary: Core routing component for Sanic
 Home-page: https://github.com/sanic-org/sanic-routing/
 Author: Adam Hopkins
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sanic-routing-22.8.0/README.md` & `sanic-routing-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing/exceptions.py` & `sanic-routing-23.6.0/sanic_routing/exceptions.py`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing/group.py` & `sanic-routing-23.6.0/sanic_routing/group.py`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing/patterns.py` & `sanic-routing-23.6.0/sanic_routing/patterns.py`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing/route.py` & `sanic-routing-23.6.0/sanic_routing/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def __init__(
         self,
         router,
         raw_path: str,
         name: str,
         handler: t.Callable[..., t.Any],
         methods: t.Union[t.Sequence[str], t.FrozenSet[str]],
-        requirements: t.Dict[str, t.Any] = None,
+        requirements: t.Optional[t.Dict[str, t.Any]] = None,
         strict: bool = False,
         unquote: bool = False,
         static: bool = False,
         regex: bool = False,
         overloaded: bool = False,
     ):
         self.router = router
```

### Comparing `sanic-routing-22.8.0/sanic_routing/router.py` & `sanic-routing-23.6.0/sanic_routing/router.py`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing/tree.py` & `sanic-routing-23.6.0/sanic_routing/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import typing as t
 from logging import getLogger
 
 from .group import RouteGroup
 from .line import Line
-from .patterns import REGEX_PARAM_NAME, REGEX_PARAM_NAME_EXT
+from .patterns import REGEX_PARAM_NAME, REGEX_PARAM_NAME_EXT, alpha, ext, slug
 
 logger = getLogger("sanic.root")
 
 
 class Node:
     def __init__(
         self,
         part: str = "",
         root: bool = False,
         parent=None,
         router=None,
         param=None,
+        unquote=False,
     ) -> None:
         self.root = root
         self.part = part
         self.parent = parent
         self.param = param
         self._children: t.Dict[str, "Node"] = {}
         self.children: t.Dict[str, "Node"] = {}
@@ -30,15 +31,15 @@
         self.dynamic = False
         self.first = False
         self.last = False
         self.children_basketed = False
         self.children_param_injected = False
         self.has_deferred = False
         self.equality_check = False
-        self.unquote = False
+        self.unquote = unquote
         self.router = router
 
     def __str__(self) -> str:
         internals = ", ".join(
             f"{prop}={getattr(self, prop)}"
             for prop in ["part", "level", "groups", "dynamic"]
             if getattr(self, prop) or prop in ["level"]
@@ -264,27 +265,32 @@
                 f"{self.param.cast.__name__}(parts[{idx}])",
                 indent + 1,
             ),
             Line("except ValueError:", indent),
             Line("pass", indent + 1),
             Line("else:", indent),
         ]
-        if self.unquote:
+        if self.unquote and self._cast_as_str(self.param.cast):
             lines.append(
                 Line(
                     f"basket['__matches__'][{idx}] = "
                     f"unquote(basket['__matches__'][{idx}])",
                     indent + 1,
                 )
             )
         self.base_indent += 1
 
         location.extend(lines)
 
     @staticmethod
+    def _cast_as_str(cast) -> bool:
+        return_type_hint = t.get_type_hints(cast).get("return")
+        return cast in (str, ext, slug, alpha) or return_type_hint is str
+
+    @staticmethod
     def _inject_method_check(location, indent, group):
         """
         Sometimes we need to check the routing methods inside the generated src
         """
         for i, route in enumerate(group.routes):
             if_stmt = "if" if i == 0 else "elif"
             location.extend(
@@ -432,14 +438,15 @@
     def generate(self, groups: t.Iterable[RouteGroup]) -> None:
         """
         Arrange RouteGroups into hierarchical nodes and arrange them into
         a tree
         """
         for group in groups:
             current = self.root
+            current.unquote = current.unquote or group.unquote
             for level, part in enumerate(group.parts):
                 param = None
                 dynamic = part.startswith("<")
                 if dynamic:
                     if not REGEX_PARAM_NAME.match(
                         part
                     ) and not REGEX_PARAM_NAME_EXT.match(part):
@@ -448,22 +455,22 @@
                     param = group.params[level]
                 if part not in current._children:
                     child = Node(
                         part=part,
                         parent=current,
                         router=self.router,
                         param=param,
+                        unquote=current.unquote,
                     )
                     child.dynamic = dynamic
                     current.add_child(child)
                 current = current._children[part]
                 current.level = level + 1
 
             current.groups.append(group)
-            current.unquote = current.unquote or group.unquote
 
     def display(self) -> None:
         """
         Debug tool to output visual of the tree
         """
         self.root.display()
```

### Comparing `sanic-routing-22.8.0/sanic_routing/utils.py` & `sanic-routing-23.6.0/sanic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `sanic-routing-22.8.0/sanic_routing.egg-info/PKG-INFO` & `sanic-routing-23.6.0/sanic_routing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-routing
-Version: 22.8.0
+Version: 23.6.0
 Summary: Core routing component for Sanic
 Home-page: https://github.com/sanic-org/sanic-routing/
 Author: Adam Hopkins
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sanic-routing-22.8.0/setup.py` & `sanic-routing-23.6.0/setup.py`

 * *Files identical despite different names*

