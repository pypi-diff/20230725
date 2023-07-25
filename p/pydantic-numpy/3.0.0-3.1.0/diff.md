# Comparing `tmp/pydantic_numpy-3.0.0.tar.gz` & `tmp/pydantic_numpy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-3.0.0.tar", max compression
+gzip compressed data, was "pydantic_numpy-3.1.0.tar", max compression
```

## Comparing `pydantic_numpy-3.0.0.tar` & `pydantic_numpy-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.0.0/LICENSE
--rw-r--r--   0        0        0     1967 2023-07-24 07:26:03.954095 pydantic_numpy-3.0.0/README.md
--rw-r--r--   0        0        0      189 2023-07-24 08:00:18.252802 pydantic_numpy-3.0.0/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 08:09:14.284263 pydantic_numpy-3.0.0/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0     5666 2023-07-24 11:20:43.842009 pydantic_numpy-3.0.0/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0     2005 2023-07-24 11:04:27.972235 pydantic_numpy-3.0.0/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0     7428 2023-07-24 12:17:49.594506 pydantic_numpy-3.0.0/pydantic_numpy/model.py
--rw-r--r--   0        0        0        0 2023-07-24 08:00:18.249803 pydantic_numpy-3.0.0/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-24 08:19:57.319153 pydantic_numpy-3.0.0/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     2285 2023-07-24 08:19:57.259153 pydantic_numpy-3.0.0/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     2284 2023-07-24 08:19:57.293153 pydantic_numpy-3.0.0/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     2036 2023-07-24 08:19:57.247153 pydantic_numpy-3.0.0/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2023-07-23 11:42:56.554729 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/__init__.py
--rw-r--r--   0        0        0     2860 2023-07-24 08:35:12.890564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/i_dimensional.py
--rw-r--r--   0        0        0     2860 2023-07-24 08:35:12.883564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/ii_dimensional.py
--rw-r--r--   0        0        0     2859 2023-07-24 08:36:13.362365 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/iii_dimensional.py
--rw-r--r--   0        0        0     2578 2023-07-24 08:35:12.875564 pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/n_dimensional.py
--rw-r--r--   0        0        0      571 2023-07-24 12:11:47.665552 pydantic_numpy-3.0.0/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1171 2023-07-24 12:41:09.789859 pydantic_numpy-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 pydantic_numpy-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2703 2023-07-25 16:31:55.726059 pydantic_numpy-3.1.0/README.md
+-rw-r--r--   0        0        0      138 2023-07-25 15:36:47.472916 pydantic_numpy-3.1.0/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:54.840721 pydantic_numpy-3.1.0/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0     5565 2023-07-25 15:51:56.951261 pydantic_numpy-3.1.0/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0     3891 2023-07-25 15:34:13.657876 pydantic_numpy-3.1.0/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0      118 2023-07-25 10:48:54.840721 pydantic_numpy-3.1.0/pydantic_numpy/model/__init__.py
+-rw-r--r--   0        0        0     1116 2023-07-25 15:40:17.968604 pydantic_numpy-3.1.0/pydantic_numpy/model/multi_array.py
+-rw-r--r--   0        0        0     8605 2023-07-25 15:45:03.591827 pydantic_numpy-3.1.0/pydantic_numpy/model/np_model.py
+-rw-r--r--   0        0        0      474 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     2285 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     2284 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     2036 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     2860 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     2860 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     2859 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     2578 2023-07-25 10:48:54.842721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0      868 2023-07-25 16:29:51.865761 pydantic_numpy-3.1.0/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1181 2023-07-25 11:13:47.189996 pydantic_numpy-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.0/PKG-INFO
```

### Comparing `pydantic_numpy-3.0.0/LICENSE` & `pydantic_numpy-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/README.md` & `pydantic_numpy-3.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 # pydantic-numpy
 
-Integrate NumPy into Pydantic, and provide tooling! `NumpyModel` make it possible to dump and load `np.ndarray` within model fields!
+Package that integrates NumPy Arrays into Pydantic!
 
-### Install
-```shell
-pip install pydantic-numpy
-```
+- `NumpyModel` make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
+- `pydantic_numpy.typing` provides many typings such as `NpNDArrayFp64`, `Np3DArrayFp64` (float64 that must be 3D)!
 
 ## Usage
 
 For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
