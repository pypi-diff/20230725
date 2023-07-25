# Comparing `tmp/pydantic_neo4j-0.3.5.tar.gz` & `tmp/pydantic_neo4j-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.3.5.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.3.6.tar", max compression
```

## Comparing `pydantic_neo4j-0.3.5.tar` & `pydantic_neo4j-0.3.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      869 2023-07-18 03:47:13.989691 pydantic_neo4j-0.3.5/pydantic_neo4j/__init__.py
--rw-r--r--   0        0        0     5892 2023-07-24 20:16:00.488940 pydantic_neo4j-0.3.5/pydantic_neo4j/create_operations.py
--rw-r--r--   0        0        0     4872 2023-07-18 00:44:33.557638 pydantic_neo4j-0.3.5/pydantic_neo4j/database_operations.py
--rw-r--r--   0        0        0     3371 2023-07-24 19:45:48.667813 pydantic_neo4j-0.3.5/pydantic_neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10443 2023-07-24 20:17:14.093485 pydantic_neo4j-0.3.5/pydantic_neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-18 02:22:59.959087 pydantic_neo4j-0.3.5/pydantic_neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      601 2023-07-24 20:50:58.209625 pydantic_neo4j-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4039 2023-07-18 03:47:13.985687 pydantic_neo4j-0.3.5/README.md
--rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pydantic_neo4j-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      869 2023-07-18 03:47:13.989691 pydantic_neo4j-0.3.6/pydantic_neo4j/__init__.py
+-rw-r--r--   0        0        0     5860 2023-07-25 01:36:45.211076 pydantic_neo4j-0.3.6/pydantic_neo4j/create_operations.py
+-rw-r--r--   0        0        0     4872 2023-07-18 00:44:33.557638 pydantic_neo4j-0.3.6/pydantic_neo4j/database_operations.py
+-rw-r--r--   0        0        0     3421 2023-07-25 01:31:09.201465 pydantic_neo4j-0.3.6/pydantic_neo4j/graph_base_models.py
+-rw-r--r--   0        0        0    10935 2023-07-25 01:41:16.724145 pydantic_neo4j-0.3.6/pydantic_neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-18 02:22:59.959087 pydantic_neo4j-0.3.6/pydantic_neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      601 2023-07-25 01:42:53.443860 pydantic_neo4j-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4039 2023-07-18 03:47:13.985687 pydantic_neo4j-0.3.6/README.md
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pydantic_neo4j-0.3.6/PKG-INFO
```

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/__init__.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/create_operations.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/create_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,22 +86,21 @@
             eager_result = await self.database_operations.run_query(query)
             result = eager_result.records[0].data()
             return self.str_to_class(model=model.__class__, **result["n"])
 
     async def match_or_create_node(
         self, model: NodeModel
     ) -> tuple[uuid.UUID, NodeModel]:
-        print(model)
+
         existing_node = await self.match_utilities.node_query(
             node_name=model.__class__.__name__,
             criteria=model.get_required_fields(),
             statement="MATCH",
         )
-        print(model.get_required_fields())
-        print(f"Existing: {existing_node}  ")
+
         if len(existing_node) == 0:
             new_node = await self.create_node(model=model)
             return new_node.graph_id, new_node
         elif len(existing_node) == 1:
             for key, value in existing_node.items():
                 existing_node_id = key
                 existing_node = value
@@ -112,23 +111,24 @@
     async def create_relationship(self, relationship: RelationshipModel):
         start_node_id, start_node = await self.match_or_create_node(
             model=relationship.start_node
         )
         end_node_id, end_node = await self.match_or_create_node(
             model=relationship.end_node
         )
-
+        print(relationship.get_required_fields())
         rel_exists = await self.match_utilities.relationship_query(
             start_node_name=start_node.__class__.__name__,
             start_criteria={"graph_id": start_node_id},
             end_node_name=end_node.__class__.__name__,
             end_criteria={"graph_id": end_node_id},
             relationship_name=relationship.__class__.__name__,
             relationship_criteria=relationship.get_required_fields(),
         )
+        #print(rel_exists)
 
         if len(rel_exists) > 0:
             # todo: make new exceptions
             raise AttributeError(
                 f"Relationship already exists: {rel_exists}"
             )
         else:
```

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/database_operations.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/database_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/graph_base_models.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/graph_base_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __eq__(self, other):
         return self.node_id == other.node_id
 
     def get_required_fields(self) -> Dict[str, Any]:
         """Fields needed for minimum compatibility between create and match modules"""
         fields = {}
         for field, value in self.__class__.model_fields.items():
-            if value.is_required():
+            if value.is_required() and field != "start_node" and field != "end_node":
                 fields[field] = getattr(self, field)
         return fields
 
     def get_identifying_fields(self) -> Dict[str, Union[uuid.UUID]]:
         fields = {}
         for field, value in self.__class__.model_fields.items():
             if value.annotation == uuid.UUID or value.annotation == Optional[uuid.UUID]:
```

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/match_operations.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/match_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,26 +201,35 @@
                                  start_node_name: str = "",
                                  start_criteria: dict = None,
                                  end_node_name: str = "",
                                  end_criteria: dict = None,
                                  relationship_name: str = "",
                                  relationship_criteria: dict = None
                                  ) -> dict[uuid.UUID, RelationshipModel]:
-        start_node = SequenceCriteriaNodeModel(name=start_node_name, criteria=start_criteria, include_with_return=True)
-        end_node = SequenceCriteriaNodeModel(name=end_node_name, criteria=end_criteria, include_with_return=True)
-        relationship_model = SequenceCriteriaRelationshipModel(name=relationship_name, criteria=relationship_criteria)
+        start_node = SequenceCriteriaNodeModel(name=start_node_name,
+                                               criteria=start_criteria,
+                                               include_with_return=True)
+        end_node = SequenceCriteriaNodeModel(name=end_node_name,
+                                             criteria=end_criteria,
+                                             include_with_return=True)
+        relationship_model = SequenceCriteriaRelationshipModel(name=relationship_name,
+                                                               criteria=relationship_criteria,
+                                                               include_with_return=True)
         sequence_query = SequenceQueryModel(node_sequence=[start_node, end_node],
                                             relationship_sequence=[relationship_model])
         sequence_query_string = MatchUtilities.build_sequence_query_string(sequence_query=sequence_query,
                                                                            keyword='MATCH')
+        print(sequence_query_string)
         eager_result = await self.database_operations.run_query(sequence_query_string)
         rel_models = {}
         for record in eager_result.records:
             for element in record:
-                if type(element) == neo4j.graph.Relationship:
+                print(f"element: {element}")
+                if type(element) != neo4j.graph.Node and type(element) != neo4j.graph.Path:
+                    print(element)
                     try:
                         rel_model = self.get_relationship_model(element)
                         if rel_model.graph_id not in rel_models:
                             rel_models[rel_model.graph_id] = rel_model
                     except Exception as e:
                         print(f"Relationship add Error: {e}")
         #print(rel_models)
```

### Comparing `pydantic_neo4j-0.3.5/pydantic_neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.3.6/pydantic_neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.5/pyproject.toml` & `pydantic_neo4j-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
```

### Comparing `pydantic_neo4j-0.3.5/README.md` & `pydantic_neo4j-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.3.5/PKG-INFO` & `pydantic_neo4j-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
```

