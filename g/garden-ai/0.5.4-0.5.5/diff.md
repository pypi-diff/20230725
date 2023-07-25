# Comparing `tmp/garden_ai-0.5.4.tar.gz` & `tmp/garden_ai-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.5.4.tar", max compression
+gzip compressed data, was "garden_ai-0.5.5.tar", max compression
```

## Comparing `garden_ai-0.5.4.tar` & `garden_ai-0.5.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-07-24 14:46:38.901248 garden_ai-0.5.4/LICENSE
--rw-r--r--   0        0        0      797 2023-07-24 14:46:38.901248 garden_ai-0.5.4/README.md
--rw-r--r--   0        0        0      418 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/__main__.py
--rw-r--r--   0        0        0     4454 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/_model.py
--rw-r--r--   0        0        0      180 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/console.py
--rw-r--r--   0        0        0    11506 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/main.py
--rw-r--r--   0        0        0     5227 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/model.py
--rw-r--r--   0        0        0    16109 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0     4002 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/backend_client.py
--rw-r--r--   0        0        0    27068 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/client.py
--rw-r--r--   0        0        0      440 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/constants.py
--rw-r--r--   0        0        0     9394 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/datacite.py
--rw-r--r--   0        0        0     1068 2023-07-24 14:46:38.901248 garden_ai-0.5.4/garden_ai/garden_file_adapter.py
--rw-r--r--   0        0        0    14824 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2802 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0      798 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7553 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/local_data.py
--rw-r--r--   0        0        0    10014 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/mlmodel.py
--rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/model_file_transfer/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/model_file_transfer/upload.py
--rw-r--r--   0        0        0    21228 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10745 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/steps.py
--rw-r--r--   0        0        0     2019 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     5797 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0      627 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0     8533 2023-07-24 14:46:38.905248 garden_ai-0.5.4/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2903 2023-07-24 14:46:52.973315 garden_ai-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 garden_ai-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-25 18:56:05.577616 garden_ai-0.5.5/LICENSE
+-rw-r--r--   0        0        0      797 2023-07-25 18:56:05.577616 garden_ai-0.5.5/README.md
+-rw-r--r--   0        0        0      418 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/__main__.py
+-rw-r--r--   0        0        0     4454 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/_model.py
+-rw-r--r--   0        0        0      180 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/main.py
+-rw-r--r--   0        0        0     5227 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/model.py
+-rw-r--r--   0        0        0    16109 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     4002 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    27049 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/client.py
+-rw-r--r--   0        0        0      440 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/datacite.py
+-rw-r--r--   0        0        0     1068 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/garden_file_adapter.py
+-rw-r--r--   0        0        0    15819 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0      798 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1404 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/local_data.py
+-rw-r--r--   0        0        0    10013 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    22709 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10745 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     5797 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0      627 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0     8533 2023-07-25 18:56:05.581616 garden_ai-0.5.5/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2951 2023-07-25 18:56:18.309511 garden_ai-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 garden_ai-0.5.5/PKG-INFO
```

### Comparing `garden_ai-0.5.4/LICENSE` & `garden_ai-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/README.md` & `garden_ai-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/_model.py` & `garden_ai-0.5.5/garden_ai/_model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/app/console.py` & `garden_ai-0.5.5/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/app/garden.py` & `garden_ai-0.5.5/garden_ai/app/garden.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/app/main.py` & `garden_ai-0.5.5/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/app/model.py` & `garden_ai-0.5.5/garden_ai/app/model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/app/pipeline.py` & `garden_ai-0.5.5/garden_ai/app/pipeline.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/backend_client.py` & `garden_ai-0.5.5/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/client.py` & `garden_ai-0.5.5/garden_ai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     stage_model_for_upload,
 )
 from garden_ai.model_file_transfer.upload import upload_mlmodel_to_s3
 from garden_ai.pipelines import Pipeline, RegisteredPipeline, Paper, Repository
 from garden_ai.steps import step
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
+
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
 
 COMPUTE_RESOURCE_SERVER_NAME = "funcx_service"
 
@@ -460,15 +461,14 @@
 
         Raises
         ------
         PipelineNotFoundException
             Raised when no known pipeline exists with the given identifier.
         """
         data = dict(kwargs)
-        print(data)
         if doi:
             data["doi"] = doi
         if url:
             data["url"] = url
         if repo_name:
             data["repo_name"] = repo_name
         pipeline = local_data.get_local_pipeline_by_doi(doi)
```

### Comparing `garden_ai-0.5.4/garden_ai/datacite.py` & `garden_ai-0.5.5/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/garden_file_adapter.py` & `garden_ai-0.5.5/garden_ai/garden_file_adapter.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/gardens.py` & `garden_ai-0.5.5/garden_ai/gardens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import logging
 from datetime import datetime
 from typing import Any, Dict, List, Optional, cast
 
+from tabulate import tabulate
 from pydantic import (
     BaseModel,
     Field,
     PrivateAttr,
     ValidationError,
     root_validator,
     validator,
@@ -151,14 +152,41 @@
         """
         names = []
         for pipeline in self.pipelines:
             name = self.pipeline_aliases.get(pipeline.short_name) or pipeline.short_name
             names += [name]
         return names
 
