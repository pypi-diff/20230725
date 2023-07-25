# Comparing `tmp/dask-deltatable-0.3.tar.gz` & `tmp/dask-deltatable-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-deltatable-0.3.tar", last modified: Fri Jul 14 12:40:13 2023, max compression
+gzip compressed data, was "dask-deltatable-0.3.1.tar", last modified: Tue Jul 25 13:22:01 2023, max compression
```

## Comparing `dask-deltatable-0.3.tar` & `dask-deltatable-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 12:39:27.000000 dask-deltatable-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 12:39:27.000000 dask-deltatable-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-14 12:40:13.605814 dask-deltatable-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-14 12:39:27.000000 dask-deltatable-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.601814 dask-deltatable-0.3/dask_deltatable/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/dask_deltatable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-14 12:39:27.000000 dask-deltatable-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 12:39:27.000000 dask-deltatable-0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:40:13.605814 dask-deltatable-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-14 12:39:27.000000 dask-deltatable-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_write.py
+drwxr-xr-x   0 fjetter    (501) staff       (20)        0 2023-07-25 13:22:01.465014 dask-deltatable-0.3.1/
+-rw-r--r--   0 fjetter    (501) staff       (20)     1517 2023-06-15 11:18:12.000000 dask-deltatable-0.3.1/LICENSE
+-rw-r--r--   0 fjetter    (501) staff       (20)       58 2023-07-10 08:31:12.000000 dask-deltatable-0.3.1/MANIFEST.in
+-rw-r--r--   0 fjetter    (501) staff       (20)     2959 2023-07-25 13:22:01.465080 dask-deltatable-0.3.1/PKG-INFO
+-rw-r--r--   0 fjetter    (501) staff       (20)     2122 2023-07-14 12:16:24.000000 dask-deltatable-0.3.1/README.md
+drwxr-xr-x   0 fjetter    (501) staff       (20)        0 2023-07-25 13:22:01.462911 dask-deltatable-0.3.1/dask_deltatable/
+-rw-r--r--   0 fjetter    (501) staff       (20)      192 2023-07-14 12:16:24.000000 dask-deltatable-0.3.1/dask_deltatable/__init__.py
+-rw-r--r--   0 fjetter    (501) staff       (20)    13508 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/dask_deltatable/_schema.py
+-rw-r--r--   0 fjetter    (501) staff       (20)     8717 2023-07-25 13:12:31.000000 dask-deltatable-0.3.1/dask_deltatable/core.py
+-rw-r--r--   0 fjetter    (501) staff       (20)        0 2023-07-10 08:31:12.000000 dask-deltatable-0.3.1/dask_deltatable/py.typed
+-rw-r--r--   0 fjetter    (501) staff       (20)      153 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/dask_deltatable/types.py
+-rw-r--r--   0 fjetter    (501) staff       (20)     1824 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/dask_deltatable/utils.py
+-rw-r--r--   0 fjetter    (501) staff       (20)    11988 2023-07-25 13:12:31.000000 dask-deltatable-0.3.1/dask_deltatable/write.py
+drwxr-xr-x   0 fjetter    (501) staff       (20)        0 2023-07-25 13:22:01.463749 dask-deltatable-0.3.1/dask_deltatable.egg-info/
+-rw-r--r--   0 fjetter    (501) staff       (20)     2959 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/PKG-INFO
+-rw-r--r--   0 fjetter    (501) staff       (20)      601 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/SOURCES.txt
+-rw-r--r--   0 fjetter    (501) staff       (20)        1 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/dependency_links.txt
+-rw-r--r--   0 fjetter    (501) staff       (20)        1 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/not-zip-safe
+-rw-r--r--   0 fjetter    (501) staff       (20)      100 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/requires.txt
+-rw-r--r--   0 fjetter    (501) staff       (20)       16 2023-07-25 13:22:01.000000 dask-deltatable-0.3.1/dask_deltatable.egg-info/top_level.txt
+-rw-r--r--   0 fjetter    (501) staff       (20)      416 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/pyproject.toml
+-rw-r--r--   0 fjetter    (501) staff       (20)       41 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/requirements.txt
+-rw-r--r--   0 fjetter    (501) staff       (20)      163 2023-07-25 13:22:01.465322 dask-deltatable-0.3.1/setup.cfg
+-rw-r--r--   0 fjetter    (501) staff       (20)     1322 2023-07-25 13:12:49.000000 dask-deltatable-0.3.1/setup.py
+drwxr-xr-x   0 fjetter    (501) staff       (20)        0 2023-07-25 13:22:01.464688 dask-deltatable-0.3.1/tests/
+-rw-r--r--   0 fjetter    (501) staff       (20)     5015 2023-07-14 12:16:24.000000 dask-deltatable-0.3.1/tests/test_acceptance.py
+-rw-r--r--   0 fjetter    (501) staff       (20)     6510 2023-07-25 13:12:31.000000 dask-deltatable-0.3.1/tests/test_core.py
+-rw-r--r--   0 fjetter    (501) staff       (20)     2458 2023-07-25 13:12:31.000000 dask-deltatable-0.3.1/tests/test_distributed.py
+-rw-r--r--   0 fjetter    (501) staff       (20)      987 2023-07-14 09:45:29.000000 dask-deltatable-0.3.1/tests/test_utils.py
+-rw-r--r--   0 fjetter    (501) staff       (20)     2180 2023-07-14 12:16:24.000000 dask-deltatable-0.3.1/tests/test_write.py
```

### Comparing `dask-deltatable-0.3/LICENSE` & `dask-deltatable-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/PKG-INFO` & `dask-deltatable-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-deltatable
-Version: 0.3
+Version: 0.3.1
 Summary: Dask + Delta Table 
 Maintainer: rajagurunath
 Maintainer-email: gurunathrajagopal@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-deltatable-0.3/README.md` & `dask-deltatable-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/dask_deltatable/_schema.py` & `dask-deltatable-0.3.1/dask_deltatable/_schema.py`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/dask_deltatable/core.py` & `dask-deltatable-0.3.1/dask_deltatable/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
+from collections.abc import Sequence
 from functools import partial
-from typing import Any
+from typing import Any, cast
 
 import dask.dataframe as dd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from dask.base import tokenize
 from dask.dataframe.utils import make_meta
 from deltalake import DataCatalog, DeltaTable
@@ -20,115 +21,104 @@
 if Version(pa.__version__) >= Version("10.0.0"):
     filters_to_expression = pq.filters_to_expression
 else:
     # fallback to older internal method
     filters_to_expression = pq._filters_to_expression
 
 
-class DeltaTableWrapper:
-    path: str
-    version: int | None
-    columns: list[str] | None
-    datetime: str | None
-    storage_options: dict[str, Any] | None
-
-    def __init__(
-        self,
-        path: str,
-        version: int | None,
-        columns: list[str] | None,
-        datetime: str | None = None,
-        storage_options: dict[str, str] | None = None,
-        delta_storage_options: dict[str, str] | None = None,
-    ) -> None:
-        self.path: str = path
-        self.version: int = version
-        self.columns = columns
-        self.datetime = datetime
-        self.storage_options = storage_options
-        self.dt = DeltaTable(
-            table_uri=self.path,
-            version=self.version,
-            storage_options=delta_storage_options,
-        )
-        self.fs, self.fs_token, _ = get_fs_token_paths(
-            path, storage_options=storage_options
-        )
-        self.schema = self.dt.schema().to_pyarrow()
+def _get_pq_files(dt: DeltaTable, filter: Filters = None) -> list[str]:
+    """
+    Get the list of parquet files after loading the
+    current datetime version
 
-    def meta(self, **kwargs):
-        """Pass kwargs to `to_pandas` call when creating the metadata"""
-        meta = make_meta(self.schema.empty_table().to_pandas(**kwargs))
-        if self.columns:
-            meta = meta[self.columns]
-        return meta
-
-    def read_delta_dataset(self, f: str, **kwargs: dict[Any, Any]):
-        schema = kwargs.pop("schema", None) or self.schema
-        filter = kwargs.pop("filter", None)
-        filter_expression = filters_to_expression(filter) if filter else None
-        to_pandas_kwargs = kwargs.pop("pyarrow_to_pandas", {})
-        return (
-            pa_ds.dataset(
-                source=f,
-                schema=schema,
-                filesystem=self.fs,
-                format="parquet",
-                partitioning="hive",
-            )
-            .to_table(filter=filter_expression, columns=self.columns)
-            .to_pandas(**to_pandas_kwargs)
-        )
+    Parameters
+    ----------
+    dt : DeltaTable
+        DeltaTable instance
+    filter : list[tuple[str, str, Any]] | list[list[tuple[str, str, Any]]] | None
+        Filters in DNF form.
 
-    def get_pq_files(self, filter: Filters = None) -> list[str]:
-        """
-        Get the list of parquet files after loading the
-        current datetime version
-
-        Parameters
-        ----------
-        filter : list[tuple[str, str, Any]] | list[list[tuple[str, str, Any]]] | None
-            Filters in DNF form.
-
-        Returns
-        -------
-        list[str]
-            List of files matching optional filter.
-        """
-        __doc__ == self.dt.load_with_datetime.__doc__
-        if self.datetime is not None:
-            self.dt.load_with_datetime(self.datetime)
-        partition_filters = get_partition_filters(
-            self.dt.metadata().partition_columns, filter
-        )
-        if not partition_filters:
-            # can't filter
-            return self.dt.file_uris()
-        file_uris = set()
-        for filter_set in partition_filters:
-            file_uris.update(self.dt.file_uris(partition_filters=filter_set))
-        return sorted(list(file_uris))
-
-    def read_delta_table(self, **kwargs) -> dd.core.DataFrame:
-        """
-        Reads the list of parquet files in parallel
-        """
-        pq_files = self.get_pq_files(filter=kwargs.get("filter", None))
-        if len(pq_files) == 0:
-            raise RuntimeError("No Parquet files are available")
-
-        meta = self.meta(**kwargs.get("pyarrow_to_pandas", {}))
-
-        return dd.from_map(
-            partial(self.read_delta_dataset, **kwargs),
-            pq_files,
-            meta=meta,
-            label="read-delta-table",
-            token=tokenize(self.fs_token, **kwargs),
+    Returns
+    -------
+    list[str]
+        List of files matching optional filter.
+    """
+    partition_filters = get_partition_filters(dt.metadata().partition_columns, filter)
+    if not partition_filters:
+        # can't filter
+        return dt.file_uris()
+    file_uris = set()
+    for filter_set in partition_filters:
+        file_uris.update(dt.file_uris(partition_filters=filter_set))
+    return sorted(list(file_uris))
+
+
+def _read_delta_partition(
+    filename: str,
+    schema: pa.Schema,
+    fs: Any,
+    columns: Sequence[str] | None,
+    filter: Filters = None,
+    pyarrow_to_pandas: dict[str, Any] | None = None,
+    **_kwargs: dict[str, Any],
+):
+    filter_expression = filters_to_expression(filter) if filter else None
+    if pyarrow_to_pandas is None:
+        pyarrow_to_pandas = {}
+    return (
+        pa_ds.dataset(
+            source=filename,
+            schema=schema,
+            filesystem=fs,
+            format="parquet",
+            partitioning="hive",
         )
+        .to_table(filter=filter_expression, columns=columns)
+        .to_pandas(**pyarrow_to_pandas)
+    )
+
+
+def _read_from_filesystem(
+    path: str,
+    version: int | None,
+    columns: Sequence[str] | None,
+    datetime: str | None = None,
+    storage_options: dict[str, str] | None = None,
+    delta_storage_options: dict[str, str] | None = None,
+    **kwargs: dict[str, Any],
+) -> dd.core.DataFrame:
+    """
+    Reads the list of parquet files in parallel
+    """
+    fs, fs_token, _ = get_fs_token_paths(path, storage_options=storage_options)
+    dt = DeltaTable(
+        table_uri=path, version=version, storage_options=delta_storage_options
+    )
+    if datetime is not None:
+        dt.load_with_datetime(datetime)
+
+    schema = dt.schema().to_pyarrow()
+
+    filter_value = cast(Filters, kwargs.get("filter", None))
+    pq_files = _get_pq_files(dt, filter=filter_value)
+    if len(pq_files) == 0:
+        raise RuntimeError("No Parquet files are available")
+
+    mapper_kwargs = kwargs.get("pyarrow_to_pandas", {})
+    meta = make_meta(schema.empty_table().to_pandas(**mapper_kwargs))
+    if columns:
+        meta = meta[columns]
+
+    return dd.from_map(
+        partial(_read_delta_partition, fs=fs, columns=columns, schema=schema, **kwargs),
+        pq_files,
+        meta=meta,
+        label="read-delta-table",
+        token=tokenize(fs_token, **kwargs),
+    )
 
 
 def _read_from_catalog(
     database_name: str, table_name: str, **kwargs
 ) -> dd.core.DataFrame:
     if ("AWS_ACCESS_KEY_ID" not in os.environ) and (
         "AWS_SECRET_ACCESS_KEY" not in os.environ
@@ -251,17 +241,17 @@
         else:
             resultdf = _read_from_catalog(
                 database_name=database_name, table_name=table_name, **kwargs
             )
     else:
         if path is None:
             raise ValueError("Please Provide Delta Table path")
-        dtw = DeltaTableWrapper(
+        resultdf = _read_from_filesystem(
             path=path,
             version=version,
             columns=columns,
             storage_options=storage_options,
             datetime=datetime,
             delta_storage_options=delta_storage_options,
+            **kwargs,
         )
-        resultdf = dtw.read_delta_table(columns=columns, **kwargs)
     return resultdf
```

