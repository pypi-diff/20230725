# Comparing `tmp/adt-decorators-0.1.1.tar.gz` & `tmp/adt-decorators-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.1.1.tar", last modified: Mon Jul 24 11:02:22 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.0.tar", last modified: Mon Jul 24 22:21:10 2023, max compression
```

## Comparing `adt-decorators-0.1.1.tar` & `adt-decorators-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.1.1/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.1.1/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     3514 2023-07-24 10:37:54.000000 adt-decorators-0.1.1/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4591 2023-07-24 11:01:15.000000 adt-decorators-0.1.1/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     3514 2023-07-24 10:37:54.000000 adt-decorators-0.1.1/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.1.1/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.1.1/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 11:01:08.000000 adt-decorators-0.1.1/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.0/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.0/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5490 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5066 2023-07-24 22:19:44.000000 adt-decorators-0.2.0/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.650898 adt-decorators-0.2.0/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 22:20:39.000000 adt-decorators-0.2.0/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5490 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5066 2023-07-24 22:19:44.000000 adt-decorators-0.2.0/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.0/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.0/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 22:20:52.000000 adt-decorators-0.2.0/setup.py
```

### Comparing `adt-decorators-0.1.1/LICENSE` & `adt-decorators-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.1.1/adt/__init__.py` & `adt-decorators-0.2.0/adt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
-def adt(Base):
-    """Class-decorator for Algebraic Data Types (ADTs), which defines the constructors as static fields of the base type.
+def adt(Class=None, export=False):
+    """Class-decorator for Algebraic Data Types (ADTs).
+
+    This function is overloaded to allow both `@adt` and
+    `@adt(OPTIONS)` annotations. In the case of `@adt` only the
+    `Class` argument is supplied and the decorator is *called*;
+     in the case of `@adt(export=True)` only the other arguments are
+     supplied and the decorator is *returned*.
+
+    Arguments:
+        export:
+            if `False`, only define the constructor classes as fields of the decorated class;
+            if `True`, also define the constructor classes in the global namespace.
 
     Examples:
         >>> @adt
         ... class Expr:
         ...     Var: str                           # Single Unnamed Con Arg
         ...     Abs: [str, 'Expr']                 # Multiple Unnamed Con Args
         ...     App: {'e1': 'Expr', 'e2': 'Expr'}  # Multiple Named Con Args
@@ -21,37 +32,32 @@
         ...         match self:
         ...             case Expr.Var(x):      return x
         ...             case Expr.Abs(x, e):   return f"(λ{x}. {e})"
         ...             case Expr.App(e1, e2): return f"({e1} {e2})"
         >>> id_expr = Expr.Abs("x", Expr.Var("x"))
         >>> str(id_expr)
         '(λx. x)'
-    """
-    return adt_with(export_cons=False)(Base)
 
-def adt_export(Base):
-    """Class-decorator for Algebraic Data Types (ADTs), which defines the Constructors as static fields of the base type and on the top-level.
-
-    Examples:
-        >>> @adt_export
+        >>> @adt(export=True)
         ... class Expr:
         ...     Var: str                           # Single Unnamed Con Arg
         ...     Abs: [str, 'Expr']                 # Multiple Unnamed Con Args
         ...     App: {'e1': 'Expr', 'e2': 'Expr'}  # Multiple Named Con Args
         ... 
         ...     def __str__(self) -> str:
         ...         match self:
         ...             case Var(x):      return x
         ...             case Abs(x, e):   return f"(λ{x}. {e})"
         ...             case App(e1, e2): return f"({e1} {e2})"
         >>> id_expr = Abs("x", Var("x"))
         >>> str(id_expr)
         '(λx. x)'
     """
-    return adt_with(export_cons=True)(Base)
+    decorator = adt_with(export)
+    return decorator if Class is None else decorator(Class)
 
 def adt_with(export_cons: bool):
     def decorator(Base):
         annotations = vars(Base)["__annotations__"]
         Base.__annotations__ = dict()
 
         def Base_init(self, *args, **kwargs):
```

### Comparing `adt-decorators-0.1.1/setup.py` & `adt-decorators-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('docs/overview.md', 'r') as f:
     desc = f.read()
 
 setup(
     name='adt-decorators',
-    version='0.1.1',    
+    version='0.2.0',    
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

