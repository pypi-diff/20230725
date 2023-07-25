# Comparing `tmp/param-2.0.0a1.tar.gz` & `tmp/param-2.0.0a2.tar.gz`

## Comparing `param-2.0.0a1.tar` & `param-2.0.0a2.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 param-2.0.0a1/numbergen/__init__.py
--rw-r--r--   0        0        0   106742 2020-02-02 00:00:00.000000 param-2.0.0a1/param/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 param-2.0.0a1/param/_utils.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 param-2.0.0a1/param/_version.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 param-2.0.0a1/param/ipython.py
--rw-r--r--   0        0        0   155561 2020-02-02 00:00:00.000000 param-2.0.0a1/param/parameterized.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 param-2.0.0a1/param/serializer.py
--rw-r--r--   0        0        0    30965 2020-02-02 00:00:00.000000 param-2.0.0a1/param/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/__init__.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testbooleanparam.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testbytesparam.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcalendardateparam.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcalendardaterangeparam.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testclassselector.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcolorparameter.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcomparator.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcompositeparams.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testcustomparam.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testdateparam.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testdaterangeparam.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testdefaults.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testdynamicparams.py
--rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testfiledeserialization.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testfileselector.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testipythonmagic.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testjsonserialization.py
--rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testlist.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testlistselector.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testmultifileselector.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testnumbergen.py
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testnumberparameter.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testnumpy.py
--rw-r--r--   0        0        0    17853 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testobjectselector.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testpandas.py
--rw-r--r--   0        0        0    28420 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testparamdepends.py
--rw-r--r--   0        0        0    28841 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testparameterizedobject.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testparameterizedrepr.py
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testparamoutput.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testparamunion.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testpathparam.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testrangeparameter.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testselector.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testsignatures.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/teststringparam.py
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testtimedependent.py
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testtupleparam.py
--rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testutils.py
--rw-r--r--   0        0        0    26268 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/testwatch.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 param-2.0.0a1/tests/utils.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 param-2.0.0a1/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 param-2.0.0a1/LICENSE.txt
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 param-2.0.0a1/README.md
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 param-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 param-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 param-2.0.0a2/numbergen/__init__.py
+-rw-r--r--   0        0        0   106697 2020-02-02 00:00:00.000000 param-2.0.0a2/param/__init__.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 param-2.0.0a2/param/_utils.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 param-2.0.0a2/param/_version.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 param-2.0.0a2/param/ipython.py
+-rw-r--r--   0        0        0   160611 2020-02-02 00:00:00.000000 param-2.0.0a2/param/parameterized.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 param-2.0.0a2/param/serializer.py
+-rw-r--r--   0        0        0    30965 2020-02-02 00:00:00.000000 param-2.0.0a2/param/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/conftest.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testaddparameter.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testbooleanparam.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testbytesparam.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcalendardateparam.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcalendardaterangeparam.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testclassselector.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcolorparameter.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcomparator.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcompositeparams.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testcustomparam.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testdateparam.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testdaterangeparam.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testdefaults.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testdeprecations.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testdynamicparams.py
+-rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testfiledeserialization.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testfileselector.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testipythonmagic.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testjsonserialization.py
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testlist.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testlistselector.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testmultifileselector.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testnumbergen.py
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testnumberparameter.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testnumpy.py
+-rw-r--r--   0        0        0    19502 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testobjectselector.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testpandas.py
+-rw-r--r--   0        0        0    38700 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testparamdepends.py
+-rw-r--r--   0        0        0    38909 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testparameterizedobject.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testparameterizedrepr.py
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testparamoutput.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testparamunion.py
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testpathparam.py
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testpickle.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testrangeparameter.py
+-rw-r--r--   0        0        0    11228 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testselector.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testsignatures.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/teststringparam.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testtimedependent.py
+-rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testtupleparam.py
+-rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testutils.py
+-rw-r--r--   0        0        0    26554 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/testwatch.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 param-2.0.0a2/tests/utils.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 param-2.0.0a2/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 param-2.0.0a2/LICENSE.txt
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 param-2.0.0a2/README.md
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 param-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 param-2.0.0a2/PKG-INFO
```

### Comparing `param-2.0.0a1/numbergen/__init__.py` & `param-2.0.0a2/numbergen/__init__.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/param/__init__.py` & `param-2.0.0a2/param/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,17 +558,14 @@
         elif (self._time + timestep) <= self.until:
             self._time += timestep
         else:
             self._exhausted = None
             raise StopIteration
         return self._time
 
-    # PARAM2_DEPRECATION: For Python 2 compatibility; can be removed for Python 3.
-    next = __next__
-
     def __call__(self, val=None, time_type=None):
         """
         When called with no arguments, returns the current time value.
 
         When called with a specified val, sets the time to it.
 
         When called with a specified time_type, changes the time_type
@@ -1690,14 +1687,16 @@
         self.check_on_set = check_on_set
 
         super().__init__(
             default=default, instantiate=instantiate, **params)
         # Required as Parameter sets allow_None=True if default is None
         if allow_None is Undefined:
             self.allow_None = self._slot_defaults['allow_None']
+        else:
+            self.allow_None = allow_None
         if self.default is not None and self.check_on_set is True:
             self._validate(self.default)
 
     @property
     def objects(self):
         return ListProxy(self._objects, self)
 
@@ -2966,15 +2965,15 @@
         super().__init__(default=default,**params)
 
     def _reset_event(self, obj, val):
         val = False
         if obj is None:
             self.default = val
         else:
-            obj.__dict__[self._internal_name] = val
+            obj._param__private.values[self.name] = val
         self._post_setter(obj, val)
 
     @instance_descriptor
     def __set__(self, obj, val):
         if self._mode in ['set-reset', 'set']:
             super().__set__(obj, val)
         if self._mode in ['set-reset', 'reset']:
```

### Comparing `param-2.0.0a1/param/_utils.py` & `param-2.0.0a2/param/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,52 @@
 import inspect
 import functools
+import re
 import warnings
 
+from textwrap import dedent
+from threading import get_ident
 
-class ParamDeprecationWarning(DeprecationWarning):
-    """Param DeprecationWarning"""
 
+class ParamWarning(Warning):
+    """Base Param Warning"""
 
-class ParamFutureWarning(FutureWarning):
-    """Param FutureWarning"""
+class ParamPendingDeprecationWarning(ParamWarning, PendingDeprecationWarning):
+    """Param PendingDeprecationWarning
+
+    This warning type is useful when the warning is not meant to be displayed
+    to REPL/notebooks users, as DeprecationWarning are displayed when triggered
+    by code in __main__ (__name__ == '__main__' in a REPL).
+    """
+
+
+class ParamDeprecationWarning(ParamWarning, DeprecationWarning):
+    """Param DeprecationWarning
+
+    Ignored by default except when triggered by code in __main__
+    """
+
+
+class ParamFutureWarning(ParamWarning, FutureWarning):
+    """Param FutureWarning
+
+    Always displayed.
+    """
 
 
 def _deprecated(extra_msg="", warning_cat=ParamDeprecationWarning):
     def decorator(func):
         """Internal decorator used to mark functions/methods as deprecated."""
         @functools.wraps(func)
         def inner(*args, **kwargs):
             msg = f"{func.__name__!r} has been deprecated and will be removed in a future version."
             if extra_msg:
-                msg = msg + ' ' + extra_msg
+                em = dedent(extra_msg)
+                em = em.strip().replace('\n', ' ')
+                msg = msg + ' ' + em
             warnings.warn(msg, category=warning_cat, stacklevel=2)
             return func(*args, **kwargs)
         return inner
     return decorator
 
 
 def _deprecate_positional_args(func):
@@ -48,19 +72,45 @@
         if n_extra_args > 0:
             extra_args = ", ".join(kwonly_args[:n_extra_args])
 
             warnings.warn(
                 f"Passing '{extra_args}' as positional argument(s) to 'param.{name}' "
                 "has been deprecated since Param 2.0,0 and will raise an error in a future version, "
                 "please pass them as keyword arguments.",
-                PendingDeprecationWarning,
+                ParamPendingDeprecationWarning,
                 stacklevel=2,
             )
 
             zip_args = zip(kwonly_args[:n_extra_args], args[-n_extra_args:])
             kwargs.update({name: arg for name, arg in zip_args})
 
             return func(*args[:-n_extra_args], **kwargs)
 
         return func(*args, **kwargs)
 
     return inner
+
+
+# Copy of Python 3.2 reprlib's recursive_repr but allowing extra arguments
+def _recursive_repr(fillvalue='...'):
+    'Decorator to make a repr function return fillvalue for a recursive call'
+
+    def decorating_function(user_function):
+        repr_running = set()
+
+        def wrapper(self, *args, **kwargs):
+            key = id(self), get_ident()
+            if key in repr_running:
+                return fillvalue
+            repr_running.add(key)
+            try:
+                result = user_function(self, *args, **kwargs)
+            finally:
+                repr_running.discard(key)
+            return result
+        return wrapper
+
+    return decorating_function
+
+
+def _is_auto_name(class_name, instance_name):
+    return re.match('^'+class_name+'[0-9]{5}$', instance_name)
```

### Comparing `param-2.0.0a1/param/ipython.py` & `param-2.0.0a2/param/ipython.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/param/parameterized.py` & `param-2.0.0a2/param/parameterized.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,39 @@
 except ImportError:
     serializer = None
 
 from collections import defaultdict, namedtuple, OrderedDict
 from functools import partial, wraps, reduce
 from html import escape
 from operator import itemgetter, attrgetter
-from threading import get_ident
 from types import FunctionType, MethodType
 
 import logging
 from contextlib import contextmanager
 from logging import DEBUG, INFO, WARNING, ERROR, CRITICAL
 
-from ._utils import _deprecated, _deprecate_positional_args
+from ._utils import (
+    _deprecated,
+    _deprecate_positional_args,
+    _is_auto_name,
+    _recursive_repr,
+    ParamDeprecationWarning as _ParamDeprecationWarning,
+)
 
 try:
-    # In case the optional ipython module is unavailable
-    from .ipython import ParamPager
-    param_pager = ParamPager(metaclass=True)  # Generates param description
-except:
+    get_ipython()
+except NameError:
     param_pager = None
+else:
+    # In case the optional ipython module is unavailable
+    try:
+        from .ipython import ParamPager
+        param_pager = ParamPager(metaclass=True)  # Generates param description
+    except:
+        param_pager = None
 
 from inspect import getfullargspec
 
 dt_types = (dt.datetime, dt.date)
 _int_types = (int,)
 
 try:
@@ -278,14 +288,16 @@
     been set, then it's an AttributeError to request the slot's
     value.)
     """
     return [slot for slot in get_all_slots(type(instance))
             if hasattr(instance,slot)]
 
 
+# PARAM3_DEPRECATION
+@_deprecated()
 def all_equal(arg1,arg2):
     """
     Return a single boolean for arg1==arg2, even for numpy arrays
     using element-wise comparison.
 
     Uses all(arg1==arg2) for sequences, and arg1==arg2 otherwise.
 
@@ -360,15 +372,15 @@
     return _f
 
 
 def no_instance_params(cls):
     """
     Disables instance parameters on the class
     """
-    cls._disable_instance__params = True
+    cls._param__private.disable_instance_params = True
     return cls
 
 
 def iscoroutinefunction(function):
     """
     Whether the function is an asynchronous coroutine function.
     """
@@ -383,15 +395,19 @@
     except AttributeError:
         return False
 
 
 def instance_descriptor(f):
     # If parameter has an instance Parameter, delegate setting
     def _f(self, obj, val):
-        instance_param = getattr(obj, '_instance__params', {}).get(self.name)
+        if obj is None:
+            # obj is None when the metaclass is setting
+            return f(self, obj, val)
+        params = obj._param__private.params
+        instance_param = None if params is None else params.get(self.name)
         if instance_param is not None and self is not instance_param:
             instance_param.__set__(obj, val)
             return
         return f(self, obj, val)
     return _f
 
 
@@ -402,35 +418,27 @@
     if not inspect.ismethod(method):
         return None
     if isinstance(method, partial):
         method = method.func
     return method.__self__
 
 
+# PARAM3_DEPRECATION
 def recursive_repr(fillvalue='...'):
-    'Decorator to make a repr function return fillvalue for a recursive call'
-    # Copy of Python 3.2 reprlib's recursive_repr but allowing extra arguments
-
-    def decorating_function(user_function):
-        repr_running = set()
-
-        @wraps(user_function)
-        def wrapper(self, *args, **kwargs):
-            key = id(self), get_ident()
-            if key in repr_running:
-                return fillvalue
-            repr_running.add(key)
-            try:
-                result = user_function(self, *args, **kwargs)
-            finally:
-                repr_running.discard(key)
-            return result
-        return wrapper
+    """
+    Decorator to make a repr function return fillvalue for a recursive call
 
-    return decorating_function
+    ..deprecated:: 1.12.0
+    """
+    warnings.warn(
+        'recursive_repr has been deprecated and will be removed in a future version.',
+        category=_ParamDeprecationWarning,
+        stacklevel=2,
+    )
+    return _recursive_repr(fillvalue=fillvalue)
 
 
 @accept_arguments
 def depends(func, *dependencies, watch=False, on_init=False, **kw):
     """Annotates a function or Parameterized method to express its dependencies.
 
     The specified dependencies can be either be Parameter instances or if a
@@ -694,32 +702,38 @@
                 old = Undefined if e.old is None else _getattrr(e.old.param[p], what, None)
                 new = Undefined if e.new is None else _getattrr(e.new.param[p], what, None)
             if not Comparator.is_equal(old, new):
                 return False
     return True
 
 
+# Two callers at the module top level to support pickling.
+async def _async_caller(*events, what='value', changed=None, callback=None, function=None):
+    if callback:
+        callback(*events)
+    if not _skip_event or not _skip_event(*events, what=what, changed=changed):
+        await function()
+
+
+def _sync_caller(*events, what='value', changed=None, callback=None, function=None):
+    if callback:
+        callback(*events)
+    if not _skip_event(*events, what=what, changed=changed):
+        return function()
+
+
 def _m_caller(self, method_name, what='value', changed=None, callback=None):
     """
     Wraps a method call adding support for scheduling a callback
     before it is executed and skipping events if a subobject has
     changed but its values have not.
     """
     function = getattr(self, method_name)
-    if iscoroutinefunction(function):
-        async def caller(*events):
-            if callback:
-                callback(*events)
-            if not _skip_event or not _skip_event(*events, what=what, changed=changed):
-                await function()
-    else:
-        def caller(*events):
-            if callback: callback(*events)
-            if not _skip_event(*events, what=what, changed=changed):
-                return function()
+    _caller = _async_caller if iscoroutinefunction(function) else _sync_caller
+    caller = partial(_caller, what=what, changed=changed, callback=callback, function=function)
     caller._watcher_name = method_name
     return caller
 
 
 def _dict_update(dictionary, **kwargs):
     """
     Small utility to update a copy of a dict with the provided keyword args.
@@ -835,23 +849,14 @@
         """
         values = dict(zip(cls_._fields, args))
         values.update(kwargs)
         if 'precedence' not in values:
             values['precedence'] = 0
         return super().__new__(cls_, **values)
 
-    def __iter__(self):
-        """
-        Backward compatibility layer to allow tuple unpacking without
-        the precedence value. Important for Panel which creates a
-        custom Watcher and uses tuple unpacking. Will be dropped in
-        Param 3.x.
-        """
-        return iter(self[:-1])
-
     def __str__(self):
         cls = type(self)
         attrs = ', '.join([f'{f}={getattr(self, f)!r}' for f in cls._fields])
         return f"{cls.__name__}({attrs})"
 
 
 
@@ -1056,52 +1061,51 @@
     #
     # * a1 and a2 share one Parameter object (A.__dict__['p']).
     #
     # * The default (class) value of p is stored in this Parameter
     #   object (A.__dict__['p'].default).
     #
     # * If the value of p is set on a1 (e.g. a1.p=2), a1's value of p
-    #   is stored in a1 itself (a1.__dict__['_p_param_value'])
+    #   is stored in a1 itself (a1._param__private.values['p'])
     #
-    # * When a1.p is requested, a1.__dict__['_p_param_value'] is
-    #   returned. When a2.p is requested, '_p_param_value' is not
-    #   found in a2.__dict__, so A.__dict__['p'].default (i.e. A.p) is
+    # * When a1.p is requested, a1._param__private.values['p'] is
+    #   returned. When a2.p is requested, 'p' is not found in
+    #   a1._param__private.values, so A.__dict__['p'].default (i.e. A.p) is
     #   returned instead.
     #
     #
     # Be careful when referring to the 'name' of a Parameter:
     #
     # * A Parameterized class has a name for the attribute which is
     #   being represented by the Parameter ('p' in the example above);
-    #   in the code, this is called the 'attrib_name'.
+    #   in the code, this is called the 'name'.
     #
     # * When a Parameterized instance has its own local value for a
-    #   parameter, it is stored as '_X_param_value' (where X is the
-    #   attrib_name for the Parameter); in the code, this is called
-    #   the internal_name.
+    #   parameter, it is stored as 'p._param__private.values[X]' where X is the
+    #   name of the Parameter
 
 
     # So that the extra features of Parameters do not require a lot of
     # overhead, Parameters are implemented using __slots__ (see
     # http://www.python.org/doc/2.4/ref/slots.html).  Instead of having
     # a full Python dictionary associated with each Parameter instance,
     # Parameter instances have an enumerated list (named __slots__) of
     # attributes, and reserve just enough space to store these
     # attributes.  Using __slots__ requires special support for
     # operations to copy and restore Parameters (e.g. for Python
     # persistent storage pickling); see __getstate__ and __setstate__.
