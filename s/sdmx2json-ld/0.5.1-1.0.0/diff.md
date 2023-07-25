# Comparing `tmp/sdmx2json_ld-0.5.1.tar.gz` & `tmp/sdmx2json_ld-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmx2json_ld-0.5.1.tar", max compression
+gzip compressed data, was "sdmx2json_ld-1.0.0.tar", max compression
```

## Comparing `sdmx2json_ld-0.5.1.tar` & `sdmx2json_ld-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,69 @@
--rw-r--r--   0        0        0    11353 2022-10-27 12:12:59.631282 sdmx2json_ld-0.5.1/LICENSE
--rw-r--r--   0        0        0      909 2022-10-27 14:47:49.068499 sdmx2json_ld-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6018 2022-10-27 14:47:49.009407 sdmx2json_ld-0.5.1/sdmx2jsonld/README.md
--rw-r--r--   0        0        0        0 2022-10-27 12:12:59.730705 sdmx2json_ld-0.5.1/sdmx2jsonld/__init__.py
--rw-r--r--   0        0        0     3924 2022-10-27 12:12:59.731879 sdmx2json_ld-0.5.1/sdmx2jsonld/common/classprecedence.py
--rw-r--r--   0        0        0     2610 2022-10-27 12:12:59.732701 sdmx2json_ld-0.5.1/sdmx2jsonld/common/commonclass.py
--rw-r--r--   0        0        0      611 2022-10-27 15:17:31.793576 sdmx2json_ld-0.5.1/sdmx2jsonld/common/config.py
--rw-r--r--   0        0        0     6337 2022-10-27 12:12:59.734148 sdmx2json_ld-0.5.1/sdmx2jsonld/common/datatypeconversion.py
--rw-r--r--   0        0        0     2478 2022-10-27 12:12:59.735010 sdmx2json_ld-0.5.1/sdmx2jsonld/common/listmanagement.py
--rw-r--r--   0        0        0      953 2022-10-27 12:12:59.735792 sdmx2json_ld-0.5.1/sdmx2jsonld/common/rdf.py
--rw-r--r--   0        0        0     1400 2022-10-27 12:12:59.737048 sdmx2json_ld-0.5.1/sdmx2jsonld/common/regparser.py
--rw-r--r--   0        0        0     2094 2022-10-27 12:12:59.738420 sdmx2json_ld-0.5.1/sdmx2jsonld/exceptions/__init__.py
--rw-r--r--   0        0        0     1864 2022-10-27 12:12:59.847165 sdmx2json_ld-0.5.1/sdmx2jsonld/grammar/grammar.lark
--rw-r--r--   0        0        0        0 2022-10-27 12:12:59.739394 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/__init__.py
--rw-r--r--   0        0        0     1113 2022-10-27 12:12:59.846100 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/attribute.py
--rw-r--r--   0        0        0     2782 2022-10-27 12:12:59.746683 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/catalogue.py
--rw-r--r--   0        0        0     6767 2022-10-27 12:12:59.844503 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/concept.py
--rw-r--r--   0        0        0     4773 2022-10-27 12:12:59.843001 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/conceptschema.py
--rw-r--r--   0        0        0     6809 2022-10-27 12:12:59.759767 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/context.py
--rw-r--r--   0        0        0     8788 2022-10-27 12:12:59.760712 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/dataset.py
--rw-r--r--   0        0        0     1093 2022-10-27 12:12:59.841826 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/dimension.py
--rw-r--r--   0        0        0     9156 2022-10-27 12:12:59.767500 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/entitytype.py
--rw-r--r--   0        0        0     4033 2022-10-27 15:19:39.327994 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/parser.py
--rw-r--r--   0        0        0     5856 2022-10-27 12:12:59.840548 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/property.py
--rw-r--r--   0        0        0     4025 2022-10-27 12:12:59.839111 sdmx2json_ld-0.5.1/sdmx2jsonld/transform/transformer.py
--rw-r--r--   0        0        0     7265 1970-01-01 00:00:00.000000 sdmx2json_ld-0.5.1/setup.py
--rw-r--r--   0        0        0     7158 1970-01-01 00:00:00.000000 sdmx2json_ld-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11353 2022-10-27 12:12:59.000000 sdmx2json_ld-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1909 2023-07-25 10:04:27.158964 sdmx2json_ld-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6018 2022-10-27 14:47:49.000000 sdmx2json_ld-1.0.0/sdmx2jsonld/README.md
+-rw-r--r--   0        0        0        0 2022-10-27 12:12:59.000000 sdmx2json_ld-1.0.0/sdmx2jsonld/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:00:49.304051 sdmx2json_ld-1.0.0/sdmx2jsonld/common/__init__.py
+-rw-r--r--   0        0        0     3893 2023-07-24 12:35:18.142352 sdmx2json_ld-1.0.0/sdmx2jsonld/common/classprecedence.py
+-rw-r--r--   0        0        0     2929 2023-07-24 12:19:25.589399 sdmx2json_ld-1.0.0/sdmx2jsonld/common/commonclass.py
+-rw-r--r--   0        0        0     1341 2023-07-24 12:19:25.553399 sdmx2json_ld-1.0.0/sdmx2jsonld/common/config.py
+-rw-r--r--   0        0        0     7446 2023-07-25 06:55:21.135608 sdmx2json_ld-1.0.0/sdmx2jsonld/common/datatypeconversion.py
+-rw-r--r--   0        0        0     4613 2023-07-25 06:55:21.079608 sdmx2json_ld-1.0.0/sdmx2jsonld/common/listmanagement.py
+-rw-r--r--   0        0        0     1183 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/common/rdf.py
+-rw-r--r--   0        0        0     1583 2023-07-24 12:19:25.561399 sdmx2json_ld-1.0.0/sdmx2jsonld/common/regparser.py
+-rw-r--r--   0        0        0     5741 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/common/tzinfos.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/cube/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-24 12:19:25.553399 sdmx2json_ld-1.0.0/sdmx2jsonld/cube/measuretype.py
+-rw-r--r--   0        0        0     1862 2023-07-25 06:55:21.011608 sdmx2json_ld-1.0.0/sdmx2jsonld/exceptions/__init__.py
+-rw-r--r--   0        0        0     3240 2023-07-24 12:19:25.569399 sdmx2json_ld-1.0.0/sdmx2jsonld/exceptions/exceptions.py
+-rw-r--r--   0        0        0     1864 2022-10-27 12:12:59.000000 sdmx2json_ld-1.0.0/sdmx2jsonld/grammar/grammar.lark
+-rw-r--r--   0        0        0        0 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/__init__.py
+-rw-r--r--   0        0        0     2638 2023-07-25 06:55:21.035608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/code.py
+-rw-r--r--   0        0        0     1532 2023-07-24 12:19:25.553399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/compilingorg.py
+-rw-r--r--   0        0        0     3117 2023-07-24 12:19:25.565399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/confirmationStatus.py
+-rw-r--r--   0        0        0     1492 2023-07-24 12:19:25.561399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/currency.py
+-rw-r--r--   0        0        0     1601 2023-07-25 06:55:20.999608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/dataComp.py
+-rw-r--r--   0        0        0     1533 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/decimals.py
+-rw-r--r--   0        0        0     1498 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/dissorg.py
+-rw-r--r--   0        0        0     3217 2023-07-24 12:19:25.597399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/observationStatus.py
+-rw-r--r--   0        0        0     1911 2023-07-25 06:55:21.019608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/sdmxattribute.py
+-rw-r--r--   0        0        0     1556 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/timeFormat.py
+-rw-r--r--   0        0        0     1850 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/timePerCollect.py
+-rw-r--r--   0        0        0     1488 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/title.py
+-rw-r--r--   0        0        0     1700 2023-07-24 12:19:25.573399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxattributes/unitmult.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-24 12:19:25.581399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/cogconceptschema.py
+-rw-r--r--   0        0        0     1594 2023-07-24 12:19:25.581399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/compilingorgconcept.py
+-rw-r--r--   0        0        0     1692 2023-07-25 06:55:21.011608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/confstatusconcept.py
+-rw-r--r--   0        0        0     1541 2023-07-24 12:19:25.585399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/currencyconcept.py
+-rw-r--r--   0        0        0     1614 2023-07-25 06:55:21.011608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/datacompconcept.py
+-rw-r--r--   0        0        0     1565 2023-07-25 06:55:21.011608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/decimals.py
+-rw-r--r--   0        0        0     1565 2023-07-25 06:55:21.015608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/dissorgconcept.py
+-rw-r--r--   0        0        0     1517 2023-07-25 06:55:21.015608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/freqconcept.py
+-rw-r--r--   0        0        0     1590 2023-07-25 06:55:21.015608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/obsstatusconcept.py
+-rw-r--r--   0        0        0     1563 2023-07-25 06:55:21.015608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/refareaconcept.py
+-rw-r--r--   0        0        0     1518 2023-07-24 12:19:25.593399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/sdmxconcept.py
+-rw-r--r--   0        0        0     1818 2023-07-24 12:19:25.589399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/timePerCollectConcept.py
+-rw-r--r--   0        0        0     1586 2023-07-25 06:55:21.023608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/timeformatconcept.py
+-rw-r--r--   0        0        0     1572 2023-07-25 06:55:21.019608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/timeperiodconcept.py
+-rw-r--r--   0        0        0     1519 2023-07-25 06:55:21.019608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/titleConcept.py
+-rw-r--r--   0        0        0     1656 2023-07-25 06:55:21.023608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxconcepts/unitmultconcept.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:00:49.308051 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/__init__.py
+-rw-r--r--   0        0        0     2309 2023-07-24 12:19:25.601399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/frequency.py
+-rw-r--r--   0        0        0     1587 2023-07-25 06:55:21.023608 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/refarea.py
+-rw-r--r--   0        0        0     2303 2023-07-24 12:19:25.609399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/sdmxdimension.py
+-rw-r--r--   0        0        0     2347 2023-07-24 12:19:25.621399 sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/timeperiod.py
+-rw-r--r--   0        0        0        0 2022-10-27 12:12:59.000000 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/__init__.py
+-rw-r--r--   0        0        0     1132 2023-07-24 12:19:25.597399 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/attribute.py
+-rw-r--r--   0        0        0     6776 2023-07-25 06:55:21.107608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/catalogue.py
+-rw-r--r--   0        0        0     6861 2023-07-25 06:55:21.119608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/concept.py
+-rw-r--r--   0        0        0     5584 2023-07-25 06:55:21.091608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/conceptschema.py
+-rw-r--r--   0        0        0     6854 2023-07-25 06:55:21.139608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/context.py
+-rw-r--r--   0        0        0    13564 2023-07-25 06:55:21.187608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/dataset.py
+-rw-r--r--   0        0        0     1129 2023-07-24 12:19:25.597399 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/dimension.py
+-rw-r--r--   0        0        0     2755 2023-07-25 06:55:21.067608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/distribution.py
+-rw-r--r--   0        0        0    10046 2023-07-25 06:55:21.155608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/entitytype.py
+-rw-r--r--   0        0        0     7274 2023-07-25 06:55:21.131608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/observation.py
+-rw-r--r--   0        0        0     5841 2023-07-24 13:50:42.942881 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/parser.py
+-rw-r--r--   0        0        0     5515 2023-07-25 06:55:21.103608 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/property.py
+-rw-r--r--   0        0        0     4654 2023-07-24 12:19:25.661399 sdmx2json_ld-1.0.0/sdmx2jsonld/transform/transformer.py
+-rw-r--r--   0        0        0     7292 1970-01-01 00:00:00.000000 sdmx2json_ld-1.0.0/PKG-INFO
```

### Comparing `sdmx2json_ld-0.5.1/LICENSE` & `sdmx2json_ld-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/README.md` & `sdmx2json_ld-1.0.0/sdmx2jsonld/README.md`

 * *Files identical despite different names*

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/common/classprecedence.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/common/classprecedence.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
 
 
 entities = {
-    'qb:DataStructureDefinition': 'Dataset',
-    'qb:ComponentSpecification': 'Component',
-    'qb:AttributeProperty': 'Attribute',
-    'qb:DimensionProperty': 'Dimension',
-    'qb:CodedProperty': 'Dimension',
-    'rdfs:Class': 'Class',
-    'owl:Class': 'Class',
-    'skos:ConceptScheme': 'ConceptScheme',
-    'skos:Concept': 'Range'
+    "qb:DataStructureDefinition": "Dataset",
+    "qb:ComponentSpecification": "Component",
+    "qb:AttributeProperty": "Attribute",
+    "qb:DimensionProperty": "Dimension",
+    "qb:CodedProperty": "Dimension",
+    "rdfs:Class": "Class",
+    "owl:Class": "Class",
+    "skos:ConceptScheme": "ConceptScheme",
+    "skos:Concept": "Range",
 }
 
 
 class Precedence:
     def __init__(self):
         self.classes = {
             "qb:DataStructureDefinition": 1000,
@@ -43,78 +43,79 @@
             "qb:AttributeProperty": 250,
             "qb:MeasureProperty": 250,
             "qb:CodedProperty": 125,
             "skos:ConceptScheme": 75,
             "skos:Concept": 40,
             "rdfs:Class": 20,
             "owl:Class": 20,
-            "qb:SliceKey": 10
+            "qb:SliceKey": 10,
         }
 
     def get_value(self, aclass: str) -> int:
         try:
             return self.classes[aclass]
         except KeyError:
             return 0
 
     def precedence(self, data: list) -> str:
         classes_values = list(map(lambda x: self.get_value(x), data))
 
         # We need to check if all element of the list are the value 250 because could not be possible to have at
-        # the same time a DimensionProperty and AttributeProperty, this is an ERROR and we need to report.
+        # the same time a DimensionProperty and AttributeProperty, this is an ERROR therefore we need to report it.
         result = all(element == 250 for element in classes_values) and len(data) > 1
         if result is True:
-            raise ClassesPrecedencePropertyError(data)
+            raise ClassPrecedencePropertyError(data)
 
         # In case that we have several values identical of type Class, we need to report a WARNING message because maybe
-        # it is not needed multitype in that case.
+        # it is not needed multi-type in that case.
         result = all(element == 20 for element in classes_values) and len(data) > 1
         if result is True:
-            raise ClassesPrecedenceClassError(data)
+            raise ClassPrecedenceClassError(data)
 
-        # In other chase, we return the max value of the list
-        aux = max(classes_values)
-        aux = data[classes_values.index(aux)]
+        # In other case, we return the max value of the list
+        aux = data[classes_values.index(max(classes_values))]
 
         return aux
 
 
-class ClassesPrecedenceError(Exception):
+class ClassPrecedenceError(Exception):
     """Base class for other exceptions"""
 
     def __init__(self, data, message):
         self.message = message
         self.data = data
 
     def __str__(self):
-        return f'{self.data} -> {self.message}'
+        return f"{self.data} -> {self.message}"
 
 
-class ClassesPrecedencePropertyError(ClassesPrecedenceError):
+class ClassPrecedencePropertyError(ClassPrecedenceError):
     """Raised when the input value is too small"""
-    """Exception raised for errors in the input salary.
+
+    """Exception raised for errors in the input data.
 
     Attributes:
-        salary -- input salary which caused the error
+        data -- input data which caused the error
         message -- explanation of the error
     """
 
     def __init__(self, data, message="Incompatible multiclass definition"):
         super().__init__(data=data, message=message)
 
 
-class ClassesPrecedenceClassError(ClassesPrecedenceError):
+class ClassPrecedenceClassError(ClassPrecedenceError):
     """Raised when the input value is too large"""
-    """Exception raised for errors in the input salary.
+
+    """Exception raised for errors in the input data.
 
     Attributes:
-        salary -- input salary which caused the error
+        data -- input data which caused the error
         message -- explanation of the error
     """
 
     def __init__(self, data, message="Possible redundant Class definition"):
         super().__init__(data=data, message=message)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pre = Precedence()
-    obtained = pre.precedence(['qb:DataStructureDefinition'])
+    obtained = pre.precedence(["qb:DataStructureDefinition"])
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/common/commonclass.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/common/commonclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,57 +29,69 @@
     def __init__(self, entity):
         self.data = dict()
         self.keys = dict()
         self.entity = entity
 
     def add_context(self, context, context_mapping):
         # Set the context as it is received and mixed with the core context
-        self.data['@context'] = context['@context']
+        self.data["@context"] = context["@context"]
 
         # Fix the prefix of the core properties of the Dataset entity
         new_data = dict()
 
         for k, v in self.data.items():
             # Return if the string matched the ReGex
-            out = k.split(':')
+            out = k.split(":")
 
             if len(out) == 2 and out[0] in context_mapping.keys():
                 new_prefix = context_mapping[out[0]]
-                new_key = new_prefix + ':' + out[1]
+                new_key = new_prefix + ":" + out[1]
 
                 new_data[new_key] = self.data[k]
                 self.keys[k] = new_key
             else:
                 new_data[k] = v
 
         self.data = new_data
 
+    def get(self):
+        return self.data
+
     def save(self):
         data = self.get()
 
-        aux = data['id'].split(":")
+        aux = data["id"].split(":")
         length_aux = len(aux)
 
         # We need to check that the output folder exist
-        if exists('./output') is False:
-            # We need to create the folder because it does not exits
-            mkdir('./output')
+        if exists("./output") is False:
+            # We need to create the folder because it does not exist
+            mkdir("./output")
 
-        filename = './output/' + '_'.join(aux[length_aux - 2:]) + '.jsonld'
+        filename = "./output/" + "_".join(aux[length_aux - 2 :]) + ".jsonld"
 
         # Serializing json
         json_object = dumps(data, indent=4, ensure_ascii=False)
 
         # Writing to sample.json
         with open(filename, "w") as outfile:
             outfile.write(json_object)
 
-    def generate_id(self, value, entity=None):
+    def generate_id(self, value, entity=None, update_id=False):
         parse = RegParser()
         aux = parse.obtain_id(value)
 
         if entity is None:
-            aux = "urn:ngsi-ld:" + self.entity + ":" + aux
+            new_aux = "urn:ngsi-ld:" + self.entity + ":" + aux
+        else:
+            new_aux = "urn:ngsi-ld:" + entity + ":" + aux
+
+        if update_id:
+            self.data["id"] = new_aux
+            return new_aux
         else:
-            aux = "urn:ngsi-ld:" + entity + ":" + aux
+            return aux, new_aux
+
+    def __generate_property__(self, key, value):
+        result = {key: {"type": "Property", "value": value}}
 
-        return aux
+        return result
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/common/datatypeconversion.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/common/datatypeconversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,123 +15,163 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
-from hidateinfer import infer
+from hidateinfer import infer  # type: ignore[import]
 from datetime import datetime, timezone
 from re import compile, sub
+from dateutil import parser
+import pytz
+from sdmx2jsonld.common.tzinfos import whois_timezone_info
 
 
 class DataTypeConversion:
     def __init__(self):
         self.types = {
-            'xsd:dateTime': 'stodt',
-            'xsd:int': 'stoi',
-            'xsd:boolean': 'stob'
+            "xsd:dateTime": "stoutc",
+            "xsd:int": "stoi",
+            "xsd:boolean": "stob",
+            "xsd:float": "stof",
         }
+
         self.regex_12hour = compile(r"(^.*T%)(I)(.*)$")
         self.regex_microseconds = compile(r"^(.*T%.*:%S\.)(%H)*$")
         self.regex_microseconds2 = compile(r"^(.*T%.*:%S\.)(%y)*$")
         self.regex_false_date = compile(r"^%Y-%d-%y(.*)%m")
         self.regex_false_date2 = compile(r"^%Y-%d-%m(.*)%f")
 
     def correct_datatype_format(self, format_dt: str, hour24: bool = True):
-
         if hour24:
             format_dt = sub(self.regex_12hour, r"\1H\3", format_dt)
 
-        format_dt = sub(self.regex_microseconds,  r"\1%f", format_dt)
+        format_dt = sub(self.regex_microseconds, r"\1%f", format_dt)
         format_dt = sub(self.regex_microseconds2, r"\1%f", format_dt)
 
-        format_dt = sub(self.regex_false_date,  r"%Y-%m-%d\1%f", format_dt)
+        format_dt = sub(self.regex_false_date, r"%Y-%m-%d\1%f", format_dt)
         format_dt = sub(self.regex_false_date2, r"%Y-%m-%d\1%f", format_dt)
 
         return format_dt
 
     def convert(self, data, datatype):
+        def stoutc(value):
+            """
+            Converts a date in string format to UTC date using
+            """
+            dt = parser.parse(value, tzinfos=whois_timezone_info)
+            dt = dt.astimezone(pytz.UTC)
+            return dt.replace(tzinfo=timezone.utc).isoformat()
+
         def stodt(value):
-            # print(f'toDateTime function, arguments {value}')
             if isinstance(value, str):
                 result = infer([value])
             elif isinstance(value, list):
                 result = infer(value)
             else:
-                raise Exception(f'Invalid format received: {type(value)}')
+                raise Exception(f"Invalid format received: {type(value)}")
 
             result = self.correct_datatype_format(result)
-
-            # print(f'format {result}')
             result = datetime.strptime(value, result).replace(tzinfo=timezone.utc).isoformat()
-            # print(f'result {result}')
+
             return result
 
         def stoi(value):
             """
-               Converts 'something' to int. Raises exception for invalid formats
+            Converts 'something' to int. Raises exception for invalid formats
             """
             if isinstance(value, str):
-                result = value.replace('"', '')
+                result = value.replace('"', "")
             elif isinstance(value, int):
                 result = value
             else:
-                raise Exception(f'Invalid format received: {type(value)}')
+                raise Exception(f"Invalid format received: {type(value)}")
 
             return int(result)
 
-        def stob(value):
+        def stof(value):
             """
-               Converts 'something' to boolean. Raises exception for invalid formats
-                   Possible True  values: 1, True, "1", "TRue", "yes", "y", "t"
-                   Possible False values: 0, False, None, [], {}, "", "0", "faLse", "no", "n", "f", 0.0, ...
+            Converts 'something' to float. Raises exception for invalid formats
             """
-            print(f'toBool function, arguments {value}')
+            if isinstance(value, str):
+                result = value.replace('"', "")
+            elif isinstance(value, float):
+                result = value
+            else:
+                raise Exception(f"Invalid format received: {type(value)}")
+
+            return float(result)
 
+        def stob(value):
+            """
+            Converts 'something' to boolean. Raises exception for invalid formats
+                Possible True  values: 1, True, "1", "TRue", "yes", "y", "t"
+                Possible False values: 0, False, None, [], {}, "", "0", "faLse", "no", "n", "f", 0.0, ...
+            """
             if str(value).lower() in ("yes", "y", "true", "t", "1"):
                 return True
 
-            if str(value).lower() in ("no", "n", "false", "f", "0", "0.0", "", "none", "[]", "{}"):
+            if str(value).lower() in (
+                "no",
+                "n",
+                "false",
+                "f",
+                "0",
+                "0.0",
+                "",
+                "none",
+                "[]",
+                "{}",
+            ):
                 return False
 
             # logger.error(f'Invalid value for boolean conversion: {str(value)}')
-            raise Exception(f'Invalid value for boolean conversion: {str(value)}')
+            raise Exception(f"Invalid value for boolean conversion: {str(value)}")
 
         try:
-            function = self.types[datatype] + '(value=' + data + ')'
+            # jicg - function = self.types[datatype] + f'(value="{data}")'
+            function = self.types[datatype] + "(value=" + data + ")"
             return eval(function)
         except KeyError:
             # logger.error(f'Datatype not defined: {datatype}')
-            print(f'Datatype not defined: {datatype}')
-            raise Exception(f'Datatype not defined: {datatype}')
+            print(f"Datatype not defined: {datatype}")
+            raise Exception(f"Datatype not defined: {datatype}")
         except NameError:
             # logger.error(f"name '{data}' is not defined")
             print(f"name '{data}' is not defined")
             raise Exception(f"name '{data}' is not defined")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from lark import Token
 
-    data1 = ['"2022-01-15T08:00:00.000"', Token('FORMATCONNECTOR', '^^'), 'xsd:dateTime']
-    data2 = ['"2"', Token('FORMATCONNECTOR', '^^'), 'xsd:int']
-    data22 = ['2', Token('FORMATCONNECTOR', '^^'), 'xsd:int']
-    data23 = ['asdfs', Token('FORMATCONNECTOR', '^^'), 'xsd:int']
-    data3 = ['"true"', Token('FORMATCONNECTOR', '^^'), 'xsd:boolean']
-    data4 = ['"fake"', Token('FORMATCONNECTOR', '^^'), 'otraCosa']
-    data5 = ['"2022-01-10T09:00:00.000"', Token('FORMATCONNECTOR', '^^'), 'xsd:dateTime']
-    data6 = ['"2021-07-01T11:50:37.3"', Token('FORMATCONNECTOR', '^^'), 'xsd:dateTime']
-    data7 = ['"2021-09-28T15:31:24.05"', Token('FORMATCONNECTOR', '^^'), 'xsd:dateTime']
+    data1 = [
+        '"2022-01-15T08:00:00.000"',
+        Token("FORMATCONNECTOR", "^^"),
+        "xsd:dateTime",
+    ]
+    data2 = ['"2"', Token("FORMATCONNECTOR", "^^"), "xsd:int"]
+    data22 = ["2", Token("FORMATCONNECTOR", "^^"), "xsd:int"]
+    data23 = ["asdfs", Token("FORMATCONNECTOR", "^^"), "xsd:int"]
+    data3 = ['"true"', Token("FORMATCONNECTOR", "^^"), "xsd:boolean"]
+    data4 = ['"fake"', Token("FORMATCONNECTOR", "^^"), "otraCosa"]
+    data5 = [
+        '"2022-01-10T09:00:00.000"',
+        Token("FORMATCONNECTOR", "^^"),
+        "xsd:dateTime",
+    ]
+    data6 = ['"2021-07-01T11:50:37.3"', Token("FORMATCONNECTOR", "^^"), "xsd:dateTime"]
+    data7 = ['"2021-09-28T15:31:24.05"', Token("FORMATCONNECTOR", "^^"), "xsd:dateTime"]
 
-    print(infer(['Mon Jan 13 09:52:52 MST 2014']))
+    print(infer(["Mon Jan 13 09:52:52 MST 2014"]))
     print(infer([data1[0]]))
     print()
 
-    print(infer(['2022-01-15T08:00:00']))
+    print(infer(["2022-01-15T08:00:00"]))
     print(infer([data1[0]]))
     print()
 
     # Resolve problem in the library
     # if we are working with 24h, infer should return %Y-%m-%dT%H:%M:%S.%f but return %Y-%m-%dT%I:%M:%S.%f
     # if we have seconds with milliseconds, infer should return %Y-%m-%dT%I:%M:%S.%f but return %Y-%m-%dT%I:%M:%S.%H
     # There is some problem with the library and the date is not inferred properly, specially in the case
@@ -145,16 +185,19 @@
     # print(dataConversionType.convert(data23[0], data23[2]) + 10)
 
     print(dataConversionType.convert(data3[0], data3[2]))
 
     try:
         print(dataConversionType.convert(data4[0], data4[2]))
     except Exception:
-        print('Exception')
+        print("Exception")
 
     # Convert datetime generated into UTC format: 2021-12-21T16:18:55Z or 2021-12-21T16:18:55+00:00, ISO8601
 
     print(dataConversionType.convert(data5[0], data5[2]))
 
     print(dataConversionType.convert(data6[0], data6[2]))
 
     print(dataConversionType.convert(data7[0], data7[2]))
+
+    data101 = ['"3016.9"', Token("FORMATCONNECTOR", "^^"), "xsd:float"]
+    print(dataConversionType.convert(data101[0], data101[2]))
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/common/rdf.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/common/rdf.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
 from rdflib import Graph
 
 
 def turtle_terse(rdf_content):
+    """
+    Function which receives a string in formatted with RDF, dialect turtle, parses it and returns the  same data
+    parsed in another string. The incoming data in the parameter is equivalent to the returned data.
+    """
     # Create a Graph
     g2 = Graph()
 
     g2 = g2.parse(data=rdf_content, format="turtle")
 
     new_rdf_content = g2.serialize(format="turtle")
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/common/regparser.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/common/regparser.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,28 +21,32 @@
 ##
 
 import re
 
 
 class RegParser:
     def __init__(self):
-        regex = "http[s]?:\/\/(.*)"
+        regex = "http[s]?:\/\/(.+)"
 
         # Compile the Regex
         self.re = re.compile(regex)
 
-    def obtain_id(self, string_to_parse):
+    def obtain_id(self, string_to_parse, prefix_string=""):
         # Return if the string matched the ReGex
         out = self.re.match(string_to_parse)
 
         if out is None:
             # Check if the prefixed name include ':'
-            obtained_id = string_to_parse.split(':')[1]
+            try:
+                obtained_id = string_to_parse.split(":")[1]
+            except IndexError:
+                # We have a normal prefix or data
+                obtained_id = string_to_parse
         else:
             # We have a URIREF
             out = out.group(1)
             out = out.split("/")
 
             # we get the last value which corresponds to the id
-            obtained_id = out[(len(out) - 1):][0]
+            obtained_id = prefix_string + out[(len(out) - 1) :][0]
 
         return obtained_id
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/exceptions/__init__.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/exceptions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,35 @@
 from lark.exceptions import UnexpectedEOF as LarkUnexpectedEOF
 from lark.exceptions import UnexpectedInput as LarkUnexpectedInput
 from lark.exceptions import UnexpectedToken as LarkUnexpectedToken
 
 
 class UnexpectedEOF(LarkUnexpectedEOF):
     def __init__(self, expected, state=None, terminals_by_name=None):
-        super(LarkUnexpectedEOF, self).__init__(expected=expected, 
-                                                state=state, 
-                                                terminals_by_name=terminals_by_name)
+        super(LarkUnexpectedEOF, self).__init__(expected=expected, state=state, terminals_by_name=terminals_by_name)
 
 
 class UnexpectedInput(LarkUnexpectedInput):
     def __init__(self):
         super(LarkUnexpectedInput, self).__init__()
 
 
 class UnexpectedToken(LarkUnexpectedToken):
-    def __init__(self, token, expected, considered_rules=None, state=None, interactive_parser=None, terminals_by_name=None, token_history=None):
-        super(LarkUnexpectedToken, self).__init__(token=token,
-                                                  expected=expected,
-                                                  considered_rules=considered_rules,
-                                                  state=state,
-                                                  interactive_parser=interactive_parser,
-                                                  terminals_by_name=terminals_by_name,
-                                                  token_history=token_history)
+    def __init__(
+        self,
+        token,
+        expected,
+        considered_rules=None,
+        state=None,
+        interactive_parser=None,
+        terminals_by_name=None,
+        token_history=None,
+    ):
+        super(LarkUnexpectedToken, self).__init__(
+            token=token,
+            expected=expected,
+            considered_rules=considered_rules,
+            state=state,
+            interactive_parser=interactive_parser,
+            terminals_by_name=terminals_by_name,
+            token_history=token_history,
+        )
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/grammar/grammar.lark` & `sdmx2json_ld-1.0.0/sdmx2jsonld/grammar/grammar.lark`

 * *Files identical despite different names*

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/attribute.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ##
 
 from sdmx2jsonld.transform.property import Property
 
 
 class Attribute(Property):
     def __init__(self):