### Comparing `dask-deltatable-0.3/dask_deltatable/utils.py` & `dask-deltatable-0.3.1/dask_deltatable/utils.py`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/dask_deltatable/write.py` & `dask-deltatable-0.3.1/dask_deltatable/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     table_or_uri: str | Path | DeltaTable,
     df: dd.DataFrame,
     *,
     schema: pa.Schema | None = None,
     partition_by: list[str] | str | None = None,
     filesystem: pa_fs.FileSystem | None = None,
     mode: Literal["error", "append", "overwrite", "ignore"] = "error",
-    file_options: ds.ParquetFileWriteOptions | None = None,
+    file_options: Mapping[str, Any] | None = None,
     max_partitions: int | None = None,
     max_open_files: int = 1024,
     max_rows_per_file: int = 10 * 1024 * 1024,
     min_rows_per_group: int = 64 * 1024,
     max_rows_per_group: int = 128 * 1024,
     name: str | None = None,
     description: str | None = None,
@@ -74,17 +74,16 @@
         be inferred from uri. The file system has to be rooted in the table root.
         Use the pyarrow.fs.SubTreeFileSystem, to adopt the root of pyarrow file systems.
     mode : Literal["error", "append", "overwrite", "ignore"]. Default "error"
         How to handle existing data. Default is to error if table already exists.
         If 'append', will add new data.
         If 'overwrite', will replace table with new data.
         If 'ignore', will not write anything if table already exists.