-import pydantic_numpy.dtype as pnd
-from pydantic_numpy import NDArray, NDArrayFp32, NumpyModel
+import numpy as np
+
+import pydantic_numpy.typing as pnd
+from pydantic_numpy import np_array_pydantic_annotated_typing
+from pydantic_numpy.model import NumpyModel, MultiArrayNumpyFile
+
+
+class MyNumpyModel(NumpyModel):
+    any_array_dtype_and_dimension: pnd.NpNDArray
+
+    # Must be numpy float32 as dtype
+    k: np_array_pydantic_annotated_typing(data_type=np.float32)
+    shorthand_for_k: pnd.NpNDArrayFp32
+
+    must_be_1d_np_array: np_array_pydantic_annotated_typing(dimensions=1)
 
 
-class MyPydanticNumpyModel(NumpyModel):
-    K: NDArray[float, pnd.float32]
-    C: NDArrayFp32  # <- Shorthand for same type as K
+class MyDemoModel(NumpyModel):
+    k: np_array_pydantic_annotated_typing(data_type=np.float32)
 
 
 # Instantiate from array
-cfg = MyPydanticNumpyModel(K=[1, 2])
+cfg = MyDemoModel(k=[1, 2])
 # Instantiate from numpy file
-cfg = MyPydanticNumpyModel(K={"path": "path_to/array.npy"})
+cfg = MyDemoModel(k="path_to/array.npy")
 # Instantiate from npz file with key
-cfg = MyPydanticNumpyModel(K={"path": "path_to/array.npz", "key": "K"})
+cfg = MyDemoModel(k=MultiArrayNumpyFile(path="path_to/array.npz", key="k"))
 