+    def _repr_html_(self) -> str:
+        style = "<style>th {text-align: left;}</style>"
+        title = f"<h2>{self.title}</h2>"
+        details = f"<p>Authors: {', '.join(self.authors)}<br>DOI: {self.doi}</p>"
+        pipelines = "<h3>Pipelines</h3>" + tabulate(
+            [
+                {
+                    key.title(): str(getattr(pipeline, key))
+                    for key in ("title", "authors", "doi")
+                }
+                for pipeline in self.pipelines
+            ],
+            headers="keys",
+            tablefmt="html",
+        )
+        optional = "<h3>Additional data</h3>" + tabulate(
+            [
+                (field, val)
+                for field, val in self.dict().items()
+                if field not in ("title", "authors", "doi")
+                and "pipeline" not in field
+                and val
+            ],
+            tablefmt="html",
+        )
+        return style + title + details + pipelines + optional
+
     def _set_pipelines_from_remote_metadata(self, pipeline_metadata: List[dict]):
         """
         Given a list of dicts in RegisteredPipeline format (as from Globus Search),
         attempt to convert them to RegisteredPipelines and use them to populate _pipelines.
         """
         pipelines = []
         for meta in pipeline_metadata:
```

### Comparing `garden_ai-0.5.4/garden_ai/globus_compute/containers.py` & `garden_ai-0.5.5/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.5.5/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/globus_search/garden_search.py` & `garden_ai-0.5.5/garden_ai/globus_search/garden_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import json
 
 from garden_ai.gardens import Garden
 from globus_sdk import SearchClient, GlobusAPIError
 from pydantic import ValidationError
+from rich.traceback import install
 
 # garden-dev index
 GARDEN_INDEX_UUID = "58e4df29-4492-4e7d-9317-b27eba62a911"
 
+install()
+
 
 class RemoteGardenException(Exception):
     """Exception raised when a requested Garden cannot be found or published"""
 
+    pass
+
 
 def get_remote_garden_by_doi(doi: str, search_client: SearchClient) -> Garden:
     try:
         res = search_client.get_subject(GARDEN_INDEX_UUID, doi)
     except GlobusAPIError as e:
