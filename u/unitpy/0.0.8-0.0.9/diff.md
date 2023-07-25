# Comparing `tmp/unitpy-0.0.8.tar.gz` & `tmp/unitpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicep\Desktop\Reseach_Post\python\unitpy\dist\.tmp-41o84gj6\unitpy-0.0.8.tar", last modified: Wed Jul  5 14:35:38 2023, max compression
+gzip compressed data, was "C:\Users\nicep\Desktop\Reseach_Post\python\unitpy\dist\.tmp-3a8ek75a\unitpy-0.0.9.tar", last modified: Tue Jul 25 18:29:05 2023, max compression
```

## Comparing `unitpy-0.0.8.tar` & `unitpy-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/
--rw-rw-rw-   0        0        0     1497 2023-04-03 12:39:22.000000 unitpy-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4550 2023-07-05 14:35:38.000000 unitpy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3749 2023-07-05 14:34:51.000000 unitpy-0.0.8/README.md
--rw-rw-rw-   0        0        0      307 2023-04-03 17:45:31.000000 unitpy-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      969 2023-07-05 14:35:38.000000 unitpy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-04-03 12:39:22.000000 unitpy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/unitpy/
--rw-rw-rw-   0        0        0      336 2023-04-03 14:05:31.000000 unitpy-0.0.8/src/unitpy/__init__.py
--rw-rw-rw-   0        0        0      451 2023-07-05 13:23:16.000000 unitpy-0.0.8/src/unitpy/config.py
--rw-rw-rw-   0        0        0    20625 2023-07-05 14:31:19.000000 unitpy-0.0.8/src/unitpy/core.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/unitpy/definitions/
--rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/constants.py
--rw-rw-rw-   0        0        0     7224 2023-04-03 16:57:14.000000 unitpy-0.0.8/src/unitpy/definitions/dimensions.py
--rw-rw-rw-   0        0        0     1511 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/entry.py
--rw-rw-rw-   0        0        0     5904 2023-07-05 13:21:40.000000 unitpy-0.0.8/src/unitpy/definitions/ledger.py
--rw-rw-rw-   0        0        0      797 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/metric.py
--rw-rw-rw-   0        0        0     1362 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/prefix.py
--rw-rw-rw-   0        0        0    16491 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/definitions/unit_NIST.py
--rw-rw-rw-   0        0        0     6166 2023-04-03 14:27:27.000000 unitpy-0.0.8/src/unitpy/definitions/unit_base.py
--rw-rw-rw-   0        0        0     3545 2023-04-03 16:16:53.000000 unitpy-0.0.8/src/unitpy/definitions/unit_derived.py
--rw-rw-rw-   0        0        0      925 2023-07-05 13:21:40.000000 unitpy-0.0.8/src/unitpy/definitions/unit_extra.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/unitpy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.8/src/unitpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1855 2023-07-05 13:23:16.000000 unitpy-0.0.8/src/unitpy/utils/equation_formating.py
--rw-rw-rw-   0        0        0     5005 2023-04-03 15:05:13.000000 unitpy-0.0.8/src/unitpy/utils/parsing.py
--rw-rw-rw-   0        0        0      356 2023-04-03 13:51:24.000000 unitpy-0.0.8/src/unitpy/utils/string_converter.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/unitpy.egg-info/
--rw-rw-rw-   0        0        0     4550 2023-07-05 14:35:37.000000 unitpy-0.0.8/src/unitpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-07-05 14:35:38.000000 unitpy-0.0.8/src/unitpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:35:37.000000 unitpy-0.0.8/src/unitpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-03 12:59:41.000000 unitpy-0.0.8/src/unitpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-05 14:35:37.000000 unitpy-0.0.8/src/unitpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 14:35:38.000000 unitpy-0.0.8/tests/
--rw-rw-rw-   0        0        0      684 2023-04-03 17:57:48.000000 unitpy-0.0.8/tests/test_define_quantity.py
--rw-rw-rw-   0        0        0     1110 2023-04-03 18:03:53.000000 unitpy-0.0.8/tests/test_define_unit.py
--rw-rw-rw-   0        0        0     1340 2023-04-03 16:57:59.000000 unitpy-0.0.8/tests/test_dimensions.py
--rw-rw-rw-   0        0        0     1927 2023-04-03 12:39:22.000000 unitpy-0.0.8/tests/test_parsing_unit.py
--rw-rw-rw-   0        0        0      205 2023-07-05 13:26:28.000000 unitpy-0.0.8/tests/test_pickle.py
--rw-rw-rw-   0        0        0     2965 2023-05-30 14:41:46.000000 unitpy-0.0.8/tests/test_quanitiy_math_operations.py
--rw-rw-rw-   0        0        0      756 2023-04-03 12:39:22.000000 unitpy-0.0.8/tests/test_unit_conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:05.000000 unitpy-0.0.9/
+-rw-rw-rw-   0        0        0     1497 2023-04-03 12:39:22.000000 unitpy-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4550 2023-07-25 18:29:05.000000 unitpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3749 2023-07-05 14:34:51.000000 unitpy-0.0.9/README.md
+-rw-rw-rw-   0        0        0      307 2023-04-03 17:45:31.000000 unitpy-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      969 2023-07-25 18:29:05.000000 unitpy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-04-03 12:39:22.000000 unitpy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/unitpy/
+-rw-rw-rw-   0        0        0      336 2023-04-03 14:05:31.000000 unitpy-0.0.9/src/unitpy/__init__.py
+-rw-rw-rw-   0        0        0      451 2023-07-05 13:23:16.000000 unitpy-0.0.9/src/unitpy/config.py
+-rw-rw-rw-   0        0        0    20673 2023-07-25 18:27:24.000000 unitpy-0.0.9/src/unitpy/core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:05.000000 unitpy-0.0.9/src/unitpy/definitions/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/constants.py
+-rw-rw-rw-   0        0        0     7224 2023-04-03 16:57:14.000000 unitpy-0.0.9/src/unitpy/definitions/dimensions.py
+-rw-rw-rw-   0        0        0     1511 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/entry.py
+-rw-rw-rw-   0        0        0     5904 2023-07-05 13:21:40.000000 unitpy-0.0.9/src/unitpy/definitions/ledger.py
+-rw-rw-rw-   0        0        0      797 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/metric.py
+-rw-rw-rw-   0        0        0     1362 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/prefix.py
+-rw-rw-rw-   0        0        0    16491 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/definitions/unit_NIST.py
+-rw-rw-rw-   0        0        0     6166 2023-04-03 14:27:27.000000 unitpy-0.0.9/src/unitpy/definitions/unit_base.py
+-rw-rw-rw-   0        0        0     3545 2023-04-03 16:16:53.000000 unitpy-0.0.9/src/unitpy/definitions/unit_derived.py
+-rw-rw-rw-   0        0        0      925 2023-07-05 13:21:40.000000 unitpy-0.0.9/src/unitpy/definitions/unit_extra.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:05.000000 unitpy-0.0.9/src/unitpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.9/src/unitpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1855 2023-07-05 13:23:16.000000 unitpy-0.0.9/src/unitpy/utils/equation_formating.py
+-rw-rw-rw-   0        0        0     5005 2023-04-03 15:05:13.000000 unitpy-0.0.9/src/unitpy/utils/parsing.py
+-rw-rw-rw-   0        0        0      356 2023-04-03 13:51:24.000000 unitpy-0.0.9/src/unitpy/utils/string_converter.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:05.000000 unitpy-0.0.9/src/unitpy.egg-info/
+-rw-rw-rw-   0        0        0     4550 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/unitpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/unitpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/unitpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-03 12:59:41.000000 unitpy-0.0.9/src/unitpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-25 18:29:04.000000 unitpy-0.0.9/src/unitpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 18:29:05.000000 unitpy-0.0.9/tests/
+-rw-rw-rw-   0        0        0      684 2023-04-03 17:57:48.000000 unitpy-0.0.9/tests/test_define_quantity.py
+-rw-rw-rw-   0        0        0     1110 2023-04-03 18:03:53.000000 unitpy-0.0.9/tests/test_define_unit.py
+-rw-rw-rw-   0        0        0     1340 2023-04-03 16:57:59.000000 unitpy-0.0.9/tests/test_dimensions.py
+-rw-rw-rw-   0        0        0     1927 2023-04-03 12:39:22.000000 unitpy-0.0.9/tests/test_parsing_unit.py
+-rw-rw-rw-   0        0        0      205 2023-07-05 13:26:28.000000 unitpy-0.0.9/tests/test_pickle.py
+-rw-rw-rw-   0        0        0     3040 2023-07-25 18:27:40.000000 unitpy-0.0.9/tests/test_quanitiy_math_operations.py
+-rw-rw-rw-   0        0        0      756 2023-04-03 12:39:22.000000 unitpy-0.0.9/tests/test_unit_conversion.py
```

### Comparing `unitpy-0.0.8/LICENSE.txt` & `unitpy-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/PKG-INFO` & `unitpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.8/README.md` & `unitpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/setup.cfg` & `unitpy-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7470 790d 0a76 6572 7369   = unitpy..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6465 7363  on = 0.0.8..desc
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6465 7363  on = 0.0.9..desc
 00000030: 7269 7074 696f 6e20 3d20 576f 726b 696e  ription = Workin
 00000040: 6720 7769 7468 2073 6369 656e 7469 6669  g with scientifi
 00000050: 6320 756e 6974 7320 696e 2070 7974 686f  c units in pytho
 00000060: 6e2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  n...long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `unitpy-0.0.8/src/unitpy/core.py` & `unitpy-0.0.9/src/unitpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             return hash(self.value)
         else:
             return hash((self._base_value, self._unit))
 
     def __getstate__(self):
         if self.compact_pickle:
             return str(self)
-        return self._base_value, self._unit
+        return self._base_value, self._unit.abbr
 
     def __setstate__(self, state):
         if isinstance(state, str):
             from unitpy.utils.parsing import parse_quantity
             qant = parse_quantity(state)
             self._base_value = qant._base_value
             self._unit = qant._unit
@@ -420,21 +420,22 @@
             self._unit /= other._unit
             return self
         else:
             raise TypeError(f"Can only divide 'Quantity' by 'int', 'float' or 'Quantity'.\n{self} / {other}")
 
     def __pow__(self, power: int | float) -> Quantity:
         if isinstance(power, int) or isinstance(power, float):
-            return Quantity(self._value ** power, self.unit)
+            return Quantity(self._value ** power, self.unit ** power)
         else:
             raise TypeError(f"Power must be a 'int' or 'float'.\n{self} ** {power}")
 
     def __ipow__(self, power: int | float) -> Quantity:
         if isinstance(power, (int, float)):
             self._base_value **= power
+            self._unit **= power
             return self
         else:
             raise TypeError(f"Power must be a 'int' or 'float'.\n{self} ** {power}")
 
     def __int__(self) -> Quantity:
         return Quantity(int(self._value), self.unit)
```

