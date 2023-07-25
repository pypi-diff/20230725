# Comparing `tmp/economic_complexity-0.1.3.tar.gz` & `tmp/economic_complexity-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "economic_complexity-0.1.3.tar", max compression
+gzip compressed data, was "economic_complexity-0.1.4.tar", max compression
```

## Comparing `economic_complexity-0.1.3.tar` & `economic_complexity-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      695 2023-04-14 20:01:48.594569 economic_complexity-0.1.3/economic_complexity/__init__.py
--rw-r--r--   0        0        0     2248 2022-11-15 21:13:07.101014 economic_complexity-0.1.3/economic_complexity/complexity.py
--rw-r--r--   0        0        0     3774 2022-05-04 21:01:08.480474 economic_complexity-0.1.3/economic_complexity/cross_space.py
--rw-r--r--   0        0        0    11108 2023-04-14 19:59:47.028046 economic_complexity-0.1.3/economic_complexity/product_space.py
--rw-r--r--   0        0        0     1431 2022-11-15 21:12:43.234320 economic_complexity-0.1.3/economic_complexity/rca.py
--rw-r--r--   0        0        0     2246 2023-04-14 19:59:47.029052 economic_complexity-0.1.3/economic_complexity/subnational.py
--rw-r--r--   0        0        0     1071 2022-05-06 03:32:39.758645 economic_complexity-0.1.3/LICENSE
--rw-r--r--   0        0        0     3032 2022-11-15 21:09:40.964713 economic_complexity-0.1.3/PACKAGE.md
--rw-r--r--   0        0        0      740 2023-04-14 20:01:42.840008 economic_complexity-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 economic_complexity-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      695 2023-07-25 20:45:29.953067 economic_complexity-0.1.4/economic_complexity/__init__.py
+-rw-r--r--   0        0        0     2248 2022-11-15 21:13:07.101014 economic_complexity-0.1.4/economic_complexity/complexity.py
+-rw-r--r--   0        0        0     3774 2022-05-04 21:01:08.480474 economic_complexity-0.1.4/economic_complexity/cross_space.py
+-rw-r--r--   0        0        0    11108 2023-04-14 19:59:47.028046 economic_complexity-0.1.4/economic_complexity/product_space.py
+-rw-r--r--   0        0        0     1431 2022-11-15 21:12:43.234320 economic_complexity-0.1.4/economic_complexity/rca.py
+-rw-r--r--   0        0        0     2470 2023-07-05 21:16:07.250839 economic_complexity-0.1.4/economic_complexity/subnational.py
+-rw-r--r--   0        0        0     1071 2022-05-06 03:32:39.758645 economic_complexity-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3032 2022-11-15 21:09:40.964713 economic_complexity-0.1.4/PACKAGE.md
+-rw-r--r--   0        0        0      715 2023-07-25 21:22:18.074857 economic_complexity-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 economic_complexity-0.1.4/PKG-INFO
```

### Comparing `economic_complexity-0.1.3/economic_complexity/__init__.py` & `economic_complexity-0.1.4/economic_complexity/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from .rca import rca
 from .complexity import complexity
 from .product_space import distance, opportunity_gain, proximity, relatedness, similarity, pgi, peii
 from .cross_space import cross_proximity, cross_relatedness
 from .subnational import complexity_subnational
 