-        super().__init__(entity='AttributeProperty')
-        self.data['type'] = 'AttributeProperty'
+        super().__init__(entity="AttributeProperty")
+        self.data["type"] = "AttributeProperty"
 
     def add_data(self, attribute_id, data):
-        super().add_data(id=id, data=data)
+        super().add_data(property_id=attribute_id, data=data)
 
         # Add the id
-        self.data['id'] = "urn:ngsi-ld:AttributeProperty:" + attribute_id
+        self.data["id"] = "urn:ngsi-ld:AttributeProperty:" + attribute_id
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/catalogue.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/sdmxdimensions/sdmxdimension.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,84 +15,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
-
-from logging import getLogger
 from sdmx2jsonld.common.commonclass import CommonClass
-import random
-
-logger = getLogger()
-
 
-class CatalogueDCATAP(CommonClass):
-    def __init__(self):
-        super().__init__(entity='CatalogueDCAT-AP')
 
+class SDMXDimension(CommonClass):
+    def __init__(
+        self,
+        entity_id,
+        identifier,
+        entity_range,
+        label=None,
+        description=None,
+        concept_id=None,
+    ):
+        super().__init__(entity="DimensionProperty")
         self.data = {
-            "id": str(),
-            "type": "CatalogueDCAT-AP",
-            "dataset": {
-                "type": "object",
-                "value": str()
-            },
-
-            "language": {
+            "id": f"urn:ngsi-ld:DimensionProperty:{entity_id}",
+            "type": "DimensionProperty",
+            "language": {"type": "Property", "value": ["en"]},
+            "label": {
                 "type": "Property",
-                "value": list()
+                "value": {
+                    "en": label,
+                },
             },
-
-
-            #################################################
-            # TODO: New ETSI CIM NGSI-LD specification 1.4.2
-            # Pending to implement in the Context Broker
-            #################################################
-            # "rdfs:label": {
-            #     "type": "LanguageProperty",
-            #     "LanguageMap": dict()
-            # },
-            #################################################
             "description": {
                 "type": "Property",
-                "value": dict()
+                "value": {
+                    "en": description,
+                },
             },
-
-            "publisher": {
-                "type": "Property",
-                "value": str()
+            "concept": {
+                "type": "Relationship",
+                "object": f"urn:ngsi-ld:Concept:{concept_id}",
             },
-
-            "title": {
-                "type": "Array",
-                "value": list()
-            },
-
-
+            "identifier": {"type": "Property", "value": identifier},
+            "range": {"type": "Property", "value": entity_range},
             "@context": [
-                "https://raw.githubusercontent.com/SEMICeu/DCAT-AP/master/releases/1.1/dcat-ap_1.1.jsonld",
-                "https://raw.githubusercontent.com/smart-data-models/dataModel.DCAT-AP/master/context.jsonld"
-            ]
+                "https://raw.githubusercontent.com/smart-data-models/dataModel.STAT-DCAT-AP/master/context.jsonld"
+            ],
         }
 
-        self.concept_id = str()
-
-    def add_dataset(self, dataset_id):
-        self.concept_id = dataset_id
-
-        # generate hash id
-        random_bits = random.getrandbits(128)
-        hash1 = "%032x" % random_bits
-
-        # Add the id
-        self.data['id'] = "urn:ngsi-ld:CatalogueDCAT-AP:" + hash1
-
-        # Add dataset id
-        self.data['dataset']['value'] = dataset_id
+        # We need to check if some of the parameters are None, in that case we have to pop the key from data
+        if label is None:
+            self.data.pop("label")
 
-    def get(self):
-        return self.data
+        if description is None:
+            self.data.pop("description")
 
-    def get_id(self):
-        return self.data['id']
+        if concept_id is None:
+            self.data.pop("concept")
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/concept.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/concept.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,159 +26,152 @@
 from sdmx2jsonld.transform.context import Context
 
 logger = getLogger()
 
 
 class Concept(CommonClass):
     def __init__(self):
-        super().__init__(entity='Concept')
+        super().__init__(entity="Concept")
 
         self.data = {
             "id": str(),
             "type": "Concept",
-            "dct:language": {
-                "type": "Property",
-                "value": list()
-            },
-            "skos:inScheme": {
-                "type": "Relationship",
-                "value": str()
-            },
-            "rdfs:subClassOf": {
-                "type": "Property",
-                "value": str()
-            },
-
+            "language": {"type": "Property", "value": list()},
+            "inScheme": {"type": "Relationship", "object": str()},
+            "rdfs:subClassOf": {"type": "Property", "value": str()},
             #################################################
             # TODO: New ETSI CIM NGSI-LD specification 1.4.2
             # Pending to implement in the Context Broker
             #################################################
             # "skos:prefLabel": {
             #     "type": "LanguageProperty",
             #     "LanguageMap": dict()
             # },
             #################################################
-            "skos:prefLabel": {
-                "type": "Property",
-                "value": dict()
-            },
-
-
-            "@context": dict()
+            "prefLabel": {"type": "Property", "value": dict()},
+            "@context": [
+                "https://raw.githubusercontent.com/smart-data-models/dataModel.STAT-DCAT-AP/master/context.jsonld"
+            ],
         }
 
         self.concept_id = str()
+        self.keys = {k: k for k in self.data.keys()}
 
     def add_data(self, concept_id, data):
         # TODO: We have to control that data include the indexes that we want to search
         # We need to complete the data corresponding to the ConceptSchema: skos:prefLabel
         # TODO: we need to extract the attribute from the context or we will have problems (e.g. skos:prefLabel should
         #       be equal to rdfs:label
         self.concept_id = concept_id
 
         try:
-            position = data.index('skos:prefLabel') + 1
+            position = data.index("skos:prefLabel") + 1
         except ValueError:
             # We could not find skos:prefLabel, try to find rdfs:label
-            position = data.index('rdfs:label') + 1
-            logger.warning(f'The Concept {concept_id} does not contain skos:prefLabel but rdfs:label. We use its '
-                           f'content to fill in the skos:prefLabel property')
+            position = data.index("rdfs:label") + 1
+            logger.warning(
+                f"The Concept {concept_id} does not contain skos:prefLabel but rdfs:label. We use its "
+                f"content to fill in the skos:prefLabel property"
+            )
 
         description = data[position]
-        descriptions = [x[0].replace("\"", "") for x in description]
+        descriptions = [x[0].replace('"', "") for x in description]
 
         languages = list()
         try:
             languages = [x[1].replace("@", "").lower() for x in description]
         except IndexError:
-            logger.warning(f'The Concept {concept_id} has a '
-                           f'skos:prefLabel without language tag: {description}')
+            logger.warning(f"The Concept {concept_id} has a " f"skos:prefLabel without language tag: {description}")
 
             aux = len(description)
             if aux != 1:
                 logger.error(f"Concept: there is more than 1 description ({aux}), values: {description}")
             else:
                 # There is no language tag, we use by default 'en'
-                languages = ['en']
+                languages = ["en"]
                 logger.warning('Concept: selecting default language "en"')
 
         # Complete the skos:prefLabel
         ###############################################################################
         # TODO: New ETSI CIM NGSI-LD specification 1.4.2
         # Pending to implement in the Context Broker
         ###############################################################################
         # for i in range(0, len(languages)):
         #     self.data['skos:prefLabel']['LanguageMap'][languages[i]] = descriptions[i]
         ###############################################################################
         for i in range(0, len(languages)):
-            self.data['skos:prefLabel']['value'][languages[i]] = descriptions[i]
+            self.data["prefLabel"]["value"][languages[i]] = descriptions[i]
 
         # Complete the information of the language with the previous information
-        key = self.keys['dct:language']
-        self.data[key]['value'] = languages
+        key = self.keys["language"]
+        self.data[key]["value"] = languages
 
         # Add the id
-        self.data['id'] = "urn:ngsi-ld:Concept:" + concept_id
+        self.data["id"] = "urn:ngsi-ld:Concept:" + concept_id
 
         # rdfs:seeAlso
         self.need_add_in_scheme(data=data)
 
         # rdfs:subClassOf
         self.need_add_subclass(data=data)
 
         # skos:notation
         self.need_add_notation(data=data)
 
-        # Simplify Context and order keys
+        # Order the keys in the final json-ld
         a = Context()
-        a.set_data(data=self.data)
-        a.new_analysis()
+        a.set_data(new_data=self.data)
         a.order_context()
         self.data = a.get_data()
 
     def get(self):
         return self.data
 
     def get_id(self):
-        return self.data['id']
+        return self.data["id"]
 
     def need_add_subclass(self, data):
         try:
-            position = data.index('rdfs:subClassOf') + 1
-            self.data['rdfs:subClassOf']['value'] = data[position][0]
+            position = data.index("rdfs:subClassOf") + 1
+            self.data["rdfs:subClassOf"]["value"] = data[position][0]
         except ValueError:
-            logger.info(f'The Concept {self.concept_id} has no rdfs:subClassOf property, deleting the key in the data')
+            logger.info(f"The Concept {self.concept_id} has no rdfs:subClassOf property, deleting the key in the data")
 
             # We delete the "rdfs:subClassOf" property from the final structure
-            self.data.pop('rdfs:subClassOf')
+            self.data.pop("rdfs:subClassOf")
 
     def need_add_in_scheme(self, data):
         position = 0
 
         try:
-            position = data.index('rdfs:seeAlso') + 1
+            position = data.index("rdfs:seeAlso") + 1
         except ValueError:
             # We will try to find the skos:inScheme
             try:
-                position = data.index('skos:inScheme') + 1
+                position = data.index("skos:inScheme") + 1
             except ValueError:
-                logger.info(f'The Concept {self.concept_id} has neither rdfs:seeAlso or skos:inScheme properties, '
-                            f'deleting the key in the data')
+                logger.info(
+                    f"The Concept {self.concept_id} has neither rdfs:seeAlso or skos:inScheme properties, "
+                    f"deleting the key in the data"
+                )
 
                 # We delete the "skos:inScheme" property from the final structure
-                self.data.pop('skos:inScheme')
+                self.data.pop("skos:inScheme")
 
         parser = RegParser()
         concept_schema = data[position][0]
         concept_schema = "urn:ngsi-ld:ConceptSchema:" + parser.obtain_id(concept_schema)
-        self.data['skos:inScheme']['value'] = concept_schema
+        if self.data["inScheme"]["type"] == "Relationship":
+            self.data["inScheme"]["object"] = concept_schema
+        else:
+            self.data["inScheme"]["value"] = concept_schema
 
     def need_add_notation(self, data):
         try:
-            position = data.index('skos:notation') + 1
+            position = data.index("skos:notation") + 1
 
-            self.data['skos:notation'] = {
-                    'type': 'Property',
-                    'value': data[position][0][0].replace("\"", "")
+            self.data["notation"] = {
+                "type": "Property",
+                "value": data[position][0][0].replace('"', ""),
             }
         except ValueError:
-            logger.info(f'The Concept {self.concept_id} has no skos:notation property')
+            logger.info(f"The Concept {self.concept_id} has no skos:notation property")
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/conceptschema.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/conceptschema.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,104 +19,115 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
 
 from logging import getLogger
 from sdmx2jsonld.common.commonclass import CommonClass
 from sdmx2jsonld.transform.context import Context
+from sdmx2jsonld.common.listmanagement import flatten_value
 
 logger = getLogger()
 
 
 class ConceptSchema(CommonClass):
     def __init__(self):
-        super().__init__(entity='ConceptScheme')
+        super().__init__(entity="ConceptScheme")
 
         self.data = {
             "id": str(),
             "type": "ConceptScheme",
-            "dct:language": {
-                "type": "Property",
-                "value": list()
-            },
-            "skos:hasTopConcept": {
-                "type": "Property",
-                "value": list()
-            },
-
-
+            "language": {"type": "Property", "value": list()},
+            "hasTopConcept": {"type": "Relationship", "object": list()},
             #################################################
             # TODO: New ETSI CIM NGSI-LD specification 1.4.2
             # Pending to implement in the Context Broker
             #################################################
             # "skos:prefLabel": {
             #     "type": "LanguageProperty",
             #     "LanguageMap": dict()
             # },
             #################################################
-            "skos:prefLabel": {
-                "type": "Property",
-                "value": dict()
-            },
-
-
-            "@context": dict()
+            "prefLabel": {"type": "Property", "value": dict()},
+            "@context": [
+                "https://raw.githubusercontent.com/smart-data-models/dataModel.STAT-DCAT-AP/master/context.jsonld"
+            ],
         }
 
+        self.keys = {k: k for k in self.data.keys()}
+
     def add_data(self, concept_schema_id, data):
         # TODO: We have to control that data include the indexes that we want to search
         # We need to complete the data corresponding to the ConceptSchema: skos:prefLabel
-        position = data.index('skos:prefLabel') + 1
+        position = data.index("skos:prefLabel") + 1
         description = data[position]
 
-        descriptions = [x[0].replace("\"", "") for x in description]
+        descriptions = [x[0].replace('"', "") for x in description]
         languages = list()
 
         try:
             languages = [x[1].replace("@", "").lower() for x in description]
         except IndexError:
-            logger.warning(f'The ConceptSchema {concept_schema_id} has a '
-                           f'skos:prefLabel without language tag: {description}')
+            logger.warning(
+                f"The ConceptSchema {concept_schema_id} has a " f"skos:prefLabel without language tag: {description}"
+            )
 
             aux = len(description)
             if aux != 1:
                 logger.error(f"ConceptSchema: there is more than 1 description ({aux}), values: {description}")
             else:
                 # There is no language tag, we use by default 'en'
-                languages = ['en']
+                languages = ["en"]
                 logger.warning('ConceptSchema: selecting default language "en"')
 
         # Complete the skos:prefLabel
         ###############################################################################
         # TODO: New ETSI CIM NGSI-LD specification 1.4.2
         # Pending to implement in the Context Broker
         ###############################################################################
         # for i in range(0, len(languages)):
         #     self.data['skos:prefLabel']['LanguageMap'][languages[i]] = descriptions[i]
         ###############################################################################
         for i in range(0, len(languages)):
-            self.data['skos:prefLabel']['value'][languages[i]] = descriptions[i]
+            self.data["prefLabel"]["value"][languages[i]] = descriptions[i]
 
         # Complete the information of the language with the previous information
-        key = self.keys['dct:language']
-        self.data[key]['value'] = languages
+        key = self.keys["language"]
+        self.data[key]["value"] = languages
 
         # Add the id
-        self.data['id'] = "urn:ngsi-ld:ConceptSchema:" + concept_schema_id
+        self.data["id"] = "urn:ngsi-ld:ConceptSchema:" + concept_schema_id
 
         # TODO: We need to control that the concept id extracted here are the same that we analyse afterwards.
         # skos:hasTopConcept, this is a list of ids
-        position = data.index('skos:hasTopConcept') + 1
-        result = list(map(lambda x: self.generate_id(value=x, entity='Concept'), data[position]))
-        self.data['skos:hasTopConcept']['value'] = result
+        position = data.index("skos:hasTopConcept") + 1
+        result = list(map(lambda x: self.generate_id(value=x, entity="Concept"), data[position]))
+        self.data["hasTopConcept"]["object"] = result
+
+        # Get the rest of data, dct:created and dct:modified properties
+        try:
+            position = data.index("dct:created") + 1
+            self.data["created"] = {
+                "type": "Property",
+                "value": flatten_value(data[position]),
+            }
+        except ValueError:
+            logger.warning(f"dct:created is not present in the Concept Schema: {concept_schema_id}")
+
+        try:
+            position = data.index("dct:modified") + 1
+            self.data["modified"] = {
+                "type": "Property",
+                "value": flatten_value(data[position]),
+            }
+        except ValueError:
+            logger.warning(f"dct:modified is not present in the Concept Schema: {concept_schema_id}")
 
-        # Simplify Context and order keys
+        # Order the keys in the final json-ld
         a = Context()
-        a.set_data(data=self.data)
-        a.new_analysis()
+        a.set_data(new_data=self.data)
         a.order_context()
         self.data = a.get_data()
 
     def get(self):
         return self.data
 
     # TODO: It should be a function of the RegParser class
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/dataset.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/catalogue.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,203 +18,153 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
 
 from logging import getLogger
 from sdmx2jsonld.common.commonclass import CommonClass
-from sdmx2jsonld.common.listmanagement import get_rest_data
+from sdmx2jsonld.common.listmanagement import get_rest_data, get_property_value
 from sdmx2jsonld.transform.context import Context
+from random import getrandbits
 
 logger = getLogger()
 
 
-class Dataset(CommonClass):
+class Catalogue(CommonClass):
     def __init__(self):
-        super().__init__(entity='Dataset')
+        super().__init__(entity="Catalogue")
 
         self.data = {
             "id": str(),
-            "type": "Dataset",
-            "dct:title": str(),
-            "dct:identifier": str(),
-            "dct:language": {
-                "type": "Property",
-                "value": list()
-            },
-
-
+            "type": "Catalogue",
+            "dataset": {"type": "Relationship", "object": str()},
+            "language": {"type": "Property", "value": list()},
             #################################################
             # TODO: New ETSI CIM NGSI-LD specification 1.4.2
             # Pending to implement in the Context Broker
             #################################################
             # "rdfs:label": {
             #     "type": "LanguageProperty",
             #     "LanguageMap": dict()
             # },
             #################################################
-            "dct:description": {
-                "type": "Property",
-                "value": dict()
-            },
-
-
-            "@context": dict()
+            "description": {"type": "Property", "value": dict()},
+            "publisher": {"type": "Property", "value": str()},
+            "title": {"type": "Property", "value": list()},
+            "@context": [
+                "https://raw.githubusercontent.com/smart-data-models/dataModel.STAT-DCAT-AP/master/context.jsonld"
+            ],
         }
 
-        self.components = {
-            'qb:attribute': {
-                'entity': 'AttributeProperty',
-                'key': 'stat:attribute',
-                'value': {
-                    "stat:attribute": {
-                        "type": "Property",
-                        "value": list()
-                    }
-                }
-            },
-            'qb:dimension': {
-                'entity': 'DimensionProperty',
-                'key': 'stat:dimension',
-                'value': {
-                    "stat:dimension": {
-                        "type": "Property",
-                        "value": list()
-                    }
-                }
-            },
-            'qb:measure': {
-                'entity': 'Measure',
-                'key': 'stat:statUnitMeasure',
-                'value': {
-                    "stat:statUnitMeasure": {
-                        "type": "Property",
-                        "value": list()
-                    }
-                }
-            }
-        }
+        self.concept_id = str()
+        self.keys = {k: k for k in self.data.keys()}
 
-        self.keys = {k: k for k in self.data.keys()} | \
-                    {self.components['qb:attribute']['key']: self.components['qb:attribute']['key']} | \
-                    {self.components['qb:dimension']['key']: self.components['qb:dimension']['key']} | \
-                    {self.components['qb:measure']['key']: self.components['qb:measure']['key']}
-
-    def add_components(self, context, component):
-        # We need to know which kind of component we have, it should be the verb:
-        # qb:attribute, qb:dimension, or qb:measure
-        list_components = ['qb:attribute', 'qb:dimension', 'qb:measure']
-        type_component = [x for x in list_components if x in component][0]
-        position = component.index(type_component) + 1
+    def add_dataset(self, dataset_id):
+        self.concept_id = dataset_id
 
-        try:
-            entity = self.components[type_component]['entity']
-            new_id = self.generate_id(entity=entity, value=component[position][0])
-            key = self.components[type_component]['key']
-
-            # It is possible that the original file contains already the description
-            if new_id in self.components[type_component]['value'][key]['value']:
-                logger.warning(
-                    f"The component {new_id} is duplicated and already defined in the {self.data['id']}")
-            else:
-                self.components[type_component]['value'][key]['value'].append(new_id)
-                self.data = self.data | self.components[type_component]['value']
-        except ValueError:
-            logger.error(f"Error, it was identified a qb:ComponentSpecification with a wrong type: {type_component}")
-
-        # Simplify Context amd order keys. It is possible that we call add_component before the dataset has been created
-        # therefore we need to add the corresponding context to the dataset
-        if len(self.data['@context']) == 0:
-            self.data['@context'] = context['@context']
+        # generate hash id
+        random_bits = getrandbits(128)
+        hash1 = "%032x" % random_bits
 
-        a = Context()
-        a.set_data(data=self.data)
-        a.new_analysis()
-        a.order_context()
-        self.data = a.get_data()
+        # Add the id
+        self.data["id"] = "urn:ngsi-ld:Catalogue:" + hash1
 
-    def get(self):
-        return self.data
+        # Add dataset id
+        self.data["dataset"]["object"] = dataset_id
 
     def add_data(self, title, dataset_id, data):
-        # We need to complete the data corresponding to the Dataset: rdfs:label
+        # We need to complete the data corresponding to the Catalogue: rdfs:label
         self.__complete_label__(title=title, data=data)
 
         # Add the title
-        key = self.keys['dct:title']
-        self.data[key] = title
+        key = self.keys["title"]
+        self.data[key]["value"] = title
 
         # Add the id
-        self.data['id'] = "urn:ngsi-ld:Dataset:" + dataset_id
+        self.data["id"] = "urn:ngsi-ld:Catalogue:" + dataset_id
 
-        # Get the rest of the data
-        data = get_rest_data(data=data,
-                             not_allowed_keys=[
-                                 'sliceKey',
-                                 'component',
-                                 'disseminationStatus',
-                                 'validationState',
-                                 'notation',
-                                 'label'
-                             ],
-                             further_process_keys=[
-                                 'component',
-                                 'label'
-                             ])
+        # Add the publisher
+        key = self.get_key(requested_key="dcterms:publisher")
+        position = data.index(key) + 1
+        self.data["publisher"]["value"] = data[position][0]
+
+        # Check if we have 'issued' in the original, then we need to create the releaseDate property
+        index, key, value = get_property_value(data=data, property_name="issued")
+        if index != -1:
+            # We found an 'issued' data
+            self.data.update(self.__generate_property__(key="releaseDate", value=value[0][0]))
+
+        # Get the rest of the data, qb:structure has the same value of qb:dataset, so we decide to
+        # use only qb:dataset in CatalogueDCAT-AP
+        data = get_rest_data(
+            data=data,
+            not_allowed_keys=["label", "publisher", "structure", "issued", "title"],
+        )
 
         # add the new data to the dataset structure
         self.patch_data(data, False)
 
+        # Order Context keys
+        a = Context()
+        a.set_data(new_data=self.data)
+        a.order_context()
+        self.data = a.get_data()
+
     def patch_data(self, data, language_map):
         if language_map:
             self.__complete_label__(title="Not specified", data=data)
         else:
             # TODO: Add only those properties that are expected, if they are not know or unexpected discard and provide
             #  a logging about the property is discarded due to it is not considered in the statSCAT-AP spec.
-            [self.data.update({k: v}) for k, v in data.items()]
+            [self.data.update(self.__generate_property__(key=k, value=v)) for k, v in data.items()]
 
     def __complete_label__(self, title, data):
         try:
-            key = self.get_key(requested_key='rdfs:label')
+            key = self.get_key(requested_key="rdfs:label")
             position = data.index(key) + 1
             description = data[position]
 
-            descriptions = [x[0].replace("\"", "") for x in description]
+            descriptions = [x[0].replace('"', "") for x in description]
 
             languages = list()
             try:
                 languages = [x[1].replace("@", "").lower() for x in description]
             except IndexError:
-                logger.warning(f'The Dataset {title} has a '
-                               f'rdfs:label without language tag: {description}')
+                logger.warning(f"The Catalogue {title} has a " f"rdfs:label without language tag: {description}")
 
                 aux = len(description)
                 if aux != 1:
-                    logger.error(f"Dataset: there is more than 1 description ({aux}), values: {description}")
+                    logger.error(f"Catalogue: there is more than 1 description ({aux}), values: {description}")
                 else:
                     # There is no language tag, we use by default 'en'
-                    languages = ['en']
-                    logger.warning('Dataset: selecting default language "en"')
+                    languages = ["en"]
+                    logger.warning('Catalogue: selecting default language "en"')
 
             ###############################################################################
             # TODO: New ETSI CIM NGSI-LD specification 1.4.2
             # Pending to implement in the Context Broker
             ###############################################################################
             # for i in range(0, len(languages)):
             #     self.data['rdfs:label']['LanguageMap'][languages[i]] = descriptions[i]
             ###############################################################################
             for i in range(0, len(languages)):
-                key = self.keys['dct:description']
-                self.data[key]['value'][languages[i]] = descriptions[i]
+                key = self.keys["description"]
+                self.data[key]["value"][languages[i]] = descriptions[i]
 
             # Complete the information of the language with the previous information
-            key = self.keys['dct:language']
-            self.data[key]['value'] = languages
+            key = self.keys["language"]
+            self.data[key]["value"] = languages
         except ValueError:
-            logger.info(f'DataStructureDefinition without rdfs:label detail: {title}')
+            logger.info(f"Dataset without rdfs:label detail: {title}")
+
+    def get(self):
+        return self.data
+
+    def get_id(self):
+        return self.data["id"]
 
     def get_key(self, requested_key):
         try:
             key = self.keys[requested_key]
             return key
         except KeyError:
             # The key did not exist therefore we add to the list with this value
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/dimension.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/dimension.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ##
 
 from sdmx2jsonld.transform.property import Property
 
 
 class Dimension(Property):
     def __init__(self):
-        super().__init__(entity='DimensionProperty')
-        self.data['type'] = 'DimensionProperty'
+        super().__init__(entity="DimensionProperty")
+        self.data["type"] = "DimensionProperty"
 
-    def add_data(self, id, data):
-        super().add_data(id=id, data=data)
+    def add_data(self, property_id, data):
+        super().add_data(property_id=property_id, data=data)
 
         # Add the id
-        self.data['id'] = "urn:ngsi-ld:DimensionProperty:" + id
+        self.data["id"] = "urn:ngsi-ld:DimensionProperty:" + property_id
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/entitytype.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/entitytype.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,204 +21,229 @@
 ##
 
 from sdmx2jsonld.transform.dataset import Dataset
 from sdmx2jsonld.transform.dimension import Dimension
 from sdmx2jsonld.transform.conceptschema import ConceptSchema
 from sdmx2jsonld.transform.concept import Concept
 from sdmx2jsonld.transform.attribute import Attribute
-from sdmx2jsonld.transform.catalogue import CatalogueDCATAP
+from sdmx2jsonld.transform.catalogue import Catalogue
+from sdmx2jsonld.transform.observation import Observation
 from logging import getLogger
 from datetime import datetime
 from sdmx2jsonld.common.regparser import RegParser
-from sdmx2jsonld.common.classprecedence import Precedence, ClassesPrecedencePropertyError, ClassesPrecedenceClassError
+from sdmx2jsonld.common.classprecedence import (
+    Precedence,
+    ClassPrecedencePropertyError,
+    ClassPrecedenceClassError,
+)
 
 logger = getLogger()
 
 
 class EntityType:
     def __init__(self):
         self.entities = {
-            'qb:DataStructureDefinition': 'Dataset',
-            'qb:ComponentSpecification': 'Component',
-            'qb:AttributeProperty': 'Attribute',
-            'qb:DimensionProperty': 'Dimension',
-            'qb:CodedProperty': 'Dimension',
-            'rdfs:Class': 'Class',
-            'owl:Class': 'Class',
-            'skos:ConceptScheme': 'ConceptScheme',
-            'skos:Concept': 'Range'
+            "qb:DataSet": "Catalogue",
+            "qb:Observation": "Observation",
+            "qb:DataStructureDefinition": "Dataset",
+            "qb:ComponentSpecification": "Component",
+            "qb:AttributeProperty": "Attribute",
+            "qb:DimensionProperty": "Dimension",
+            "qb:CodedProperty": "Dimension",
+            "rdfs:Class": "Class",
+            "owl:Class": "Class",
+            "skos:ConceptScheme": "ConceptScheme",
+            "skos:Concept": "Range",
         }
 
         self.dataset = Dataset()
         self.dimensions = list()
         self.attributes = list()
         self.conceptSchemas = list()
         self.conceptLists = list()
         self.conceptListsIds = dict()
         self.context = dict()
         self.context_mapping = dict()
-        self.catalogue = CatalogueDCATAP()
+        self.catalogue = Catalogue()
+        self.observations = list()
 
         self.pre = Precedence()
+        self.parser = RegParser()
 
     def __find_entity_type__(self, string):
         """
         Find the index position of the 'a' SDMX key and return the following data with the corresponding EntityType
         """
-        is_new = bool()
-
         # Index maybe 0 in case of ComponentSpecification or 1 in case of DataStructureDefinition
         index = len(string) - 1
         string1 = string[index]
 
         # We can get a 'verb' 'objectlist' or an 'objectlist', where verb is 'a'
         # in case that there is no verb, we are talking about a triples whose id was previously
         # created.
         try:
-            position = string1.index('a') + 1
+            position = string1.index("a") + 1
+            data = ""
 
             try:
                 data = self.pre.precedence(string1[position])
 
                 # We have two options, a well-know object list to be found in the self.entities or
                 # the conceptList defined in the turtle file
                 data = self.entities[data]
-            except ClassesPrecedencePropertyError as error:
+            except ClassPrecedencePropertyError as error:
                 logger.error(str(error))
                 data = self.entities[data[0]]
-            except ClassesPrecedenceClassError as error:
+            except ClassPrecedenceClassError as error:
                 logger.warning(str(error))
-                data = self.entities['rdfs:Class']
+                data = self.entities["rdfs:Class"]
             except KeyError:
                 # We found a CodeList or any other thing, check the list of codeList found in the turtle file
                 if data not in self.conceptListsIds:
                     logger.warning(f"Received a unexpected entity type: {data}")
                 else:
-                    data = 'Range'
+                    data = "Range"
 
             is_new = True
         except ValueError:
-            logger.info(f'Not a definition triples {string}, need to find the proper structure')
+            logger.info(f"Not a definition triples {string}, need to find the proper structure")
             is_new = False
             data = self.__get_subject__(title=string[0])
             string1 = string[1:]
 
         return data, string1, is_new
 
     def transform(self, string):
-        if len(self.context) == 0:
-            raise AssertionError("Context should be passed before to the EntityType Class, "
-                                 "call EntityType.set_context() before, {'__file__': this_file}))")
-
         data_type, new_string, is_new = self.__find_entity_type__(string=string)
 
         if is_new:
-            self.create_data(type=data_type, data=new_string, title=string[0])
+            self.create_data(entity_type=data_type, data=new_string, title=string[0])
         else:
-            logger.info(f'Checking previous subjects to find if it was created previously')
+            logger.info(f"Checking previous subjects to find if it was created previously")
             self.patch_data(datatype=data_type, data=new_string)
 
     def patch_data(self, datatype, data):
         def flatten_value(y):
             if isinstance(y, list):
                 return flatten_value(y[0])
             elif isinstance(y, datetime):
                 return y
             else:
-                return y.replace('"', '')
+                return y.replace('"', "")
 
         flatten_data = [item for sublist in data for item in sublist]
 
-        if flatten_data[0] != 'rdfs:label':
+        if flatten_data[0] != "rdfs:label":
             flatten_data = {flatten_data[i]: flatten_value(flatten_data[i + 1]) for i in range(0, len(flatten_data), 2)}
             language_map = False
         else:
             language_map = True
 
-        if datatype == 'Dataset':
+        if datatype == "Dataset":
             self.dataset.patch_data(data=flatten_data, language_map=language_map)
 
-    def create_data(self, type, data, title):
-        parser = RegParser()
-
-        if type == 'Component':
-            self.dataset.add_components(context=self.context, component=data)
-        elif type == 'Dataset':
-            identifier = parser.obtain_id(title)
-            self.dataset.add_context(context=self.context, context_mapping=self.context_mapping)
+    def create_data(self, entity_type, data, title):
+        if entity_type == "Component":
+            (
+                some_new_component,
+                some_new_concept,
+                some_new_concept_schema,
+            ) = self.dataset.add_components(component=data)
+
+            if some_new_component is not None:
+                if some_new_component.data["type"] == "DimensionProperty":
+                    # we have found special sdmx_dimensions that we have to add to dimensions list
+                    self.dimensions.append(some_new_component)
+                elif some_new_component.data["type"] == "AttributeProperty":
+                    # we have found special sdmx_attribute that we have to add to attributes list
+                    self.attributes.append(some_new_component)
+                else:
+                    # You should not be here, reporting error...
+                    logger.error(
+                        f'Unexpected entity type, id: {some_new_component.data["id"]}    '
+                        f'type: {some_new_component.data["type"]}'
+                    )
+
+                if some_new_concept is not None:
+                    self.conceptLists.append(some_new_concept)
+
+                # we need to check that the conceptSchema is not already defined in the structure
+                if some_new_concept_schema not in self.conceptSchemas:
+                    self.conceptSchemas.append(some_new_concept_schema)
+        elif entity_type == "Catalogue":
+            identifier = self.parser.obtain_id(title)
+            self.catalogue.add_data(title=title, dataset_id=identifier, data=data)
+        elif entity_type == "Observation":
+            observation = Observation()
+            identifier = self.parser.obtain_id(title)
+            observation.add_data(title=title, observation_id=identifier, data=data)
+            self.observations.append(observation)
+        elif entity_type == "Dataset":
+            identifier = self.parser.obtain_id(title)
             self.dataset.add_data(title=title, dataset_id=identifier, data=data)
 
             # Create the CatalogueDCAT-AP and assign the dataset id
-            self.catalogue.add_dataset(dataset_id=self.dataset.data['id'])
-        elif type == 'Dimension':
+            self.catalogue.add_dataset(dataset_id=self.dataset.data["id"])
+        elif entity_type == "Dimension":
             dimension = Dimension()
-            dimension.add_context(context=self.context, context_mapping=self.context_mapping)
-            dimension_id = parser.obtain_id(title)
-            dimension.add_data(id=dimension_id, data=data)
+            dimension_id = self.parser.obtain_id(title)
+            dimension.add_data(property_id=dimension_id, data=data)
             self.dimensions.append(dimension)
-        elif type == 'Attribute':
+        elif entity_type == "Attribute":
             attribute = Attribute()
-            attribute.add_context(context=self.context, context_mapping=self.context_mapping)
-            attribute_id = parser.obtain_id(title)
+            attribute_id = self.parser.obtain_id(title)
             attribute.add_data(attribute_id=attribute_id, data=data)
             self.attributes.append(attribute)
-        elif type == 'ConceptScheme':
+        elif entity_type == "ConceptScheme":
             concept_schema = ConceptSchema()
-            concept_schema.add_context(context=self.context, context_mapping=self.context_mapping)
-            concept_schema_id = parser.obtain_id(title)
+            concept_schema_id = self.parser.obtain_id(title)
             concept_schema.add_data(concept_schema_id=concept_schema_id, data=data)
             self.conceptSchemas.append(concept_schema)
-        elif type == 'Class':
+        elif entity_type == "Class":
             # We need the Concept because each of the Range description is of the type Concept
             concept_list = Concept()
-            concept_list.add_context(context=self.context, context_mapping=self.context_mapping)
-            concept_list_id = parser.obtain_id(title)
+            concept_list_id = self.parser.obtain_id(title)
             concept_list.add_data(concept_id=concept_list_id, data=data)
             self.conceptLists.append(concept_list)
             self.conceptListsIds[title] = concept_list.get_id()
-        elif type == 'Range':
+        elif entity_type == "Range":
             # TODO: Range is associated to a Concept and identified properly in the ConceptSchema
             data_range = Concept()
-            data_range.add_context(context=self.context, context_mapping=self.context_mapping)
-            data_range_id = parser.obtain_id(title)
+            data_range_id = self.parser.obtain_id(title)
             data_range.add_data(concept_id=data_range_id, data=data)
             self.conceptLists.append(data_range)
             self.conceptListsIds[title] = data_range.get_id()
-
-            # for i in range(0, len(self.conceptSchemas)):
-            #    concept_schema = self.conceptSchemas[i].data
-            #    has_top_concept_values = concept_schema['skos:hasTopConcept']['value']
-            #
-            #    out = [data_range.data['skos:notation']
-            #           if x == data_range.data['id'] else x for x in has_top_concept_values]
-            #
-            #    self.conceptSchemas[i].data['skos:hasTopConcept']['value'] = out
+        else:
+            logger.error(f'Entity type "{entity_type}" not processed.')
 
     def __get_subject__(self, title):
-        if self.dataset.get()['dct:title'] == title:
-            return 'Dataset'
+        if self.dataset.get()["dct:title"] == title:
+            return "Dataset"
         else:
             AssertionError(f"Still not defined: {title}")
 
     def get_catalogue(self):
         return self.catalogue.get()
 
+    def get_observation(self):
+        return self.observations
+
     def get_dataset(self):
         return self.dataset.get()
 
     def get_dimensions(self):
         return self.dimensions
 
     def get_attributes(self):
         return self.attributes
 
-    def get_conceptSchemas(self):
+    def get_concept_schemas(self):
         return self.conceptSchemas
 
-    def get_conceptList(self):
+    def get_concept_list(self):
         return self.conceptLists
 
     def set_context(self, context, mapping):
         self.context = context
         self.context_mapping = mapping
 
     def save(self, param):
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/property.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/property.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,124 +31,108 @@
 class Property(CommonClass):
     def __init__(self, entity):
         super().__init__(entity=entity)
 
         self.data = {
             "id": str(),
             "type": "",
-            "dct:language": {
-                "type": "Property",
-                "value": list()
-            },
-
+            "language": {"type": "Property", "value": list()},
             #################################################
             # TODO: New ETSI CIM NGSI-LD specification 1.4.2
             # Pending to implement in the Context Broker
             #################################################
-            # "rdfs:label": {
+            # "label": {
             #     "type": "LanguageProperty",
             #     "LanguageMap": dict()
             # },
             #################################################
-            "rdfs:label": {
-                "type": "Property",
-                "value": dict()
-            },
-
-
-            "qb:codeList": {
-                "type": "Relationship",
-                "object": str()
-            },
-            "qb:concept": {
-                "type": "Property",
-                "value": str()
-            },
-            "@context": dict()
+            "label": {"type": "Property", "value": dict()},
+            "codeList": {"type": "Relationship", "object": str()},
+            "concept": {"type": "Relationship", "object": str()},
+            "@context": [
+                "https://raw.githubusercontent.com/smart-data-models/dataModel.STAT-DCAT-AP/master/context.jsonld"
+            ],
         }
 
         self.keys = {k: k for k in self.data.keys()}
 
-    def add_data(self, id, data):
+    def add_data(self, property_id, data):
         # TODO: We have to control that data include the indexes that we want to search
         # We need to complete the data corresponding to the Dimension: rdfs:label
-        position = data.index('rdfs:label') + 1
+        position = data.index("rdfs:label") + 1
         description = data[position]
 
-        descriptions = [x[0].replace("\"", "") for x in description]
+        descriptions = [x[0].replace('"', "") for x in description]
 
         languages = list()
         try:
             languages = [x[1].replace("@", "").lower() for x in description]
         except IndexError:
-            logger.warning(f'The Property {id} has a '
-                           f'rdfs:label without language tag: {description}')
+            logger.warning(f"The Property {property_id} has a " f"rdfs:label without language tag: {description}")
 
             aux = len(description)
             if aux != 1:
                 logger.error(f"Property: there is more than 1 description ({aux}), values: {description}")
             else:
                 # There is no language tag, we use by default 'en'
-                languages = ['en']
+                languages = ["en"]
                 logger.warning('Property: selecting default language "en"')
 
         ###############################################################################
         # TODO: New ETSI CIM NGSI-LD specification 1.4.2
         # Pending to implement in the Context Broker
         ###############################################################################
         # for i in range(0, len(languages)):
-        #     self.data['rdfs:label']['LanguageMap'][languages[i]] = descriptions[i]
+        #     self.data['label']['LanguageMap'][languages[i]] = descriptions[i]
         ###############################################################################
         for i in range(0, len(languages)):
-            self.data['rdfs:label']['value'][languages[i]] = descriptions[i]
+            self.data["label"]["value"][languages[i]] = descriptions[i]
 
         # Complete the information of the language with the previous information
-        key = self.keys['dct:language']
-        self.data[key]['value'] = languages
+        key = self.keys["language"]
+        self.data[key]["value"] = languages
 
         # qb:codeList, this attribute might not be presented, so we need to check it.
         # TODO: We need to control that the codeList id extracted here are the same that we analyse afterwards.
         try:
-            position = data.index('qb:codeList') + 1
+            position = data.index("qb:codeList") + 1
             code_list = self.generate_id(entity="ConceptSchema", value=data[position][0])
-            self.data['qb:codeList']['object'] = code_list
+            self.data["codeList"]["object"] = code_list
         except ValueError:
-            logger.warning(f'Property: {id} has not qb:codeList, deleting the key in the data')
+            logger.warning(f"Property: {property_id} has not qb:codeList, deleting the key in the data")
 
             # If we have not the property, we delete it from data
-            self.data.pop('qb:codeList')
+            self.data.pop("codeList")
 
         # qb:concept
         # TODO: the concept id need to check if it is a normal id or an url
-        position = data.index('qb:concept') + 1
+        position = data.index("qb:concept") + 1
         concept = self.generate_id(entity="Concept", value=data[position][0])
-        self.data['qb:concept']['value'] = concept
+        self.data["concept"]["object"] = concept
 
         # Get the rest of the data
-        data = get_rest_data(data=data,
-                             not_allowed_keys=[
-                                 'sliceKey',
-                                 'component',
-                                 'disseminationStatus',
-                                 'validationState',
-                                 'notation',
-                                 'label',
-                                 'codeList',
-                                 'concept'
-                             ],
-                             further_process_keys=[
-                                 'component',
-                                 'label'
-                             ])
+        data = get_rest_data(
+            data=data,
+            not_allowed_keys=[
+                "sliceKey",
+                "component",
+                "disseminationStatus",
+                "validationState",
+                "notation",
+                "label",
+                "codeList",
+                "concept",
+            ],
+            further_process_keys=["component", "label"],
+        )
 
         # add the new data to the dataset structure
-        [self.data.update({k: v}) for k, v in data.items()]
+        [self.data.update(self.__generate_property__(key=k, value=v)) for k, v in data.items()]
 
-        # Simplify Context and order keys
+        # Order the keys in the final json-ld
         a = Context()
-        a.set_data(data=self.data)
-        a.new_analysis()
+        a.set_data(new_data=self.data)
         a.order_context()
         self.data = a.get_data()
 
     def get(self):
         return self.data
```

### Comparing `sdmx2json_ld-0.5.1/sdmx2jsonld/transform/transformer.py` & `sdmx2json_ld-1.0.0/sdmx2jsonld/transform/transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,46 +16,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 ##
 
-from lark import Transformer, Tree, Token
+from lark import Transformer
 from sdmx2jsonld.transform.context import Context
 from sdmx2jsonld.transform.entitytype import EntityType
 from sdmx2jsonld.common.datatypeconversion import DataTypeConversion
+from sdmx2jsonld.transform.distribution import Distribution
 import re
 
 
 class TreeToJson(Transformer):
     def __init__(self):
         super().__init__()
         self.context = Context()
         self.entity_type = EntityType()
 
         # Regex to check valid URL
-        # regex = "<http[s]?:\/\/(.*)>"
         regex = "http[s]?:\/\/(.*)"
 
         # Compile the Regex
         self.re = re.compile(regex)
 
     def prefixid(self, s):
         context = dict()
         context[str(s[0].children[0])] = s[1]
         self.context.add_context(context)
 
     def triples(self, triple):
-        self.entity_type.set_context(context=self.get_context(), mapping=self.get_context_mapping())
         self.entity_type.transform(string=triple)
         return triple
 
     def predicate(self, pre):
-        result = ''
+        result = ""
         if isinstance(pre[0], str):
             result = pre[0]
         else:
             result = str(pre[0].children[0].children[0])
 
         return result
 
@@ -89,16 +88,16 @@
     def iri(self, iri):
         return str(iri[0])
         # return iri
 
     def verb(self, verb):
         return str(verb[0])
 
-    def object(self, object):
-        return object[0]
+    def object(self, my_object):
+        return my_object[0]
 
     def literal(self, literal):
         return literal[0]
 
     def uriref(self, uriref):
         return str(uriref[0])
 
@@ -111,39 +110,55 @@
 
     def get_context_mapping(self):
         return self.context.get_context_mapping()
 
     def get_catalogue(self):
         return self.entity_type.get_catalogue()
 
+    def get_observation(self):
+        if self.entity_type.observations.data["id"] != "":
+            return self.entity_type.get_observation()
+
     def get_dataset(self):
-        return self.entity_type.get_dataset()
+        if self.entity_type.dataset.data["id"] != "":
+            return self.entity_type.get_dataset()
+        return None
 
     def get_dimensions(self):
         return self.entity_type.get_dimensions()
 
     def get_attributes(self):
         return self.entity_type.get_attributes()
 
-    def get_conceptSchemas(self):
-        return self.entity_type.get_conceptSchemas()
+    def get_concept_schemas(self):
+        return self.entity_type.get_concept_schemas()
 
-    def get_conceptLists(self):
-        return self.entity_type.get_conceptList()
+    def get_concept_lists(self):
+        return self.entity_type.get_concept_list()
 
     def save(self):
-        self.entity_type.save('catalogue')
+        self.entity_type.save("catalogue")
 
-        self.entity_type.save('dataset')
+        if self.entity_type.dataset.data["id"] != "":
+            self.entity_type.save("dataset")
 
         dimensions = self.entity_type.get_dimensions()
         [dimension.save() for dimension in dimensions]
 
         attributes = self.entity_type.get_attributes()
         [attribute.save() for attribute in attributes]
 
-        concept_schemas = self.entity_type.get_conceptSchemas()
+        concept_schemas = self.entity_type.get_concept_schemas()
         [x.save() for x in concept_schemas]
 
-        concept_lists = self.entity_type.get_conceptList()
+        concept_lists = self.entity_type.get_concept_list()
         [x.save() for x in concept_lists]
 
+        if len(self.entity_type.observations) != 0:
+            observations = self.entity_type.get_observation()
+            [observation.save() for observation in observations]
+
+            # If we have several observations, we need to generate the DCAT-AP:Distribution class
+            distribution = Distribution()
+            distribution.generate_data(catalogue=self.entity_type.catalogue)
+
+            distribution.save()
```

### Comparing `sdmx2json_ld-0.5.1/setup.py` & `sdmx2json_ld-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sdmx2json-ld
+Version: 1.0.0
+Summary: A SDMX in RDF Turtle 1.1 format parser to generate valid JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-LD.
+Home-page: https://github.com/flopezag/IoTAgent-Turtle
+Keywords: parsing,ETSI NGSI-LD,SDMX
+Author: Fernando López
+Author-email: fernando.lopez@fiware.org
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: docopt (==0.6.2)
+Requires-Dist: fastapi (==0.100.0)
+Requires-Dist: hi-dateinfer (==0.4.6)
+Requires-Dist: lark (==1.1.7)
+Requires-Dist: loguru (==0.7.0)
+Requires-Dist: python-dateutil (==2.8.2)
+Requires-Dist: python-multipart (==0.0.6)
+Requires-Dist: rdflib (==6.3.2)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: schema (==0.7.5)
+Requires-Dist: secure (==0.3.0)
+Requires-Dist: uvicorn (==0.23.1)
+Project-URL: Repository, https://github.com/flopezag/IoTAgent-Turtle
+Description-Content-Type: text/markdown
 
-packages = \
-['sdmx2jsonld',
- 'sdmx2jsonld.common',
- 'sdmx2jsonld.exceptions',
- 'sdmx2jsonld.transform']
-
-package_data = \
-{'': ['*'], 'sdmx2jsonld': ['grammar/*']}
-
-install_requires = \
-['docopt==0.6.2',
- 'fastapi==0.85.1',
- 'hi-dateinfer==0.4.6',
- 'lark==1.1.3',
- 'loguru==0.6.0',
- 'python-multipart==0.0.5',
- 'rdflib>=6.2.0,<6.3.0',
- 'requests==2.28.1',
- 'schema==0.7.5',
- 'secure==0.3.0',
- 'uvicorn==0.19.0']
-
-setup_kwargs = {
-    'name': 'sdmx2json-ld',
-    'version': '0.5.1',
-    'description': 'A SDMX in RDF Turtle 1.1 format parser to generate valid JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-LD.',
-    'long_description': '<div id="top"></div>\n\n# SDMX to JSON-LD Parser\n\n<!-- PROJECT SHIELDS -->\n[![Stable Version][version-shield]][version-url]\n[![Issues][issues-shield]][issues-url]\n[![Apache2.0 License][license-shield]][license-url]\n[![Python Versions][python-shield]][python-url]\n[![Package Status][package-shield]][package-url]\n[![LinkedIn][linkedin-shield]][linkedin-url]\n\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/flopezag/IoTAgent-Turtle">\n    <img src="https://raw.githubusercontent.com/flopezag/IoTAgent-Turtle/master/images/logo.png" \nalt="Logo" width="280" height="160">\n  </a>\n\n<h3 align="center">SDMX (Turtle) to NGSI-LD (JSON-LD) converter</h3>\n\n  <p align="center">\n    A SDMX to JSON-LD parser to communicate with FIWARE Context Brokers using ETSI NGSI-LD.\n    <br />\n    <a href="https://github.com/flopezag/IoTAgent-Turtle"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/flopezag/IoTAgent-Turtle">View Demo</a>\n    ·\n    <a href="https://github.com/flopezag/IoTAgent-Turtle/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/flopezag/IoTAgent-Turtle/issues">Request Feature</a>\n  </p>\n</div>\n\n\n<!-- ABOUT THE PROJECT -->\n## About The Project\n\nA SDMX in RDF Turtle 1.1 format parser to generate valid JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-LD.\n\nIt is based on a \n[EBNF LALR(1) grammar](https://github.com/flopezag/IoTAgent-Turtle/blob/master/sdmx2jsonld/grammar/grammar.lark).\n\nThis project is part of INTERSTAT. For more information about the INTERSTAT Project, please check the url \nhttps://cef-interstat.eu.\n\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n### Dependencies\n\nThe dependencies of the sdmx2jsonld python package are the following:\n\n* [Lark - a modern general-purpose parsing library for Python](https://lark-parser.readthedocs.io/en/latest).\n* [hi-dateinfer - a python library to infer date format from examples](https://github.com/hi-primus/hi-dateinfer).\n* [Loguru - a library which aims to bring enjoyable logging in Python](https://loguru.readthedocs.io/en/stable/index.html).\n* [Requests - an elegant and simple HTTP library for Python, built for human beings](https://requests.readthedocs.io).\n* [RDFLib - a pure Python package for working with RDF](https://rdflib.readthedocs.io).\n\nFor more details about the versions of each library, please refer to \n[requirements.txt](https://github.com/flopezag/IoTAgent-Turtle/blob/master/requirements.txt).\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n\n<!-- GETTING STARTED -->\n## Installing SDMX2JSON-LD and Supported Versions\nSDMX2JSON-LD is available on PyPI:\n\n```bash\n$ python -m pip install sdmx2jsonld\n```\n\nSDMX2JSON-LD officially supports Python 3.10+.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nTo execute the python module you can follow the following code to parse the RDF Turtle file to generate the JSON-LD \ncontent to be sent to the FIWARE Context Broker:\n\n```python\nfrom sdmx2jsonld.transform.parser import Parser\nfrom sdmx2jsonld.exceptions import UnexpectedEOF, UnexpectedInput, UnexpectedToken\n\nfile_in = open("structures-accounts.ttl")\ngenerate_files = True\n\n# Start parsing the file\nmy_parser = Parser()\n\ntry:\n    my_parser.parsing(content=file_in, out=generate_files)\nexcept UnexpectedToken as e:\n    print(e)\nexcept UnexpectedInput as e:\n    print(e)\nexcept UnexpectedEOF as e:\n    print(e)\n```\n\nWhere:\n* `file_in` is the RDF Turtle content that can be a string in StringIO class or a read file in TextIOWrapper class.\n* `file_out` is a boolean variable to indicate if we want to save the JSON-LD parser content into files (True) or we \nwant to show the content in the screen (False).\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- CONTRIBUTING -->\n## Contributing\n\nContributions are what make the open source community such an amazing place to learn, inspire, and create. \nAny contributions you make are **greatly appreciated**. If you have a suggestion that would make this better, \nplease fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".\nDon\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- CONTACT -->\n## Contact\n\nFernando López - [@flopezaguilar](https://twitter.com/flopezaguilar) - fernando.lopez@fiware.org\n\nProject Link: [https://github.com/flopezag/IoTAgent-Turtle](https://github.com/flopezag/IoTAgent-Turtle)\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the Apache2.0 License. See [LICENSE](https://github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE) \nfor more information.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[issues-shield]: https://img.shields.io/github/issues/flopezag/IoTAgent-Turtle.svg?style=flat\n[issues-url]: https://github.com/flopezag/IoTAgent-Turtle/issues\n\n[license-shield]: https://img.shields.io/github/license/flopezag/IoTAgent-Turtle\n[license-url]: https://github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE\n\n[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555\n[linkedin-url]: https://linkedin.com/in/fernandolopezaguilar\n\n[python-shield]: https://img.shields.io/pypi/pyversions/sdmx2json-ld\n[python-url]: https://pypi.org/project/sdmx2json-ld\n\n[version-shield]: https://img.shields.io/pypi/v/sdmx2json-ld\n[version-url]: https://pypi.org/project/sdmx2json-ld/#history\n\n[package-shield]: https://img.shields.io/pypi/status/sdmx2json-ld\n[package-url]: https://pypi.org/project/sdmx2json-ld\n',
-    'author': 'Fernando López',
-    'author_email': 'fernando.lopez@fiware.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/flopezag/IoTAgent-Turtle',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+<div id="top"></div>
 
+# SDMX to JSON-LD Parser
+
+<!-- PROJECT SHIELDS -->
+[![Stable Version][version-shield]][version-url]
+[![Issues][issues-shield]][issues-url]
+[![Apache2.0 License][license-shield]][license-url]
+[![Python Versions][python-shield]][python-url]
+[![Package Status][package-shield]][package-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/flopezag/IoTAgent-Turtle">
+    <img src="https://raw.githubusercontent.com/flopezag/IoTAgent-Turtle/master/images/logo.png" 
+alt="Logo" width="280" height="160">
+  </a>
+
+<h3 align="center">SDMX (Turtle) to NGSI-LD (JSON-LD) converter</h3>
+
+  <p align="center">
+    A SDMX to JSON-LD parser to communicate with FIWARE Context Brokers using ETSI NGSI-LD.
+    <br />
+    <a href="https://github.com/flopezag/IoTAgent-Turtle"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/flopezag/IoTAgent-Turtle">View Demo</a>
+    ·
+    <a href="https://github.com/flopezag/IoTAgent-Turtle/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/flopezag/IoTAgent-Turtle/issues">Request Feature</a>
+  </p>
+</div>
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+
+A SDMX in RDF Turtle 1.1 format parser to generate valid JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-LD.
+
+It is based on a 
+[EBNF LALR(1) grammar](https://github.com/flopezag/IoTAgent-Turtle/blob/master/sdmx2jsonld/grammar/grammar.lark).
+
+This project is part of INTERSTAT. For more information about the INTERSTAT Project, please check the url 
+https://cef-interstat.eu.
+
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+### Dependencies
+
+The dependencies of the sdmx2jsonld python package are the following:
+
+* [Lark - a modern general-purpose parsing library for Python](https://lark-parser.readthedocs.io/en/latest).
+* [hi-dateinfer - a python library to infer date format from examples](https://github.com/hi-primus/hi-dateinfer).
+* [Loguru - a library which aims to bring enjoyable logging in Python](https://loguru.readthedocs.io/en/stable/index.html).
+* [Requests - an elegant and simple HTTP library for Python, built for human beings](https://requests.readthedocs.io).
+* [RDFLib - a pure Python package for working with RDF](https://rdflib.readthedocs.io).
+
+For more details about the versions of each library, please refer to 
+[requirements.txt](https://github.com/flopezag/IoTAgent-Turtle/blob/master/requirements.txt).
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+
+<!-- GETTING STARTED -->
+## Installing SDMX2JSON-LD and Supported Versions
+SDMX2JSON-LD is available on PyPI:
+
+```bash
+$ python -m pip install sdmx2jsonld
+```
+
+SDMX2JSON-LD officially supports Python 3.10+.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+
+<!-- USAGE EXAMPLES -->
+## Usage
+
+To execute the python module you can follow the following code to parse the RDF Turtle file to generate the JSON-LD 
+content to be sent to the FIWARE Context Broker:
+
+```python
+from sdmx2jsonld.transform.parser import Parser
+from sdmx2jsonld.exceptions import UnexpectedEOF, UnexpectedInput, UnexpectedToken
+
+file_in = open("structures-accounts.ttl")
+generate_files = True
+
+# Start parsing the file
+my_parser = Parser()
+
+try:
+    my_parser.parsing(content=file_in, out=generate_files)
+except UnexpectedToken as e:
+    print(e)
+except UnexpectedInput as e:
+    print(e)
+except UnexpectedEOF as e:
+    print(e)
+```
+
+Where:
+* `file_in` is the RDF Turtle content that can be a string in StringIO class or a read file in TextIOWrapper class.
+* `file_out` is a boolean variable to indicate if we want to save the JSON-LD parser content into files (True) or we 
+want to show the content in the screen (False).
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-- CONTRIBUTING -->
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. 
+Any contributions you make are **greatly appreciated**. If you have a suggestion that would make this better, 
+please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-- CONTACT -->
+## Contact
+
+Fernando López - [@flopezaguilar](https://twitter.com/flopezaguilar) - fernando.lopez@fiware.org
+
+Project Link: [https://github.com/flopezag/IoTAgent-Turtle](https://github.com/flopezag/IoTAgent-Turtle)
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-- LICENSE -->
+## License
+
+Distributed under the Apache2.0 License. See [LICENSE](https://github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE) 
+for more information.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[issues-shield]: https://img.shields.io/github/issues/flopezag/IoTAgent-Turtle.svg?style=flat
+[issues-url]: https://github.com/flopezag/IoTAgent-Turtle/issues
+
+[license-shield]: https://img.shields.io/github/license/flopezag/IoTAgent-Turtle
+[license-url]: https://github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE
+
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/fernandolopezaguilar
+
+[python-shield]: https://img.shields.io/pypi/pyversions/sdmx2json-ld
+[python-url]: https://pypi.org/project/sdmx2json-ld
+
+[version-shield]: https://img.shields.io/pypi/v/sdmx2json-ld
+[version-url]: https://pypi.org/project/sdmx2json-ld/#history
+
+[package-shield]: https://img.shields.io/pypi/status/sdmx2json-ld
+[package-url]: https://pypi.org/project/sdmx2json-ld
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,98 +1,94 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['sdmx2jsonld', 'sdmx2jsonld.common', 'sdmx2jsonld.exceptions',
-'sdmx2jsonld.transform'] package_data = \ {'': ['*'], 'sdmx2jsonld': ['grammar/
-*']} install_requires = \ ['docopt==0.6.2', 'fastapi==0.85.1', 'hi-
-dateinfer==0.4.6', 'lark==1.1.3', 'loguru==0.6.0', 'python-multipart==0.0.5',
-'rdflib>=6.2.0,<6.3.0', 'requests==2.28.1', 'schema==0.7.5', 'secure==0.3.0',
-'uvicorn==0.19.0'] setup_kwargs = { 'name': 'sdmx2json-ld', 'version': '0.5.1',
-'description': 'A SDMX in RDF Turtle 1.1 format parser to generate valid JSON-
-LD and send to FIWARE Context Brokers using ETSI NGSI-LD.', 'long_description':
-'
-\n\n# SDMX to JSON-LD Parser\n\n\n[![Stable Version][version-shield]][version-
-url]\n[![Issues][issues-shield]][issues-url]\n[![Apache2.0 License][license-
-shield]][license-url]\n[![Python Versions][python-shield]][python-url]\n[!
-[Package Status][package-shield]][package-url]\n[![LinkedIn][linkedin-shield]]
-[linkedin-url]\n\n\n\n
-\n
-               \n \n_nalt="Logo"_width="280"_height="160">\n\n\n
+Metadata-Version: 2.1 Name: sdmx2json-ld Version: 1.0.0 Summary: A SDMX in RDF
+Turtle 1.1 format parser to generate valid JSON-LD and send to FIWARE Context
+Brokers using ETSI NGSI-LD. Home-page: https://github.com/flopezag/IoTAgent-
+Turtle Keywords: parsing,ETSI NGSI-LD,SDMX Author: Fernando LÃ³pez Author-
+email: fernando.lopez@fiware.org Requires-Python: >=3.8,<4.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: docopt (==0.6.2) Requires-Dist: fastapi (==0.100.0) Requires-
+Dist: hi-dateinfer (==0.4.6) Requires-Dist: lark (==1.1.7) Requires-Dist:
+loguru (==0.7.0) Requires-Dist: python-dateutil (==2.8.2) Requires-Dist:
+python-multipart (==0.0.6) Requires-Dist: rdflib (==6.3.2) Requires-Dist:
+requests (==2.31.0) Requires-Dist: schema (==0.7.5) Requires-Dist: secure
+(==0.3.0) Requires-Dist: uvicorn (==0.23.1) Project-URL: Repository, https://
+github.com/flopezag/IoTAgent-Turtle Description-Content-Type: text/markdown
+# SDMX to JSON-LD Parser  [![Stable Version][version-shield]][version-url] [!
+[Issues][issues-shield]][issues-url] [![Apache2.0 License][license-shield]]
+[license-url] [![Python Versions][python-shield]][python-url] [![Package
+Status][package-shield]][package-url] [![LinkedIn][linkedin-shield]][linkedin-
+url]
+                                    [Logo]
             **** SDMX (Turtle) to NGSI-LD (JSON-LD) converter ****
-                                     \n\n
- \n A SDMX to JSON-LD parser to communicate with FIWARE Context Brokers using
-                               ETSI NGSI-LD.\n
-                           \n Explore_the_docs_Â»\n
-                                      \n
-            \n View_Demo\n Â·\n Report_Bug\n Â·\n Request_Feature\n
-                                      \n
-\n\n\n\n## About The Project\n\nA SDMX in RDF Turtle 1.1 format parser to
-generate valid JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-
-LD.\n\nIt is based on a \n[EBNF LALR(1) grammar](https://github.com/flopezag/
-IoTAgent-Turtle/blob/master/sdmx2jsonld/grammar/grammar.lark).\n\nThis project
-is part of INTERSTAT. For more information about the INTERSTAT Project, please
-check the url \nhttps://cef-interstat.eu.\n\n\n
-                                                                  (back_to_top)
-\n\n\n### Dependencies\n\nThe dependencies of the sdmx2jsonld python package
-are the following:\n\n* [Lark - a modern general-purpose parsing library for
-Python](https://lark-parser.readthedocs.io/en/latest).\n* [hi-dateinfer - a
-python library to infer date format from examples](https://github.com/hi-
-primus/hi-dateinfer).\n* [Loguru - a library which aims to bring enjoyable
-logging in Python](https://loguru.readthedocs.io/en/stable/index.html).\n*
-[Requests - an elegant and simple HTTP library for Python, built for human
-beings](https://requests.readthedocs.io).\n* [RDFLib - a pure Python package
-for working with RDF](https://rdflib.readthedocs.io).\n\nFor more details about
-the versions of each library, please refer to \n[requirements.txt](https://
-github.com/flopezag/IoTAgent-Turtle/blob/master/requirements.txt).\n\n
-                                                                  (back_to_top)
-\n\n\n\n\n## Installing SDMX2JSON-LD and Supported Versions\nSDMX2JSON-LD is
-available on PyPI:\n\n```bash\n$ python -m pip install
-sdmx2jsonld\n```\n\nSDMX2JSON-LD officially supports Python 3.10+.\n\n
-                                                                  (back_to_top)
-\n\n\n\n\n## Usage\n\nTo execute the python module you can follow the following
-code to parse the RDF Turtle file to generate the JSON-LD \ncontent to be sent
-to the FIWARE Context Broker:\n\n```python\nfrom sdmx2jsonld.transform.parser
-import Parser\nfrom sdmx2jsonld.exceptions import UnexpectedEOF,
-UnexpectedInput, UnexpectedToken\n\nfile_in = open("structures-
-accounts.ttl")\ngenerate_files = True\n\n# Start parsing the file\nmy_parser =
-Parser()\n\ntry:\n my_parser.parsing(content=file_in,
-out=generate_files)\nexcept UnexpectedToken as e:\n print(e)\nexcept
-UnexpectedInput as e:\n print(e)\nexcept UnexpectedEOF as e:\n print
-(e)\n```\n\nWhere:\n* `file_in` is the RDF Turtle content that can be a string
-in StringIO class or a read file in TextIOWrapper class.\n* `file_out` is a
-boolean variable to indicate if we want to save the JSON-LD parser content into
-files (True) or we \nwant to show the content in the screen (False).\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contributing\n\nContributions are what make the open source
-community such an amazing place to learn, inspire, and create. \nAny
-contributions you make are **greatly appreciated**. If you have a suggestion
-that would make this better, \nplease fork the repo and create a pull request.
-You can also simply open an issue with the tag "enhancement".\nDon\'t forget to
-give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your
-Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your
-Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch
-(`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contact\n\nFernando LÃ³pez - [@flopezaguilar](https://twitter.com/
-flopezaguilar) - fernando.lopez@fiware.org\n\nProject Link: [https://
-github.com/flopezag/IoTAgent-Turtle](https://github.com/flopezag/IoTAgent-
-Turtle)\n\n
-                                                                  (back_to_top)
-\n\n\n\n## License\n\nDistributed under the Apache2.0 License. See [LICENSE]
-(https://github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE) \nfor more
-information.\n\n
-                                                                  (back_to_top)
-\n\n\n\n\n[issues-shield]: https://img.shields.io/github/issues/flopezag/
-IoTAgent-Turtle.svg?style=flat\n[issues-url]: https://github.com/flopezag/
-IoTAgent-Turtle/issues\n\n[license-shield]: https://img.shields.io/github/
-license/flopezag/IoTAgent-Turtle\n[license-url]: https://github.com/flopezag/
-IoTAgent-Turtle/blob/master/LICENSE\n\n[linkedin-shield]: https://
-img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555\n
-[linkedin-url]: https://linkedin.com/in/fernandolopezaguilar\n\n[python-
-shield]: https://img.shields.io/pypi/pyversions/sdmx2json-ld\n[python-url]:
-https://pypi.org/project/sdmx2json-ld\n\n[version-shield]: https://
-img.shields.io/pypi/v/sdmx2json-ld\n[version-url]: https://pypi.org/project/
-sdmx2json-ld/#history\n\n[package-shield]: https://img.shields.io/pypi/status/
-sdmx2json-ld\n[package-url]: https://pypi.org/project/sdmx2json-ld\n',
-'author': 'Fernando LÃ³pez', 'author_email': 'fernando.lopez@fiware.org',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-flopezag/IoTAgent-Turtle', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+A SDMX to JSON-LD parser to communicate with FIWARE Context Brokers using ETSI
+                                   NGSI-LD.
+                             Explore_the_docs_Â»
+
+                  View_Demo Â· Report_Bug Â· Request_Feature
+ ## About The Project A SDMX in RDF Turtle 1.1 format parser to generate valid
+JSON-LD and send to FIWARE Context Brokers using ETSI NGSI-LD. It is based on a
+[EBNF LALR(1) grammar](https://github.com/flopezag/IoTAgent-Turtle/blob/master/
+sdmx2jsonld/grammar/grammar.lark). This project is part of INTERSTAT. For more
+information about the INTERSTAT Project, please check the url https://cef-
+interstat.eu.
+                                                                  (back_to_top)
+### Dependencies The dependencies of the sdmx2jsonld python package are the
+following: * [Lark - a modern general-purpose parsing library for Python]
+(https://lark-parser.readthedocs.io/en/latest). * [hi-dateinfer - a python
+library to infer date format from examples](https://github.com/hi-primus/hi-
+dateinfer). * [Loguru - a library which aims to bring enjoyable logging in
+Python](https://loguru.readthedocs.io/en/stable/index.html). * [Requests - an
+elegant and simple HTTP library for Python, built for human beings](https://
+requests.readthedocs.io). * [RDFLib - a pure Python package for working with
+RDF](https://rdflib.readthedocs.io). For more details about the versions of
+each library, please refer to [requirements.txt](https://github.com/flopezag/
+IoTAgent-Turtle/blob/master/requirements.txt).
+                                                                  (back_to_top)
+ ## Installing SDMX2JSON-LD and Supported Versions SDMX2JSON-LD is available on
+PyPI: ```bash $ python -m pip install sdmx2jsonld ``` SDMX2JSON-LD officially
+supports Python 3.10+.
+                                                                  (back_to_top)
+ ## Usage To execute the python module you can follow the following code to
+parse the RDF Turtle file to generate the JSON-LD content to be sent to the
+FIWARE Context Broker: ```python from sdmx2jsonld.transform.parser import
+Parser from sdmx2jsonld.exceptions import UnexpectedEOF, UnexpectedInput,
+UnexpectedToken file_in = open("structures-accounts.ttl") generate_files = True
+# Start parsing the file my_parser = Parser() try: my_parser.parsing
+(content=file_in, out=generate_files) except UnexpectedToken as e: print(e)
+except UnexpectedInput as e: print(e) except UnexpectedEOF as e: print(e) ```
+Where: * `file_in` is the RDF Turtle content that can be a string in StringIO
+class or a read file in TextIOWrapper class. * `file_out` is a boolean variable
+to indicate if we want to save the JSON-LD parser content into files (True) or
+we want to show the content in the screen (False).
+                                                                  (back_to_top)
+ ## Contributing Contributions are what make the open source community such an
+amazing place to learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. If you have a suggestion that would make this better,
+please fork the repo and create a pull request. You can also simply open an
+issue with the tag "enhancement". Don't forget to give the project a star!
+Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
+-b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
+AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request
+                                                                  (back_to_top)
+ ## Contact Fernando LÃ³pez - [@flopezaguilar](https://twitter.com/
+flopezaguilar) - fernando.lopez@fiware.org Project Link: [https://github.com/
+flopezag/IoTAgent-Turtle](https://github.com/flopezag/IoTAgent-Turtle)
+                                                                  (back_to_top)
+ ## License Distributed under the Apache2.0 License. See [LICENSE](https://
+github.com/flopezag/IoTAgent-Turtle/blob/master/LICENSE) for more information.
+                                                                  (back_to_top)
+  [issues-shield]: https://img.shields.io/github/issues/flopezag/IoTAgent-
+Turtle.svg?style=flat [issues-url]: https://github.com/flopezag/IoTAgent-
+Turtle/issues [license-shield]: https://img.shields.io/github/license/flopezag/
+IoTAgent-Turtle [license-url]: https://github.com/flopezag/IoTAgent-Turtle/
+blob/master/LICENSE [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
+black.svg?style=flat&logo=linkedin&colorB=555 [linkedin-url]: https://
+linkedin.com/in/fernandolopezaguilar [python-shield]: https://img.shields.io/
+pypi/pyversions/sdmx2json-ld [python-url]: https://pypi.org/project/sdmx2json-
+ld [version-shield]: https://img.shields.io/pypi/v/sdmx2json-ld [version-url]:
+https://pypi.org/project/sdmx2json-ld/#history [package-shield]: https://
+img.shields.io/pypi/status/sdmx2json-ld [package-url]: https://pypi.org/
+project/sdmx2json-ld
```

