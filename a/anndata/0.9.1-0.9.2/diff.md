# Comparing `tmp/anndata-0.9.1.tar.gz` & `tmp/anndata-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anndata-0.9.1.tar", last modified: Wed Apr 12 12:00:50 2023, max compression
+gzip compressed data, was "anndata-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `anndata-0.9.1.tar` & `anndata-0.9.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1544 2023-04-11 09:10:06.142630 anndata-0.9.1/LICENSE
--rw-r--r--   0        0        0     1901 2023-04-11 09:10:11.930300 anndata-0.9.1/README.md
--rw-r--r--   0        0        0      697 2023-04-11 09:10:06.142925 anndata-0.9.1/anndata/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 09:10:06.143030 anndata-0.9.1/anndata/_core/__init__.py
--rw-r--r--   0        0        0      818 2023-04-11 09:10:06.143156 anndata-0.9.1/anndata/_core/access.py
--rw-r--r--   0        0        0    11532 2023-04-11 09:10:06.143336 anndata-0.9.1/anndata/_core/aligned_mapping.py
--rw-r--r--   0        0        0    76595 2023-04-11 09:10:06.144196 anndata-0.9.1/anndata/_core/anndata.py
--rw-r--r--   0        0        0     3590 2023-04-11 09:10:06.144348 anndata-0.9.1/anndata/_core/file_backing.py
--rw-r--r--   0        0        0     7084 2023-04-11 09:10:06.144533 anndata-0.9.1/anndata/_core/index.py
--rw-r--r--   0        0        0    36304 2023-04-11 09:10:06.144873 anndata-0.9.1/anndata/_core/merge.py
--rw-r--r--   0        0        0     6836 2023-04-11 09:10:06.145065 anndata-0.9.1/anndata/_core/raw.py
--rw-r--r--   0        0        0    13269 2023-04-11 09:10:06.145253 anndata-0.9.1/anndata/_core/sparse_dataset.py
--rw-r--r--   0        0        0     9696 2023-04-11 09:10:06.145441 anndata-0.9.1/anndata/_core/views.py
--rw-r--r--   0        0        0      246 2023-04-11 09:10:06.145612 anndata-0.9.1/anndata/_io/__init__.py
--rw-r--r--   0        0        0    13086 2023-04-11 09:10:06.145854 anndata-0.9.1/anndata/_io/h5ad.py
--rw-r--r--   0        0        0    15794 2023-04-11 09:10:06.146055 anndata-0.9.1/anndata/_io/read.py
--rw-r--r--   0        0        0      111 2023-04-11 09:10:06.146232 anndata-0.9.1/anndata/_io/specs/__init__.py
--rw-r--r--   0        0        0    28569 2023-04-11 09:10:06.146471 anndata-0.9.1/anndata/_io/specs/methods.py
--rw-r--r--   0        0        0    11019 2023-04-12 12:00:07.463142 anndata-0.9.1/anndata/_io/specs/registry.py
--rw-r--r--   0        0        0     7780 2023-04-11 09:10:06.146830 anndata-0.9.1/anndata/_io/utils.py
--rw-r--r--   0        0        0     4602 2023-04-11 09:10:06.146973 anndata-0.9.1/anndata/_io/write.py
--rw-r--r--   0        0        0     4294 2023-04-11 09:10:06.147145 anndata-0.9.1/anndata/_io/zarr.py
--rw-r--r--   0        0        0     1312 2023-04-11 09:10:06.147287 anndata-0.9.1/anndata/_metadata.py
--rw-r--r--   0        0        0      436 2023-04-11 09:10:06.147393 anndata-0.9.1/anndata/_types.py
--rw-r--r--   0        0        0      695 2023-04-11 09:10:06.147508 anndata-0.9.1/anndata/_warnings.py
--rw-r--r--   0        0        0     9180 2023-04-11 09:10:06.147750 anndata-0.9.1/anndata/compat/__init__.py
--rw-r--r--   0        0        0      141 2023-04-11 09:10:06.147890 anndata-0.9.1/anndata/core.py
--rw-r--r--   0        0        0     3428 2023-04-11 09:10:06.148063 anndata-0.9.1/anndata/experimental/__init__.py
--rw-r--r--   0        0        0       42 2023-04-11 09:10:06.148221 anndata-0.9.1/anndata/experimental/multi_files/__init__.py
--rw-r--r--   0        0        0    34530 2023-04-11 09:10:06.148503 anndata-0.9.1/anndata/experimental/multi_files/_anncollection.py
--rw-r--r--   0        0        0       34 2023-04-11 09:10:06.148677 anndata-0.9.1/anndata/experimental/pytorch/__init__.py
--rw-r--r--   0        0        0     7097 2023-04-11 09:10:06.148822 anndata-0.9.1/anndata/experimental/pytorch/_annloader.py
--rw-r--r--   0        0        0     1429 2023-04-11 09:10:06.148954 anndata-0.9.1/anndata/logging.py
--rw-r--r--   0        0        0      144 2023-04-11 09:10:06.149047 anndata-0.9.1/anndata/readwrite.py
--rw-r--r--   0        0        0      101 2023-04-11 09:10:06.149197 anndata-0.9.1/anndata/tests/adata-comments.tsv
--rw-r--r--   0        0        0       39 2023-04-11 09:10:06.149294 anndata-0.9.1/anndata/tests/adata.csv
--rw-r--r--   0        0        0      309 2023-04-11 09:10:06.149392 anndata-0.9.1/anndata/tests/conftest.py
--rw-r--r--   0        0        0    17343 2023-04-12 12:00:07.463554 anndata-0.9.1/anndata/tests/helpers.py
--rw-r--r--   0        0        0    12139 2023-04-11 09:10:06.158385 anndata-0.9.1/anndata/utils.py
--rw-r--r--   0        0        0     4800 2023-04-11 09:10:06.163479 anndata-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 anndata-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1544 2018-12-12 17:31:51.886476 anndata-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3448 2023-07-25 10:50:11.481929 anndata-0.9.2/README.md
+-rw-r--r--   0        0        0      697 2023-07-25 10:50:11.481929 anndata-0.9.2/anndata/__init__.py
+-rw-r--r--   0        0        0        0 2020-07-31 11:20:24.672195 anndata-0.9.2/anndata/_core/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-26 16:06:33.160672 anndata-0.9.2/anndata/_core/access.py
+-rw-r--r--   0        0        0    11532 2023-07-25 10:50:11.481929 anndata-0.9.2/anndata/_core/aligned_mapping.py
+-rw-r--r--   0        0        0    76783 2023-07-21 08:45:59.554657 anndata-0.9.2/anndata/_core/anndata.py
+-rw-r--r--   0        0        0     3590 2023-04-11 12:29:17.389572 anndata-0.9.2/anndata/_core/file_backing.py
+-rw-r--r--   0        0        0     7084 2023-04-11 12:29:17.389572 anndata-0.9.2/anndata/_core/index.py
+-rw-r--r--   0        0        0    36304 2023-07-25 10:50:11.481929 anndata-0.9.2/anndata/_core/merge.py
+-rw-r--r--   0        0        0     6836 2023-07-25 10:50:11.481929 anndata-0.9.2/anndata/_core/raw.py
+-rw-r--r--   0        0        0    13269 2022-02-18 10:59:50.152894 anndata-0.9.2/anndata/_core/sparse_dataset.py
+-rw-r--r--   0        0        0    11083 2023-07-25 10:50:11.481929 anndata-0.9.2/anndata/_core/views.py
+-rw-r--r--   0        0        0      246 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/__init__.py
+-rw-r--r--   0        0        0    13086 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/h5ad.py
+-rw-r--r--   0        0        0    15794 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/read.py
+-rw-r--r--   0        0        0      111 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/specs/__init__.py
+-rw-r--r--   0        0        0    28629 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/specs/methods.py
+-rw-r--r--   0        0        0    11019 2023-07-17 11:13:14.217473 anndata-0.9.2/anndata/_io/specs/registry.py
+-rw-r--r--   0        0        0     7780 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/utils.py
+-rw-r--r--   0        0        0     4602 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/write.py
+-rw-r--r--   0        0        0     4364 2023-07-25 10:50:11.483929 anndata-0.9.2/anndata/_io/zarr.py
+-rw-r--r--   0        0        0     1312 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/_metadata.py
+-rw-r--r--   0        0        0      436 2023-04-11 12:29:17.391572 anndata-0.9.2/anndata/_types.py
+-rw-r--r--   0        0        0      695 2023-06-26 15:49:26.391250 anndata-0.9.2/anndata/_warnings.py
+-rw-r--r--   0        0        0     9180 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/compat/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/core.py
+-rw-r--r--   0        0        0     3428 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/experimental/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/experimental/multi_files/__init__.py
+-rw-r--r--   0        0        0    34530 2023-07-17 14:23:22.579353 anndata-0.9.2/anndata/experimental/multi_files/_anncollection.py
+-rw-r--r--   0        0        0       34 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/experimental/pytorch/__init__.py
+-rw-r--r--   0        0        0     7097 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/experimental/pytorch/_annloader.py
+-rw-r--r--   0        0        0     1429 2022-08-08 11:48:39.113628 anndata-0.9.2/anndata/logging.py
+-rw-r--r--   0        0        0      144 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/readwrite.py
+-rw-r--r--   0        0        0      101 2020-12-04 09:59:32.819435 anndata-0.9.2/anndata/tests/adata-comments.tsv
+-rw-r--r--   0        0        0       39 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/tests/adata.csv
+-rw-r--r--   0        0        0      309 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/tests/conftest.py
+-rw-r--r--   0        0        0    17343 2023-07-25 10:50:11.484929 anndata-0.9.2/anndata/tests/helpers.py
+-rw-r--r--   0        0        0    12139 2023-04-11 12:29:17.393572 anndata-0.9.2/anndata/utils.py
+-rw-r--r--   0        0        0     4798 2023-07-25 10:50:11.486929 anndata-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     6113 1970-01-01 00:00:00.000000 anndata-0.9.2/PKG-INFO
```

### Comparing `anndata-0.9.1/LICENSE` & `anndata-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/__init__.py` & `anndata-0.9.2/anndata/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/access.py` & `anndata-0.9.2/anndata/_core/access.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/aligned_mapping.py` & `anndata-0.9.2/anndata/_core/aligned_mapping.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/anndata.py` & `anndata-0.9.2/anndata/_core/anndata.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,31 +95,37 @@
             f"X needs to be 2-dimensional, not {len(X.shape)}-dimensional."
         )
 
 
 @singledispatch
 def _gen_dataframe(anno, length, index_names):
     if anno is None or len(anno) == 0:
-        return pd.DataFrame({}, index=pd.RangeIndex(0, length, name=None).astype(str))
+        anno = {}
     for index_name in index_names:
         if index_name in anno:
             return pd.DataFrame(
                 anno,
                 index=anno[index_name],
                 columns=[k for k in anno.keys() if k != index_name],
             )
-    return pd.DataFrame(anno, index=pd.RangeIndex(0, length, name=None).astype(str))
+    return pd.DataFrame(
+        anno,
+        index=pd.RangeIndex(0, length, name=None).astype(str),
+        columns=None if len(anno) else [],
+    )
 
 
 @_gen_dataframe.register(pd.DataFrame)
 def _(anno, length, index_names):
     anno = anno.copy(deep=False)
     if not is_string_dtype(anno.index):
         warnings.warn("Transforming to str index.", ImplicitModificationWarning)
         anno.index = anno.index.astype(str)
+    if not len(anno.columns):
+        anno.columns = anno.columns.astype(str)
     return anno
 
 
 @_gen_dataframe.register(pd.Series)
 @_gen_dataframe.register(pd.Index)
 def _(anno, length, index_names):
     raise ValueError(f"Cannot convert {type(anno)} to DataFrame")
@@ -414,19 +420,19 @@
 
             # init from DataFrame
             elif isinstance(X, pd.DataFrame):
                 # to verify index matching, we wait until obs and var are DataFrames
                 if obs is None:
                     obs = pd.DataFrame(index=X.index)
                 elif not isinstance(X.index, pd.RangeIndex):
