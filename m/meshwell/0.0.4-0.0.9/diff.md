# Comparing `tmp/meshwell-0.0.4.tar.gz` & `tmp/meshwell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshwell-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meshwell-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meshwell-0.0.4.tar` & `meshwell-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-07-17 23:34:56.292923 meshwell-0.0.4/LICENSE
--rw-r--r--   0        0        0     2927 2023-07-17 23:34:56.292923 meshwell-0.0.4/README.md
--rw-r--r--   0        0        0      137 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/__init__.py
--rw-r--r--   0        0        0      465 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/config.py
--rw-r--r--   0        0        0     1608 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/gmsh_entity.py
--rw-r--r--   0        0        0     1315 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/labeledentity.py
--rw-r--r--   0        0        0    11397 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/model.py
--rw-r--r--   0        0        0     2180 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/polysurface.py
--rw-r--r--   0        0        0     5694 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/prism.py
--rw-r--r--   0        0        0      715 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/refinement.py
--rw-r--r--   0        0        0     2220 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/tag.py
--rw-r--r--   0        0        0      527 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/validation.py
--rw-r--r--   0        0        0     3235 2023-07-17 23:34:56.296923 meshwell-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4384 1970-01-01 00:00:00.000000 meshwell-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 16:49:43.722288 meshwell-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2927 2023-07-25 16:49:43.722288 meshwell-0.0.9/README.md
+-rw-r--r--   0        0        0      137 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/config.py
+-rw-r--r--   0        0        0     1608 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/gmsh_entity.py
+-rw-r--r--   0        0        0     1315 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/labeledentity.py
+-rw-r--r--   0        0        0    11952 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/model.py
+-rw-r--r--   0        0        0     2180 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/polysurface.py
+-rw-r--r--   0        0        0     5694 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/prism.py
+-rw-r--r--   0        0        0      715 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/refinement.py
+-rw-r--r--   0        0        0     3503 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/samples/001_device.py
+-rw-r--r--   0        0        0     1744 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/tag.py
+-rw-r--r--   0        0        0      527 2023-07-25 16:49:43.730288 meshwell-0.0.9/meshwell/validation.py
+-rw-r--r--   0        0        0     3247 2023-07-25 16:49:43.730288 meshwell-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 meshwell-0.0.9/PKG-INFO
```

### Comparing `meshwell-0.0.4/LICENSE` & `meshwell-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/README.md` & `meshwell-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/gmsh_entity.py` & `meshwell-0.0.9/meshwell/gmsh_entity.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/labeledentity.py` & `meshwell-0.0.9/meshwell/labeledentity.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/model.py` & `meshwell-0.0.9/meshwell/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,16 +133,18 @@
         resolutions: Optional[Dict] = None,
         default_characteristic_length: float = 0.5,
         global_scaling: float = 1.0,
         global_2D_algorithm: int = 6,
         global_3D_algorithm: int = 1,
         filename: Optional[str] = None,
         verbosity: Optional[int] = 0,
+        progress_bars: bool = True,
         interface_delimiter: str = "___",
         boundary_delimiter: str = "None",
+        gmsh_version: Optional[float] = None,
         finalize: bool = True,
     ):
         """Creates a GMSH mesh with proper physical tagging from a dict of {labels: list( (GMSH entity dimension, GMSH entity tag) )}.
 
         Args:
             entities_dict: OrderedDict of key: physical name, and value: meshwell entity
             resolutions (Dict): Pairs {"physical name": {"resolution": float, "distance": "float}}
@@ -150,49 +152,60 @@
             global_scaling: factor to scale all mesh coordinates by (e.g. 1E-6 to go from um to m)
             global_2D_algorithm: gmsh surface default meshing algorithm, see https://gmsh.info/doc/texinfo/gmsh.html#Mesh-options
             global_3D_algorithm: gmsh volume default meshing algorithm, see https://gmsh.info/doc/texinfo/gmsh.html#Mesh-options
             filename (str, path): if True, filepath where to save the mesh
             verbosity: GMSH stdout while meshing (True or False)
             interface_delimiter: string characters to use when naming interfaces between entities
             boundary_delimiter: string characters to use when defining an interface between an entity and nothing (simulation boundary)
+            gmsh_version: Gmsh mesh format version. For example, Palace requires an older version of 2.2,
+                see https://mfem.org/mesh-formats/#gmsh-mesh-formats.
             finalize: if True (default), finalizes the GMSH model after execution
 
         Returns:
-            meshio object with mesh information
+            meshio object with mWesh information
         """
         resolutions = resolutions if resolutions else {}
         gmsh.option.setNumber("General.Terminal", verbosity)  # 1 verbose, 0 otherwise
         gmsh.option.setNumber(
             "Mesh.CharacteristicLengthMax", default_characteristic_length
         )
         gmsh.option.setNumber("Mesh.Algorithm", global_2D_algorithm)
         gmsh.option.setNumber("Mesh.Algorithm3D", global_3D_algorithm)