-cfg.K
-# np.ndarray[np.float32]
+cfg.k   # np.ndarray[np.float32]
 
 cfg.dump("path_to_dump_dir", "object_id")
 cfg.load("path_to_dump_dir", "object_id")
 ```
 
-`NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model.
+`NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model:
+```python
+from pydantic_numpy.model.np_model import model_agnostic_load
+
+cfg.dump("path_to_dump_dir", "object_id")
+equals_cfg = model_agnostic_load("path_to_dump_dir", "object_id", models=[MyNumpyModel, MyDemoModel])
+```
 
 ### Data type (dtype) support!
 
-This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
+This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NpNDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
+
+### Install
+```shell
+pip install pydantic-numpy
+```
 
 ## Considerations
 You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only support Pydantic V1 and will not work with V2.
 
 ### Licensing notice
 As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
-## History
+### History
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-3.1.0/pydantic_numpy/helper/annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 from pydantic import FilePath, GetJsonSchemaHandler, PositiveInt
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
 from typing_extensions import Annotated
 
 from pydantic_numpy.helper.validation import (
     create_array_validator,
-    read_and_verify_numpy_file,
+    validate_multi_array_numpy_file,
+    validate_numpy_array_file,
 )
+from pydantic_numpy.model.multi_array import MultiArrayNumpyFile
 
 
 class NpArrayPydanticAnnotation:
     dimensions: ClassVar[Optional[PositiveInt]]
 
     data_type: ClassVar[DTypeLike]
     strict_data_typing: ClassVar[bool]
 
     @classmethod
-    def factory(cls, *, data_type: DTypeLike, dimensions: Optional[int], strict_data_typing: bool = False) -> type:
+    def factory(
+        cls, *, data_type: DTypeLike, dimensions: Optional[int] = None, strict_data_typing: bool = False
+    ) -> type:
         """
         Create an instance NpArrayPydanticAnnotation that is configured for a specific dimension and dtype.
 
         The signature of the function is data_type, dimension and not dimension, data_type to reduce amount of
         code for all the types.
 
         Parameters
@@ -62,91 +66,90 @@
         _source_type: Any,
         _handler: Callable[[Any], core_schema.CoreSchema],
     ) -> core_schema.CoreSchema:
         np_array_validator = create_array_validator(cls.dimensions, cls.data_type, cls.strict_data_typing)
         np_array_schema = core_schema.no_info_plain_validator_function(np_array_validator)
 
         return core_schema.json_or_python_schema(
-            python_schema=core_schema.chain_schema(
-                [
-                    core_schema.union_schema(
-                        [
-                            core_schema.chain_schema(
-                                [
-                                    core_schema.is_instance_schema(Path),
-                                    core_schema.no_info_plain_validator_function(read_and_verify_numpy_file),
-                                ]
-                            ),
-                            core_schema.is_instance_schema(np.ndarray),
-                            core_schema.chain_schema(
-                                [
-                                    core_schema.is_instance_schema(Sequence),
-                                    core_schema.no_info_plain_validator_function(lambda v: np.asarray(v)),
-                                ]
-                            ),
-                        ]
-                    ),
-                    np_array_schema,
-                ]
-            ),
+            python_schema=core_schema.chain_schema([_common_numpy_array_validator, np_array_schema]),
             json_schema=np_array_schema,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda arr: np.array2string(arr), when_used="json"
             ),
         )
 
     @classmethod
     def __get_pydantic_json_schema__(
         cls, _core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         return handler(
             dict(
                 type=(
                     f"np.ndarray[{_int_to_dim_type[cls.dimensions] if cls.dimensions else 'Any'}, "
-                    f"{np.dtype[cls.data_type.__name__] if _data_type_resolver(cls.data_type) else cls.data_type}]"
+                    f"{np.dtype[cls.data_type.__name__] if _data_type_resolver(cls.data_type) else cls.data_type}]"  # type: ignore[name-defined]
                 ),
                 strict_data_typing=cls.strict_data_typing,
             )
         )
 
 
 def np_array_pydantic_annotated_typing(
     data_type: DTypeLike = None, dimensions: Optional[int] = None, strict_data_typing: bool = False
 ):
+    """
+    Generates typing and pydantic annotation of a np.ndarray parametrized with given constraints
+
+    Parameters
+    ----------
+    data_type: DTypeLike
+    dimensions: Optional[int]
+        Number of dimensions determine the depth of the numpy array.
+    strict_data_typing: bool
+        If True, the dtype of the numpy array must be identical to the data_type. No conversion attempts.
+
+    Returns
+    -------
+    type-hint for np.ndarray with Pydantic support
+    """
     return Annotated[
         Union[
             FilePath,
-            np.ndarray[
+            MultiArrayNumpyFile,
+            np.ndarray[  # type: ignore[misc]
                 _int_to_dim_type[dimensions] if dimensions else Any,
                 np.dtype[data_type] if _data_type_resolver(data_type) else data_type,
             ],
         ],
         NpArrayPydanticAnnotation.factory(
             data_type=data_type, dimensions=dimensions, strict_data_typing=strict_data_typing
         ),
     ]
 
 
 def _data_type_resolver(data_type: DTypeLike):
     return data_type is not None and issubclass(data_type, np.generic)
 
 
-def _read_and_verify_numpy_file(v: FilePath) -> npt.NDArray:
-    result = np.load(v)
-
-    if isinstance(result, NpzFile):
-        files = result.files
-        if len(files) > 1:
-            msg = (
-                f"The provided file path is a multi array NpzFile, which is not supported; "
-                f"convert to single array NpzFiles.\n"
-                f"Path to multi array file: {result}\n"
-                f"Array keys: {', '.join(result.files)}"
-            )
-            raise ValueError(msg)
-        result = result[files[0]]
-
-    return result
-
-
-_read_and_verify_numpy_file_validator = core_schema.no_info_plain_validator_function(_read_and_verify_numpy_file)
 _int_to_dim_type = {1: tuple[int], 2: tuple[int, int], 3: tuple[int, int, int]}
+_common_numpy_array_validator = core_schema.union_schema(
+    [
+        core_schema.chain_schema(
+            [
+                core_schema.is_instance_schema(Path),
+                core_schema.no_info_plain_validator_function(validate_numpy_array_file),
+            ]
+        ),
+        core_schema.chain_schema(
+            [
+                core_schema.is_instance_schema(MultiArrayNumpyFile),
+                core_schema.no_info_plain_validator_function(validate_multi_array_numpy_file),
+            ]
+        ),
+        core_schema.is_instance_schema(np.ndarray),
+        core_schema.chain_schema(
+            [
+                core_schema.is_instance_schema(Sequence),
+                core_schema.no_info_plain_validator_function(lambda v: np.asarray(v)),
+            ]
+        ),
+    ]
+)
```

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/model.py` & `pydantic_numpy-3.1.0/pydantic_numpy/model/np_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle as pickle_pkg
 from pathlib import Path