-                    x_indices.append(("obs", "index", X.index))
+                    x_indices.append(("obs", "index", X.index.astype(str)))
                 if var is None:
                     var = pd.DataFrame(index=X.columns)
                 elif not isinstance(X.columns, pd.RangeIndex):
-                    x_indices.append(("var", "columns", X.columns))
+                    x_indices.append(("var", "columns", X.columns.astype(str)))
                 X = ensure_df_homogeneous(X, "X")
 
         # ----------------------------------------------------------------------
         # actually process the data
         # ----------------------------------------------------------------------
 
         # check data type of X
@@ -780,14 +786,16 @@
         if not isinstance(value, pd.DataFrame):
             raise ValueError(f"Can only assign pd.DataFrame to {attr}.")
         value_idx = self._prep_dim_index(value.index, attr)
         if self.is_view:
             self._init_as_actual(self.copy())
         setattr(self, f"_{attr}", value)
         self._set_dim_index(value_idx, attr)
+        if not len(value.columns):
+            value.columns = value.columns.astype(str)
 
     def _prep_dim_index(self, value, attr: str) -> pd.Index:
         """Prepares index to be uses as obs_names or var_names for AnnData object.AssertionError
 
         If a pd.Index is passed, this will use a reference, otherwise a new index object is created.
         """
         if self.shape[attr == "var"] != len(value):
