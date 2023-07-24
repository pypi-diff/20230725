# Comparing `tmp/sympytorch-0.1.3.tar.gz` & `tmp/sympytorch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympytorch-0.1.3.tar", last modified: Mon May 29 18:55:02 2023, max compression
+gzip compressed data, was "sympytorch-0.1.4.tar", last modified: Mon Jul 24 22:55:54 2023, max compression
```

## Comparing `sympytorch-0.1.3.tar` & `sympytorch-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.025046 sympytorch-0.1.3/
--rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-16 17:42:44.000000 sympytorch-0.1.3/LICENSE
--rw-r--r--   0 kidger    (1000) kidger    (1000)       28 2023-04-16 17:42:44.000000 sympytorch-0.1.3/MANIFEST.in
--rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-05-29 18:55:02.025046 sympytorch-0.1.3/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2223 2023-04-16 17:42:44.000000 sympytorch-0.1.3/README.md
--rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-05-29 18:55:02.025046 sympytorch-0.1.3/setup.cfg
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2136 2023-04-16 17:42:44.000000 sympytorch-0.1.3/setup.py
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.024047 sympytorch-0.1.3/sympytorch/
--rw-r--r--   0 kidger    (1000) kidger    (1000)      100 2023-05-29 18:54:33.000000 sympytorch-0.1.3/sympytorch/__init__.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)      851 2023-04-16 17:42:44.000000 sympytorch-0.1.3/sympytorch/hide_floats_m.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)     6867 2023-05-29 18:54:10.000000 sympytorch-0.1.3/sympytorch/sympy_module.py
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.025046 sympytorch-0.1.3/sympytorch.egg-info/
--rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)      318 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/SOURCES.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/dependency_links.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:43:02.000000 sympytorch-0.1.3/sympytorch.egg-info/not-zip-safe
--rw-r--r--   0 kidger    (1000) kidger    (1000)       26 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/requires.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)       11 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/top_level.txt
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-07-24 22:55:54.323727 sympytorch-0.1.4/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-16 17:42:44.000000 sympytorch-0.1.4/LICENSE
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       28 2023-04-16 17:42:44.000000 sympytorch-0.1.4/MANIFEST.in
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-07-24 22:55:54.323727 sympytorch-0.1.4/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     2223 2023-04-16 17:42:44.000000 sympytorch-0.1.4/README.md
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-07-24 22:55:54.323727 sympytorch-0.1.4/setup.cfg
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     1888 2023-07-24 22:53:38.000000 sympytorch-0.1.4/setup.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-07-24 22:55:54.321728 sympytorch-0.1.4/sympytorch/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      131 2023-07-24 22:53:52.000000 sympytorch-0.1.4/sympytorch/__init__.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     1114 2023-07-24 22:53:32.000000 sympytorch-0.1.4/sympytorch/hide_floats_m.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        0 2023-07-24 22:42:16.000000 sympytorch-0.1.4/sympytorch/py.typed
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     8958 2023-07-24 22:54:56.000000 sympytorch-0.1.4/sympytorch/sympy_module.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-07-24 22:55:54.323727 sympytorch-0.1.4/sympytorch.egg-info/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-07-24 22:55:54.000000 sympytorch-0.1.4/sympytorch.egg-info/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      338 2023-07-24 22:55:54.000000 sympytorch-0.1.4/sympytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-07-24 22:55:54.000000 sympytorch-0.1.4/sympytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:43:02.000000 sympytorch-0.1.4/sympytorch.egg-info/not-zip-safe
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       26 2023-07-24 22:55:54.000000 sympytorch-0.1.4/sympytorch.egg-info/requires.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       11 2023-07-24 22:55:54.000000 sympytorch-0.1.4/sympytorch.egg-info/top_level.txt
```

### Comparing `sympytorch-0.1.3/LICENSE` & `sympytorch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.3/PKG-INFO` & `sympytorch-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.3
+Version: 0.1.4
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```

### Comparing `sympytorch-0.1.3/README.md` & `sympytorch-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.3/setup.py` & `sympytorch-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 import pathlib
 import re
+
 import setuptools
 
+
 _here = pathlib.Path(__file__).resolve().parent
 
 
-name = 'sympytorch'
+name = "sympytorch"
 
-# for simplicity we actually store the version in the __version__ attribute in the source
-with open(_here / name / '__init__.py') as f:
+# for simplicity we actually store the version in the __version__ attribute in the
+# source
+with open(_here / name / "__init__.py") as f:
     meta_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", f.read(), re.M)
     if meta_match:
         version = meta_match.group(1)
     else:
         raise RuntimeError("Unable to find __version__ string.")
 