-from typing import Any, Callable, ClassVar, Iterable, Optional, Type
+from typing import Any, Callable, ClassVar, Iterable, Optional
 
 import compress_pickle
 import numpy as np
 import numpy.typing as npt
-from pydantic import BaseModel, DirectoryPath, FilePath, validate_call
+from pydantic import BaseModel, DirectoryPath, FilePath, computed_field, validate_call
 from ruamel.yaml import YAML
 
 from pydantic_numpy.util import np_general_all_close
 
 yaml = YAML()
 
 
@@ -18,17 +18,14 @@
     _dump_numpy_savez_file_name: ClassVar[str] = "arrays.npz"
     _dump_non_array_file_stem: ClassVar[str] = "object_info"
 
     _directory_suffix: ClassVar[str] = ".pdnp"
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, NumpyModel):
-            # When comparing instances of generic types for equality, as long as all field values are equal,
-            # only require their generic origin types to be equal, rather than exact type equality.
-            # This prevents headaches like MyGeneric(x=1) != MyGeneric[Any](x=1).
             self_type = self.__pydantic_generic_metadata__["origin"] or self.__class__
             other_type = other.__pydantic_generic_metadata__["origin"] or other.__class__
 
             self_ndarray_field_to_array, self_other_field_to_value = self._dump_numpy_split_dict()
             other_ndarray_field_to_array, other_other_field_to_value = other._dump_numpy_split_dict()
 
             return (
@@ -44,17 +41,64 @@
             return NotImplemented  # delegate to the other item in the comparison
 
     @classmethod
     @validate_call
     def model_directory_path(cls, output_directory: DirectoryPath, object_id: str) -> DirectoryPath:
         return output_directory / f"{object_id}.{cls.__name__}{cls._directory_suffix}"
 
+    @classmethod
+    @validate_call
+    def load(
+        cls,
+        output_directory: DirectoryPath,
+        object_id: str,
+        *,
+        pre_load_modifier: Optional[Callable[[dict[str, Any]], dict[str, Any]]] = None,
+    ):
+        """
+        Load NumpyModel instance
+
+        Parameters
+        ----------
+        output_directory: DirectoryPath
+            The root directory where all model instances of interest are stored
+        object_id: String
+            The ID of the model instance
+        pre_load_modifier: Callable[[dict[str, Any]], dict[str, Any]] | None
+            Optional function that modifies the loaded arrays
+
+        Returns
+        -------
+        NumpyModel instance
+        """
+        object_directory_path = cls.model_directory_path(output_directory, object_id)
+
+        npz_file = np.load(object_directory_path / cls._dump_numpy_savez_file_name)
+
+        other_path: FilePath
+        if (other_path := object_directory_path / cls._dump_compressed_pickle_file_name).exists():
+            other_field_to_value = compress_pickle.load(other_path)
+        elif (other_path := object_directory_path / cls._dump_pickle_file_name).exists():
+            with open(other_path, "rb") as in_pickle:
+                other_field_to_value = pickle_pkg.load(in_pickle)
+        elif (other_path := object_directory_path / cls._dump_non_array_yaml_name).exists():
+            with open(other_path, "r") as in_yaml:
+                other_field_to_value = yaml.load(in_yaml)
+        else:
+            other_field_to_value = {}
+
+        field_to_value = {**npz_file, **other_field_to_value}
+        if pre_load_modifier:
+            field_to_value = pre_load_modifier(field_to_value)
+
+        return cls(**field_to_value)
+
     @validate_call
     def dump(
-        self, output_directory: Path, object_id: str, compress: bool = True, pickle: bool = False
+        self, output_directory: Path, object_id: str, *, compress: bool = True, pickle: bool = False
     ) -> DirectoryPath:
         assert "arbitrary_types_allowed" not in self.model_config or (
             self.model_config["arbitrary_types_allowed"] and pickle
         ), "Arbitrary types are only supported in pickle mode"
 
         dump_directory_path = self.model_directory_path(output_directory, object_id)
         dump_directory_path.mkdir(parents=True, exist_ok=True)
@@ -80,82 +124,73 @@
 
             else:
                 with open(dump_directory_path / self._dump_non_array_yaml_name, "w") as out_yaml:
                     yaml.dump(other_field_to_value, out_yaml)
 
         return dump_directory_path
 
-    @classmethod
-    @validate_call
-    def load(
-        cls,
-        output_directory: DirectoryPath,
-        object_id: str,
-        pre_load_modifier: Optional[Callable[[dict[str, Any]], dict[str, Any]]] = None,
-    ):
-        object_directory_path = cls.model_directory_path(output_directory, object_id)
-
-        npz_file = np.load(object_directory_path / cls._dump_numpy_savez_file_name)
-
-        other_path: FilePath
-        if (other_path := object_directory_path / cls._dump_compressed_pickle_file_name).exists():
-            other_field_to_value = compress_pickle.load(other_path)
-        elif (other_path := object_directory_path / cls._dump_pickle_file_name).exists():
-            with open(other_path, "rb") as in_pickle:
-                other_field_to_value = pickle_pkg.load(in_pickle)
-        elif (other_path := object_directory_path / cls._dump_non_array_yaml_name).exists():
-            with open(other_path, "r") as in_yaml:
-                other_field_to_value = yaml.load(in_yaml)
-        else:
-            other_field_to_value = {}
-
-        field_to_value = {**npz_file, **other_field_to_value}
-        if pre_load_modifier:
-            field_to_value = pre_load_modifier(field_to_value)
-
-        return cls(**field_to_value)
-
     def _dump_numpy_split_dict(self) -> tuple[dict, dict]:
         ndarray_field_to_array = {}
         other_field_to_value = {}
 
         for k, v in self.model_dump(exclude_unset=True).items():
             if isinstance(v, np.ndarray):
                 ndarray_field_to_array[k] = v
             else:
                 other_field_to_value[k] = v
 
         return ndarray_field_to_array, other_field_to_value
 
-    @classmethod
+    @classmethod  # type: ignore[misc]
+    @computed_field(return_type=str)
     @property
     def _dump_compressed_pickle_file_name(cls) -> str:
         return f"{cls._dump_non_array_file_stem}.pickle.{cls._dump_compression}"
 
-    @classmethod
+    @classmethod  # type: ignore[misc]
+    @computed_field(return_type=str)
     @property
     def _dump_pickle_file_name(cls) -> str:
         return f"{cls._dump_non_array_file_stem}.pickle"
 
-    @classmethod
+    @classmethod  # type: ignore[misc]
+    @computed_field(return_type=str)
     @property
     def _dump_non_array_yaml_name(cls) -> str:
         return f"{cls._dump_non_array_file_stem}.yaml"
 
 
-NumpyModelCLS = Type[NumpyModel]
-
-
 def model_agnostic_load(
     output_directory: DirectoryPath,
     object_id: str,
-    models: Iterable[NumpyModelCLS],
+    models: Iterable[type[NumpyModel]],
     not_found_error: bool = False,
     **load_kwargs,
 ) -> Optional[NumpyModel]:
+    """
+    Provided an Iterable containing possible models, and the directory where they have been dumped. Load the first
+    instance of model that matches the provided object ID.
+
+    Parameters
+    ----------
+    output_directory: DirectoryPath
+        The root directory where all model instances of interest are stored
+    object_id: String
+        The ID of the model instance
+    models: Iterable[type[NumpyModel]]
+        All NumpyModel instances of interest, note that they should have differing names
+    not_found_error: bool
+        If True, throw error when the respective model instance was not found
+    load_kwargs
+        Key-word arguments to pass to the load function
+
+    Returns
+    -------
+    NumpyModel instance if found
+    """
     for model in models:
         if model.model_directory_path(output_directory, object_id).exists():
             return model.load(output_directory, object_id, **load_kwargs)
 
     if not_found_error:
         raise FileNotFoundError(
             f"Could not find NumpyModel with {object_id} in {output_directory}."
@@ -188,11 +223,14 @@
     for key in keys1:
         arr_a = dict_a[key]
         arr_b = dict_b[key]
 
         if arr_a.shape != arr_b.shape:
             raise ValueError(f"Arrays for key '{key}' have different shapes")
 
-        if not np_general_all_close(arr_a, arr_b):
+        if not np_general_all_close(arr_a, arr_b, rtol, atol):
             return False
 
     return True
+
+
+__all__ = ["NumpyModel", "model_agnostic_load"]
```

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/i_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/ii_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/iii_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pydantic_numpy/typing/strict/n_dimensional.py` & `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.0.0/pyproject.toml` & `pydantic_numpy-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "3.0.0"
+version = "3.1.0"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
 
@@ -20,22 +20,24 @@
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 compress-pickle = { version = "*", extras = ["lz4"] }
 ruamel-yaml = "^0.17.21"
 
 numpy = "*"
 pydantic = "^2.0"
-coverage = "^7.2.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 parameterized = "^0.9.0"
 hypothesis = "^6.82.0"
 setuptools = "^68.0.0"
-pytest-xdist = "^3.3.1"
+
+
+[tool.poetry.group.ci.dependencies]
+mypy = "^1.4.1"
 
 [tool.black]
 line-length = 120
 target-version = ["py311"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `pydantic_numpy-3.0.0/PKG-INFO` & `pydantic_numpy-3.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 3.0.0
+Version: 3.1.0
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
@@ -14,64 +14,83 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: compress-pickle[lz4]
-Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: numpy
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Description-Content-Type: text/markdown
 
 # pydantic-numpy
 
-Integrate NumPy into Pydantic, and provide tooling! `NumpyModel` make it possible to dump and load `np.ndarray` within model fields!
+Package that integrates NumPy Arrays into Pydantic!
 
-### Install
-```shell
-pip install pydantic-numpy
-```
+- `NumpyModel` make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
+- `pydantic_numpy.typing` provides many typings such as `NpNDArrayFp64`, `Np3DArrayFp64` (float64 that must be 3D)!
 
 ## Usage
 
 For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
-import pydantic_numpy.dtype as pnd
-from pydantic_numpy import NDArray, NDArrayFp32, NumpyModel
+import numpy as np
+
+import pydantic_numpy.typing as pnd
+from pydantic_numpy import np_array_pydantic_annotated_typing
+from pydantic_numpy.model import NumpyModel, MultiArrayNumpyFile
+
+
+class MyNumpyModel(NumpyModel):
+    any_array_dtype_and_dimension: pnd.NpNDArray
+
+    # Must be numpy float32 as dtype
+    k: np_array_pydantic_annotated_typing(data_type=np.float32)
+    shorthand_for_k: pnd.NpNDArrayFp32
+
+    must_be_1d_np_array: np_array_pydantic_annotated_typing(dimensions=1)
 
 
-class MyPydanticNumpyModel(NumpyModel):
-    K: NDArray[float, pnd.float32]
-    C: NDArrayFp32  # <- Shorthand for same type as K
+class MyDemoModel(NumpyModel):
+    k: np_array_pydantic_annotated_typing(data_type=np.float32)
 
 
 # Instantiate from array
-cfg = MyPydanticNumpyModel(K=[1, 2])
+cfg = MyDemoModel(k=[1, 2])
 # Instantiate from numpy file
-cfg = MyPydanticNumpyModel(K={"path": "path_to/array.npy"})
+cfg = MyDemoModel(k="path_to/array.npy")
 # Instantiate from npz file with key
-cfg = MyPydanticNumpyModel(K={"path": "path_to/array.npz", "key": "K"})
+cfg = MyDemoModel(k=MultiArrayNumpyFile(path="path_to/array.npz", key="k"))
 
-cfg.K
-# np.ndarray[np.float32]
+cfg.k   # np.ndarray[np.float32]
 
 cfg.dump("path_to_dump_dir", "object_id")
 cfg.load("path_to_dump_dir", "object_id")
 ```
 
-`NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model.
+`NumpyModel.load` requires the original mode, use `model_agnostic_load` when you have several models that may be the right model:
+```python
+from pydantic_numpy.model.np_model import model_agnostic_load
+
+cfg.dump("path_to_dump_dir", "object_id")
+equals_cfg = model_agnostic_load("path_to_dump_dir", "object_id", models=[MyNumpyModel, MyDemoModel])
+```
 
 ### Data type (dtype) support!
 
-This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
+This package also comes with `pydantic_numpy.dtype`, which adds subtyping support such as `NpNDArray[float, pnd.float32]`. All subfields must be from this package as numpy dtypes have no Pydantic support, which is implemented in this package through the [generic class workflow](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
+
+### Install
+```shell
+pip install pydantic-numpy
+```
 
 ## Considerations
 You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only support Pydantic V1 and will not work with V2.
 
 ### Licensing notice
 As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
-## History
+### History
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