```

### Comparing `anndata-0.9.1/anndata/_core/file_backing.py` & `anndata-0.9.2/anndata/_core/file_backing.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/index.py` & `anndata-0.9.2/anndata/_core/index.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/merge.py` & `anndata-0.9.2/anndata/_core/merge.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/raw.py` & `anndata-0.9.2/anndata/_core/raw.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/sparse_dataset.py` & `anndata-0.9.2/anndata/_core/sparse_dataset.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_core/views.py` & `anndata-0.9.2/anndata/_core/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 from contextlib import contextmanager
 from copy import deepcopy
-from enum import Enum
+from collections.abc import Sequence, KeysView, Callable, Iterable
 from functools import reduce, singledispatch, wraps
-from typing import Any, KeysView, Optional, Sequence, Tuple
+from typing import Any, Optional, Tuple, Literal
 import warnings
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_bool_dtype
 from scipy import sparse
 
@@ -60,14 +62,17 @@
 
     # TODO: This makes `deepcopy(obj)` return `obj._view_args.parent._adata_ref`, fix it
     def __deepcopy__(self, memo):
         parent, attrname, keys = self._view_args
         return deepcopy(getattr(parent._adata_ref, attrname))
 
 
+_UFuncMethod = Literal["__call__", "reduce", "reduceat", "accumulate", "outer", "inner"]
+
+
 class ArrayView(_SetItemMixin, np.ndarray):
     def __new__(
         cls,
         input_array: Sequence[Any],
         view_args: Tuple["anndata.AnnData", str, Tuple[str, ...]] = None,
     ):
         arr = np.asanyarray(input_array).view(cls)
@@ -77,14 +82,52 @@
         arr._view_args = view_args
         return arr
 
     def __array_finalize__(self, obj: Optional[np.ndarray]):
         if obj is not None:
             self._view_args = getattr(obj, "_view_args", None)
 
+    def __array_ufunc__(
+        self: ArrayView,
+        ufunc: Callable[..., Any],
+        method: _UFuncMethod,
+        *inputs,
+        out: tuple[np.ndarray, ...] | None = None,
+        **kwargs,
+    ) -> np.ndarray:
+        """Makes numpy ufuncs convert all instances of views to plain arrays.
+
+        See https://numpy.org/devdocs/user/basics.subclassing.html#array-ufunc-for-ufuncs
+        """
+
+        def convert_all(arrs: Iterable[np.ndarray]) -> Iterable[np.ndarray]:
+            return (
+                arr.view(np.ndarray) if isinstance(arr, ArrayView) else arr
+                for arr in arrs
+            )
+
+        if out is None:
+            outputs = (None,) * ufunc.nout
+        else:
+            out = outputs = tuple(convert_all(out))
+
+        results = super().__array_ufunc__(
+            ufunc, method, *convert_all(inputs), out=out, **kwargs
+        )
+        if results is NotImplemented:
+            return NotImplemented
+
+        if ufunc.nout == 1:
+            results = (results,)
+        results = tuple(
+            (np.asarray(result) if output is None else output)
+            for result, output in zip(results, outputs)
+        )
+        return results[0] if len(results) == 1 else results
+
     def keys(self) -> KeysView[str]:
         # it’s a structured array
         return self.dtype.names
 
     def copy(self, order: str = "C") -> np.ndarray:
         # we want a conventional array
         return np.array(self)