### Comparing `unitpy-0.0.8/src/unitpy/definitions/constants.py` & `unitpy-0.0.9/src/unitpy/definitions/constants.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/dimensions.py` & `unitpy-0.0.9/src/unitpy/definitions/dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/entry.py` & `unitpy-0.0.9/src/unitpy/definitions/entry.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/ledger.py` & `unitpy-0.0.9/src/unitpy/definitions/ledger.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/metric.py` & `unitpy-0.0.9/src/unitpy/definitions/metric.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/prefix.py` & `unitpy-0.0.9/src/unitpy/definitions/prefix.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/unit_NIST.py` & `unitpy-0.0.9/src/unitpy/definitions/unit_NIST.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/unit_base.py` & `unitpy-0.0.9/src/unitpy/definitions/unit_base.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/unit_derived.py` & `unitpy-0.0.9/src/unitpy/definitions/unit_derived.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/definitions/unit_extra.py` & `unitpy-0.0.9/src/unitpy/definitions/unit_extra.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/utils/equation_formating.py` & `unitpy-0.0.9/src/unitpy/utils/equation_formating.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy/utils/parsing.py` & `unitpy-0.0.9/src/unitpy/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/src/unitpy.egg-info/PKG-INFO` & `unitpy-0.0.9/src/unitpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.8/src/unitpy.egg-info/SOURCES.txt` & `unitpy-0.0.9/src/unitpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/tests/test_define_quantity.py` & `unitpy-0.0.9/tests/test_define_quantity.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/tests/test_define_unit.py` & `unitpy-0.0.9/tests/test_define_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/tests/test_dimensions.py` & `unitpy-0.0.9/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/tests/test_parsing_unit.py` & `unitpy-0.0.9/tests/test_parsing_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.8/tests/test_quanitiy_math_operations.py` & `unitpy-0.0.9/tests/test_quanitiy_math_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,7 +126,12 @@
     q = Q("1.2345 ft")
     assert (round(q) == Q("1 ft")) is True
 
 
 def test_round_3():
     q = Q("1.2345 ft")
     assert (round(q, 3) == Q("1.234 ft")) is True
+
+
+def test_power():
+    q = Q("2 ft")
+    assert Q("4 ft**2") == q**2
```

### Comparing `unitpy-0.0.8/tests/test_unit_conversion.py` & `unitpy-0.0.9/tests/test_unit_conversion.py`

 * *Files identical despite different names*