-        if e.code == 404:
-            raise RemoteGardenException(
-                f"Could not reach find garden with id {doi}"
-            ) from e
+        if e.http_status == 404:
+            raise RemoteGardenException(f"Could not find Garden with doi {doi}") from e
         else:
             raise RemoteGardenException(
-                f"Could not reach index {GARDEN_INDEX_UUID}"
+                f"Could not reach Globus Search Index {GARDEN_INDEX_UUID}"
             ) from e
     try:
         garden_meta = json.loads(res.text)["entries"][0]["content"]
         garden = Garden(**garden_meta)
     except (ValueError, KeyError, IndexError, ValidationError) as e:
         raise RemoteGardenException(
             f"Could not parse search response {res.text}"
```

### Comparing `garden_ai-0.5.4/garden_ai/local_data.py` & `garden_ai-0.5.5/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/mlmodel.py` & `garden_ai-0.5.5/garden_ai/mlmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import pathlib
 import pickle
 import shutil
 from enum import Enum
 from typing import Optional
 import functools
-
 import mlflow  # type: ignore
 from pydantic import BaseModel, Field, validator
 
 from garden_ai import GardenConstants
 from garden_ai._model import _Model
```

### Comparing `garden_ai-0.5.4/garden_ai/model_file_transfer/upload.py` & `garden_ai-0.5.5/garden_ai/model_file_transfer/upload.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/pipelines.py` & `garden_ai-0.5.5/garden_ai/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from uuid import UUID
 
 import dparse  # type: ignore
 import globus_compute_sdk  # type: ignore
 from packaging.requirements import InvalidRequirement, Requirement
 from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 from pydantic.dataclasses import dataclass
+from tabulate import tabulate
 
 import garden_ai
 from garden_ai.app.console import console
 from garden_ai.constants import GardenConstants
 from garden_ai.datacite import (
     Contributor,
     Creator,
@@ -63,15 +64,15 @@
     url: str = Field(...)
     contributors: List[str] = Field(default_factory=list)
 
 
 class Paper(BaseModel):
     """
     The `Paper` class represents all the metadata we want to \
-    publically expose about the papers used to build the pipeline.
+    publically expose about the paper used to build the pipeline.
 
     Attributes:
         title (str):
             The official title that the paper can be referenced by.
         authors List[str]:
             The main researchers involved in producing the paper. Personal name \
             format should be: "Family, Given". Order is preserved. (at least one required)
@@ -245,14 +246,17 @@
 
         if not any(req.startswith("mlflow") for req in pip_deps):
             pip_deps += [f"mlflow-skinny=={mlflow.__version__}"]
         if not any(req.startswith("pandas") for req in pip_deps):
             pip_deps += ["pandas<3"]
         return pip_deps
 
+    def _repr_html_(self) -> str:
+        return pipeline_repr_html(self)
+
     def _collect_requirements(self):
         """collect requirements to pass to Globus Compute container service.
 
         Populates attributes `self.python_version, self.pip_dependencies, self.conda_dependencies` per
         `self.requirements_file`, as well as `self.model_full_names` from steps' metadata.
         """
         # collect explicit pipeline dependencies for the container
@@ -492,14 +496,17 @@
         # note: we want every RegisteredPipeline to be re-constructible
         # from mere json, so as a sanity check we use pipeline.json() instead of
         # pipeline.dict() directly
         record = pipeline.json()
         data = json.loads(record)
         return cls(**data)
 
+    def _repr_html_(self) -> str:
+        return pipeline_repr_html(self)
+
     def collect_models(self) -> List[ModelMetadata]:
         """Collect the RegisteredModel objects that are present in the local DB corresponding to this Pipeline's list of `model_full_names`."""
         from .local_data import get_local_model_by_name
 
         models = []
         for model_name in self.model_full_names:
             model = get_local_model_by_name(model_name)
@@ -524,7 +531,46 @@
 
         Returns:
             ``RegisteredPipeline`` metadata dict augmented with a list of ``RegisteredModel`` metadata
         """
         data = self.dict()
         data["models"] = [m.dict() for m in self.collect_models()]
         return data
+
+
+def pipeline_repr_html(pipeline: Union[Pipeline, RegisteredPipeline]) -> str:
+    def prettify_type_repr(s: str) -> str:
+        if "<" in s:
+            return s[s.find("<class '") + 8 : s.rfind("'")]
+        return s
+
+    style = "<style>th {text-align: left;}</style>"
+    title = f"<h2>{pipeline.title}</h2>"
+    details = f"<p>Authors: {', '.join(pipeline.authors)}<br>DOI: {pipeline.doi}</p>"
+    steps = "<h3>Steps</h3>" + tabulate(
+        [
+            {
+                key.title(): prettify_type_repr(
+                    # handle both Pipelines and RegisteredPipelines
+                    str(getattr(step, key) if isinstance(step, Step) else step[key])
+                )
+                for key in (
+                    "title",
+                    "model_full_names",
+                    "input_info",
+                    "output_info",
+                )
+            }
+            for step in pipeline.steps
+        ],
+        headers="keys",
+        tablefmt="html",
+    )
+    optional = "<h3>Additional data</h3>" + tabulate(
+        [
+            (field, val)
+            for field, val in pipeline.dict().items()
+            if field not in ("title", "authors", "doi", "steps") and val
+        ],
+        tablefmt="html",
+    )
+    return style + title + details + steps + optional
```

### Comparing `garden_ai-0.5.4/garden_ai/steps.py` & `garden_ai-0.5.5/garden_ai/steps.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/templates/pipeline` & `garden_ai-0.5.5/garden_ai/templates/pipeline`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/utils/_meta.py` & `garden_ai-0.5.5/garden_ai/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/utils/filesystem.py` & `garden_ai-0.5.5/garden_ai/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/garden_ai/utils/misc.py` & `garden_ai-0.5.5/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.4/pyproject.toml` & `garden_ai-0.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.5.4" # placeholder
+version = "0.5.5" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -39,14 +39,16 @@
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
 globus-compute-sdk = "^2.2.0"
+tabulate = "^0.9.0"
+types-tabulate = "^0.9.0.3"
 # Be sure to add additional flavors as optional below as support is added and update tool.poetry.extras
 torch = { version = "^2.0.0, !=2.0.1", optional = true }
 tensorflow = { version = "^2.11.0", optional = true, python = ">=3.8,<3.12" }
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
```

### Comparing `garden_ai-0.5.4/PKG-INFO` & `garden_ai-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.5.4
+Version: 0.5.5
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -26,17 +26,19 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mlflow (>=2.4.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
 Requires-Dist: torch (>=2.0.0,<3.0.0,!=2.0.1) ; extra == "torch" or extra == "all"
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: types-tabulate (>=0.9.0.3,<0.10.0.0)
 Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
 
 [![NSF-2209892](https://img.shields.io/badge/NSF-2209892-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209892&HistoricalAwards=false)
```