-author = 'Patrick Kidger'
+author = "Patrick Kidger"
 
-author_email = 'contact@kidger.site'
+author_email = "contact@kidger.site"
 
 description = "Turning SymPy expressions into PyTorch modules."
 
-with open(_here / 'README.md', 'r') as f:
+with open(_here / "README.md", "r") as f:
     readme = f.read()
 
 url = "https://github.com/patrick-kidger/sympytorch"
 
 license = "Apache-2.0"
 
-classifiers = ["Development Status :: 3 - Alpha",
-               "Intended Audience :: Developers",
-               "Intended Audience :: Financial and Insurance Industry",
-               "Intended Audience :: Information Technology",
-               "Intended Audience :: Science/Research",
-               "License :: OSI Approved :: Apache Software License",
-               "Natural Language :: English",
-               "Programming Language :: Python :: 3",
-               "Topic :: Scientific/Engineering :: Artificial Intelligence",
-               "Topic :: Scientific/Engineering :: Information Analysis",
-               "Topic :: Scientific/Engineering :: Mathematics"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Financial and Insurance Industry",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: Apache Software License",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Scientific/Engineering :: Mathematics",
+]
 
 python_requires = "~=3.7"
 
-install_requires = ['torch>=1.6.0', 'sympy>=1.7.1']
+install_requires = ["torch>=1.6.0", "sympy>=1.7.1"]
 
-setuptools.setup(name=name,
-                 version=version,
-                 author=author,
-                 author_email=author_email,
-                 maintainer=author,
-                 maintainer_email=author_email,
-                 description=description,
-                 long_description=readme,
-                 long_description_content_type='text/markdown',
-                 url=url,
-                 license=license,
-                 classifiers=classifiers,
-                 zip_safe=False,
-                 python_requires=python_requires,
-                 install_requires=install_requires,
-                 packages=[name])
+setuptools.setup(
+    name=name,
+    version=version,
+    author=author,
+    author_email=author_email,
+    maintainer=author,
+    maintainer_email=author_email,
+    description=description,
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url=url,
+    license=license,
+    classifiers=classifiers,
+    zip_safe=False,
+    python_requires=python_requires,
+    install_requires=install_requires,
+    packages=[name],
+    package_data={name: ["py.typed"]},
+)
```

### Comparing `sympytorch-0.1.3/sympytorch/hide_floats_m.py` & `sympytorch-0.1.4/sympytorch/hide_floats_m.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,38 @@
+from typing import Dict, TypeVar
+
 import sympy
 
 
-def hide_floats(expression):
-    _memodict = {}
+ExprType = TypeVar("ExprType", bound=sympy.Expr)
+
+
+def hide_floats(expression: ExprType) -> ExprType:
+    _memodict: Dict[ExprType, ExprType] = {}
     return _hide_floats(expression, _memodict)
 
 
-def _hide_floats(expression, _memodict):
+def _hide_floats(expression: ExprType, _memodict: Dict[ExprType, ExprType]) -> ExprType:
     try:
         return _memodict[expression]
     except KeyError:
         pass
 
     if issubclass(expression.func, (sympy.Min, sympy.Max)):
         evaluate = False
     else:
         evaluate = True
 
+    new_expression: ExprType
     if issubclass(expression.func, sympy.Float):
-        new_expression = sympy.UnevaluatedExpr(expression)
+        new_expression = sympy.UnevaluatedExpr(expression)  # type: ignore
     elif issubclass(expression.func, sympy.Integer):
         new_expression = expression
     elif issubclass(expression.func, sympy.Symbol):
         new_expression = expression
     else:
         new_expression = expression.func(
-            *[_hide_floats(arg, _memodict) for arg in expression.args], evaluate=evaluate)
+            *[_hide_floats(arg, _memodict) for arg in expression.args],
+            evaluate=evaluate
+        )  # type: ignore
     _memodict[expression] = new_expression
     return new_expression
```

### Comparing `sympytorch-0.1.3/sympytorch/sympy_module.py` & `sympytorch-0.1.4/sympytorch/sympy_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,54 @@
+from __future__ import annotations
+
 import collections as co
 import functools as ft
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Sequence,
+    Tuple,
+    Type,
+    TYPE_CHECKING,
+    TypeVar,
+    Union,
+)
+
 import sympy
 import torch
 
 
-def _reduce(fn):
-    def fn_(*args):
+ExprType = TypeVar("ExprType", bound=sympy.Expr)
+T = TypeVar("T")
+
+if TYPE_CHECKING:
+    # Because there are methods of our class objects below called `sympy` that
+    # implicitly override the `sympy` name in the global namespace while defining other
+    # methods, our type checker needs to know that we're referring to the sympy module
+    # in our type annotations.
+    import sympy as sympy_
+
+
+def _reduce(fn: Callable[..., T]) -> Callable[..., T]:
+    def fn_(*args: Any) -> T:
         return ft.reduce(fn, args)