+        if gmsh_version is not None:
+            gmsh.option.setNumber("Mesh.MshFileVersion", gmsh_version)
 
         # Initial synchronization
         self.occ.synchronize()
 
         # Parse strutural and boundary entities
         full_entities_dict = OrderedDict()
+        keep = True
+        for key, value in entities_dict.items():
+            full_entities_dict[key] = (value, keep)
         keep = False
         if boundaries_dict is not None:
             for key, value in boundaries_dict.items():
                 full_entities_dict[key] = (value, keep)
-        keep = True
-        for key, value in entities_dict.items():
-            full_entities_dict[key] = (value, keep)
 
         # Preserve ID numbering
         gmsh.option.setNumber("Geometry.OCCBooleanPreserveNumbering", 1)
 
         # Main loop:
         # Iterate through OrderedDict of entities, generating and logging the volumes/surfaces in order
         # Manually remove intersections so that BooleanFragments from removeAllDuplicates does not reassign entity tags
         final_entity_list = []
         max_dim = 0
-        for index, (label, (entity_obj, keep)) in enumerate(full_entities_dict.items()):
+
+        enumerator = enumerate(full_entities_dict.items())
+        if progress_bars:
+            from tqdm import tqdm
+
+            enumerator = tqdm(list(enumerator))
+
+        for index, (label, (entity_obj, keep)) in enumerator:
             # First create the shape
             dimtags_out = entity_obj.instanciate()
 
             # Parse dimension
             dim = validate_dimtags(dimtags_out)
             max_dim = max(dim, max_dim)
             dimtags = unpack_dimtags(dimtags_out)
@@ -227,15 +240,16 @@
                     # Heal interfaces now that there are no volume conflicts
                     self.occ.removeAllDuplicates()
                     self.sync_model()
                     # Make sure the most up-to-date surfaces are logged as boundaries
                     previous_entities.update_boundaries()
                 current_entities.dimtags = list(set(current_dimtags_cut))
             current_entities.update_boundaries()
-            final_entity_list.append(current_entities)
+            if current_entities.dimtags:
+                final_entity_list.append(current_entities)
 
         # Tag entities, interfaces, and boundaries
         tag_entities(final_entity_list)
         final_entity_list = tag_interfaces(
             final_entity_list, max_dim, interface_delimiter
         )
         tag_boundaries(
```

### Comparing `meshwell-0.0.4/meshwell/polysurface.py` & `meshwell-0.0.9/meshwell/polysurface.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/prism.py` & `meshwell-0.0.9/meshwell/prism.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/refinement.py` & `meshwell-0.0.9/meshwell/refinement.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/meshwell/tag.py` & `meshwell-0.0.9/meshwell/tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,32 +22,19 @@
         else:
             common_interfaces = list(
                 set(entity1.boundaries).intersection(entity2.boundaries)
             )
             # Remember which boundaries were interfaces with another entity
             entity1.interfaces.extend(common_interfaces)
             entity2.interfaces.extend(common_interfaces)
-            if entity1.keep is False:
-                gmsh.model.addPhysicalGroup(
-                    max_dim - 1,
-                    common_interfaces,
-                    name=f"{entity1.label}",
-                )
-            elif entity2.keep is False:
-                gmsh.model.addPhysicalGroup(
-                    max_dim - 1,
-                    common_interfaces,
-                    name=f"{entity2.label}",
-                )
-            else:
-                gmsh.model.addPhysicalGroup(
-                    max_dim - 1,
-                    common_interfaces,
-                    name=f"{entity1.label}{boundary_delimiter}{entity2.label}",
-                )
+            gmsh.model.addPhysicalGroup(
+                max_dim - 1,
+                common_interfaces,
+                name=f"{entity1.label}{boundary_delimiter}{entity2.label}",
+            )
 
     return entity_list
 
 
 def tag_boundaries(entity_list, max_dim, boundary_delimiter, mesh_edge_name):
     """Adds physical labels to the boundaries of the entities in entity_list."""
     for entity in entity_list:
```

### Comparing `meshwell-0.0.4/meshwell/validation.py` & `meshwell-0.0.9/meshwell/validation.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.4/pyproject.toml` & `meshwell-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version="0.0.4"
+version="0.0.9"
 authors = [
     {name = "Simon Bilodeau", email = "sb30@princeton.edu"},
 ]
 keywords = ["python"]
 license = {file = "LICENSE"}
 dependencies = [
     "shapely",
     "gmsh",
-    "meshio"
+    "meshio",
+    "tqdm"
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov"]
 dev = [
```

### Comparing `meshwell-0.0.4/PKG-INFO` & `meshwell-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: meshwell
-Version: 0.0.4
+Version: 0.0.9
 Summary: GMSH wrapper, with integrated photonics focus
 Keywords: python
 Author-email: Simon Bilodeau <sb30@princeton.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Dist: shapely
 Requires-Dist: gmsh
 Requires-Dist: meshio
+Requires-Dist: tqdm
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: autodoc_pydantic ; extra == "docs"
 Requires-Dist: jupytext ; extra == "docs"
```

