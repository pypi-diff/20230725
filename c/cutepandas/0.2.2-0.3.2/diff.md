# Comparing `tmp/cutepandas-0.2.2.tar.gz` & `tmp/cutepandas-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutepandas-0.2.2.tar", max compression
+gzip compressed data, was "cutepandas-0.3.2.tar", max compression
```

## Comparing `cutepandas-0.2.2.tar` & `cutepandas-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0      197 2022-11-11 20:39:08.140466 cutepandas-0.2.2/cutepandas/__init__.py
--rw-r--r--   0        0        0     3953 2022-11-10 19:34:23.590833 cutepandas-0.2.2/cutepandas/constants/iconnames.py
--rw-r--r--   0        0        0      323 2022-11-10 23:49:56.265238 cutepandas-0.2.2/cutepandas/pandasmodels/__init__.py
--rw-r--r--   0        0        0     1673 2022-11-10 19:22:26.840916 cutepandas-0.2.2/cutepandas/pandasmodels/basedatasetmodel.py
--rw-r--r--   0        0        0     4981 2022-11-10 23:43:52.625149 cutepandas-0.2.2/cutepandas/pandasmodels/pandasindexmodel.py
--rw-r--r--   0        0        0     7240 2022-11-10 23:44:29.165055 cutepandas-0.2.2/cutepandas/pandasmodels/pandasmodel.py
--rw-r--r--   0        0        0      212 2022-11-07 14:44:43.365780 cutepandas-0.2.2/cutepandas/pandaswidgets/__init__.py
--rw-r--r--   0        0        0     2532 2022-11-11 17:02:50.567774 cutepandas-0.2.2/cutepandas/pandaswidgets/dataframeindexwidget.py
--rw-r--r--   0        0        0     3683 2022-11-07 15:28:46.024265 cutepandas-0.2.2/cutepandas/pandaswidgets/dataframewidget.py
--rw-r--r--   0        0        0        0 2021-10-14 11:29:00.667619 cutepandas-0.2.2/cutepandas/py.typed
--rw-r--r--   0        0        0      643 2022-11-10 19:32:25.555130 cutepandas-0.2.2/cutepandas/util/helpers.py
--rw-r--r--   0        0        0     1672 2022-11-10 19:34:50.430865 cutepandas-0.2.2/cutepandas/util/icons.py
--rw-r--r--   0        0        0     2326 2022-11-07 14:18:54.414007 cutepandas-0.2.2/docs/index.md
--rw-r--r--   0        0        0     1100 2021-10-14 11:29:00.237913 cutepandas-0.2.2/LICENSE
--rw-r--r--   0        0        0     4559 2022-11-11 20:39:08.320459 cutepandas-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 cutepandas-0.2.2/setup.py
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 cutepandas-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-25 15:07:27.246957 cutepandas-0.3.2/LICENSE
+-rw-r--r--   0        0        0      187 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/__init__.py
+-rw-r--r--   0        0        0     3921 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/constants/iconnames.py
+-rw-r--r--   0        0        0     2579 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/__init__.py
+-rw-r--r--   0        0        0     4916 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/pandascategorylistmodel.py
+-rw-r--r--   0        0        0    12845 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/pandascolumnlistmodel.py
+-rw-r--r--   0        0        0     8556 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/pandasdataframemodel.py
+-rw-r--r--   0        0        0    10091 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/pandasindexfilterproxymodel.py
+-rw-r--r--   0        0        0     3454 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandasmodels/polarsdataframemodel.py
+-rw-r--r--   0        0        0      383 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/dataframelistwidget.py
+-rw-r--r--   0        0        0     1736 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/dataframemanagerwidget.py
+-rw-r--r--   0        0        0    24841 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/dataframeviewer.py
+-rw-r--r--   0        0        0    19678 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/dataframeviewer2.py
+-rw-r--r--   0        0        0     2989 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/pandaswidgets/dataframewidget.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/py.typed
+-rw-r--r--   0        0        0        0 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/qtframe/__init__.py
+-rw-r--r--   0        0        0     3655 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/qtframe/qtframe.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/utils/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/utils/helpers.py
+-rw-r--r--   0        0        0     1642 2023-07-25 15:07:27.246957 cutepandas-0.3.2/cutepandas/utils/icons.py
+-rw-r--r--   0        0        0      820 2023-07-25 15:07:27.246957 cutepandas-0.3.2/docs/index.md
+-rw-r--r--   0        0        0     6384 2023-07-25 15:07:27.250957 cutepandas-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 cutepandas-0.3.2/PKG-INFO
```

### Comparing `cutepandas-0.2.2/cutepandas/constants/iconnames.py` & `cutepandas-0.3.2/cutepandas/constants/iconnames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""
-@author: Philipp Temminghoff
-
-for full list, see:
-- https://cdn.materialdesignicons.com/5.4.55/
-"""
+"""for full list, see: https://cdn.materialdesignicons.com/5.4.55/ ."""
 
 BOOKMARK = "mdi.bookmark-outline"
 BOOL = "mdi.toggle-switch-outline"
 TIME = "mdi.timer"
 DATE = "mdi.calendar-blank-outline"
 NUMERIC = "mdi.chart-line-variant"
 CATEGORY = "mdi.folder-outline"
```

### Comparing `cutepandas-0.2.2/cutepandas/util/helpers.py` & `cutepandas-0.3.2/cutepandas/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-@author: Philipp Temminghoff
-"""
-
 from __future__ import annotations
 
 import logging
 import logging.config
 
 import numpy as np
 
@@ -19,15 +15,15 @@
             return int(text)
         return float(text)
     except (TypeError, ValueError):
         return text
 
 
 def format_name(name) -> str:
-    if isinstance(name, (tuple, list)):
+    if isinstance(name, tuple | list):
         return " | ".join(str(i) for i in name)
     return str(name)
 
 
 def is_nan(obj) -> bool:
     try:
         return np.isnan(obj) if isinstance(obj, float) else False
```

### Comparing `cutepandas-0.2.2/cutepandas/util/icons.py` & `cutepandas-0.3.2/cutepandas/utils/icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-"""
-@author: Philipp Temminghoff
-
-for full list, see:
-- https://cdn.materialdesignicons.com/5.4.55/
-"""
+"""for full list, see:- https://cdn.materialdesignicons.com/5.4.55/ ."""
 
 import pandas as pd
+
 from prettyqt import iconprovider
 
 from cutepandas.constants import iconnames
 
 
 def icon_for_dtype(dtype):
     if dtype == bool:
```

### Comparing `cutepandas-0.2.2/LICENSE` & `cutepandas-0.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2019, Philipp Temminghoff
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2019, Philipp Temminghoff
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

