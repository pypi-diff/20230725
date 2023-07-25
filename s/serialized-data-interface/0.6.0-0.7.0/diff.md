# Comparing `tmp/serialized_data_interface-0.6.0.tar.gz` & `tmp/serialized_data_interface-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialized_data_interface-0.6.0.tar", max compression
+gzip compressed data, was "serialized_data_interface-0.7.0.tar", max compression
```

## Comparing `serialized_data_interface-0.6.0.tar` & `serialized_data_interface-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-03-20 12:37:48.518112 serialized_data_interface-0.6.0/LICENSE
--rw-r--r--   0        0        0     1681 2023-03-20 12:37:48.518246 serialized_data_interface-0.6.0/README.md
--rw-r--r--   0        0        0     1220 2023-03-21 12:15:55.875706 serialized_data_interface-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      592 2023-03-20 12:37:48.518571 serialized_data_interface-0.6.0/serialized_data_interface/__init__.py
--rw-r--r--   0        0        0     7318 2023-03-20 12:37:48.518765 serialized_data_interface-0.6.0/serialized_data_interface/errors.py
--rw-r--r--   0        0        0      904 2023-03-20 12:37:48.518917 serialized_data_interface-0.6.0/serialized_data_interface/events.py
--rw-r--r--   0        0        0     2058 2023-03-20 12:37:48.519065 serialized_data_interface-0.6.0/serialized_data_interface/local_sdi.py
--rw-r--r--   0        0        0    11289 2023-03-20 16:39:48.267583 serialized_data_interface-0.6.0/serialized_data_interface/relation.py
--rw-r--r--   0        0        0    15760 2023-03-20 12:37:48.519520 serialized_data_interface-0.6.0/serialized_data_interface/sdi.py
--rw-r--r--   0        0        0      265 2023-03-20 12:37:48.519641 serialized_data_interface-0.6.0/serialized_data_interface/shims.py
--rw-r--r--   0        0        0     6912 2023-03-20 12:37:48.519814 serialized_data_interface-0.6.0/serialized_data_interface/testing.py
--rw-r--r--   0        0        0     3306 2023-03-20 12:37:48.519986 serialized_data_interface-0.6.0/serialized_data_interface/utils.py
--rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 serialized_data_interface-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-20 12:37:48.518112 serialized_data_interface-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1681 2023-07-25 12:46:48.317445 serialized_data_interface-0.7.0/README.md
+-rw-r--r--   0        0        0     1588 2023-07-25 15:04:57.517029 serialized_data_interface-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      592 2023-07-25 10:45:33.384222 serialized_data_interface-0.7.0/serialized_data_interface/__init__.py
+-rw-r--r--   0        0        0     7318 2023-07-25 10:45:33.384411 serialized_data_interface-0.7.0/serialized_data_interface/errors.py
+-rw-r--r--   0        0        0      904 2023-07-25 10:45:33.384576 serialized_data_interface-0.7.0/serialized_data_interface/events.py
+-rw-r--r--   0        0        0     2090 2023-07-25 10:45:33.384744 serialized_data_interface-0.7.0/serialized_data_interface/local_sdi.py
+-rw-r--r--   0        0        0    11339 2023-07-25 15:04:57.517512 serialized_data_interface-0.7.0/serialized_data_interface/relation.py
+-rw-r--r--   0        0        0    15908 2023-07-25 15:04:57.517918 serialized_data_interface-0.7.0/serialized_data_interface/sdi.py
+-rw-r--r--   0        0        0      265 2023-07-25 10:45:33.385449 serialized_data_interface-0.7.0/serialized_data_interface/shims.py
+-rw-r--r--   0        0        0     6912 2023-07-25 10:45:33.385635 serialized_data_interface-0.7.0/serialized_data_interface/testing.py
+-rw-r--r--   0        0        0     3338 2023-07-25 10:45:33.386138 serialized_data_interface-0.7.0/serialized_data_interface/utils.py
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 serialized_data_interface-0.7.0/PKG-INFO
```

### Comparing `serialized_data_interface-0.6.0/LICENSE` & `serialized_data_interface-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialized_data_interface-0.6.0/README.md` & `serialized_data_interface-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/__init__.py` & `serialized_data_interface-0.7.0/serialized_data_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 # flake8: noqa: ignore=F401
 # type: ignore
 
 # Direct imports for namespaced references.
 from . import errors, relation, testing
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/errors.py` & `serialized_data_interface-0.7.0/serialized_data_interface/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 from typing import List, Set, Union
 
 from ops.model import Application, Relation, Unit
 
 
 class SDIException(Exception):
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/events.py` & `serialized_data_interface-0.7.0/serialized_data_interface/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 from ops.charm import RelationEvent
 from ops.framework import EventSource, ObjectEvents
 
 
 class RelationAvailableEvent(RelationEvent):
     """Event triggered when a relation is ready for requests."""
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/local_sdi.py` & `serialized_data_interface-0.7.0/serialized_data_interface/local_sdi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Canonical Ltd.
 import os
 import sys
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from zipfile import ZIP_DEFLATED, ZipFile
 
 import yaml
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/relation.py` & `serialized_data_interface-0.7.0/serialized_data_interface/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 """Base class for libraries which wrap a relation endpoint with a Python API.
 
 This provides the base for implementing relation libraries which use SDI
 for data validation and de/serialization but provide a Python API on top
 of that for ease of use.
 """
 import logging
 from functools import cached_property
 from pathlib import Path
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 import yaml
 from ops.charm import CharmBase
 from ops.framework import Object
 from ops.model import (
     ActiveStatus,
     Application,
@@ -59,15 +59,15 @@
     ROLE: str
     INTERFACE: str
     SCHEMA: Union[str, dict]
     LIMIT: Union[int, None] = None
 
     on = EndpointWrapperEvents()
 
-    def __init__(self, charm: CharmBase, endpoint: str = None):
+    def __init__(self, charm: CharmBase, endpoint: Optional[str] = None):
         """Constructor for EndpointWrapper.
 
         Args:
             charm: The charm that is instantiating the library.
             endpoint: The name of the relation endpoint to bind to
                 (defaults to the INTERFACE, with any underscores
                 changed to dashes).
@@ -178,15 +178,15 @@
                 # Otherwise, we might just not have seen the versions yet.
                 return WaitingStatus(f"Waiting on relation: {relation.name}")
         elif not self.is_ready(relation):
             return WaitingStatus(f"Waiting on relation: {relation.name}")
         return ActiveStatus()
 
     @cache
-    def is_available(self, relation: Relation = None):
+    def is_available(self, relation: Optional[Relation] = None):
         """Checks whether the given relation, or any relation if not specified, is available.
 
         A given relation is available if the version negotation has succeeded.
         """
         if relation is None:
             return any(self.is_available(relation) for relation in self.relations)
         if relation.app.name == "":  # type: ignore
@@ -197,15 +197,15 @@
             self._sdi.get_version(relation)
         except errors.RelationException:
             return False
         else:
             return True
 
     @cache
-    def is_ready(self, relation: Relation = None):
+    def is_ready(self, relation: Optional[Relation] = None):
         """Checks whether the given relation, or any relation if not specified, is ready.
 
         A given relation is ready if the remote side has sent valid data.
         """
         if relation is None:
             return any(self.is_ready(relation) for relation in self.relations)
         if relation.app.name == "":  # type: ignore
@@ -218,15 +218,15 @@
             return False
         else:
             return any(
                 data[entity] for entity in data if entity not in (self.app, self.unit)
             )
 
     @cache
-    def is_failed(self, relation: Relation = None):
+    def is_failed(self, relation: Optional[Relation] = None):
         """Checks whether the given relation, or any relation if not specified, has an error."""
         if relation is None:
             return any(self.is_failed(relation) for relation in self.relations)
         if relation.app.name == "":  # type: ignore
             # Juju doesn't provide JUJU_REMOTE_APP during relation-broken
             # hooks. See https://github.com/canonical/operator/issues/693
             return False
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/sdi.py` & `serialized_data_interface-0.7.0/serialized_data_interface/sdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Canonical Ltd.
 from functools import cached_property
 from typing import Dict, Optional, Set, Tuple, Union
 
 import jsonschema
 import yaml
 from ops.charm import CharmBase
 from ops.model import Application, Relation, RelationDataContent, Unit
@@ -19,15 +20,15 @@
     def __init__(
         self,
         charm: CharmBase,
         endpoint: str,
         schemas: dict,
         versions: Set[Union[int, str]],
         role: str,
-        ignored_fields: Set[str] = None,
+        ignored_fields: Optional[Set[str]] = None,
     ):
         """Initialize the SDI instance.
 
         Args:
             charm: The charm that this is being used with.
             endpoint: The name of the relation endpoint to use.
             schemas: The mapping of versions to role-entity-schema mappings.
@@ -101,15 +102,15 @@
         Can raise:
             * UnversionedRelation
             * RelationParseError
             * IncompatibleVersionsError
         """
         local_versions = self.versions
         local_versions_parsed = self._parse_versions(local_versions)
-        remote_versions_raw = relation.data[relation.app].get(utils.VERSION_KEY)
+        remote_versions_raw = relation.data[relation.app].get(utils.VERSION_KEY)  # type: ignore
         if not remote_versions_raw:
             raise errors.UnversionedRelation(relation)
         try:
             if not isinstance(remote_versions_raw, str):
                 raise TypeError(f"should be str, not {type(remote_versions_raw)}")
             remote_versions = set(yaml.safe_load(remote_versions_raw))
             remote_versions_parsed = self._parse_versions(remote_versions)
@@ -171,15 +172,15 @@
             rel_data = self.unwrap(relation)
             if rel_data[relation.app]:
                 data[(relation, relation.app)] = rel_data[relation.app]
             if self.unit.is_leader() and rel_data[self.app]:
                 data[(relation, self.app)] = rel_data[self.app]
         return data
 
-    def send_data(self, data: dict, app_name: str = None):
+    def send_data(self, data: dict, app_name: Optional[str] = None):
         """Send data to related app(s).
 
         If `app_name` is given, the data will only be sent to relations with that remote
         application. Otherwise, it will be sent to all relations. Note that this means that
         either the data given has to be compatible with any established relation versions.
         """
         if not app_name:
@@ -200,30 +201,36 @@
             if not relations:
                 raise errors.InvalidAppNameError(self.endpoint, app_name)
         data = {self.app: data}
         for relation in relations:
             self.wrap(relation, data)
 
     def _deserialize_flat(
-        self, relation: Relation, entity: Union[Application, Unit], data: dict
+        self,
+        relation: Relation,
+        entity: Union[Application, Unit],
+        data: RelationDataContent,
     ):
         # Deserialize "flat" schema data, where each field is serliazed directly
         # into the relation data bucket, rather than under a nested "data" field.
         deserialized = {}
         for key, value in data.items():
             if key in self.ignored_fields:
                 continue
             try:
                 deserialized[key] = yaml.safe_load(value)
             except yaml.YAMLError as e:
                 raise errors.RelationParseError(relation, entity, key) from e
         return deserialized
 
     def _deserialize_nested(
-        self, relation: Relation, entity: Union[Application, Unit], data: dict
+        self,
+        relation: Relation,
+        entity: Union[Application, Unit],
+        data: RelationDataContent,
     ):
         # Deserialize "nested" schema data, where all data is serialized under
         # a single "data" key.
         try:
             return yaml.safe_load(data.get("data", "{}"))
         except yaml.YAMLError as e:
             raise errors.RelationParseError(relation, entity, "data") from e
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/testing.py` & `serialized_data_interface-0.7.0/serialized_data_interface/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 # The mixin pattern is difficult to get working with static type checking.
 # type: ignore
 
 from contextlib import contextmanager
 from functools import cached_property
```

### Comparing `serialized_data_interface-0.6.0/serialized_data_interface/utils.py` & `serialized_data_interface-0.7.0/serialized_data_interface/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Canonical Ltd.
 import hashlib
 import os
 import time
 from pathlib import Path
 from zipfile import ZipFile, ZipInfo
 
 import requests
```

### Comparing `serialized_data_interface-0.6.0/PKG-INFO` & `serialized_data_interface-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: serialized-data-interface
-Version: 0.6.0
+Version: 0.7.0
 Summary: Serialized Data Interface for Juju Operators
 Home-page: https://github.com/canonical/serialized-data-interface/
 License: Apache-2.0
 Author: Dominik Fleischmann
 Author-email: dominik.fleischmann@canonical.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: jsonschema
+Requires-Dist: jsonschema (>4,<4.18)
 Requires-Dist: ops
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/canonical/serialized-data-interface/
 Description-Content-Type: text/markdown
 
 # Serialized Data Interface Library
```