@@ -229,15 +272,15 @@
 
             Need to override __copy__ instead of `.copy()` as awkward arrays don't implement `.copy()`
             and are copied using python's standard copy mechanism in `aligned_mapping.py`.
             """
             array = self
             # makes a shallow copy and removes the reference to the original AnnData object
             array = ak.with_parameter(self, _PARAM_NAME, None)
-            array = ak.with_parameter(array, "__array__", None)
+            array = ak.with_parameter(array, "__list__", None)
             return array
 
     @as_view.register(AwkArray)
     def as_view_awkarray(array, view_args):
         parent, attrname, keys = view_args
         parent_key = f"target-{id(parent)}"
         _registry[parent_key] = parent
@@ -247,15 +290,15 @@
         # https://github.com/scikit-hep/awkward/issues/1391#issuecomment-1412297114
         if type(array).__name__ != "Array":
             raise NotImplementedError(
                 "Cannot create a view of an awkward array with __array__ parameter. "
                 "Please open an issue in the AnnData repo and describe your use-case."
             )
         array = ak.with_parameter(array, _PARAM_NAME, (parent_key, attrname, keys))
-        array = ak.with_parameter(array, "__array__", "AwkwardArrayView")
+        array = ak.with_parameter(array, "__list__", "AwkwardArrayView")
         return array
 
     ak.behavior["AwkwardArrayView"] = AwkwardArrayView
 
 except ImportError:
 
     class AwkwardArrayView:
```

### Comparing `anndata-0.9.1/anndata/_io/h5ad.py` & `anndata-0.9.2/anndata/_io/h5ad.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_io/read.py` & `anndata-0.9.2/anndata/_io/read.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_io/specs/methods.py` & `anndata-0.9.2/anndata/_io/specs/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
 @_REGISTRY.register_read(ZarrGroup, IOSpec("dataframe", "0.2.0"))
 def read_dataframe(elem, _reader):
     columns = list(_read_attr(elem.attrs, "column-order"))
     idx_key = _read_attr(elem.attrs, "_index")
     df = pd.DataFrame(
         {k: _reader.read_elem(elem[k]) for k in columns},
         index=_reader.read_elem(elem[idx_key]),
-        columns=list(columns),
+        columns=columns if len(columns) else None,
     )
     if idx_key != "_index":
         df.index.name = idx_key
     return df
 
 
 # TODO: Figure out what indices is allowed to be at each element
@@ -608,15 +608,15 @@
         ]
     else:
         columns = list(_read_attr(elem.attrs, "column-order"))
     idx_key = _read_attr(elem.attrs, "_index")
     df = pd.DataFrame(
         {k: read_elem_partial(elem[k], indices=indices[0]) for k in columns},
         index=read_elem_partial(elem[idx_key], indices=indices[0]),
-        columns=list(columns),
+        columns=columns if len(columns) else None,
     )
     if idx_key != "_index":
         df.index.name = idx_key
     return df
 
 
 # Backwards compat dataframe reading
@@ -626,15 +626,15 @@
 @_REGISTRY.register_read(ZarrGroup, IOSpec("dataframe", "0.1.0"))
 def read_dataframe_0_1_0(elem, _reader):
     columns = _read_attr(elem.attrs, "column-order")
     idx_key = _read_attr(elem.attrs, "_index")
     df = pd.DataFrame(
         {k: read_series(elem[k]) for k in columns},
         index=read_series(elem[idx_key]),
-        columns=list(columns),
+        columns=columns if len(columns) else None,
     )
     if idx_key != "_index":
         df.index.name = idx_key
     return df
 
 
 def read_series(dataset: h5py.Dataset) -> Union[np.ndarray, pd.Categorical]:
```

### Comparing `anndata-0.9.1/anndata/_io/specs/registry.py` & `anndata-0.9.2/anndata/_io/specs/registry.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_io/utils.py` & `anndata-0.9.2/anndata/_io/utils.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_io/write.py` & `anndata-0.9.2/anndata/_io/write.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_io/zarr.py` & `anndata-0.9.2/anndata/_io/zarr.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,18 @@
     ----------
     store
         The filename, a :class:`~typing.MutableMapping`, or a Zarr storage class.
     """
     if isinstance(store, Path):
         store = str(store)
 
