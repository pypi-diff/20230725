# Comparing `tmp/bstk_datatables-0.1.9.tar.gz` & `tmp/bstk_datatables-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.1.9.tar", max compression
+gzip compressed data, was "bstk_datatables-0.2.0.tar", max compression
```

## Comparing `bstk_datatables-0.1.9.tar` & `bstk_datatables-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/README.md
--rw-r--r--   0        0        0     2358 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/merge.py
--rw-r--r--   0        0        0     7894 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-20 01:49:23.681001 bstk_datatables-0.1.9/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-07-20 01:49:44.265191 bstk_datatables-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/README.md
+-rw-r--r--   0        0        0     2358 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3248 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     8118 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-07-25 05:46:45.349943 bstk_datatables-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.0/PKG-INFO
```

### Comparing `bstk_datatables-0.1.9/README.md` & `bstk_datatables-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/bstk_datatables/__init__.py` & `bstk_datatables-0.2.0/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/bstk_datatables/entry.py` & `bstk_datatables-0.2.0/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/bstk_datatables/enum.py` & `bstk_datatables-0.2.0/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/bstk_datatables/merge.py` & `bstk_datatables-0.2.0/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/bstk_datatables/schema.py` & `bstk_datatables-0.2.0/bstk_datatables/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,29 +171,31 @@
 
 @dataclass
 class SchemaFieldFormat:
     type: typing.Optional[typing.AnyStr]
     values: typing.Optional[typing.Any] = None
     lookup: typing.Optional[typing.Any] = None
     required: typing.Optional[bool] = field(default=False)
+    readonly: typing.Optional[bool] = field(default=False)
     many: typing.Optional[bool] = field(default=False)
+    markup: typing.Optional[typing.Dict] = field(default=None)
     _field: marshmallow_fields.Field = field(init=False, default=None)
     _missing_lookup: bool = field(init=False, default=False)
 
     def __post_init__(self):
         self._generate_marshmallow_field()
 
     def attach_lookup(
         self, lookup_value: typing.Union[typing.List[typing.AnyStr], PyEnum]
     ):
         self.lookup = lookup_value
         self._generate_marshmallow_field()
 
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
-        _fields = ["type", "values", "lookup", "required", "many"]
+        _fields = ["type", "values", "lookup", "required", "readonly", "many", "markup"]
         rtn = {}
         for _exportfield in _fields:
             if _exportfield == "lookup" and isinstance(
                 self.__dict__[_exportfield], Enum
             ):
                 rtn[_exportfield] = self.__dict__[_exportfield].code
                 continue
@@ -207,14 +209,16 @@
 
         raise ValueError(f"Field format type `{self.type}` is invalid")
 
     def _get_field_params(self) -> typing.Union[None, typing.Dict]:
         _field_params = {}
         if self.required is not None:
             _field_params["required"] = self.required
+        if self.readonly is True:
+            _field_params["dump_only"] = True
         if self.type == "enum":
             self._missing_lookup = False
             if self.values:
                 _field_params["enum"] = PyEnum("enum", self.values)
             elif self.lookup and isinstance(self.lookup, Enum):
                 _field_params["enum"] = self.lookup.values
             else:
```

### Comparing `bstk_datatables-0.1.9/bstk_datatables/table.py` & `bstk_datatables-0.2.0/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.9/pyproject.toml` & `bstk_datatables-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.1.9"
+version = "0.2.0"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.1.9/PKG-INFO` & `bstk_datatables-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.1.9
+Version: 0.2.0
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