-    __slots__ = ['name', '_internal_name', 'default', 'doc',
+    __slots__ = ['name', 'default', 'doc',
                  'precedence', 'instantiate', 'constant', 'readonly',
                  'pickle_default_value', 'allow_None', 'per_instance',
                  'watchers', 'owner', '_label']
 
     # Note: When initially created, a Parameter does not know which
     # Parameterized class owns it, nor does it know its names
     # (attribute name, internal name). Once the owning Parameterized
-    # class is created, owner, name, and _internal_name are
+    # class is created, owner, and name are
     # set.
 
     _serializers = {'json': serializer.JSONSerialization}
 
     _slot_defaults = dict(
         default=None, precedence=None, doc=None, _label=None, instantiate=False,
         constant=False, readonly=False, pickle_default_value=True, allow_None=False,
@@ -1199,15 +1203,14 @@
         self.owner = None
         self.precedence = precedence
         self.default = default
         self.doc = doc
         self.constant = constant is True or readonly is True # readonly => constant
         self.readonly = readonly
         self._label = label
-        self._internal_name = None
         self._set_instantiate(instantiate)
         self.pickle_default_value = pickle_default_value
         self._set_allow_None(allow_None)
         self.watchers = {}
         self.per_instance = per_instance
 
     @classmethod
@@ -1254,16 +1257,14 @@
     def _set_instantiate(self,instantiate):
         """Constant parameters must be instantiated."""
         # instantiate doesn't actually matter for read-only
         # parameters, since they can't be set even on a class.  But
         # having this code avoids needless instantiation.
         if self.readonly:
             self.instantiate = False
-        elif self.constant is True:
-            self.instantiate = True
         elif instantiate is not Undefined:
             self.instantiate = instantiate
         else:
             # Default value
             self.instantiate = self._slot_defaults['instantiate']
 
     def __setattr__(self, attribute, value):
@@ -1336,28 +1337,34 @@
         If called for a Parameterized instance, produce that
         instance's value, if one has been set - otherwise produce the
         class's value (default).
         """
         if obj is None: # e.g. when __get__ called for a Parameterized class
             result = self.default
         else:
-            result = obj.__dict__.get(self._internal_name,self.default)
+            # Attribute error when .values does not exist (_ClassPrivate)
+            # and KeyError when there's no cached value for this parameter.
+            try:
+                result = obj._param__private.values[self.name]
+            except (AttributeError, KeyError):
+                result = self.default
         return result
 
     @instance_descriptor
     def __set__(self, obj, val):
         """
         Set the value for this Parameter.
 
         If called for a Parameterized class, set that class's
         value (i.e. set this Parameter object's 'default' attribute).
 
         If called for a Parameterized instance, set the value of
         this Parameter on that instance (i.e. in the instance's
-        __dict__, under the parameter's internal_name).
+        `values` dictionary located in the private namespace `_param__private`,
+        under the parameter's name).
 
         If the Parameter's constant attribute is True, only allows
         the value to be set for a Parameterized class or on
         uninitialized Parameterized instances.
 
         If the Parameter's readonly attribute is True, only allows the
         value to be specified in the Parameter declaration inside the
@@ -1373,52 +1380,58 @@
         # Deprecated Number set_hook called here to avoid duplicating setter
         if hasattr(self, 'set_hook'):
             val = self.set_hook(obj, val)
             if self.set_hook is not _identity_hook:
                 # PARAM3_DEPRECATION
                 warnings.warn(
                     'Number.set_hook has been deprecated.',
-                    category=DeprecationWarning,
+                    category=_ParamDeprecationWarning,
+                    stacklevel=5,
                 )
 
         self._validate(val)
 
         _old = NotImplemented
         # obj can be None if __set__ is called for a Parameterized class
         if self.constant or self.readonly:
             if self.readonly:
                 raise TypeError("Read-only parameter '%s' cannot be modified" % self.name)
             elif obj is None:
                 _old = self.default
                 self.default = val
-            elif not obj.initialized:
-                _old = obj.__dict__.get(self._internal_name, self.default)
-                obj.__dict__[self._internal_name] = val
+            elif not obj._param__private.initialized:
+                _old = obj._param__private.values.get(self.name, self.default)
+                obj._param__private.values[self.name] = val
             else:
-                _old = obj.__dict__.get(self._internal_name, self.default)
+                _old = obj._param__private.values.get(self.name, self.default)
                 if val is not _old:
                     raise TypeError("Constant parameter '%s' cannot be modified"%self.name)
         else:
             if obj is None:
                 _old = self.default
                 self.default = val
             else:
-                _old = obj.__dict__.get(self._internal_name, self.default)
-                obj.__dict__[self._internal_name] = val
+                # When setting a Parameter before calling super.
+                if not isinstance(obj._param__private, _InstancePrivate):
+                    obj._param__private = _InstancePrivate()
+                _old = obj._param__private.values.get(self.name, self.default)
+                obj._param__private.values[self.name] = val
 
         self._post_setter(obj, val)
 
         if obj is not None:
-            if not getattr(obj, 'initialized', False):
+            if not hasattr(obj, '_param__private') or not getattr(obj._param__private, 'initialized', False):
                 return
             obj.param._update_deps(self.name)
 
         if obj is None:
             watchers = self.watchers.get("value")
+        # elif hasattr(obj, '_param__private') and hasattr(obj._param__private, 'watchers') and obj._param__private.watchers is not None and self.name in obj._param__private.watchers:
         elif hasattr(obj, '_param_watchers') and self.name in obj._param_watchers:
+            # watchers = obj._param__private.watchers[self.name].get('value')
             watchers = obj._param_watchers[self.name].get('value')
             if watchers is None:
                 watchers = self.watchers.get("value")
         else:
             watchers = None
 
         obj = self.owner if obj is None else obj
@@ -1454,15 +1467,14 @@
                                  'assigned a name by the {} class, '
                                  'could not assign new name {!r}. Parameters '
                                  'may not be shared by multiple classes; '
                                  'ensure that you create a new parameter '
                                  'instance for each new class.'.format(type(self).__name__, self.name,
                                     self.owner.name, attrib_name))
         self.name = attrib_name
-        self._internal_name = "_%s_param_value" % attrib_name
 
     def __getstate__(self):
         """
         All Parameters have slots, not a dict, so we have to support
         pickle and deepcopy ourselves.
         """
         state = {}
@@ -1569,18 +1581,18 @@
 
     (Used to decorate Parameterized methods that must alter
     a constant Parameter.)
     """
     @wraps(fn)
     def override_initialization(self_,*args,**kw):
         parameterized_instance = self_.self
-        original_initialized = parameterized_instance.initialized
-        parameterized_instance.initialized = False
+        original_initialized = parameterized_instance._param__private.initialized
+        parameterized_instance._param__private.initialized = False
         fn(parameterized_instance, *args, **kw)
-        parameterized_instance.initialized = original_initialized
+        parameterized_instance._param__private.initialized = original_initialized
     return override_initialization
 
 
 class Comparator:
     """
     Comparator defines methods for determining whether two objects
     should be considered equal. It works by registering custom
@@ -1599,23 +1611,29 @@
     """
 
     equalities = {
         numbers.Number: operator.eq,
         str: operator.eq,
         bytes: operator.eq,
         type(None): operator.eq,
+        lambda o: hasattr(o, '_infinitely_iterable'): operator.eq,  # Time
     }
     equalities.update({dtt: operator.eq for dtt in dt_types})
 
     @classmethod
     def is_equal(cls, obj1, obj2):
         for eq_type, eq in cls.equalities.items():
-            if ((isinstance(eq_type, FunctionType)
-                 and eq_type(obj1) and eq_type(obj2))
-                or (isinstance(obj1, eq_type) and isinstance(obj2, eq_type))):
+            try:
+                are_instances = isinstance(obj1, eq_type) and isinstance(obj2, eq_type)
+            except TypeError:
+                pass
+            else:
+                if are_instances:
+                    return eq(obj1, obj2)
+            if isinstance(eq_type, FunctionType) and eq_type(obj1) and eq_type(obj2):
                 return eq(obj1, obj2)
         if isinstance(obj2, (list, set, tuple)):
             return cls.compare_iterator(obj1, obj2)
         elif isinstance(obj2, dict):
             return cls.compare_mapping(obj1, obj2)
         return False
 
@@ -1636,14 +1654,33 @@
                 if not cls.is_equal(obj1[k], obj2[k]):
                     return False
             else:
                 return False
         return True
 
 
+class _ParametersRestorer:
+    """
+    Context-manager to handle the reset of parameter values after an update.
+    """
+
+    def __init__(self, *, parameters, restore):
+        self._parameters = parameters
+        self._restore = restore
+
+    def __enter__(self):
+        return self._restore
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        try:
+            self._parameters._update(self._restore)
+        finally:
+            self._restore = {}
+
+
 class Parameters:
     """Object that holds the namespace and implementation of Parameterized
     methods as well as any state that is not in __slots__ or the
     Parameters themselves.
 
     Exists at both the metaclass level (instantiated by the metaclass)
     and at the instance level. Can contain state specific to either the
@@ -1656,86 +1693,87 @@
         self is the instance if set.
         """
         self_.cls = cls
         self_.self = self
 
     @property
     def _BATCH_WATCH(self_):
-        return self_.self_or_cls._parameters_state['BATCH_WATCH']
+        return self_.self_or_cls._param__private.parameters_state['BATCH_WATCH']
 
     @_BATCH_WATCH.setter
     def _BATCH_WATCH(self_, value):
-        self_.self_or_cls._parameters_state['BATCH_WATCH'] = value
+        self_.self_or_cls._param__private.parameters_state['BATCH_WATCH'] = value
 
     @property
     def _TRIGGER(self_):
-        return self_.self_or_cls._parameters_state['TRIGGER']
+        return self_.self_or_cls._param__private.parameters_state['TRIGGER']
 
     @_TRIGGER.setter
     def _TRIGGER(self_, value):
-        self_.self_or_cls._parameters_state['TRIGGER'] = value
+        self_.self_or_cls._param__private.parameters_state['TRIGGER'] = value
 
     @property
     def _events(self_):
-        return self_.self_or_cls._parameters_state['events']
+        return self_.self_or_cls._param__private.parameters_state['events']
 
     @_events.setter
     def _events(self_, value):
-        self_.self_or_cls._parameters_state['events'] = value
+        self_.self_or_cls._param__private.parameters_state['events'] = value
 
     @property
     def _watchers(self_):
-        return self_.self_or_cls._parameters_state['watchers']
+        return self_.self_or_cls._param__private.parameters_state['watchers']
 
     @_watchers.setter
     def _watchers(self_, value):
-        self_.self_or_cls._parameters_state['watchers'] = value
+        self_.self_or_cls._param__private.parameters_state['watchers'] = value
 
     @property
     def watchers(self):
         """Read-only list of watchers on this Parameterized"""
         return self._watchers
 
     @property
     def self_or_cls(self_):
         return self_.cls if self_.self is None else self_.self
 
     def __setstate__(self, state):
-        # Set old parameters state on Parameterized._parameters_state
-        self_or_cls = state.get('self', state.get('cls'))
-        for k in self_or_cls._parameters_state:
+        # Set old parameters state on Parameterized.parameters_state
+        self_, cls = state.get('self'), state.get('cls')
+        self_or_cls = self_ if self_ is not None else cls
+        for k in self_or_cls._param__private.parameters_state:
             key = '_'+k
             if key in state:
-                self_or_cls._parameters_state[k] = state.pop(key)
+                self_or_cls._param__private.parameters_state[k] = state.pop(key)
         for k, v in state.items():
             setattr(self, k, v)
 
     def __getitem__(self_, key):
         """
         Returns the class or instance parameter
         """
         inst = self_.self
         parameters = self_.objects(False) if inst is None else inst.param.objects(False)
         p = parameters[key]
-        if (inst is not None and getattr(inst, 'initialized', False) and p.per_instance and
-            not getattr(inst, '_disable_instance__params', False)):
-            if key not in inst._instance__params:
+        if (inst is not None and getattr(inst._param__private, 'initialized', False) and p.per_instance and
+            not getattr(self_.cls._param__private, 'disable_instance_params', False)):
+            if key not in inst._param__private.params:
                 try:
                     # Do not copy watchers on class parameter
                     watchers = p.watchers
                     p.watchers = {}
                     p = copy.copy(p)
                 except:
                     raise
                 finally:
                     p.watchers = {k: list(v) for k, v in watchers.items()}
                 p.owner = inst
-                inst._instance__params[key] = p
+                inst._param__private.params[key] = p
             else:
-                p = inst._instance__params[key]
+                p = inst._param__private.params[key]
         return p
 
 
     def __dir__(self_):
         """
         Adds parameters to dir
         """
@@ -1757,69 +1795,70 @@
         """
         Extends attribute access to parameter objects.
         """
         cls = self_.__dict__.get('cls')
         if cls is None: # Class not initialized
             raise AttributeError
 
-        try:
-            params = list(getattr(cls, '_%s__params' % cls.__name__))
-        except AttributeError:
+        params = list(cls._param__private.params)
+        if not params:
             params = [n for class_ in classlist(cls) for n, v in class_.__dict__.items()
                       if isinstance(v, Parameter)]
 
         if attr in params:
             return self_.__getitem__(attr)
         elif self_.self is None:
             raise AttributeError(f"type object '{self_.cls.__name__}.param' has no attribute {attr!r}")
         else:
             raise AttributeError(f"'{self_.cls.__name__}.param' object has no attribute {attr!r}")
 
-
     @as_uninitialized
     def _set_name(self_, name):
         self = self_.param.self
         self.name=name
 
-
     @as_uninitialized
     def _generate_name(self_):
         self = self_.param.self
         self.param._set_name('%s%05d' % (self.__class__.__name__ ,object_count))
 
-
     @as_uninitialized
     def _setup_params(self_,**params):
         """
         Initialize default and keyword parameter values.
 
-        First, ensures that all Parameters with 'instantiate=True'
-        (typically used for mutable Parameters) are copied directly
-        into each object, to ensure that there is an independent copy
-        (to avoid surprising aliasing errors).  Then sets each of the
-        keyword arguments, warning when any of them are not defined as
-        parameters.
-
-        Constant Parameters can be set during calls to this method.
+        First, ensures that all Parameters with 'instantiate=True' (typically
+        used for mutable Parameters) are copied directly into each object, to
+        ensure that there is an independent copy (to avoid surprising aliasing
+        errors). Second, ensures that Parameters with 'constant=True' are
+        referenced on the instance, to make sure that setting a constant
+        Parameter on the class doesn't affect already created instances. Then
+        sets each of the keyword arguments, raising when any of them are not
+        defined as parameters.
         """
         self = self_.param.self
         ## Deepcopy all 'instantiate=True' parameters
         # (building a set of names first to avoid redundantly
         # instantiating a later-overridden parent class's parameter)
-        params_to_instantiate = {}
+        params_to_deepcopy = {}
+        params_to_ref = {}
         for class_ in classlist(type(self)):
             if not issubclass(class_, Parameterized):
                 continue
             for (k, v) in class_.param._parameters.items():
                 # (avoid replacing name with the default of None)
                 if v.instantiate and k != "name":
-                    params_to_instantiate[k] = v
+                    params_to_deepcopy[k] = v
+                elif v.constant and k != 'name':
+                    params_to_ref[k] = v
 
-        for p in params_to_instantiate.values():
+        for p in params_to_deepcopy.values():
             self.param._instantiate_param(p)
+        for p in params_to_ref.values():
+            self.param._instantiate_param(p, deepcopy=False)
 
         ## keyword arg setting
         for name, val in params.items():
             desc = self.__class__.get_param_descriptor(name)[0] # pylint: disable-msg=E1101
             if not desc:
                 raise TypeError(
                     f"{self.__class__.__name__}.__init__() got an unexpected "
@@ -1832,29 +1871,31 @@
     def _changed(cls, event):
         """
         Predicate that determines whether a Event object has actually
         changed such that old != new.
         """
         return not Comparator.is_equal(event.old, event.new)
 
-    def _instantiate_param(self_, param_obj, dict_=None, key=None):
-        # deepcopy param_obj.default into self.__dict__ (or dict_ if supplied)
-        # under the parameter's _internal_name (or key if supplied)
+    def _instantiate_param(self_, param_obj, dict_=None, key=None, deepcopy=True):
+        # deepcopy or store a reference to reference param_obj.default into
+        # self._param__private.values (or dict_ if supplied) under the
+        # parameter's name (or key if supplied)
+        instantiator = copy.deepcopy if deepcopy else lambda o: o
         self = self_.self
-        dict_ = dict_ or self.__dict__
-        key = key or param_obj._internal_name
+        dict_ = dict_ or self._param__private.values
+        key = key or param_obj.name
         if shared_parameters._share:
             param_key = (str(type(self)), param_obj.name)
             if param_key in shared_parameters._shared_cache:
                 new_object = shared_parameters._shared_cache[param_key]
             else:
-                new_object = copy.deepcopy(param_obj.default)
+                new_object = instantiator(param_obj.default)
                 shared_parameters._shared_cache[param_key] = new_object
         else:
-            new_object = copy.deepcopy(param_obj.default)
+            new_object = instantiator(param_obj.default)
 
         dict_[key] = new_object
 
         if isinstance(new_object, Parameterized):
             global object_count
             object_count += 1
             # Writes over name given to the original object;
@@ -1874,28 +1915,28 @@
                     constant_grouped[(id(dep.inst), id(dep.cls), dep.what)].append((None, dep))
                 for group in constant_grouped.values():
                     self_._watch_group(obj, method, queued, group)
                 m = getattr(self_.self, method)
                 if on_init and m not in init_methods:
                     init_methods.append(m)
             elif dynamic:
-                for w in obj._dynamic_watchers.pop(method, []):
+                for w in obj._param__private.dynamic_watchers.pop(method, []):
                     (w.cls if w.inst is None else w.inst).param.unwatch(w)
             else:
                 continue
 
             # Resolve dynamic dependencies one-by-one to be able to trace their watchers
             grouped = defaultdict(list)
             for ddep in dynamic:
                 for dep in _resolve_mcs_deps(obj, [], [ddep]):
                     grouped[(id(dep.inst), id(dep.cls), dep.what)].append((ddep, dep))
 
             for group in grouped.values():
                 watcher = self_._watch_group(obj, method, queued, group, attribute)
-                obj._dynamic_watchers[method].append(watcher)
+                obj._param__private.dynamic_watchers[method].append(watcher)
         for m in init_methods:
             m()
 
     def _resolve_dynamic_deps(self, obj, dynamic_dep, param_dep, attribute):
         """
         If a subobject whose parameters are being depended on changes
         we should only trigger events if the actual parameter values
@@ -1962,15 +2003,15 @@
             subparams, callback, what = self_._resolve_dynamic_deps(
                 obj, dynamic_dep, param_dep, attribute)
 
         mcaller = _m_caller(obj, name, what, subparams, callback)
         return dep_obj.param._watch(
             mcaller, params, param_dep.what, queued=queued, precedence=-1)
 
-    @recursive_repr()
+    @_recursive_repr()
     def _repr_html_(self_, open=True):
         return _parameterized_repr_html(self_.self_or_cls, open)
 
     # Classmethods
 
     # PARAM3_DEPRECATION
     @_deprecated(extra_msg="""Use instead `for k,v in p.param.objects().items(): print(f"{p.__class__.name}.{k}={repr(v.default)}")`""")
@@ -1995,15 +2036,14 @@
 
         ..deprecated:: 1.12.0
              Use instead `p.param.default =`
         """
         cls = self_.cls
         setattr(cls,param_name,value)
 
-
     def add_parameter(self_, param_name, param_obj):
         """
         Add a new Parameter object into this object's class.
 
         Should result in a Parameter equivalent to one declared
         in the class's source code.
         """
@@ -2011,18 +2051,15 @@
         # which is supported by the metaclass's __setattr__ , but
         # would need to handle the params() cache as well
         # (which is tricky but important for startup speed).
         cls = self_.cls
         type.__setattr__(cls,param_name,param_obj)
         ParameterizedMetaclass._initialize_parameter(cls,param_name,param_obj)
         # delete cached params()
-        try:
-            delattr(cls,'_%s__params'%cls.__name__)
-        except AttributeError:
-            pass
+        cls._param__private.params.clear()
 
     # PARAM3_DEPRECATION
     @_deprecated(extra_msg="Use instead `.param.add_parameter`")
     def _add_parameter(self_,param_name, param_obj):
         """Add a new Parameter object into this object's class.
 
         ..deprecated :: 1.12.0
@@ -2048,54 +2085,69 @@
         else:
             return pdict[parameter_name]
 
     # Bothmethods
 
     def update(self_, *args, **kwargs):
         """
-        For the given dictionary or iterable or set of param=value keyword arguments,
-        sets the corresponding parameter of this object or class to the given value.
-        """
-        BATCH_WATCH = self_.self_or_cls.param._BATCH_WATCH
-        self_.self_or_cls.param._BATCH_WATCH = True
+        For the given dictionary or iterable or set of param=value
+        keyword arguments, sets the corresponding parameter of this
+        object or class to the given value.
+
+        May also be used as a context manager to temporarily set and
+        then reset parameter values.
+        """
+        restore = self_._update(*args, **kwargs)
+        return _ParametersRestorer(parameters=self_, restore=restore)
+
+    def _update(self_, *args, **kwargs):
+        BATCH_WATCH = self_._BATCH_WATCH
+        self_._BATCH_WATCH = True
         self_or_cls = self_.self_or_cls
         if args:
             if len(args) == 1 and not kwargs:
                 kwargs = args[0]
             else:
-                self_.self_or_cls.param._BATCH_WATCH = False
-                raise ValueError("%s.update accepts *either* an iterable or key=value pairs, not both" %
-                                 (self_or_cls.name))
+                self_._BATCH_WATCH = False
+                raise ValueError(
+                    f"{self_.cls.__name__}.param.update accepts *either* an iterable "
+                    "or key=value pairs, not both."
+                )
 
-        trigger_params = [k for k in kwargs
-                          if ((k in self_.self_or_cls.param) and
-                              hasattr(self_.self_or_cls.param[k], '_autotrigger_value'))]
+        trigger_params = [
+            k for k in kwargs
+            if k in self_ and hasattr(self_[k], '_autotrigger_value')
+        ]
 
         for tp in trigger_params:
             self_.self_or_cls.param[tp]._mode = 'set'
 
+        values = self_.values()
+        restore = {k: values[k] for k, v in kwargs.items() if k in values}
+
         for (k, v) in kwargs.items():
-            if k not in self_or_cls.param:
-                self_.self_or_cls.param._BATCH_WATCH = False
-                raise ValueError(f"'{k}' is not a parameter of {self_or_cls.name}")
+            if k not in self_:
+                self_._BATCH_WATCH = False
+                raise ValueError(f"{k!r} is not a parameter of {self_.cls.__name__}")
             try:
                 setattr(self_or_cls, k, v)
             except:
-                self_.self_or_cls.param._BATCH_WATCH = False
+                self_._BATCH_WATCH = False
                 raise
 
-        self_.self_or_cls.param._BATCH_WATCH = BATCH_WATCH
+        self_._BATCH_WATCH = BATCH_WATCH
         if not BATCH_WATCH:
             self_._batch_call_watchers()
 
         for tp in trigger_params:
-            p = self_.self_or_cls.param[tp]
+            p = self_[tp]
             p._mode = 'reset'
             setattr(self_or_cls, tp, p._autotrigger_reset_value)
             p._mode = 'set-reset'
+        return restore
 
     # PARAM3_DEPRECATION
     @_deprecated(extra_msg="Use instead `.param.update`")
     def set_param(self_, *args,**kwargs):
         """
         For each param=value keyword argument, sets the corresponding
         parameter of this object or class to the given value.
@@ -2113,15 +2165,14 @@
             if len(args) == 2 and not args[0] in kwargs and not kwargs:
                 kwargs[args[0]] = args[1]
             else:
                 raise ValueError("Invalid positional arguments for %s.set_param" %
                                  (self_or_cls.name))
         return self_.update(kwargs)
 
-
     def objects(self_, instance=True):
         """
         Returns the Parameters of this instance or class
 
         If instance=True and called on a Parameterized instance it
         will create instance parameters for all Parameters defined on
         the class. To force class parameters to be returned use
@@ -2129,34 +2180,34 @@
         parameters unless necessary you may also request only existing
         instance parameters to be returned by setting
         instance='existing'.
         """
         cls = self_.cls
         # We cache the parameters because this method is called often,
         # and parameters are rarely added (and cannot be deleted)
-        try:
-            pdict = getattr(cls, '_%s__params' % cls.__name__)
-        except AttributeError:
+        pdict = cls._param__private.params
+        if not pdict:
             paramdict = {}
             for class_ in classlist(cls):
                 for name, val in class_.__dict__.items():
                     if isinstance(val, Parameter):
                         paramdict[name] = val
 
             # We only want the cache to be visible to the cls on which
             # params() is called, so we mangle the name ourselves at
             # runtime (if we were to mangle it now, it would be
             # _Parameterized.__params for all classes).
-            setattr(cls, '_%s__params' % cls.__name__, paramdict)
+            # cls._param__private.params[f'_{cls.__name__}__params'] = paramdict
+            cls._param__private.params = paramdict
             pdict = paramdict
 
         if instance and self_.self is not None:
             if instance == 'existing':
-                if getattr(self_.self, 'initialized', False) and self_.self._instance__params:
-                    return dict(pdict, **self_.self._instance__params)
+                if getattr(self_.self._param__private, 'initialized', False) and self_.self._param__private.params:
+                    return dict(pdict, **self_.self._param__private.params)
                 return pdict
             else:
                 return {k: self_.self.param[k] for k in pdict}
         return pdict
 
 
     def trigger(self_, *param_names):
@@ -2359,15 +2410,17 @@
         only return values that are not equal to the default value
         (onlychanged has no effect when called on a class).
         """
         self_or_cls = self_.self_or_cls
         vals = []
         for name, val in self_or_cls.param.objects('existing').items():
             value = self_or_cls.param.get_value_generator(name)
-            if not onlychanged or not all_equal(value, val.default):
+            if name == 'name' and onlychanged and _is_auto_name(self_.cls.__name__, value):
+                continue
+            if not onlychanged or not Comparator.is_equal(value, val.default):
                 vals.append((name, value))
 
         vals.sort(key=itemgetter(0))
         return dict(vals)
 
     def force_new_dynamic_value(self_, name): # pylint: disable-msg=E0213
         """
@@ -2415,18 +2468,18 @@
 
         # not a Dynamic Parameter
         elif not hasattr(param_obj,'_value_is_dynamic'):
             value = getattr(cls_or_slf,name)
 
         # Dynamic Parameter...
         else:
-            internal_name = "_%s_param_value"%name
-            if hasattr(cls_or_slf,internal_name):
+            # TODO: is this always an instance?
+            if isinstance(cls_or_slf, Parameterized) and name in cls_or_slf._param__private.values:
                 # dealing with object and it's been set on this object
-                value = getattr(cls_or_slf,internal_name)
+                value = cls_or_slf._param__private.values[name]
             else:
                 # dealing with class or isn't set on the object
                 value = param_obj.default
 
         return value
 
     def inspect_value(self_,name): # pylint: disable-msg=E0213
@@ -2601,14 +2654,15 @@
         parameter_names = watcher.parameter_names
         for parameter_name in parameter_names:
             if parameter_name not in self_.cls.param:
                 raise ValueError("{} parameter was not found in list of "
                                  "parameters of class {}".format(parameter_name, self_.cls.__name__))
 
             if self_.self is not None and what == "value":
+                # watchers = self_.self._param__private.watchers
                 watchers = self_.self._param_watchers
                 if parameter_name not in watchers:
                     watchers[parameter_name] = {}
                 if what not in watchers[parameter_name]:
                     watchers[parameter_name][what] = []
                 getattr(watchers[parameter_name][what], action)(watcher)
             else:
@@ -2821,21 +2875,153 @@
             if warnings_as_exceptions:
                 raise Exception("Warning: " + msg % args)
             else:
                 global warning_count
                 warning_count+=1
         self_.__db_print(level, msg, *args, **kw)
 
+    # Note that there's no state_push method on the class, so
+    # dynamic parameters set on a class can't have state saved. This
+    # is because, to do this, state_push() would need to be a
+    # @bothmethod, but that complicates inheritance in cases where we
+    # already have a state_push() method.
+    # (isinstance(g,Parameterized) below is used to exclude classes.)
+
+    def _state_push(self_):
+        """
+        Save this instance's state.
+
+        For Parameterized instances, this includes the state of
+        dynamically generated values.
+
+        Subclasses that maintain short-term state should additionally
+        save and restore that state using state_push() and
+        state_pop().
+
+        Generally, this method is used by operations that need to test
+        something without permanently altering the objects' state.
+        """
+        self = self_.self_or_cls
+        if not isinstance(self, Parameterized):
+            raise NotImplementedError('_state_push is not implemented at the class level')
+        for pname, p in self.param.objects('existing').items():
+            g = self.param.get_value_generator(pname)
+            if hasattr(g,'_Dynamic_last'):
+                g._saved_Dynamic_last.append(g._Dynamic_last)
+                g._saved_Dynamic_time.append(g._Dynamic_time)
+                # CB: not storing the time_fn: assuming that doesn't
+                # change.
+            elif hasattr(g,'state_push') and isinstance(g,Parameterized):
+                g.state_push()
+
+    def _state_pop(self_):
+        """
+        Restore the most recently saved state.
+
+        See state_push() for more details.
+        """
+        self = self_.self_or_cls
+        if not isinstance(self, Parameterized):
+            raise NotImplementedError('_state_pop is not implemented at the class level')
+        for pname, p in self.param.objects('existing').items():
+            g = self.param.get_value_generator(pname)
+            if hasattr(g,'_Dynamic_last'):
+                g._Dynamic_last = g._saved_Dynamic_last.pop()
+                g._Dynamic_time = g._saved_Dynamic_time.pop()
+            elif hasattr(g,'state_pop') and isinstance(g,Parameterized):
+                g.state_pop()
 
     def pprint(self_, imports=None, prefix=" ", unknown_value='<?>',
                qualify=False, separator=""):
-        """See Parameterized.pprint"""
-        self = self_.self
-        return self._pprint(imports, prefix, unknown_value, qualify, separator)
+        """
+        (Experimental) Pretty printed representation that may be
+        evaluated with eval. See pprint() function for more details.
+        """
+        self = self_.self_or_cls
+        if not isinstance(self, Parameterized):
+            raise NotImplementedError('pprint is not implemented at the class level')
+        # Wrapping the staticmethod _pprint with partial to pass `self` as the `_recursive_repr`
+        # decorator expects `self`` to be the pprinted object (not `self_`).
+        return partial(self_._pprint, self, imports=imports, prefix=prefix,
+                       unknown_value=unknown_value, qualify=qualify, separator=separator)()
+
+    @staticmethod
+    @_recursive_repr()
+    def _pprint(self, imports=None, prefix=" ", unknown_value='<?>',
+               qualify=False, separator=""):
+        if imports is None:
+            imports = [] # would have been simpler to use a set from the start
+        imports[:] = list(set(imports))
+
+        # Generate import statement
+        mod = self.__module__
+        bits = mod.split('.')
+        imports.append("import %s"%mod)
+        imports.append("import %s"%bits[0])
+
+        changed_params = self.param.values(onlychanged=script_repr_suppress_defaults)
+        values = self.param.values()
+        spec = getfullargspec(type(self).__init__)
+        if 'self' not in spec.args or spec.args[0] != 'self':
+            raise KeyError(f"'{type(self).__name__}.__init__.__signature__' must contain 'self' as its first Parameter.")
+        args = spec.args[1:]
+
+        if spec.defaults is not None:
+            posargs = spec.args[:-len(spec.defaults)]
+            kwargs = dict(zip(spec.args[-len(spec.defaults):], spec.defaults))
+        else:
+            posargs, kwargs = args, []
+
+        parameters = self.param.objects('existing')
+        ordering = sorted(
+            sorted(changed_params), # alphanumeric tie-breaker
+            key=lambda k: (- float('inf')  # No precedence is lowest possible precendence
+                           if parameters[k].precedence is None else
+                           parameters[k].precedence))
 
+        arglist, keywords, processed = [], [], []
+        for k in args + ordering:
+            if k in processed: continue
+
+            # Suppresses automatically generated names.
+            if k == 'name' and (values[k] is not None
+                                and re.match('^'+self.__class__.__name__+'[0-9]+$', values[k])):
+                continue
+
+            value = pprint(values[k], imports, prefix=prefix,settings=[],
+                           unknown_value=unknown_value,
+                           qualify=qualify) if k in values else None
+
+            if value is None:
+                if unknown_value is False:
+                    raise Exception(f"{self.name}: unknown value of {k!r}")
+                elif unknown_value is None:
+                    # i.e. suppress repr
+                    continue
+                else:
+                    value = unknown_value
+
+            # Explicit kwarg (unchanged, known value)
+            if (k in kwargs) and (k in values) and kwargs[k] == values[k]: continue
+
+            if k in posargs:
+                # value will be unknown_value unless k is a parameter
+                arglist.append(value)
+            elif (k in kwargs or
+                  (hasattr(spec, 'varkw') and (spec.varkw is not None)) or
+                  (hasattr(spec, 'keywords') and (spec.keywords is not None))):
+                # Explicit modified keywords or parameters in
+                # precendence order (if **kwargs present)
+                keywords.append(f'{k}={value}')
+
+            processed.append(k)
+
+        qualifier = mod + '.'  if qualify else ''
+        arguments = arglist + keywords + (['**%s' % spec.varargs] if spec.varargs else [])
+        return qualifier + '{}({})'.format(self.__class__.__name__,  (','+separator+prefix).join(arguments))
 
 
 class ParameterizedMetaclass(type):
     """
     The metaclass of Parameterized (and all its descendents).
 
     The metaclass overrides type.__setattr__ to allow us to set
@@ -2864,54 +3050,48 @@
 
         Initializes all the Parameters by looking up appropriate
         default values (see __param_inheritance()) and setting
         attrib_names (see _set_names()).
         """
         type.__init__(mcs, name, bases, dict_)
 
+        _param__private = _ClassPrivate()
+        mcs._param__private = _param__private
         mcs.__set_name(name, dict_)
-
-        mcs._parameters_state = {
-            "BATCH_WATCH": False, # If true, Event and watcher objects are queued.
-            "TRIGGER": False,
-            "events": [], # Queue of batched events
-            "watchers": [] # Queue of batched watchers
-        }
-        mcs._param = Parameters(mcs)
+        mcs._param__parameters = Parameters(mcs)
 
         # All objects (with their names) of type Parameter that are
         # defined in this class
         parameters = [(n, o) for (n, o) in dict_.items()
                       if isinstance(o, Parameter)]
 
-        mcs._param._parameters = dict(parameters)
+        mcs._param__parameters._parameters = dict(parameters)
 
         for param_name,param in parameters:
             mcs._initialize_parameter(param_name, param)
 
         # retrieve depends info from methods and store more conveniently
         dependers = [(n, m, m._dinfo) for (n, m) in dict_.items()
                      if hasattr(m, '_dinfo')]
 
         # Resolve dependencies of current class
         _watch = []
         for name, method, dinfo in dependers:
             watch = dinfo.get('watch', False)
             on_init = dinfo.get('on_init', False)
-            if not watch:
-                continue
             minfo = MInfo(cls=mcs, inst=None, name=name,
                           method=method)
             deps, dynamic_deps = _params_depended_on(minfo, dynamic=False)
-            _watch.append((name, watch == 'queued', on_init, deps, dynamic_deps))
+            if watch:
+                _watch.append((name, watch == 'queued', on_init, deps, dynamic_deps))
 
         # Resolve dependencies in class hierarchy
         _inherited = []
         for cls in classlist(mcs)[:-1][::-1]:
-            if not hasattr(cls, '_param'):
+            if not hasattr(cls, '_param__parameters'):
                 continue
             for dep in cls.param._depends['watch']:
                 method = getattr(mcs, dep[0], None)
                 dinfo = getattr(method, '_dinfo', {'watch': False})
                 if (not any(dep[0] == w[0] for w in _watch+_inherited)
                     and dinfo.get('watch')):
                     _inherited.append(dep)
@@ -2924,33 +3104,32 @@
     def __set_name(mcs, name, dict_):
         """
         Give Parameterized classes a useful 'name' attribute that is by
         default the class name, unless a class in the hierarchy has defined
         a `name` String Parameter with a defined `default` value, in which case
         that value is used to set the class name.
         """
-        mcs.__renamed = False
         name_param = dict_.get("name", None)
         if name_param is not None:
             if not type(name_param) is String:
                 raise TypeError(
                     f"Parameterized class {name!r} cannot override "
                     f"the 'name' Parameter with type {type(name_param)}. "
                     "Overriding 'name' is only allowed with a 'String' Parameter."
                 )
             if name_param.default:
                 mcs.name = name_param.default
-                mcs.__renamed = True
+                mcs._param__private.renamed = True
             else:
                 mcs.name = name
         else:
             classes = classlist(mcs)[::-1]
             found_renamed = False
             for c in classes:
-                if getattr(c, "_ParameterizedMetaclass__renamed", False):
+                if hasattr(c, '_param__private') and c._param__private.renamed:
                     found_renamed = True
                     break
             if not found_renamed:
                 mcs.name = name
 
     def __class_docstring_signature(mcs, max_repr_len=15):
         """
@@ -3007,15 +3186,15 @@
             return getattr(mcs,'_%s__abstract'%mcs.__name__.lstrip("_"))
         except AttributeError:
             return False
 
     abstract = property(__is_abstract)
 
     def _get_param(mcs):
-        return mcs._param
+        return mcs._param__parameters
 
     param = property(_get_param)
 
     def __setattr__(mcs, attribute_name, value):
         """
         Implements 'self.attribute_name=value' in a way that also supports Parameters.
 
@@ -3259,16 +3438,16 @@
 
     if isinstance(val,type):
         rep = type_script_repr(val,imports,prefix,settings)
 
     elif type(val) in script_repr_reg:
         rep = script_repr_reg[type(val)](val,imports,prefix,settings)
 
-    elif hasattr(val,'_pprint'):
-        rep=val._pprint(imports=imports, prefix=prefix+"    ",
+    elif isinstance(val, Parameterized) or (type(val) is type and issubclass(val, Parameterized)):
+        rep=val.param.pprint(imports=imports, prefix=prefix+"    ",
                         qualify=qualify, unknown_value=unknown_value,
                         separator=separator)
     else:
         rep=repr(val)
 
     return rep
 
@@ -3431,14 +3610,123 @@
         ' <div style="padding-left:10px; padding-bottom:5px;">\n'
         '  <table style="max-width:100%; border:1px solid #AAAAAA;">\n'
         f'   <tr><th>Name</th><th>Type</th><th>{value_field}</th><th>Bounds/Objects</th><th>Mode</th></tr>\n'
         f'{contents}\n'
         '  </table>\n </div>\n</details>\n'
     )
 
+# _ClassPrivate and _InstancePrivate are the private namespaces of Parameterized
+# classes and instance respectively, stored on the `_param__private` attribute.
+# They are implemented with slots for performance reasons.
+
+class _ClassPrivate:
+    """
+    parameters_state: dict
+        Dict holding some transient states
+    disable_instance_params: bool
+        Whether to disable instance parameters
+    renamed: bool
+        Whethe the class has been renamed by a super class
+    params: dict
+        Dict of parameter_name:parameter
+    """
+
+    __slots__ = [
+        'parameters_state',
+        'disable_instance_params',
+        'renamed',
+        'params',
+        'initialized',
+    ]
+
+    def __init__(
+        self,
+        parameters_state=None,
+        disable_instance_params=False,
+        renamed=False,
+        params=None,
+    ):
+        if parameters_state is None:
+            parameters_state = {
+                "BATCH_WATCH": False, # If true, Event and watcher objects are queued.
+                "TRIGGER": False,
+                "events": [], # Queue of batched events
+                "watchers": [] # Queue of batched watchers
+            }
+        self.parameters_state = parameters_state
+        self.disable_instance_params = disable_instance_params
+        self.renamed = renamed
+        self.params = {} if params is None else params
+        self.initialized = False
+
+    def __getstate__(self):
+        return {slot: getattr(self, slot) for slot in self.__slots__}
+
+    def __setstate__(self, state):
+        for k, v in state.items():
+            setattr(self, k, v)
+
+
+class _InstancePrivate:
+    """
+    initialized: bool
+        Flag that can be tested to see if e.g. constant Parameters can still be set
+    parameters_state: dict
+        Dict holding some transient states
+    dynamic_watchers: defaultdict
+        Dynamic watchers
+    params: dict
+        Dict of parameter_name:parameter
+    # watchers: dict
+    #     Dict of dict:
+    #         parameter_name:
+    #             parameter_attribute (e.g. 'value'): list of `Watcher`s
+    values: dict
+        Dict of parameter name: value
+    """
+
+    __slots__ = [
+        'initialized',
+        'parameters_state',
+        'dynamic_watchers',
+        'params',
+        # 'watchers',
+        'values',
+    ]
+
+    def __init__(
+        self,
+        initialized=False,
+        parameters_state=None,
+        dynamic_watchers=None,
+        params=None,
+        # watchers=None,
+        values=None,
+    ):
+        self.initialized = initialized
+        if parameters_state is None:
+            parameters_state = {
+                "BATCH_WATCH": False, # If true, Event and watcher objects are queued.
+                "TRIGGER": False,
+                "events": [], # Queue of batched events
+                "watchers": [] # Queue of batched watchers
+            }
+        self.parameters_state = parameters_state
+        self.dynamic_watchers = defaultdict(list) if dynamic_watchers is None else dynamic_watchers
+        self.params = {} if params is None else params
+        # self.watchers = {} if watchers is None else watchers
+        self.values = {} if values is None else values
+
+    def __getstate__(self):
+        return {slot: getattr(self, slot) for slot in self.__slots__}
+
+    def __setstate__(self, state):
+        for k, v in state.items():
+            setattr(self, k, v)
+
 
 class Parameterized(metaclass=ParameterizedMetaclass):
     """
     Base class for named objects that support Parameters and message
     formatting.
 
     Automatic object naming: Every Parameterized instance has a name
@@ -3481,37 +3769,32 @@
 
     name = String(default=None, constant=True, doc="""
         String identifier for this object.""")
 
     def __init__(self, **params):
         global object_count
 
-        # Flag that can be tested to see if e.g. constant Parameters
-        # can still be set
-        self.initialized = False
-        self._parameters_state = {
-            "BATCH_WATCH": False, # If true, Event and watcher objects are queued.
-            "TRIGGER": False,
-            "events": [], # Queue of batched events
-            "watchers": [] # Queue of batched watchers
-        }
-        self._instance__params = {}
+        # Setting a Parameter value in an __init__ block before calling
+        # Parameterized.__init__ (via super() generally) already sets the
+        # _InstancePrivate namespace over the _ClassPrivate namespace
+        # (see Parameter.__set__) so we shouldn't override it here.
+        if not isinstance(self._param__private, _InstancePrivate):
+            self._param__private = _InstancePrivate()
         self._param_watchers = {}
-        self._dynamic_watchers = defaultdict(list)
 
         # Skip generating a custom instance name when a class in the hierarchy
         # has overriden the default of the `name` Parameter.
         if self.param.name.default == self.__class__.__name__:
             self.param._generate_name()
         self.param._setup_params(**params)
         object_count += 1
 
         self.param._update_deps(init=True)
 
-        self.initialized = True
+        self._param__private.initialized = True
 
     @property
     def param(self):
         return Parameters(self.__class__, self=self)
 
     # 'Special' methods
 
@@ -3537,19 +3820,26 @@
 
     def __setstate__(self, state):
         """
         Restore objects from the state dictionary to this object.
 
         During this process the object is considered uninitialized.
         """
-        self.initialized=False
+        self._param__private = _InstancePrivate()
+        self._param__private.initialized = False
+
+        _param__private = state.get('_param__private', None)
+        if _param__private is None:
+            _param__private = _InstancePrivate()
 
         # When making a copy the internal watchers have to be
         # recreated and point to the new instance
+        # if _param__private.watchers:
         if '_param_watchers' in state:
+            # param_watchers = _param__private.watchers
             param_watchers = state['_param_watchers']
             for p, attrs in param_watchers.items():
                 for attr, watchers in attrs.items():
                     new_watchers = []
                     for watcher in watchers:
                         watcher_args = list(watcher)
                         if watcher.inst is not None:
@@ -3558,25 +3848,24 @@
                         if hasattr(fn, '_watcher_name'):
                             watcher_args[2] = _m_caller(self, fn._watcher_name)
                         elif get_method_owner(fn) is watcher.inst:
                             watcher_args[2] = getattr(self, fn.__name__)
                         new_watchers.append(Watcher(*watcher_args))
                     param_watchers[p][attr] = new_watchers
 
-        if '_instance__params' not in state:
-            state['_instance__params'] = {}
         if '_param_watchers' not in state:
             state['_param_watchers'] = {}
+
         state.pop('param', None)
 
         for name,value in state.items():
             setattr(self,name,value)
-        self.initialized=True
+        self._param__private.initialized = True
 
-    @recursive_repr()
+    @_recursive_repr()
     def __repr__(self):
         """
         Provide a nearly valid Python representation that could be used to recreate
         the item with its parameters, if executed in the appropriate environment.
 
         Returns 'classname(parameter1=x,parameter2=y,...)', listing
         all the parameters of this object.
@@ -3588,180 +3877,14 @@
             settings = []
         return self.__class__.__name__ + "(" + ", ".join(settings) + ")"
 
     def __str__(self):
         """Return a short representation of the name and class of this object."""
         return f"<{self.__class__.__name__} {self.name}>"
 
-    # PARAM3_DEPRECATION
-    @_deprecated(extra_msg="Use instead `.param.pprint()`")
-    def script_repr(self,imports=[],prefix="    "):
-        """
-        Deprecated variant of __repr__ designed for generating a runnable script.
-
-        ..deprecated:: 1.12.0
-            Use instead `.param.pprint()`
-        """
-        return self.pprint(imports,prefix, unknown_value=None, qualify=True,
-                           separator="\n")
-
-    @recursive_repr()
-    def _pprint(self, imports=None, prefix=" ", unknown_value='<?>',
-               qualify=False, separator=""):
-        """
-        (Experimental) Pretty printed representation that may be
-        evaluated with eval. See pprint() function for more details.
-        """
-        if imports is None:
-            imports = [] # would have been simpler to use a set from the start
-        imports[:] = list(set(imports))
-
-        # Generate import statement
-        mod = self.__module__
-        bits = mod.split('.')
-        imports.append("import %s"%mod)
-        imports.append("import %s"%bits[0])
-
-        changed_params = self.param.values(onlychanged=script_repr_suppress_defaults)
-        values = self.param.values()
-        spec = getfullargspec(self.__init__)
-        args = spec.args[1:] if spec.args[0] == 'self' else spec.args
-
-        if spec.defaults is not None:
-            posargs = spec.args[:-len(spec.defaults)]
-            kwargs = dict(zip(spec.args[-len(spec.defaults):], spec.defaults))
-        else:
-            posargs, kwargs = args, []
-
-        parameters = self.param.objects('existing')
-        ordering = sorted(
-            sorted(changed_params), # alphanumeric tie-breaker
-            key=lambda k: (- float('inf')  # No precedence is lowest possible precendence
-                           if parameters[k].precedence is None else
-                           parameters[k].precedence))
-
-        arglist, keywords, processed = [], [], []
-        for k in args + ordering:
-            if k in processed: continue
-
-            # Suppresses automatically generated names.
-            if k == 'name' and (values[k] is not None
-                                and re.match('^'+self.__class__.__name__+'[0-9]+$', values[k])):
-                continue
-
-            value = pprint(values[k], imports, prefix=prefix,settings=[],
-                           unknown_value=unknown_value,
-                           qualify=qualify) if k in values else None
-
-            if value is None:
-                if unknown_value is False:
-                    raise Exception(f"{self.name}: unknown value of {k!r}")
-                elif unknown_value is None:
-                    # i.e. suppress repr
-                    continue
-                else:
-                    value = unknown_value
-
-            # Explicit kwarg (unchanged, known value)
-            if (k in kwargs) and (k in values) and kwargs[k] == values[k]: continue
-
-            if k in posargs:
-                # value will be unknown_value unless k is a parameter
-                arglist.append(value)
-            elif (k in kwargs or
-                  (hasattr(spec, 'varkw') and (spec.varkw is not None)) or
-                  (hasattr(spec, 'keywords') and (spec.keywords is not None))):
-                # Explicit modified keywords or parameters in
-                # precendence order (if **kwargs present)
-                keywords.append(f'{k}={value}')
-
-            processed.append(k)
-
-        qualifier = mod + '.'  if qualify else ''
-        arguments = arglist + keywords + (['**%s' % spec.varargs] if spec.varargs else [])
-        return qualifier + '{}({})'.format(self.__class__.__name__,  (','+separator+prefix).join(arguments))
-
-    # PARAM3_DEPRECATION
-    def pprint(self, imports=None, prefix=" ", unknown_value='<?>',
-               qualify=False, separator=""):
-        warnings.warn(
-            message="'pprint' is deprecated. Use instead `.param.pprint`",
-            category=DeprecationWarning,
-            stacklevel=2
-        )
-        return self._pprint(imports=imports, prefix=prefix, unknown_value=unknown_value,
-               qualify=qualify, separator=separator)
-
-    # Note that there's no state_push method on the class, so
-    # dynamic parameters set on a class can't have state saved. This
-    # is because, to do this, state_push() would need to be a
-    # @bothmethod, but that complicates inheritance in cases where we
-    # already have a state_push() method.
-    # (isinstance(g,Parameterized) below is used to exclude classes.)
-
-    # PARAM3_DEPRECATION
-    @_deprecated()
-    def state_push(self):
-        """Save this instance's state.
-
-        ..deprecated:: 2.0.0
-        """
-        return self._state_push()
-
-    def _state_push(self):
-        """
-        Save this instance's state.
-
-        For Parameterized instances, this includes the state of
-        dynamically generated values.
-
-        Subclasses that maintain short-term state should additionally
-        save and restore that state using state_push() and
-        state_pop().
-
-        Generally, this method is used by operations that need to test
-        something without permanently altering the objects' state.
-        """
-        for pname, p in self.param.objects('existing').items():
-            g = self.param.get_value_generator(pname)
-            if hasattr(g,'_Dynamic_last'):
-                g._saved_Dynamic_last.append(g._Dynamic_last)
-                g._saved_Dynamic_time.append(g._Dynamic_time)
-                # CB: not storing the time_fn: assuming that doesn't
-                # change.
-            elif hasattr(g,'state_push') and isinstance(g,Parameterized):
-                g.state_push()
-
-    def state_pop(self):
-        """
-        Restore the most recently saved state.
-
-        ..deprecated:: 2.0.0
-        """
-        return self._state_pop()
-
-    def _state_pop(self):
-        """
-        Restore the most recently saved state.
-
-        See state_push() for more details.
-        """
-        for pname, p in self.param.objects('existing').items():
-            g = self.param.get_value_generator(pname)
-            if hasattr(g,'_Dynamic_last'):
-                g._Dynamic_last = g._saved_Dynamic_last.pop()
-                g._Dynamic_time = g._saved_Dynamic_time.pop()
-            elif hasattr(g,'state_pop') and isinstance(g,Parameterized):
-                g.state_pop()
-
-    @bothmethod
-    @recursive_repr()
-    def _repr_html_(self_or_cls, open=True):
-        return _parameterized_repr_html(self_or_cls, open)
-
 
 def print_all_param_defaults():
     """Print the default values for all imported Parameters."""
     print("_______________________________________________________________________________")
     print("")
     print("                           Parameter Default Values")
     print("")
@@ -3943,41 +4066,27 @@
         state = ParameterizedFunction.__getstate__(self)
         # Here it's necessary to use a function defined at the
         # module level rather than Parameterized.__new__ directly
         # because otherwise pickle will find .__new__'s module to be
         # __main__. Pretty obscure aspect of pickle.py...
         return (_new_parameterized,(self.__class__,),state)
 
-    # PARAM3_DEPRECATION: Remove this compatibility alias for param 2.0 and later; use self.param.pprint instead
-    @_deprecated()
-    def script_repr(self,imports=[],prefix="    "):
-        """
-        Same as Parameterized.script_repr, except that X.classname(Y
-        is replaced with X.classname.instance(Y
-
-        ..deprecated:: 2.0.0
-        """
-        return self.pprint(imports,prefix,unknown_value='',qualify=True,
-                           separator="\n")
-
-
     def _pprint(self, imports=None, prefix="\n    ",unknown_value='<?>',
                 qualify=False, separator=""):
         """
-        Same as Parameterized._pprint, except that X.classname(Y
+        Same as self.param.pprint, except that X.classname(Y
         is replaced with X.classname.instance(Y
         """
-        r = Parameterized._pprint(self,imports,prefix,
-                                  unknown_value=unknown_value,
-                                  qualify=qualify,separator=separator)
+        r = self.param.pprint(imports,prefix,
+                              unknown_value=unknown_value,
+                              qualify=qualify,separator=separator)
         classname=self.__class__.__name__
         return r.replace(".%s("%classname,".%s.instance("%classname)
 
 
-
 class default_label_formatter(ParameterizedFunction):
     "Default formatter to turn parameter names into appropriate widget labels."
 
     capitalize = Parameter(default=True, doc="""
         Whether or not the label should be capitalized.""")
 
     replace_underscores = Parameter(default=True, doc="""
@@ -4017,15 +4126,15 @@
     # than finding them when the class is first created.
 
     # Based on the emulation of PyProperty_Type() in Objects/descrobject.c
 
     def __init__(self, fget=None, fset=None, fdel=None, doc=None):
         warnings.warn(
             message="overridable_property has been deprecated.",
-            category=DeprecationWarning,
+            category=_ParamDeprecationWarning,
             stacklevel=2,
         )
         self.fget = fget
         self.fset = fset
         self.fdel = fdel
         self.__doc__ = doc
```

### Comparing `param-2.0.0a1/param/serializer.py` & `param-2.0.0a2/param/serializer.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/param/version.py` & `param-2.0.0a2/param/version.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testbooleanparam.py` & `param-2.0.0a2/tests/testbooleanparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testbytesparam.py` & `param-2.0.0a2/tests/testbytesparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcalendardateparam.py` & `param-2.0.0a2/tests/testcalendardateparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcalendardaterangeparam.py` & `param-2.0.0a2/tests/testcalendardaterangeparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testclassselector.py` & `param-2.0.0a2/tests/testclassselector.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcolorparameter.py` & `param-2.0.0a2/tests/testcolorparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcomparator.py` & `param-2.0.0a2/tests/testcomparator.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcompositeparams.py` & `param-2.0.0a2/tests/testcompositeparams.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testcustomparam.py` & `param-2.0.0a2/tests/testcustomparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testdateparam.py` & `param-2.0.0a2/tests/testdateparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testdaterangeparam.py` & `param-2.0.0a2/tests/testdaterangeparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testdefaults.py` & `param-2.0.0a2/tests/testdefaults.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testdynamicparams.py` & `param-2.0.0a2/tests/testdynamicparams.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         self.TestPO2.y = 10
         # t6 got a dynamic value, but shouldn't have changed Parameter's instantiate
         self.assertEqual(t8.y, 10)
 
     def test_setting_y_param_numbergen(self):
         self.TestPO2.y=numbergen.UniformRandom()  # now the Parameter instantiate should be true
         t9 = self.TestPO2()
-        self.assertEqual('_y_param_value' in t9.__dict__, True)
+        self.assertEqual('y' in t9._param__private.values, True)
 
     def test_shared_numbergen(self):
         """
         Instances of TestPO2 that don't have their own value for the
         parameter share one UniformRandom object
         """
         self.TestPO2.y=numbergen.UniformRandom()  # now the Parameter instantiate should be true
```

### Comparing `param-2.0.0a1/tests/testfiledeserialization.py` & `param-2.0.0a2/tests/testfiledeserialization.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testfileselector.py` & `param-2.0.0a2/tests/testfileselector.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testipythonmagic.py` & `param-2.0.0a2/tests/testipythonmagic.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testjsonserialization.py` & `param-2.0.0a2/tests/testjsonserialization.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testlist.py` & `param-2.0.0a2/tests/testlist.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testlistselector.py` & `param-2.0.0a2/tests/testlistselector.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testmultifileselector.py` & `param-2.0.0a2/tests/testmultifileselector.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testnumbergen.py` & `param-2.0.0a2/tests/testnumbergen.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testnumberparameter.py` & `param-2.0.0a2/tests/testnumberparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testnumpy.py` & `param-2.0.0a2/tests/testnumpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,7 +69,14 @@
         class Z(param.Parameterized):
             z = param.Array(numpy.array([1]))
 
         _is_array_and_equal(Z.z,[1])
 
         z = Z(z=numpy.array([1,2]))
         _is_array_and_equal(z.z,[1,2])
+
+    def test_array_pprint(self):
+        class MatParam(param.Parameterized):
+            mat = param.Array(numpy.zeros((2, 2)))
+
+        mp = MatParam()
+        mp.param.pprint()
```

### Comparing `param-2.0.0a1/tests/testobjectselector.py` & `param-2.0.0a2/tests/testobjectselector.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 import unittest
 
 from collections import OrderedDict
 
 import param
+import pytest
 
 from .utils import check_defaults
 
 opts=dict(A=[1,2],B=[3,4],C=dict(a=1,b=2))
 
 
 class TestObjectSelectorParameters(unittest.TestCase):
@@ -100,14 +101,59 @@
         assert s2.check_on_set is False
 
     def test_unbound_allow_None_not_dynamic(self):
         s = param.ObjectSelector(objects=[0, 1, 2])
 
         assert s.allow_None is None
 
+    def test_allow_None_set_and_behavior_class(self):
+        class P(param.Parameterized):
+            a = param.ObjectSelector(objects=dict(a=1), allow_None=True)
+            b = param.ObjectSelector(objects=dict(a=1), allow_None=False)
+            c = param.ObjectSelector(default=1, objects=dict(a=1), allow_None=True)
+            d = param.ObjectSelector(default=1, objects=dict(a=1), allow_None=False)
+
+        assert P.param.a.allow_None is True
+        assert P.param.b.allow_None is False
+        assert P.param.c.allow_None is True
+        assert P.param.d.allow_None is False
+
+        P.a = None
+        assert P.a is None
+        with pytest.raises(ValueError):
+            P.b = None
+        P.c = None
+        assert P.c is None
+        with pytest.raises(ValueError):
+            P.d = None
+
+    def test_allow_None_set_and_behavior_instance(self):
+        class P(param.Parameterized):
+            a = param.ObjectSelector(objects=dict(a=1), allow_None=True)
+            b = param.ObjectSelector(objects=dict(a=1), allow_None=False)
+            c = param.ObjectSelector(default=1, objects=dict(a=1), allow_None=True)
+            d = param.ObjectSelector(default=1, objects=dict(a=1), allow_None=False)
+
+        p = P()
+
+        assert p.param.a.allow_None is True
+        assert p.param.b.allow_None is False
+        assert p.param.c.allow_None is True
+        assert p.param.d.allow_None is False
+
+        p.a = None
+        assert p.a is None
+        with pytest.raises(ValueError):
+            p.b = None
+        p.c = None
+        assert p.c is None
+        with pytest.raises(ValueError):
+            p.d = None
+
+
     def test_set_object_constructor(self):
         p = self.P(e=6)
         self.assertEqual(p.e, 6)
 
     def test_allow_None_is_None(self):
         p = self.P()
         assert p.param.e.allow_None is None
```

### Comparing `param-2.0.0a1/tests/testpandas.py` & `param-2.0.0a2/tests/testpandas.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testparamdepends.py` & `param-2.0.0a2/tests/testparamdepends.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,47 @@
 """
 Unit test for param.depends.
 """
 
 import asyncio
-import unittest
 
 import param
 import pytest
 
 from param.parameterized import _parse_dependency_spec
 
 
 def async_executor(func):
+    # Using nest_asyncio to simplify the async_executor implementation
+    nest_asyncio = pytest.importorskip("nest_asyncio")
+    nest_asyncio.apply()
     asyncio.run(func())
 
 
-class TestDependencyParser(unittest.TestCase):
+@pytest.fixture
+def use_async_executor():
+    param.parameterized.async_executor = async_executor
+    try:
+        yield
+    finally:
+        param.parameterized.async_executor = None
+
+
+@pytest.fixture
+def class_name(request):
+    if request.param.startswith('AP'):
+        param.parameterized.async_executor = async_executor
+    try:
+        yield request.param
+    finally:
+        if request.param.startswith('AP'):
+            param.parameterized.async_executor = None
+
+
+class TestDependencyParser:
 
     def test_parameter_value(self):
         obj, attr, what = _parse_dependency_spec('parameter')
         assert obj is None
         assert attr == 'parameter'
         assert what == 'value'
 
@@ -50,15 +72,15 @@
     def test_sub_subobject_parameter_attribute(self):
         obj, attr, what = _parse_dependency_spec('subobject.subsubobject.parameter:constant')
         assert obj == '.subobject.subsubobject'
         assert attr == 'parameter'
         assert what == 'constant'
 
 
-class TestParamDependsSubclassing(unittest.TestCase):
+class TestParamDependsSubclassing:
 
     def test_param_depends_override_depends_subset(self):
 
         class A(param.Parameterized):
             a = param.Parameter()
             b = param.Parameter()
 
@@ -153,17 +175,17 @@
 
         b.a = 'a'
 
         assert values == ['a', 'A']
 
 
 
-class TestParamDepends(unittest.TestCase):
+class TestParamDepends:
 
-    def setUp(self):
+    def setup_method(self):
 
         class P(param.Parameterized):
             a = param.Parameter()
             b = param.Parameter()
 
             single_count = param.Integer()
             attr_count = param.Integer()
@@ -192,22 +214,67 @@
             def nested_attribute(self):
                 self.nested_attr_count += 1
 
             @param.depends('b.param', watch=True)
             def nested(self):
                 self.nested_count += 1
 
+        class AP(param.Parameterized):
+            a = param.Parameter()
+            b = param.Parameter()
+
+            single_count = param.Integer()
+            attr_count = param.Integer()
+            single_nested_count = param.Integer()
+            double_nested_count = param.Integer()
+            nested_attr_count = param.Integer()
+            nested_count = param.Integer()
+
+            @param.depends('a', watch=True)
+            async def single_parameter(self):
+                self.single_count += 1
+
+            @param.depends('a:constant', watch=True)
+            async def constant(self):
+                self.attr_count += 1
+
+            @param.depends('b.a', watch=True)
+            async def single_nested(self):
+                self.single_nested_count += 1
+
+            @param.depends('b.b.a', watch=True)
+            async def double_nested(self):
+                self.double_nested_count += 1
+
+            @param.depends('b.a:constant', watch=True)
+            async def nested_attribute(self):
+                self.nested_attr_count += 1
+
+            @param.depends('b.param', watch=True)
+            async def nested(self):
+                self.nested_count += 1
+
+
         class P2(param.Parameterized):
 
             @param.depends(P.param.a)
             def external_param(self, a):
                 pass
 
+        class AP2(param.Parameterized):
+
+            @param.depends(AP.param.a)
+            async def external_param(self, a):
+                pass
+
+
         self.P = P
+        self.AP = AP
         self.P2 = P2
+        self.AP2 = AP2
 
     def test_param_depends_on_init(self):
         class A(param.Parameterized):
 
             a = param.Parameter()
 
             value = param.Integer()
@@ -239,14 +306,36 @@
             def test(self):
                 self.test_count += 1
 
         b = B(a=A(c=1))
         b.a = A(c=1)
         assert b.test_count == 0
 
+    @pytest.mark.usefixtures("use_async_executor")
+    def test_param_nested_depends_value_unchanged_async(self):
+        class A(param.Parameterized):
+
+            c = param.Parameter()
+
+            d = param.Parameter()
+
+        class B(param.Parameterized):
+
+            a = param.Parameter()
+
+            test_count = param.Integer()
+
+            @param.depends('a.c', 'a.d', watch=True)
+            async def test(self):
+                self.test_count += 1
+
+        b = B(a=A(c=1))
+        b.a = A(c=1)
+        assert b.test_count == 0
+
     def test_param_nested_at_class_definition(self):
 
         class A(param.Parameterized):
 
             c = param.Parameter()
 
             d = param.Parameter()
@@ -271,14 +360,47 @@
 
         b.a = A()
         assert b.test_count == 3
 
         B.a.c = 5
         assert b.test_count == 3
 
+    @pytest.mark.usefixtures("use_async_executor")
+    def test_param_nested_at_class_definition_async(self):
+
+        class A(param.Parameterized):
+
+            c = param.Parameter()
+
+            d = param.Parameter()
+
+        class B(param.Parameterized):
+
+            a = param.Parameter(A())
+
+            test_count = param.Integer()
+
+            @param.depends('a.c', 'a.d', watch=True)
+            async def test(self):
+                self.test_count += 1
+
+        b = B()
+
+        b.a.c = 1
+        assert b.test_count == 1
+
+        b.a.param.update(c=2, d=1)
+        assert b.test_count == 2
+
+        b.a = A()
+        assert b.test_count == 3
+
+        B.a.c = 5
+        assert b.test_count == 3
+
     def test_param_nested_depends_expands(self):
         class A(param.Parameterized):
 
             c = param.Parameter()
 
             d = param.Parameter()
 
@@ -292,14 +414,36 @@
             def test(self):
                 self.test_count += 1
 
         b = B(a=A(c=1, name='A'))
         b.a = A(c=1, name='A')
         assert b.test_count == 0
 
+    @pytest.mark.usefixtures("use_async_executor")
+    def test_param_nested_depends_expands_async(self):
+        class A(param.Parameterized):
+
+            c = param.Parameter()
+
+            d = param.Parameter()
+
+        class B(param.Parameterized):
+
+            a = param.Parameter()
+
+            test_count = param.Integer()
+
+            @param.depends('a.param', watch=True)
+            async def test(self):
+                self.test_count += 1
+
+        b = B(a=A(c=1, name='A'))
+        b.a = A(c=1, name='A')
+        assert b.test_count == 0
+
     def test_param_depends_class_default_dynamic(self):
 
         class A(param.Parameterized):
             c = param.Parameter()
 
         class B(param.Parameterized):
             a = param.Parameter(A())
@@ -314,378 +458,414 @@
 
         b.a.c = 1
         assert b.nested_count == 1
 
         b.a = A()
         assert b.nested_count == 2
 
-    def test_param_instance_depends_dynamic_single_nested(self):
-        inst = self.P()
+    @pytest.mark.usefixtures("use_async_executor")
+    def test_param_depends_class_default_dynamic_async(self):
+
+        class A(param.Parameterized):
+            c = param.Parameter()
+
+        class B(param.Parameterized):
+            a = param.Parameter(A())
+
+            nested_count = param.Integer()
+
+            @param.depends('a.c', watch=True)
+            async def nested(self):
+                self.nested_count += 1
+
+        b = B()
+
+        b.a.c = 1
+        assert b.nested_count == 1
+
+        b.a = A()
+        assert b.nested_count == 2
+
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_single_nested(self, class_name):
+        inst = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('single_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 0)
+        assert len(pinfos) == 0
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('single_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo2 = pinfos[(inst.b, 'a')]
-        self.assertIs(pinfo2.cls, self.P)
-        self.assertIs(pinfo2.inst, inst.b)
-        self.assertEqual(pinfo2.name, 'a')
-        self.assertEqual(pinfo2.what, 'value')
+        assert pinfo2.cls is getattr(self, class_name)
+        assert pinfo2.inst is inst.b
+        assert pinfo2.name == 'a'
+        assert pinfo2.what == 'value'
 
         assert inst.single_nested_count == 1
 
         inst.b.a = 1
         assert inst.single_nested_count == 2
 
-    def test_param_instance_depends_dynamic_single_nested_initialized_no_intermediates(self):
-        init_b = self.P()
-        inst = self.P(b=init_b)
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_single_nested_initialized_no_intermediates(self, class_name):
+        init_b = getattr(self, class_name)()
+        inst = getattr(self, class_name)(b=init_b)
         pinfos = inst.param.method_dependencies('single_nested', intermediate=False)
-        self.assertEqual(len(pinfos), 1)
+        assert len(pinfos) == 1
 
         assert pinfos[0].inst is init_b
         assert pinfos[0].name == 'a'
 
-        new_b = self.P()
+        new_b = getattr(self, class_name)()
         inst.b = new_b
 
         pinfos = inst.param.method_dependencies('single_nested', intermediate=False)
-        self.assertEqual(len(pinfos), 1)
+        assert len(pinfos) == 1
         assert pinfos[0].inst is new_b
         assert pinfos[0].name == 'a'
 
-    def test_param_instance_depends_dynamic_single_nested_initialized_only_intermediates(self):
-        init_b = self.P()
-        inst = self.P(b=init_b)
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_single_nested_initialized_only_intermediates(self, class_name):
+        init_b = getattr(self, class_name)()
+        inst = getattr(self, class_name)(b=init_b)
         pinfos = inst.param.method_dependencies('single_nested', intermediate='only')
-        self.assertEqual(len(pinfos), 1)
+        assert len(pinfos) == 1
 
         assert pinfos[0].inst is inst
         assert pinfos[0].name == 'b'
 
-    def test_param_instance_depends_dynamic_single_nested_initialized(self):
-        init_b = self.P()
-        inst = self.P(b=init_b)
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_single_nested_initialized(self, class_name):
+        init_b = getattr(self, class_name)()
+        inst = getattr(self, class_name)(b=init_b)
         pinfos = inst.param.method_dependencies('single_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('single_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        pinfo.cls is getattr(self, class_name)
+        pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo2 = pinfos[(inst.b, 'a')]
-        self.assertIs(pinfo2.cls, self.P)
-        self.assertIs(pinfo2.inst, inst.b)
-        self.assertEqual(pinfo2.name, 'a')
-        self.assertEqual(pinfo2.what, 'value')
+        pinfo2.cls is getattr(self, class_name)
+        pinfo2.inst is inst.b
+        assert pinfo2.name == 'a'
+        assert pinfo2.what == 'value'
 
         assert inst.single_nested_count == 0
 
         inst.b.a = 1
         assert inst.single_nested_count == 1
 
         # Ensure watcher on initial value does not trigger event
         init_b.a = 2
         assert inst.single_nested_count == 1
 
-    def test_param_instance_depends_dynamic_double_nested(self):
-        inst = self.P()
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_double_nested(self, class_name):
+        inst = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('double_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 0)
+        assert len(pinfos) == 0
 
-        inst.b = self.P(b=self.P())
+        inst.b = getattr(self, class_name)(b=getattr(self, class_name)())
         pinfos = inst.param.method_dependencies('double_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 3)
+        assert len(pinfos) == 3
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo2 = pinfos[(inst.b, 'b')]
-        self.assertIs(pinfo2.cls, self.P)
-        self.assertIs(pinfo2.inst, inst.b)
-        self.assertEqual(pinfo2.name, 'b')
-        self.assertEqual(pinfo2.what, 'value')
+        assert pinfo2.cls is getattr(self, class_name)
+        assert pinfo2.inst is inst.b
+        assert pinfo2.name == 'b'
+        assert pinfo2.what == 'value'
         pinfo3 = pinfos[(inst.b.b, 'a')]
-        self.assertIs(pinfo3.cls, self.P)
-        self.assertIs(pinfo3.inst, inst.b.b)
-        self.assertEqual(pinfo3.name, 'a')
-        self.assertEqual(pinfo3.what, 'value')
+        assert pinfo3.cls is getattr(self, class_name)
+        assert pinfo3.inst is inst.b.b
+        assert pinfo3.name == 'a'
+        assert pinfo3.what == 'value'
 
         assert inst.double_nested_count == 1
 
         inst.b.b.a = 1
         assert inst.double_nested_count == 2
 
         old_subobj = inst.b.b
-        inst.b.b = self.P(a=3)
+        inst.b.b = getattr(self, class_name)(a=3)
         assert inst.double_nested_count == 3
 
         old_subobj.a = 4
         assert inst.double_nested_count == 3
 
-        inst.b.b = self.P(a=3)
+        inst.b.b = getattr(self, class_name)(a=3)
         assert inst.double_nested_count == 3
 
         inst.b.b.a = 4
         assert inst.double_nested_count == 4
 
-        inst.b.b = self.P(a=3)
+        inst.b.b = getattr(self, class_name)(a=3)
         assert inst.double_nested_count == 5
 
-    def test_param_instance_depends_dynamic_double_nested_partially_initialized(self):
-        inst = self.P(b=self.P())
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_double_nested_partially_initialized(self, class_name):
+        inst = getattr(self, class_name)(b=getattr(self, class_name)())
         pinfos = inst.param.method_dependencies('double_nested', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
 
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls == getattr(self, class_name)
+        assert pinfo.inst == inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo = pinfos[(inst.b, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst.b)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls == getattr(self, class_name)
+        assert pinfo.inst == inst.b
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
 
-        inst.b.b = self.P()
+        inst.b.b = getattr(self, class_name)()
         assert inst.double_nested_count == 1
 
         inst.b.b.a = 1
         assert inst.double_nested_count == 2
 
-    def test_param_instance_depends_dynamic_nested_attribute(self):
-        inst = self.P()
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_nested_attribute(self, class_name):
+        inst = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested_attribute', intermediate=True)
-        self.assertEqual(len(pinfos), 0)
+        assert len(pinfos) == 0
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested_attribute', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls == getattr(self, class_name)
+        assert pinfo.inst == inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo2 = pinfos[(inst.b, 'a')]
-        self.assertIs(pinfo2.cls, self.P)
-        self.assertIs(pinfo2.inst, inst.b)
-        self.assertEqual(pinfo2.name, 'a')
-        self.assertEqual(pinfo2.what, 'constant')
+        assert pinfo2.cls == getattr(self, class_name)
+        assert pinfo2.inst == inst.b
+        assert pinfo2.name == 'a'
+        assert pinfo2.what == 'constant'
 
         assert inst.nested_attr_count == 1
 
         inst.b.param.a.constant = True
         assert inst.nested_attr_count == 2
 
-        new_b = self.P()
+        new_b = getattr(self, class_name)()
         new_b.param.a.constant = True
         inst.b = new_b
         assert inst.nested_attr_count == 2
 
-    def test_param_instance_depends_dynamic_nested_attribute_initialized(self):
-        inst = self.P(b=self.P())
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_nested_attribute_initialized(self, class_name):
+        inst = getattr(self, class_name)(b=getattr(self, class_name)())
         pinfos = inst.param.method_dependencies('nested_attribute', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested_attribute', intermediate=True)
-        self.assertEqual(len(pinfos), 2)
+        assert len(pinfos) == 2
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls == getattr(self, class_name)
+        assert pinfo.inst == inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         pinfo2 = pinfos[(inst.b, 'a')]
-        self.assertIs(pinfo2.cls, self.P)
-        self.assertIs(pinfo2.inst, inst.b)
-        self.assertEqual(pinfo2.name, 'a')
-        self.assertEqual(pinfo2.what, 'constant')
+        assert pinfo2.cls == getattr(self, class_name)
+        assert pinfo2.inst == inst.b
+        assert pinfo2.name == 'a'
+        assert pinfo2.what == 'constant'
 
         assert inst.nested_attr_count == 0
 
         inst.b.param.a.constant = True
         assert inst.nested_attr_count == 1
 
-    def test_param_instance_depends_dynamic_nested(self):
-        inst = self.P()
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_nested(self, class_name):
+        inst = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 0)
+        assert len(pinfos) == 0
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         for p in ['a', 'b', 'name', 'nested_count', 'single_count', 'attr_count']:
             pinfo2 = pinfos[(inst.b, p)]
-            self.assertIs(pinfo2.cls, self.P)
-            self.assertIs(pinfo2.inst, inst.b)
-            self.assertEqual(pinfo2.name, p)
-            self.assertEqual(pinfo2.what, 'value')
+            assert pinfo2.cls is getattr(self, class_name)
+            assert pinfo2.inst is inst.b
+            assert pinfo2.name == p
+            assert pinfo2.what == 'value'
 
         assert inst.nested_count == 1
 
         inst.b.a = 1
         assert inst.nested_count == 3
 
-    def test_param_instance_depends_dynamic_nested_initialized(self):
-        init_b = self.P()
-        inst = self.P(b=init_b)
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_nested_initialized(self, class_name):
+        init_b = getattr(self, class_name)()
+        inst = getattr(self, class_name)(b=init_b)
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
 
-        inst.b = self.P()
+        inst.b = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         for p in ['a', 'b', 'name', 'nested_count', 'single_count', 'attr_count']:
             pinfo2 = pinfos[(inst.b, p)]
-            self.assertIs(pinfo2.cls, self.P)
-            self.assertIs(pinfo2.inst, inst.b)
-            self.assertEqual(pinfo2.name, p)
-            self.assertEqual(pinfo2.what, 'value')
+            assert pinfo2.cls is getattr(self, class_name)
+            assert pinfo2.inst is inst.b
+            assert pinfo2.name == p
+            assert pinfo2.what == 'value'
 
         assert inst.single_nested_count == 0
 
         inst.b.a = 1
         assert inst.single_nested_count == 1
 
         # Ensure watcher on initial value does not trigger event
         init_b.a = 2
         assert inst.single_nested_count == 1
 
-    def test_param_instance_depends_dynamic_nested_changed_value(self):
-        init_b = self.P(a=1)
-        inst = self.P(b=init_b)
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends_dynamic_nested_changed_value(self, class_name):
+        init_b = getattr(self, class_name)(a=1)
+        inst = getattr(self, class_name)(b=init_b)
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
 
-        inst.b = self.P(a=2)
+        inst.b = getattr(self, class_name)(a=2)
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         for p in ['a', 'b', 'name', 'nested_count', 'single_count', 'attr_count']:
             pinfo2 = pinfos[(inst.b, p)]
-            self.assertIs(pinfo2.cls, self.P)
-            self.assertIs(pinfo2.inst, inst.b)
-            self.assertEqual(pinfo2.name, p)
-            self.assertEqual(pinfo2.what, 'value')
+            assert pinfo2.cls is getattr(self, class_name)
+            assert pinfo2.inst is inst.b
+            assert pinfo2.name == p
+            assert pinfo2.what == 'value'
 
         assert inst.single_nested_count == 1
 
         inst.b.a = 1
         assert inst.single_nested_count == 2
 
         # Ensure watcher on initial value does not trigger event
         init_b.a = 2
         assert inst.single_nested_count == 2
 
-    def test_param_instance_depends(self):
-        p = self.P()
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_instance_depends(self, class_name):
+        p = getattr(self, class_name)()
         pinfos = p.param.method_dependencies('single_parameter')
-        self.assertEqual(len(pinfos), 1)
+        assert len(pinfos) == 1
         pinfo = pinfos[0]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, p)
-        self.assertEqual(pinfo.name, 'a')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is p
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'value'
 
         p.a = 1
         assert p.single_count == 1
 
-    def test_param_class_depends(self):
-        pinfos = self.P.param.method_dependencies('single_parameter')
-        self.assertEqual(len(pinfos), 1)
-        pinfo = pinfos[0]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, None)
-        self.assertEqual(pinfo.name, 'a')
-        self.assertEqual(pinfo.what, 'value')
-
-    def test_param_class_depends_constant(self):
-        pinfos = self.P.param.method_dependencies('constant')
-        self.assertEqual(len(pinfos), 1)
-        pinfo = pinfos[0]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, None)
-        self.assertEqual(pinfo.name, 'a')
-        self.assertEqual(pinfo.what, 'constant')
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_class_depends(self, class_name):
+        pinfos = getattr(self, class_name).param.method_dependencies('single_parameter')
+        assert len(pinfos) == 1
+        pinfo = pinfos[0]
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is None
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'value'
+
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_class_depends_constant(self, class_name):
+        pinfos = getattr(self, class_name).param.method_dependencies('constant')
+        assert len(pinfos) == 1
+        pinfo = pinfos[0]
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is None
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'constant'
 
-    def test_param_inst_depends_nested(self):
-        inst = self.P(b=self.P())
+    @pytest.mark.parametrize('class_name', ['P', 'AP'], indirect=True)
+    def test_param_inst_depends_nested(self, class_name):
+        inst = getattr(self, class_name)(b=getattr(self, class_name)())
         pinfos = inst.param.method_dependencies('nested')
-        self.assertEqual(len(pinfos), 10)
+        assert len(pinfos) == 10
         pinfos = {(pi.inst, pi.name): pi for pi in pinfos}
         pinfo = pinfos[(inst, 'b')]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, inst)
-        self.assertEqual(pinfo.name, 'b')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name)
+        assert pinfo.inst is inst
+        assert pinfo.name == 'b'
+        assert pinfo.what == 'value'
         for p in ['name', 'a', 'b']:
             info = pinfos[(inst.b, p)]
-            self.assertEqual(info.name, p)
-            self.assertIs(info.inst, inst.b)
+            assert info.name == p
+            assert info.inst is inst.b
 
-    def test_param_external_param_instance(self):
-        inst = self.P2()
+    @pytest.mark.parametrize('class_name', ['P2', 'AP2'], indirect=True)
+    def test_param_external_param_instance(self, class_name):
+        inst = getattr(self, class_name)()
         pinfos = inst.param.method_dependencies('external_param')
         pinfo = pinfos[0]
-        self.assertIs(pinfo.cls, self.P)
-        self.assertIs(pinfo.inst, None)
-        self.assertEqual(pinfo.name, 'a')
-        self.assertEqual(pinfo.what, 'value')
+        assert pinfo.cls is getattr(self, class_name[:-1])
+        assert pinfo.inst is None
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'value'
 
+    @pytest.mark.usefixtures('use_async_executor')
     def test_async(self):
-        try:
-            param.parameterized.async_executor = async_executor
-            class P(param.Parameterized):
-                a = param.Parameter()
-                single_count = param.Integer()
-
-                @param.depends('a', watch=True)
-                async def single_parameter(self):
-                    self.single_count += 1
-
-            inst = P()
-            inst.a = 'test'
-            assert inst.single_count == 1
-        finally:
-            param.parameterized.async_executor = None
+        class P(param.Parameterized):
+            a = param.Parameter()
+            single_count = param.Integer()
+
+            @param.depends('a', watch=True)
+            async def single_parameter(self):
+                self.single_count += 1
+
+        inst = P()
+        inst.a = 'test'
+        assert inst.single_count == 1
 
     def test_param_depends_on_parameterized_attribute(self):
         # Issue https://github.com/holoviz/param/issues/635
 
         called = []
 
         class Sub(param.Parameterized):
@@ -703,14 +883,39 @@
                 called.append(1)
 
         p = P()
         p.test_param = 'modified'
 
         assert not called
 
+    @pytest.mark.usefixtures('use_async_executor')
+    def test_param_depends_on_parameterized_attribute_async(self):
+        # Issue https://github.com/holoviz/param/issues/635
+
+        called = []
+
+        class Sub(param.Parameterized):
+            s = param.String()
+
+        class P(param.Parameterized):
+            test_param = param.Parameter()
+
+            def __init__(self, **params):
+                self._sub = Sub()
+                super().__init__(**params)
+
+            @param.depends('_sub.s', watch=True)
+            async def cb(self):
+                called.append(1)
+
+        p = P()
+        p.test_param = 'modified'
+
+        assert not called
+
     def test_param_depends_on_method(self):
 
         method_count = 0
 
         class A(param.Parameterized):
             a = param.Integer()
 
@@ -732,14 +937,44 @@
         assert pinfo.inst is inst
         assert pinfo.name == 'a'
         assert pinfo.what == 'value'
 
         inst.a = 2
         assert method_count == 1
 
+    @pytest.mark.usefixtures('use_async_executor')
+    def test_param_depends_on_method_async(self):
+
+        method_count = 0
+
+        class A(param.Parameterized):
+            a = param.Integer()
+
+            @param.depends('a', watch=True)
+            async def method1(self):
+                pass
+
+            @param.depends('method1', watch=True)
+            async def method2(self):
+                nonlocal method_count
+                method_count += 1
+
+        inst = A()
+        pinfos = inst.param.method_dependencies('method2')
+        assert len(pinfos) == 1
+
+        pinfo = pinfos[0]
+        assert pinfo.cls is A
+        assert pinfo.inst is inst
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'value'
+
+        inst.a = 2
+        assert method_count == 1
+
     def test_param_depends_on_method_subparameter(self):
 
         method1_count = 0
         method2_count = 0
 
         class Sub(param.Parameterized):
             a = param.Integer()
@@ -768,14 +1003,50 @@
         assert pinfo.name == 'a'
         assert pinfo.what == 'value'
 
         sub.a = 2
         assert method1_count == 0
         assert method2_count == 1
 
+    @pytest.mark.usefixtures('use_async_executor')
+    def test_param_depends_on_method_subparameter_async(self):
+
+        method1_count = 0
+        method2_count = 0
+
+        class Sub(param.Parameterized):
+            a = param.Integer()
+
+            @param.depends('a')
+            async def method1(self):
+                nonlocal method1_count
+                method1_count += 1
+
+        class Main(param.Parameterized):
+            sub = param.Parameter()
+
+            @param.depends('sub.method1', watch=True)
+            async def method2(self):
+                nonlocal method2_count
+                method2_count += 1
+
+        sub = Sub()
+        main = Main(sub=sub)
+        pinfos = main.param.method_dependencies('method2')
+        assert len(pinfos) == 1
+
+        pinfo = pinfos[0]
+        assert pinfo.cls is Sub
+        assert pinfo.inst is sub
+        assert pinfo.name == 'a'
+        assert pinfo.what == 'value'
+
+        sub.a = 2
+        assert method1_count == 0
+        assert method2_count == 1
 
     def test_param_depends_on_method_subparameter_after_init(self):
         # Setup inspired from https://github.com/holoviz/param/issues/764
 
         method1_count = 0
         method2_count = 0
 
@@ -816,14 +1087,62 @@
         assert pinfo.what == 'value'
 
         explorer.x = 'b'
 
         assert method1_count == 0
         assert method2_count == 1
 
+    @pytest.mark.usefixtures('use_async_executor')
+    def test_param_depends_on_method_subparameter_after_init_async(self):
+        # Setup inspired from https://github.com/holoviz/param/issues/764
+
+        method1_count = 0
+        method2_count = 0
+
+        class Controls(param.Parameterized):
+
+            explorer = param.Parameter()
+
+            @param.depends('explorer.method1', watch=True)
+            async def method2(self):
+                nonlocal method2_count
+                method2_count += 1
+
+
+        class Explorer(param.Parameterized):
+
+            controls = param.Parameter()
+
+            x = param.Selector(objects=['a', 'b'])
+
+            def __init__(self, **params):
+                super().__init__(**params)
+                self.controls = Controls(explorer=self)
+
+            @param.depends('x')
+            async def method1(self):
+                nonlocal method1_count
+                method1_count += 1
+
+        explorer = Explorer()
+
+        pinfos = explorer.controls.param.method_dependencies('method2')
+        assert len(pinfos) == 1
+
+        pinfo = pinfos[0]
+        assert pinfo.cls is Explorer
+        assert pinfo.inst is explorer
+        assert pinfo.name == 'x'
+        assert pinfo.what == 'value'
+
+        explorer.x = 'b'
+
+        assert method1_count == 0
+        assert method2_count == 1
+
     def test_param_depends_class_with_len(self):
         # https://github.com/holoviz/param/issues/747
 
         count = 0
 
         class P(param.Parameterized):
             x = param.Parameter()
@@ -837,18 +1156,44 @@
             def __len__(self):
                 return 0
 
         p = P()
         p.x = 1
         assert count == 1
 
+    def test_param_depends_subobject_before_super_init(self):
+        count = 0
+
+        class X(param.Parameterized):
+            p = param.Parameter()
 
-class TestParamDependsFunction(unittest.TestCase):
+        class Y(param.Parameterized):
 
-    def setUp(self):
+            def __init__(self, **params):
+                self.x = X()
+                super().__init__(**params)
+
+            # Check that creating this class doesn't error when resolving x.p
+            @param.depends('x.p')
+            def cb(self):
+                nonlocal count
+                count += 1
+
+        y = Y()
+        pinfos = y.param.method_dependencies('cb')
+        assert len(pinfos) == 1
+        pinfo = pinfos[0]
+        assert pinfo.inst == y.x
+        assert pinfo.cls == X
+        assert pinfo.name == 'p'
+
+
+class TestParamDependsFunction:
+
+    def setup_method(self):
         class P(param.Parameterized):
             a = param.Parameter()
             b = param.Parameter()
 
 
         self.P = P
 
@@ -861,91 +1206,94 @@
 
         dependencies = {
             'dependencies': (p.param.a,),
             'kw': {'c': p.param.b},
             'watch': False,
             'on_init': False
         }
-        self.assertEqual(function._dinfo, dependencies)
+        assert function._dinfo == dependencies
 
     def test_param_depends_function_class_params(self):
         p = self.P
 
         @param.depends(p.param.a, c=p.param.b)
         def function(value, c):
             pass
 
         dependencies = {
             'dependencies': (p.param.a,),
             'kw': {'c': p.param.b},
             'watch': False,
             'on_init': False
         }
-        self.assertEqual(function._dinfo, dependencies)
+        assert function._dinfo == dependencies
 
     def test_param_depends_function_instance_params_watch(self):
         p = self.P(a=1, b=2)
 
         d = []
 
         @param.depends(p.param.a, c=p.param.b, watch=True)
         def function(value, c):
             d.append(value+c)
 
         p.a = 2
-        self.assertEqual(d, [4])
+        assert d == [4]
         p.b = 3
-        self.assertEqual(d, [4, 5])
+        assert d == [4, 5]
 
     def test_param_depends_function_class_params_watch(self):
         p = self.P
         p.a = 1
         p.b = 2
 
         d = []
 
         @param.depends(p.param.a, c=p.param.b, watch=True)
         def function(value, c):
             d.append(value+c)
 
         p.a = 2
-        self.assertEqual(d, [4])
+        assert d == [4]
         p.b = 3
-        self.assertEqual(d, [4, 5])
+        assert d == [4, 5]
 
+    @pytest.mark.usefixtures('use_async_executor')
     def test_async(self):
-        try:
-            param.parameterized.async_executor = async_executor
-            p = self.P(a=1)
+        p = self.P(a=1)
 
-            d = []
+        d = []
 
-            @param.depends(p.param.a, watch=True)
-            async def function(value):
-                d.append(value)
+        @param.depends(p.param.a, watch=True)
+        async def function(value):
+            d.append(value)
 
-            p.a = 2
+        p.a = 2
 
-            assert d == [2]
-        finally:
-            param.parameterized.async_executor = None
+        assert d == [2]
 
 
 def test_misspelled_parameter_in_depends():
-    class Example(param.Parameterized):
-        xlim = param.Range((0, 10), bounds=(0, 100))
+    with pytest.raises(AttributeError, match="Attribute 'tlim' could not be resolved on"):
+        class Example(param.Parameterized):
+            xlim = param.Range((0, 10), bounds=(0, 100))
 
-        @param.depends("tlim")  # <- Misspelled xlim
-        def test(self):
-            return True
+            @param.depends("tlim")  # <- Misspelled xlim
+            def test(self):
+                return True
 
-    example = Example()
-    with pytest.raises(AttributeError, match="Attribute 'tlim' could not be resolved on"):
-        # Simulating: pn.panel(example.test)
-        example.param.method_dependencies(example.test.__name__)
+
+def test_misspelled_parameter_in_depends_non_Parameter():
+    with pytest.raises(AttributeError, match="Attribute 'foo' could not be resolved on"):
+        class Example(param.Parameterized):
+            foo = 1
+
+            @param.depends("foo")  # <- Not a Parameter
+            def test(self):
+                return True
 
 
 def test_misspelled_parameter_in_depends_watch():
     with pytest.raises(AttributeError, match="Attribute 'tlim' could not be resolved on"):
         class Example(param.Parameterized):
             xlim = param.Range((0, 10), bounds=(0, 100))
```

### Comparing `param-2.0.0a1/tests/testparameterizedobject.py` & `param-2.0.0a2/tests/testparameterizedobject.py`

 * *Files 18% similar despite different names*

```diff
@@ -259,71 +259,56 @@
         class B(param.Parameterized):
             name = param.String(default='BB')
 
         class C(A, B): pass
 
         assert C.name == 'AA'
 
+    def test_constant_parameter_modify_class_before(self):
+        """Test you can set on class and the new default is picked up
+        by new instances"""
+        TestPO.const=9
+        testpo = TestPO()
+        self.assertEqual(testpo.const,9)
+
+    def test_constant_parameter_modify_class_after_init(self):
+        """Test that setting the value on the class doesn't update the instance value
+        even when the instance value hasn't yet been set"""
+        oobj = []
+        class P(param.Parameterized):
+            x = param.Parameter(default=oobj, constant=True)
+
+        p1 = P()
+
+        P.x = nobj = [0]
+        assert P.x is nobj
+        assert p1.x == oobj
+        assert p1.x is oobj
+
+        p2 = P()
+        assert p2.x == nobj
+        assert p2.x is nobj
+
+    def test_constant_parameter_after_init(self):
+        """Test that you can't set a constant parameter after construction."""
+        testpo = TestPO(const=17)
+        self.assertEqual(testpo.const,17)
+        self.assertRaises(TypeError,setattr,testpo,'const',10)
+
     def test_constant_parameter(self):
         """Test that you can't set a constant parameter after construction."""
         testpo = TestPO(const=17)
         self.assertEqual(testpo.const,17)
         self.assertRaises(TypeError,setattr,testpo,'const',10)
 
         # check you can set on class
         TestPO.const=9
         testpo = TestPO()
         self.assertEqual(testpo.const,9)
 
-    def test_parameter_constant_instantiate(self):
-        # instantiate is automatically set to True when constant=True
-        assert TestPO.param.const.instantiate is True
-
-        class C(param.Parameterized):
-            # instantiate takes precedence when True
-            a = param.Parameter(instantiate=True, constant=False)
-            b = param.Parameter(instantiate=False, constant=False)
-            c = param.Parameter(instantiate=False, constant=True)
-            d = param.Parameter(constant=True)
-            e = param.Parameter(constant=False)
-            f = param.Parameter()
-
-        assert C.param.a.constant is False
-        assert C.param.a.instantiate is True
-        assert C.param.b.constant is False
-        assert C.param.b.instantiate is False
-        assert C.param.c.constant is True
-        assert C.param.c.instantiate is True
-        assert C.param.d.constant is True
-        assert C.param.d.instantiate is True
-        assert C.param.e.constant is False
-        assert C.param.e.instantiate is False
-        assert C.param.f.constant is False
-        assert C.param.f.instantiate is False
-
-    def test_parameter_constant_instantiate_subclass(self):
-
-        obj = object()
-
-        class A(param.Parameterized):
-            x = param.Parameter(obj)
-
-        class B(param.Parameterized):
-            x = param.Parameter(constant=True)
-
-        assert A.param.x.constant is False
-        assert A.param.x.instantiate is False
-        assert B.param.x.constant is True
-        assert B.param.x.instantiate is True
-
-        a = A()
-        b = B()
-        assert a.x is obj
-        assert b.x is not obj
-
     def test_readonly_parameter(self):
         """Test that you can't set a read-only parameter on construction or as an attribute."""
         testpo = TestPO()
         self.assertEqual(testpo.ro,"Hello")
 
         with self.assertRaises(TypeError):
             t = TestPO(ro=20)
@@ -389,27 +374,171 @@
     def test_remove_class_param_validation(self):
         test = TestPOValidation()
         test.param.value.bounds = None
         test.value = 20
         with self.assertRaises(ValueError):
             TestPOValidation.value = 10
 
+    def test_instantiation_set_before_super(self):
+        count = 0
+        class P(param.Parameterized):
+
+            x = param.Parameter(0)
+
+            def __init__(self, x=1):
+                self.x = x
+                super().__init__()
+
+            @param.depends('x', watch=True)
+            def cb(self):
+                nonlocal count
+                count += 1
+
+        p = P()
+
+        assert p.x == 1
+        assert count == 0
+
+    def test_instantiation_set_before_super_contrived(self):
+        # https://github.com/holoviz/param/pull/790#discussion_r1263483293
+        class P(param.Parameterized):
+
+            value = param.String(default="A")
+
+            def __init__(self, depth=0):
+                self.value = 'B'
+                if depth < 2:
+                    self.sub = P(depth+1)
+                super().__init__()
+
+        p = P()
+
+        assert p.value == 'B'
+        assert p.sub.value == 'B'
+
+    def test_instantiation_set_before_super_subclass(self):
+        # Inspired by a HoloViews use case (GenericElementPlot, GenericOverlayPlot)
+        class A(param.Parameterized):
+
+            def __init__(self, batched=False, **params):
+                self.batched = batched
+                super().__init__(**params)
+
+        class B(A):
+
+            batched = param.Boolean()
+
+            def __init__(self, batched=True, **params):
+                super().__init__(batched=batched, **params)
+
+        a = A()
+        assert a.batched is False
+
+        # When b is instantiated the `batched` Parameter of B is set before
+        # Parameterized.__init__ is called.
+        b = B()
+        assert b.batched is True
+
+    def test_instantiation_param_objects_before_super_subclass(self):
+        # Testing https://github.com/holoviz/param/pull/420
+
+
+        class P(param.Parameterized):
+            x = param.Parameter()
+
+            def __init__(self):
+                objs = self.param.objects(instance='existing')
+                assert isinstance(objs, dict)
+                super().__init__()
+
+        P()
+
+    @pytest.mark.xfail(
+        raises=AttributeError,
+        reason='Behavior not defined when setting a constant parameter before calling super()',
+    )
+    def test_instantiation_set_before_super_constant(self):
+        count = 0
+        class P(param.Parameterized):
+
+            x = param.Parameter(0, constant=True)
+
+            def __init__(self, x=1):
+                self.x = x
+                super().__init__()
+
+            @param.depends('x', watch=True)
+            def cb(self):
+                nonlocal count
+                count += 1
+
+        p = P()
+
+        assert p.x == 1
+        assert count == 0
+
+    def test_instantiation_set_before_super_readonly(self):
+        class P(param.Parameterized):
+
+            x = param.Parameter(0, readonly=True)
+
+            def __init__(self, x=1):
+                self.x = x
+                super().__init__()
+
+        with pytest.raises(TypeError, match="Read-only parameter 'x' cannot be modified"):
+            P()
+
+    def test_parameter_constant_iadd_allowed(self):
+        # Testing https://github.com/holoviz/param/pull/400
+        class P(param.Parameterized):
+
+            list = param.List([], constant=True)
+
+        p = P()
+        p.list += [1, 2, 3]
+
+        # Just to make sure that normal setting is still forbidden
+        with pytest.raises(TypeError, match="Constant parameter 'list' cannot be modified"):
+            p.list = [0]
+
+    def test_parameter_constant_same_notallowed(self):
+        L = [0, 1]
+        class P(param.Parameterized):
+
+            list = param.List(L, constant=True)
+
+        p = P()
+
+        # instantiate is set to true internally so a deepcopy is made of L,
+        # it's no longer the same object
+        with pytest.raises(TypeError, match="Constant parameter 'list' cannot be modified"):
+            p.list = L
+
     def test_values(self):
         """Basic tests of params() method."""
 
         # CB: test not so good because it requires changes if params
         # of PO are changed
         assert 'name' in param.Parameterized.param.values()
         assert len(param.Parameterized.param.values()) in [1,2]
 
         ## check for bug where subclass Parameters were not showing up
         ## if values() already called on a super class.
         assert 'inst' in TestPO.param.values()
         assert 'notinst' in TestPO.param.values()
 
+    def test_values_name_ignored_for_instances_and_onlychanged(self):
+        default_inst = param.Parameterized()
+        assert 'Parameterized' in default_inst.name
+        # name ignored when automatically computed (behavior inherited from all_equal)
+        assert 'name' not in default_inst.param.values(onlychanged=True)
+        # name not ignored when set
+        assert param.Parameterized(name='foo').param.values(onlychanged=True)['name'] == 'foo'
+
     def test_param_iterator(self):
         self.assertEqual(set(TestPO.param), {'name', 'inst', 'notinst', 'const', 'dyn',
                                              'ro', 'ro2', 'ro_label', 'ro_format'})
 
     def test_param_contains(self):
         for p in ['name', 'inst', 'notinst', 'const', 'dyn', 'ro', 'ro2']:
             self.assertIn(p, TestPO.param)
@@ -494,18 +623,18 @@
 
     def test_state_saving(self):
         t = TestPO(dyn=_SomeRandomNumbers())
         g = t.param.get_value_generator('dyn')
         g._Dynamic_time_fn=None
         assert t.dyn!=t.dyn
         orig = t.dyn
-        t._state_push()
+        t.param._state_push()
         t.dyn
         assert t.param.inspect_value('dyn')!=orig
-        t.state_pop()
+        t.param._state_pop()
         assert t.param.inspect_value('dyn')==orig
 
     def test_label(self):
         t = TestPO()
         assert t.param['ro_label'].label == 'Ro Label'
 
     def test_label_set(self):
@@ -531,14 +660,182 @@
         param.parameterized.label_formatter = default_label_formatter
 
     def test_error_if_non_param_in_constructor(self):
         msg = "TestPO.__init__() got an unexpected keyword argument 'not_a_param'"
         with pytest.raises(TypeError, match=re.escape(msg)):
             TestPO(not_a_param=2)
 
+    def test_update_class(self):
+        class P(param.Parameterized):
+            x = param.Parameter()
+
+        p = P()
+
+        P.param.update(x=10)
+
+        assert P.x == p.x == 10
+
+    def test_update_context_class(self):
+        class P(param.Parameterized):
+            x = param.Parameter(10)
+
+        p = P()
+
+        with P.param.update(x=20):
+            assert P.x == p.x == 20
+
+        assert P.x == p.x == 10
+
+    def test_update_class_watcher(self):
+        class P(param.Parameterized):
+            x = param.Parameter()
+
+        events = []
+        P.param.watch(events.append, 'x')
+
+        P.param.update(x=10)
+
+        assert len(events) == 1
+        assert events[0].name == 'x' and events[0].new == 10
+
+    def test_update_context_class_watcher(self):
+        class P(param.Parameterized):
+            x = param.Parameter(0)
+
+        events = []
+        P.param.watch(events.append, 'x')
+
+        with P.param.update(x=20):
+            pass
+
+        assert len(events) == 2
+        assert events[0].name == 'x' and events[0].new == 20
+        assert events[1].name == 'x' and events[1].new == 0
+
+    def test_update_instance_watcher(self):
+        class P(param.Parameterized):
+            x = param.Parameter()
+
+        p = P()
+
+        events = []
+        p.param.watch(events.append, 'x')
+
+        p.param.update(x=10)
+
+        assert len(events) == 1
+        assert events[0].name == 'x' and events[0].new == 10
+
+    def test_update_context_instance_watcher(self):
+        class P(param.Parameterized):
+            x = param.Parameter(0)
+
+        p = P()
+
+        events = []
+        p.param.watch(events.append, 'x')
+
+        with p.param.update(x=20):
+            pass
+
+        assert len(events) == 2
+        assert events[0].name == 'x' and events[0].new == 20
+        assert events[1].name == 'x' and events[1].new == 0
+
+    def test_update_error_not_param_class(self):
+        with pytest.raises(ValueError, match="'not_a_param' is not a parameter of TestPO"):
+            TestPO.param.update(not_a_param=1)
+
+    def test_update_error_not_param_instance(self):
+        t = TestPO(inst='foo')
+        with pytest.raises(ValueError, match="'not_a_param' is not a parameter of TestPO"):
+            t.param.update(not_a_param=1)
+
+    def test_update_context_error_not_param_class(self):
+        with pytest.raises(ValueError, match="'not_a_param' is not a parameter of TestPO"):
+            with TestPO.param.update(not_a_param=1):
+                pass
+
+    def test_update_context_error_not_param_instance(self):
+        t = TestPO(inst='foo')
+        with pytest.raises(ValueError, match="'not_a_param' is not a parameter of TestPO"):
+            with t.param.update(not_a_param=1):
+                pass
+
+    def test_update_error_while_updating(self):
+        class P(param.Parameterized):
+            x = param.Parameter(0, readonly=True)
+
+        with pytest.raises(TypeError):
+            P.param.update(x=1)
+
+        assert P.x == 0
+
+        with pytest.raises(TypeError):
+            with P.param.update(x=1):
+                pass
+
+        assert P.x == 0
+
+        p = P()
+
+        with pytest.raises(TypeError):
+            p.param.update(x=1)
+
+        assert p.x == 0
+
+        with pytest.raises(TypeError):
+            with p.param.update(x=1):
+                pass
+
+        assert p.x == 0
+
+    def test_update_error_dict_and_kwargs_instance(self):
+        t = TestPO(inst='foo')
+        with pytest.raises(ValueError, match=re.escape("TestPO.param.update accepts *either* an iterable or key=value pairs, not both")):
+            t.param.update(dict(a=1), a=1)
+
+    def test_update_context_error_dict_and_kwargs_instance(self):
+        t = TestPO(inst='foo')
+        with pytest.raises(ValueError, match=re.escape("TestPO.param.update accepts *either* an iterable or key=value pairs, not both")):
+            with t.param.update(dict(a=1), a=1):
+                pass
+
+    def test_update_error_dict_and_kwargs_class(self):
+        with pytest.raises(ValueError, match=re.escape("TestPO.param.update accepts *either* an iterable or key=value pairs, not both")):
+            TestPO.param.update(dict(a=1), a=1)
+
+    def test_update_context_error_dict_and_kwargs_class(self):
+        with pytest.raises(ValueError, match=re.escape("TestPO.param.update accepts *either* an iterable or key=value pairs, not both")):
+            with TestPO.param.update(dict(a=1), a=1):
+                pass
+
+    def test_update_context_single_parameter(self):
+        t = TestPO(inst='foo')
+        with t.param.update(inst='bar'):
+            assert t.inst == 'bar'
+        assert t.inst == 'foo'
+
+    def test_update_context_does_not_set_other_params(self):
+        t = TestPO(inst='foo')
+        events = []
+        t.param.watch(events.append, list(t.param), onlychanged=False)
+        with t.param.update(inst='bar'):
+            pass
+        assert len(events) == 2
+        assert all(e.name == 'inst' for e in events)
+
+    def test_update_context_multi_parameter(self):
+        t = TestPO(inst='foo', notinst=1)
+        with t.param.update(inst='bar', notinst=2):
+            assert t.inst == 'bar'
+            assert t.notinst == 2
+        assert t.inst == 'foo'
+        assert t.notinst == 1
+
 
 class some_fn(param.ParameterizedFunction):
     __test__ = False
 
     num_phase = param.Number(18)
     frequencies = param.List([99])
     scale = param.Number(0.3)
@@ -1032,7 +1329,66 @@
         def __init__(self, foo=param.Undefined, **params):
             super().__init__(**params)
             self.foo = foo
 
     with pytest.raises(KeyError, match="Slot 'foo' of parameter 'c' has no default value defined in `_slot_defaults`"):
         class A(param.Parameterized):
             c = CustomParameter()
+
+
+def _dir(obj):
+    return [attr for attr in dir(obj) if not attr.startswith('__')]
+
+
+def test_namespace_class():
+
+    class P(param.Parameterized):
+        x = param.Parameter()
+
+        @param.depends('x', watch=True)
+        def foo(self): pass
+
+    P.x = 1
+    P.param.x
+
+    assert _dir(P) == [
+        '_param__parameters',
+        '_param__private',
+        'foo',
+        'name',
+        'param',
+        'x'
+    ]
+
+
+def test_namespace_inst():
+
+    class P(param.Parameterized):
+        x = param.Parameter()
+
+        @param.depends('x', watch=True)
+        def foo(self): pass
+
+    p = P(x=2)
+    p.param.x
+
+    assert _dir(p) == [
+        '_param__parameters',
+        '_param__private',
+        '_param_watchers',
+        'foo',
+        'name',
+        'param',
+        'x'
+    ]
+
+
+def test_parameterized_access_param_before_super():
+    class P(param.Parameterized):
+        x = param.Parameter(1)
+
+        def __init__(self, **params):
+            # Reaching out to a Parameter default before calling super
+            assert self.x == 1
+            super().__init__(**params)
+
+    P()
```

### Comparing `param-2.0.0a1/tests/testparamoutput.py` & `param-2.0.0a2/tests/testparamoutput.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testparamunion.py` & `param-2.0.0a2/tests/testparamunion.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testpathparam.py` & `param-2.0.0a2/tests/testpathparam.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import tempfile
 import unittest
 
 import param
 import pytest
 
-from .utils import check_defaults
+from .utils import warnings_as_excepts, check_defaults
 
 
 class TestPathParameters(unittest.TestCase):
 
     def setUp(self):
         super().setUp()
 
@@ -76,15 +76,16 @@
         assert p.a == self.fa
 
     def test_set_to_None_allowed(self):
         p = self.P()
 
         assert p.param.b.allow_None is False
         # This should probably raise an error (#708)
-        p.b = None
+        with warnings_as_excepts(match='None is not allowed'):
+            p.b = None
 
     def test_search_paths(self):
         p = self.P()
 
         assert isinstance(p.c, str)
         assert os.path.isfile(p.c)
         assert os.path.isabs(p.c)
@@ -185,15 +186,16 @@
         assert p.a == self.fa
 
     def test_set_to_None_allowed(self):
         p = self.P()
 
         assert p.param.b.allow_None is False
         # This should probably raise an error (#708)
-        p.b = None
+        with warnings_as_excepts(match='None is not allowed'):
+            p.b = None
 
     def test_search_paths(self):
         p = self.P()
 
         assert isinstance(p.c, str)
         assert os.path.isfile(p.c)
         assert os.path.isabs(p.c)
@@ -264,15 +266,16 @@
         assert p.a == self.da
 
     def test_set_to_None_allowed(self):
         p = self.P()
 
         assert p.param.b.allow_None is False
         # This should probably raise an error (#708)
-        p.b = None
+        with warnings_as_excepts(match='None is not allowed'):
+            p.b = None
 
     def test_search_paths(self):
         p = self.P()
 
         assert isinstance(p.c, str)
         assert os.path.isdir(p.c)
         assert os.path.isabs(p.c)
```

### Comparing `param-2.0.0a1/tests/testrangeparameter.py` & `param-2.0.0a2/tests/testrangeparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testselector.py` & `param-2.0.0a2/tests/testselector.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 testEnumerationParameter.txt
 """
 import unittest
 
 from collections import OrderedDict
 
 import param
+import pytest
 
-from.utils import check_defaults
+from .utils import check_defaults
 
 opts=dict(A=[1,2],B=[3,4],C=dict(a=1,b=2))
 
 
 class TestSelectorParameters(unittest.TestCase):
 
     def setUp(self):
@@ -99,14 +100,58 @@
         assert p.param.f.allow_None is None
         assert p.param.g.allow_None is None
         assert p.param.h.allow_None is None
         assert p.param.i.allow_None is None
         assert p.param.s.allow_None is None
         assert p.param.d.allow_None is None
 
+    def test_allow_None_set_and_behavior_class(self):
+        class P(param.Parameterized):
+            a = param.Selector(objects=dict(a=1), allow_None=True)
+            b = param.Selector(objects=dict(a=1), allow_None=False)
+            c = param.Selector(default=1, objects=dict(a=1), allow_None=True)
+            d = param.Selector(default=1, objects=dict(a=1), allow_None=False)
+
+        assert P.param.a.allow_None is True
+        assert P.param.b.allow_None is False
+        assert P.param.c.allow_None is True
+        assert P.param.d.allow_None is False
+
+        P.a = None
+        assert P.a is None
+        with pytest.raises(ValueError):
+            P.b = None
+        P.c = None
+        assert P.c is None
+        with pytest.raises(ValueError):
+            P.d = None
+
+    def test_allow_None_set_and_behavior_instance(self):
+        class P(param.Parameterized):
+            a = param.Selector(objects=dict(a=1), allow_None=True)
+            b = param.Selector(objects=dict(a=1), allow_None=False)
+            c = param.Selector(default=1, objects=dict(a=1), allow_None=True)
+            d = param.Selector(default=1, objects=dict(a=1), allow_None=False)
+
+        p = P()
+
+        assert p.param.a.allow_None is True
+        assert p.param.b.allow_None is False
+        assert p.param.c.allow_None is True
+        assert p.param.d.allow_None is False
+
+        p.a = None
+        assert p.a is None
+        with pytest.raises(ValueError):
+            p.b = None
+        p.c = None
+        assert p.c is None
+        with pytest.raises(ValueError):
+            p.d = None
+
     def test_autodefault(self):
         class P(param.Parameterized):
             o1 = param.Selector(objects=[6, 7])
             o2 = param.Selector(objects={'a': 1, 'b': 2})
 
         assert P.o1 == 6
         assert P.o2 == 1
@@ -333,7 +378,17 @@
         assert B.param.p.check_on_set is True
 
         b = B()
 
         assert b.param.p.objects == [0, 1]
         assert b.param.p.default == 1
         assert b.param.p.check_on_set is True
+
+    def test_no_instantiate_when_constant(self):
+        # https://github.com/holoviz/param/issues/287
+        objs = [object(), object()]
+
+        class A(param.Parameterized):
+            p = param.Selector(default=objs[0], objects=objs, constant=True)
+
+        a = A()
+        assert a.p is objs[0]
```

### Comparing `param-2.0.0a1/tests/testsignatures.py` & `param-2.0.0a2/tests/testsignatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,21 @@
                 for p in parameters.values()
             )
 
 
 def test_signature_warning_by_position():
     # Simple test as it's tricky to automatically test all the Parameters
     with pytest.warns(
-        PendingDeprecationWarning,
+        param._utils.ParamPendingDeprecationWarning,
         match=r"Passing 'objects' as positional argument\(s\) to 'param.Selector' has been deprecated since Param 2.0.0 and will raise an error in a future version, please pass them as keyword arguments"
     ):
         param.Selector([0, 1])  # objects
     with pytest.warns(
-        PendingDeprecationWarning,
+        param._utils.ParamPendingDeprecationWarning,
         match=r"Passing 'class_' as positional argument\(s\) to 'param.ClassSelector' has been deprecated since Param 2.0.0 and will raise an error in a future version, please pass them as keyword arguments"
     ):
         param.ClassSelector(int)  # class_
     with pytest.warns(
-        PendingDeprecationWarning,
+        param._utils.ParamPendingDeprecationWarning,
         match=r"Passing 'bounds, softbounds' as positional argument\(s\) to 'param.Number' has been deprecated since Param 2.0.0 and will raise an error in a future version, please pass them as keyword arguments"
     ):
         param.Number(1, (0, 2), (0, 2))  # default (OK), bounds (not OK), softbounds (not OK)
```

### Comparing `param-2.0.0a1/tests/teststringparam.py` & `param-2.0.0a2/tests/teststringparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testtimedependent.py` & `param-2.0.0a2/tests/testtimedependent.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 except ImportError:
     import os
     if os.getenv('PARAM_TEST_GMPY','0') == '1':
         raise ImportError("PARAM_TEST_GMPY=1 but gmpy not available.")
     else:
         gmpy = None
 
+from .utils import warnings_as_excepts
+
 
 class TestTimeClass(unittest.TestCase):
 
     def test_time_init(self):
         param.Time()
 
     def test_time_init_int(self):
@@ -265,33 +267,38 @@
         """
         hashfn = numbergen.Hash("test", input_count=1)
         hash_1 = hashfn(1)
         hash_42 = hashfn(42)
         hash_200001 = hashfn(200001)
 
         self.assertEqual(hash_1, hashfn(fractions.Fraction(1)))
-        self.assertEqual(hash_1, hashfn("1"))
+        with warnings_as_excepts(match="Casting type 'str' to Fraction.fraction"):
+            self.assertEqual(hash_1, hashfn("1"))
 
         self.assertEqual(hash_42, hashfn(fractions.Fraction(42)))
-        self.assertEqual(hash_42, hashfn("42"))
+        with warnings_as_excepts(match="Casting type 'str' to Fraction.fraction"):
+            self.assertEqual(hash_42, hashfn("42"))
 
         self.assertEqual(hash_200001, hashfn(fractions.Fraction(200001)))
-        self.assertEqual(hash_200001, hashfn("200001"))
+        with warnings_as_excepts(match="Casting type 'str' to Fraction.fraction"):
+            self.assertEqual(hash_200001, hashfn("200001"))
 
 
     def test_time_hashing_rationals(self):
         """
         Check that hashes fractions and strings match for some
         reasonable rational numbers.
         """
         hashfn = numbergen.Hash("test", input_count=1)
         pi = "3.141592"
         half = fractions.Fraction(0.5)
-        self.assertEqual(hashfn(0.5), hashfn(half))
-        self.assertEqual(hashfn(pi), hashfn(fractions.Fraction(pi)))
+        with warnings_as_excepts(match="Casting type 'float' to Fraction.fraction"):
+            self.assertEqual(hashfn(0.5), hashfn(half))
+        with warnings_as_excepts(match="Casting type 'str' to Fraction.fraction"):
+            self.assertEqual(hashfn(pi), hashfn(fractions.Fraction(pi)))
 
 
     @pytest.mark.skipif(gmpy is None, reason="gmpy is not installed")
     def test_time_hashing_integers_gmpy(self):
         """
         Check that hashes for gmpy values at the integers also matches
         those of ints, fractions and strings.
@@ -310,9 +317,11 @@
     def test_time_hashing_rationals_gmpy(self):
         """
         Check that hashes of fractions and gmpy mpqs match for some
         reasonable rational numbers.
         """
         pi = "3.141592"
         hashfn = numbergen.Hash("test", input_count=1)
-        self.assertEqual(hashfn(0.5), hashfn(gmpy.mpq(0.5)))
-        self.assertEqual(hashfn(pi), hashfn(gmpy.mpq(3.141592)))
+        with warnings_as_excepts(match="Casting type 'float' to Fraction.fraction"):
+            self.assertEqual(hashfn(0.5), hashfn(gmpy.mpq(0.5)))
+        with warnings_as_excepts(match="Casting type 'str' to Fraction.fraction"):
+            self.assertEqual(hashfn(pi), hashfn(gmpy.mpq(3.141592)))
```

### Comparing `param-2.0.0a1/tests/testtupleparam.py` & `param-2.0.0a2/tests/testtupleparam.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testutils.py` & `param-2.0.0a2/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/tests/testwatch.py` & `param-2.0.0a2/tests/testwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 import unittest
 
 import param
 
 from param.parameterized import discard_events
 
-from .utils import MockLoggingHandler
+from .utils import MockLoggingHandler, warnings_as_excepts
 
 
 class Accumulator:
 
     def __init__(self):
         self.args = []
         self.kwargs = []
@@ -230,17 +230,23 @@
     def test_warning_unwatching_when_unwatched(self):
         def accumulator(change):
             self.accumulator += change.new
 
         obj = SimpleWatchExample()
         watcher = obj.param.watch(accumulator, 'a')
         obj.param.unwatch(watcher)
-        obj.param.unwatch(watcher)
-        self.log_handler.assertEndsWith('WARNING',
-                            ' to remove.')
+        with warnings_as_excepts(match='No such watcher'):
+            obj.param.unwatch(watcher)
+        try:
+            param.parameterized.warnings_as_exceptions = False
+            obj.param.unwatch(watcher)
+            self.log_handler.assertEndsWith('WARNING',
+                                ' to remove.')
+        finally:
+            param.parameterized.warnings_as_exceptions = True
 
     def test_simple_batched_watch_setattr(self):
 
         accumulator = Accumulator()
 
         obj = SimpleWatchExample()
         obj.param.watch(accumulator, ['a', 'b'])
```

### Comparing `param-2.0.0a1/tests/utils.py` & `param-2.0.0a2/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import logging
 
+from contextlib import contextmanager
+
+import param
+
+
 class MockLoggingHandler(logging.Handler):
     """Mock logging handler to check for expected logs.
 
     Messages are available from an instance's ``messages`` dict, in
     order, indexed by a lowercase log level string (e.g., 'debug',
     'info', etc.).
 
@@ -89,7 +94,20 @@
         assert parameter.readonly is False
     if 'pickle_default_value' not in skip:
         assert parameter.pickle_default_value is True
     if 'per_instance' not in skip:
         assert parameter.per_instance is True
     if 'label' not in skip:
         assert parameter.label == label
+
+
+@contextmanager
+def warnings_as_excepts(match=None):
+    orig = param.parameterized.warnings_as_exceptions
+    param.parameterized.warnings_as_exceptions = True
+    try:
+        yield
+    except Exception as e:
+        if match and match not in str(e):
+            raise ValueError(f'Exception emitted {str(e)!r} does not contain {match!r}')
+    finally:
+        param.parameterized.warnings_as_exceptions = orig
```

### Comparing `param-2.0.0a1/LICENSE.txt` & `param-2.0.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/README.md` & `param-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `param-2.0.0a1/pyproject.toml` & `param-2.0.0a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 [project]
 name = "param"
 dynamic = ["version"]
 description = "Make your Python code clearer and more reliable by declaring Parameters."
 readme = "README.md"
 license = { text = "BSD-3-Clause" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "HoloViz", email = "developers@holoviz.org" },
 ]
 maintainers = [
     { name = "HoloViz", email = "developers@holoviz.org" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
 ]
@@ -65,14 +64,16 @@
     "param[tests-examples]",
     "param[tests-deser]",
     "numpy",
     "pandas",
     "ipython",
     "jsonschema",
     "gmpy",
+    "cloudpickle",
+    "nest_asyncio",
 ]
 lint = [
     "flake8",
     "pre-commit",
 ]
 all = [
     "param[tests-full]",
@@ -118,14 +119,16 @@
     "param[tests-deser]",
     # Additional tests dependencies, not including gmpy as
     # it's tricky to install.
     "ipython",
     "jsonschema",
     "numpy",
     "pandas",
+    "cloudpickle",
+    "nest_asyncio",
     # To keep __version__ up-to-date in editable installs
     "setuptools_scm",
 ]
 post-install-commands = [
   "python -m pip install pre-commit",
   "pre-commit install",
 ]
@@ -151,15 +154,14 @@
     "param[tests]",
     "ipython",
     "jsonschema",
 ]
 
 [[tool.hatch.envs.tests.matrix]]
 python = [
-    "3.7",
     "3.8",
     "3.9",
     "3.10",
     "3.11",
     "pypy3.9",
 ]
 
@@ -177,40 +179,45 @@
     "numpy",
     "pandas",
     "xlrd",
     "openpyxl",
     "odfpy",
     "feather-format",
     "pyarrow",
+    "cloudpickle",
+    "nest_asyncio",
 ]
 # Only install gmpy on Linux on these version
 # Only install tables (deser HDF5) on Linux on these version
 matrix.python.dependencies = [
-    { value = "gmpy", if = ["3.7", "3.8", "3.9", "3.10"], platform = ["linux"] },
-    { value = "tables", if = ["3.7", "3.8", "3.9", "3.10", "3.11"], platform = ["linux"] },
+    { value = "gmpy", if = ["3.8", "3.9", "3.10"], platform = ["linux"] },
+    { value = "tables", if = ["3.8", "3.9", "3.10", "3.11"], platform = ["linux"] },
 ]
 
 [tool.hatch.envs.tests_examples]
 template = "tests_examples"
 dependencies = [
     "param[tests-examples]",
     "ipython",
     "jsonschema",
 ]
 
 [[tool.hatch.envs.tests_examples.matrix]]
 python = [
-    "3.7",
     "3.8",
     "3.9",
     "3.10",
     "3.11",
 ]
 
 [tool.hatch.envs.tests_examples.scripts]
 examples = "pytest -v -n logical --dist loadscope --nbval-lax {args:examples}"
 
 [tool.pytest.ini_options]
 python_files = "test*.py"
+filterwarnings = [
+  "error",
+]
+xfail_strict = "true"
 
 [tool.coverage.report]
 omit = ["param/version.py"]
```

### Comparing `param-2.0.0a1/PKG-INFO` & `param-2.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Make your Python code clearer and more reliable by declaring Parameters.
 Project-URL: Homepage, https://param.holoviz.org/
 Project-URL: Tracker, https://github.com/holoviz/param/issues
 Project-URL: Releases, https://github.com/holoviz/param/releases
 Project-URL: Source, https://github.com/holoviz/param
 Project-URL: HoloViz, https://holoviz.org/
 Author-email: HoloViz <developers@holoviz.org>
@@ -14,22 +14,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: all
 Requires-Dist: param[doc]; extra == 'all'
 Requires-Dist: param[lint]; extra == 'all'
 Requires-Dist: param[tests-full]; extra == 'all'
 Provides-Extra: doc
 Requires-Dist: nbsite==0.8.0; extra == 'doc'
 Requires-Dist: param[examples]; extra == 'doc'
@@ -51,17 +50,19 @@
 Requires-Dist: xlrd; extra == 'tests-deser'
 Provides-Extra: tests-examples
 Requires-Dist: nbval; extra == 'tests-examples'
 Requires-Dist: param[examples]; extra == 'tests-examples'
 Requires-Dist: pytest; extra == 'tests-examples'
 Requires-Dist: pytest-xdist; extra == 'tests-examples'
 Provides-Extra: tests-full
+Requires-Dist: cloudpickle; extra == 'tests-full'
 Requires-Dist: gmpy; extra == 'tests-full'
 Requires-Dist: ipython; extra == 'tests-full'
 Requires-Dist: jsonschema; extra == 'tests-full'
+Requires-Dist: nest-asyncio; extra == 'tests-full'
 Requires-Dist: numpy; extra == 'tests-full'
 Requires-Dist: pandas; extra == 'tests-full'
 Requires-Dist: param[tests-deser]; extra == 'tests-full'
 Requires-Dist: param[tests-examples]; extra == 'tests-full'
 Requires-Dist: param[tests]; extra == 'tests-full'
 Description-Content-Type: text/markdown
```