-    f = zarr.open(store, mode="r")
+    if isinstance(store, zarr.Group):
+        f = store
+    else:
+        f = zarr.open(store, mode="r")
 
     # Read with handling for backwards compat
     def callback(func, elem_name: str, elem, iospec):
         if iospec.encoding_type == "anndata" or elem_name.endswith("/"):
             return AnnData(
                 **{
                     k: read_dispatched(v, callback)
```

### Comparing `anndata-0.9.1/anndata/_metadata.py` & `anndata-0.9.2/anndata/_metadata.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/_warnings.py` & `anndata-0.9.2/anndata/_warnings.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/compat/__init__.py` & `anndata-0.9.2/anndata/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/experimental/__init__.py` & `anndata-0.9.2/anndata/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/experimental/multi_files/_anncollection.py` & `anndata-0.9.2/anndata/experimental/multi_files/_anncollection.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/experimental/pytorch/_annloader.py` & `anndata-0.9.2/anndata/experimental/pytorch/_annloader.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/logging.py` & `anndata-0.9.2/anndata/logging.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/tests/helpers.py` & `anndata-0.9.2/anndata/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/anndata/utils.py` & `anndata-0.9.2/anndata/utils.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.1/pyproject.toml` & `anndata-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Visualization",
 ]
 dependencies = [
-    "pandas>=1.1.1",  # pandas <1.1.1 has pandas/issues/35446
+    "pandas>=1.1.1,!=2.0.1",  # pandas <1.1.1 has pandas/issues/35446
     "numpy>=1.16.5",  # required by pandas 1.x
     "scipy>1.4",
     "h5py>=3",
     "natsort",
     "packaging>=20",
 ]
 dynamic = ["version"]
@@ -55,26 +55,25 @@
 Home-page = "https://github.com/scverse/anndata"
 
 
 [project.optional-dependencies]
 dev = [
     # dev version generation
     "setuptools_scm",
-    # static checking
-    "black>=20.8b1",
-    "docutils",
+    # test speedups
+    "pytest-xdist",
 ]
 doc = [
     "sphinx>=4.4",
     "sphinx-rtd-theme>=1.1.1",
     "sphinx-autodoc-typehints>=1.11.0",
     "sphinx_issues",
     "sphinxext.opengraph",
     "nbsphinx",
-    "scanpydoc>=0.7.7",
+    "scanpydoc[theme]>=0.9",
     "zarr",
     "awkward>=2.0.7",
     "IPython", # For syntax highlighting in notebooks
     "myst_parser",
 ]
 test = [
     "loompy>=3.0.5",
@@ -84,15 +83,15 @@
     "matplotlib",
     "scikit-learn",
     "openpyxl",
     "joblib",
     "boltons",
     "scanpy",
     "dask[array]",
-    "awkward>=2.0.6",
+    "awkward>=2.3",
     "pytest_memray",
 ]
 
 [tool.flit.sdist]
 exclude = [
     'anndata/tests/test_*.py',
     'anndata/tests/data',
@@ -106,15 +105,15 @@
 	"anndata/_version.py",
 	"**/test_*.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 python_files = "test_*.py"
-testpaths = ["anndata", "docs/concatenation.rst"]
+testpaths = ["anndata/tests", "docs/concatenation.rst"]
 filterwarnings = [
     'ignore:X\.dtype being converted to np.float32:FutureWarning'
 ]
 # For some reason this effects how logging is shown when tests are run
 xfail_strict = true
 
 [tool.black]
```