-__version_info__ = ('0', '1', '3')
+__version_info__ = ('0', '1', '4')
 __version__ = '.'.join(__version_info__)
 
 __all__ = (
     "rca",
     "complexity",
     "distance",
     "opportunity_gain",
```

### Comparing `economic_complexity-0.1.3/economic_complexity/complexity.py` & `economic_complexity-0.1.4/economic_complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/economic_complexity/cross_space.py` & `economic_complexity-0.1.4/economic_complexity/cross_space.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/economic_complexity/product_space.py` & `economic_complexity-0.1.4/economic_complexity/product_space.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/economic_complexity/rca.py` & `economic_complexity-0.1.4/economic_complexity/rca.py`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/economic_complexity/subnational.py` & `economic_complexity-0.1.4/economic_complexity/subnational.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Subnational Method module
 """
-from typing import Tuple
+from typing import Tuple, Optional
 
 import pandas as pd
 
 
 def complexity_subnational(
     rcas: pd.DataFrame,
     pci_external: pd.Series,
+    standardize: Optional[bool]=False,
 ) -> Tuple[pd.Series, pd.Series]:
     """
     Calculates the Economic Complexity Index for the subnational (AKA external method). Here a RCA matrix and an external Product Complexity is used.
     Args:
         rcas (pd.DataFrame) -- Pivotted RCA matrix.
         pci_external (pd.Series) -- PCI values from an external source.
+        standardize (bool, optional) -- Boolean value to choose if the ECI vector is standardized: x-µ/σ. Default value: False.
+
 
     Returns:
         ((pd.Series, pd.Series)) -- A tuple of ECI and PCI values using the subnational method.
 
 
     """
     # This functions computes the ECI for a RCA matrix using an external PCI index.
@@ -47,14 +50,15 @@
         pci_rca = pci_external[pci_external.index.isin(spec_cat)]
 
         # Compute the ECI for the current country using the retrieved PCI values
         eci = pci_rca.sum()/len(pci_rca)
 
         # Append the ECI value to the eci_external DataFrame
         eci_external = pd.concat([eci_external, pd.Series({index:eci})], axis=0, ignore_index=False)
-
-    # Standardize the ECI values by subtracting the mean and dividing by the standard deviation
-    eci_external = (eci_external-eci_external.mean())/eci_external.std()
+    
+    if standardize == True:
+        # Standardize the ECI values by subtracting the mean and dividing by the standard deviation
+        eci_external = (eci_external-eci_external.mean())/eci_external.std()
 
     eci_external.index.name=geo_col_name
 
     return eci_external, pci_external
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `economic_complexity-0.1.3/LICENSE` & `economic_complexity-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/PACKAGE.md` & `economic_complexity-0.1.4/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `economic_complexity-0.1.3/pyproject.toml` & `economic_complexity-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-[tool.poetry]
-name = "economic-complexity"
-version = "0.1.3"
-description = "Functions to calculate Economic Complexity indicators."
-authors = [
-  "Jelmy Hermosilla <jelmy@datawheel.us>",
-  "Nicolas Netz <nicolas.netz@datawheel.us>",
-  "Marcos Perez <marcos@datawheel.us>",
-]
-maintainers = [
-  "Francisco Abarzua <francisco@datawheel.us>",
-]
-license = "MIT"
-readme = "PACKAGE.md"
-repository = "https://github.com/Datawheel/py-economic-complexity"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-numpy = "^1.24.0"
-pandas = "^1.1.0"
-
-[tool.poetry.dev-dependencies]
-ipykernel = "^6.0.3"
-pytest = "^6.2.4"
-pytest-cov = "^3.0.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "economic-complexity"
+version = "0.1.4"
+description = "Functions to calculate Economic Complexity indicators."
+authors = [
+  "Jelmy Hermosilla <jelmy@datawheel.us>",
+  "Nicolas Netz <nicolas.netz@datawheel.us>",
+  "Marcos Perez <marcos@datawheel.us>",
+]
+maintainers = [
+  "Francisco Abarzua <francisco@datawheel.us>",
+]
+license = "MIT"
+readme = "PACKAGE.md"
+repository = "https://github.com/Datawheel/py-economic-complexity"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+numpy = "^1.24.0"
+pandas = "^1.1.0"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.25.0"
+pytest = "^7.4.0"
+polars = "^0.18.0"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `economic_complexity-0.1.3/PKG-INFO` & `economic_complexity-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: economic-complexity
-Version: 0.1.3
+Version: 0.1.4
 Summary: Functions to calculate Economic Complexity indicators.
 Home-page: https://github.com/Datawheel/py-economic-complexity
 License: MIT
 Author: Jelmy Hermosilla
 Author-email: jelmy@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: economic-complexity Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: economic-complexity Version: 0.1.4 Summary:
 Functions to calculate Economic Complexity indicators. Home-page: https://
 github.com/Datawheel/py-economic-complexity License: MIT Author: Jelmy
 Hermosilla Author-email: jelmy@datawheel.us Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