+
     return fn_
 
-def _I(*args):
+
+def _I(*args: Any) -> torch.Tensor:
     return torch.tensor(1j)
 
-_global_func_lookup = {
+
+_global_func_lookup: Dict[
+    Union[Type[sympy.Basic], Callable[..., Any]], Callable[..., torch.Tensor]
+] = {
     sympy.Mul: _reduce(torch.mul),
     sympy.Add: _reduce(torch.add),
     sympy.div: torch.div,
     sympy.Abs: torch.abs,
     sympy.sign: torch.sign,
     # Note: May raise error for ints.
     sympy.ceiling: torch.ceil,
@@ -60,102 +92,141 @@
     sympy.MatAdd: torch.add,
     sympy.HadamardProduct: torch.mul,
     sympy.Trace: torch.trace,
     # Note: May raise error for integer matrices.
     sympy.Determinant: torch.det,
     sympy.core.numbers.ImaginaryUnit: _I,
     sympy.conjugate: torch.conj,
-
 }
 
 number_symbols = [cls for cls in sympy.NumberSymbol.__subclasses__()]
 
-def number_symbol_to_torch(symbol, *args):
+
+def number_symbol_to_torch(symbol: sympy.NumberSymbol, *args: Any) -> torch.Tensor:
     return torch.tensor(float(symbol))
 
-_global_func_lookup.update({s: ft.partial(number_symbol_to_torch, s()) for s in number_symbols})
 
+_global_func_lookup.update(
+    {s: ft.partial(number_symbol_to_torch, s()) for s in number_symbols}
+)
 
-class _Node(torch.nn.Module):
-    def __init__(self, *, expr, _memodict, _func_lookup, **kwargs):
+
+class _Node(torch.nn.Module, Generic[ExprType]):
+    def __init__(
+        self,
+        *,
+        expr: ExprType,
+        _memodict: Dict[sympy.Basic, torch.nn.Module],
+        _func_lookup,
+        **kwargs,
+    ) -> None:
         super().__init__(**kwargs)
 
-        self._sympy_func = expr.func
+        self._sympy_func: Type[ExprType] = expr.func
+
+        self._torch_func: Callable[..., torch.Tensor]
+        self._args: Union[
+            torch.nn.ModuleList,
+            Tuple[Callable[[Dict[str, torch.Tensor]], torch.Tensor], ...],
+        ]
+        self._value: Any
 
         if issubclass(expr.func, sympy.Float):
             self._value = torch.nn.Parameter(torch.tensor(float(expr)))
             self._torch_func = lambda: self._value
             self._args = ()
         elif issubclass(expr.func, sympy.Integer):
-            self._value = int(expr)
+            self._value = torch.tensor(int(expr))
             self._torch_func = lambda: self._value
             self._args = ()
         elif issubclass(expr.func, sympy.Rational):
-            self.register_buffer('_numerator', torch.tensor(expr.p, dtype=torch.get_default_dtype()))
-            self.register_buffer('_denominator', torch.tensor(expr.q, dtype=torch.get_default_dtype()))
+            self._numerator: torch.Tensor
+            self._denominator: torch.Tensor
+            assert isinstance(expr, sympy.Rational)
+            self.register_buffer(
+                "_numerator", torch.tensor(expr.p, dtype=torch.get_default_dtype())
+            )
+            self.register_buffer(
+                "_denominator", torch.tensor(expr.q, dtype=torch.get_default_dtype())
+            )
             self._torch_func = lambda: self._numerator / self._denominator
             self._args = ()
         elif issubclass(expr.func, sympy.UnevaluatedExpr):
             if len(expr.args) != 1 or not issubclass(expr.args[0].func, sympy.Float):
                 raise ValueError("UnevaluatedExpr should only be used to wrap floats.")
-            self.register_buffer('_value', torch.tensor(float(expr.args[0])))
+            assert isinstance(expr.args[0], sympy.Float)
+            self.register_buffer("_value", torch.tensor(float(expr.args[0])))
             self._torch_func = lambda: self._value
             self._args = ()
         elif issubclass(expr.func, sympy.Symbol):
+            assert isinstance(expr, sympy.Symbol)
             self._name = expr.name
             self._torch_func = lambda value: value
             self._args = ((lambda memodict: memodict[expr.name]),)
         else:
             self._torch_func = _func_lookup[expr.func]
-            args = []
+            args: List[torch.nn.Module] = []
             for arg in expr.args:
                 try:
                     arg_ = _memodict[arg]
                 except KeyError:
-                    arg_ = type(self)(expr=arg, _memodict=_memodict, _func_lookup=_func_lookup, **kwargs)
+                    arg_ = type(self)(
+                        expr=arg,  # type: ignore
+                        _memodict=_memodict,
+                        _func_lookup=_func_lookup,
+                        **kwargs,
+                    )
                     _memodict[arg] = arg_
                 args.append(arg_)
             self._args = torch.nn.ModuleList(args)
 
-    def sympy(self, _memodict):
+    def sympy(self, _memodict: Dict[_Node, sympy_.Expr]) -> ExprType:
         if issubclass(self._sympy_func, sympy.Float):
+            assert isinstance(self._value, torch.nn.Parameter)
             return self._sympy_func(self._value.item())
         elif issubclass(self._sympy_func, sympy.UnevaluatedExpr):
+            assert isinstance(self._value, torch.Tensor)
             return self._sympy_func(self._value.item())
-        elif issubclass(self._sympy_func, (type(sympy.S.NegativeOne), type(sympy.S.One), type(sympy.S.Zero))):
+        elif issubclass(
+            self._sympy_func,
+            (type(sympy.S.NegativeOne), type(sympy.S.One), type(sympy.S.Zero)),
+        ):
             return self._sympy_func()
         elif issubclass(self._sympy_func, sympy.Integer):
             return self._sympy_func(self._value)
         elif issubclass(self._sympy_func, sympy.Rational):
             if issubclass(self._sympy_func, type(sympy.S.Half)):
                 return sympy.S.Half
             else:
-                return self._sympy_func(self._numerator.item(), self._denominator.item())
+                return self._sympy_func(
+                    self._numerator.item(), self._denominator.item()
+                )
         elif issubclass(self._sympy_func, sympy.Symbol):
             return self._sympy_func(self._name)
         elif issubclass(self._sympy_func, sympy.core.numbers.ImaginaryUnit):
             return sympy.I
         elif issubclass(self._sympy_func, sympy.core.numbers.NumberSymbol):
             return self._sympy_func()
         else:
             if issubclass(self._sympy_func, (sympy.Min, sympy.Max)):
                 evaluate = False
             else:
                 evaluate = True
             args = []
             for arg in self._args:
+                assert isinstance(arg, _Node)
                 try:
                     arg_ = _memodict[arg]
                 except KeyError:
                     arg_ = arg.sympy(_memodict)
                     _memodict[arg] = arg_
                 args.append(arg_)
-            return self._sympy_func(*args, evaluate=evaluate)
+            return self._sympy_func(*args, evaluate=evaluate)  # type: ignore
 
-    def forward(self, memodict):
+    def forward(self, memodict) -> torch.Tensor:
         args = []
         for arg in self._args:
             try:
                 arg_ = memodict[arg]
             except KeyError:
                 arg_ = arg(memodict)
                 memodict[arg] = arg_
@@ -164,30 +235,32 @@
 
 
 class SymPyModule(torch.nn.Module):
     def __init__(self, *, expressions, extra_funcs=None, **kwargs):
         super().__init__(**kwargs)
 
         expressions = tuple(expressions)
-        
+
         if extra_funcs is None:
             extra_funcs = {}
         _func_lookup = co.ChainMap(_global_func_lookup, extra_funcs)
 
         _memodict = {}
-        self._nodes = torch.nn.ModuleList(
-            [_Node(expr=expr, _memodict=_memodict, _func_lookup=_func_lookup) for expr in expressions]
+        self._nodes: Sequence[_Node] = torch.nn.ModuleList(  # type: ignore
+            [
+                _Node(expr=expr, _memodict=_memodict, _func_lookup=_func_lookup)
+                for expr in expressions
+            ]
         )
         self._expressions_string = str(expressions)
 
     def __repr__(self):
         return f"{type(self).__name__}(expressions={self._expressions_string})"
 
-    def sympy(self):
-        _memodict = {}
+    def sympy(self) -> List[sympy.Expr]:
+        _memodict: Dict[_Node, sympy.Expr] = {}
         return [node.sympy(_memodict) for node in self._nodes]
 
-    def forward(self, **symbols):
+    def forward(self, **symbols: Any) -> torch.Tensor:
         out = [node(symbols) for node in self._nodes]
         out = torch.broadcast_tensors(*out)
         return torch.stack(out, dim=-1)
-
```

### Comparing `sympytorch-0.1.3/sympytorch.egg-info/PKG-INFO` & `sympytorch-0.1.4/sympytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.3
+Version: 0.1.4
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```