-    file_options : ds.ParquetFileWriteOptions | None. Default None
-        Optional write options for Parquet (ParquetFileWriteOptions).
-        Can be provided with defaults using ParquetFileWriteOptions().make_write_options().
+    file_options : Mapping[str, Any] | None. Default None
+        Optional dict of options that can be used to initialize ParquetFileWriteOptions.
         Please refer to https://github.com/apache/arrow/blob/master/python/pyarrow/_dataset_parquet.pyx
         for the list of available options
     max_partitions : int | None. Default None
         The maximum number of partitions that will be used.
     max_open_files : int. Default 1024
         Limits the maximum number of
         files that can be left open while writing. If an attempt is made to open
@@ -311,14 +310,17 @@
                 partition_values,
                 int(datetime.now().timestamp() * 1000),
                 True,
                 json.dumps(stats, cls=DeltaJSONEncoder),
             )
         )
 
+    if file_options is not None:
+        file_options = ds.ParquetFileFormat().make_write_options(**file_options)
+
     ds.write_dataset(
         data,
         base_dir="/",
         basename_template=f"{current_version + 1}-{uuid.uuid4()}-{{i}}.parquet",
         format="parquet",
         partitioning=partitioning,
         # It will not accept a schema if using a RBR
```

### Comparing `dask-deltatable-0.3/dask_deltatable.egg-info/PKG-INFO` & `dask-deltatable-0.3.1/dask_deltatable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-deltatable
-Version: 0.3
+Version: 0.3.1
 Summary: Dask + Delta Table 
 Maintainer: rajagurunath
 Maintainer-email: gurunathrajagopal@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-deltatable-0.3/dask_deltatable.egg-info/SOURCES.txt` & `dask-deltatable-0.3.1/dask_deltatable.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 dask_deltatable.egg-info/SOURCES.txt
 dask_deltatable.egg-info/dependency_links.txt
 dask_deltatable.egg-info/not-zip-safe
 dask_deltatable.egg-info/requires.txt
 dask_deltatable.egg-info/top_level.txt
 tests/test_acceptance.py
 tests/test_core.py
+tests/test_distributed.py
 tests/test_utils.py
 tests/test_write.py
```

### Comparing `dask-deltatable-0.3/setup.py` & `dask-deltatable-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dask-deltatable",
-    version="0.3",
+    version="0.3.1",
     description="Dask + Delta Table ",
     maintainer="rajagurunath",
     maintainer_email="gurunathrajagopal@gmail.com",
     license="BSD-3-Clause",
     packages=["dask_deltatable"],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `dask-deltatable-0.3/tests/test_acceptance.py` & `dask-deltatable-0.3.1/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/tests/test_core.py` & `dask-deltatable-0.3.1/tests/test_core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,21 @@
 from __future__ import annotations
 
 import glob
 import os
-import zipfile
 from unittest.mock import MagicMock, patch
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pytest
 from deltalake import DeltaTable
 
 import dask_deltatable as ddt
 
-ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
-DATA_DIR = os.path.join(ROOT_DIR, "data")
-
-
-@pytest.fixture()
-def simple_table(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/simple.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/test1/"
-
-
-@pytest.fixture()
-def simple_table2(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/simple2.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/simple_table/"
-
-
-@pytest.fixture()
-def partition_table(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/partition.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/test2/"
-
-
-@pytest.fixture()
-def empty_table1(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/empty1.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/empty/"
-
-
-@pytest.fixture()
-def empty_table2(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/empty2.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/empty2/"
-
-
-@pytest.fixture()
-def checkpoint_table(tmpdir):
-    output_dir = tmpdir
-    deltaf = zipfile.ZipFile(f"{DATA_DIR}/checkpoint.zip")
-    deltaf.extractall(output_dir)
-    return str(output_dir) + "/checkpoint/"
-
 
 def test_read_delta(simple_table):
     df = ddt.read_deltalake(simple_table)
 
     assert df.columns.tolist() == ["id", "count", "temperature", "newColumn"]
     assert df.compute().shape == (200, 4)
```

### Comparing `dask-deltatable-0.3/tests/test_utils.py` & `dask-deltatable-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-deltatable-0.3/tests/test_write.py` & `dask-deltatable-0.3.1/tests/test_write.py`

 * *Files identical despite different names*

