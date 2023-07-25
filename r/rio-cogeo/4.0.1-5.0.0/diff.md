# Comparing `tmp/rio_cogeo-4.0.1.tar.gz` & `tmp/rio_cogeo-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_cogeo-4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rio_cogeo-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio_cogeo-4.0.1.tar` & `rio_cogeo-5.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      213 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1172 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/.gitignore
--rw-r--r--   0        0        0      799 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1517 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/LICENSE
--rw-r--r--   0        0        0     3373 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/README.md
--rw-r--r--   0        0        0     2329 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      218 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/__init__.py
--rw-r--r--   0        0        0    28480 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/cogeo.py
--rw-r--r--   0        0        0      406 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/errors.py
--rw-r--r--   0        0        0     1950 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/models.py
--rw-r--r--   0        0        0     4521 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/profiles.py
--rw-r--r--   0        0        0       21 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/scripts/__init__.py
--rw-r--r--   0        0        0    13775 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/scripts/cli.py
--rw-r--r--   0        0        0     4615 2023-07-11 06:52:37.883419 rio_cogeo-4.0.1/rio_cogeo/utils.py
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 rio_cogeo-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-07-25 15:31:26.175768 rio_cogeo-5.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-07-25 15:31:26.175768 rio_cogeo-5.0.0/.gitignore
+-rw-r--r--   0        0        0      799 2023-07-25 15:31:26.175768 rio_cogeo-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1517 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/LICENSE
+-rw-r--r--   0        0        0     3373 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/README.md
+-rw-r--r--   0        0        0     2329 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/__init__.py
+-rw-r--r--   0        0        0    28480 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/cogeo.py
+-rw-r--r--   0        0        0      406 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/errors.py
+-rw-r--r--   0        0        0     2017 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/models.py
+-rw-r--r--   0        0        0     4521 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/profiles.py
+-rw-r--r--   0        0        0       21 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/scripts/__init__.py
+-rw-r--r--   0        0        0    13786 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/scripts/cli.py
+-rw-r--r--   0        0        0     4615 2023-07-25 15:31:26.179768 rio_cogeo-5.0.0/rio_cogeo/utils.py
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 rio_cogeo-5.0.0/PKG-INFO
```

### Comparing `rio_cogeo-4.0.1/.gitignore` & `rio_cogeo-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/.pre-commit-config.yaml` & `rio_cogeo-5.0.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     rev: v0.991
     hooks:
       - id: mypy
         language_version: python
         # No reason to run if only tests have changed. They intentionally break typing.
         exclude: tests/.*
         additional_dependencies:
-          - pydantic~=1.0
+          - pydantic~=2.0
```

### Comparing `rio_cogeo-4.0.1/LICENSE` & `rio_cogeo-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/README.md` & `rio_cogeo-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/pyproject.toml` & `rio_cogeo-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "click>=7.0",
     "rasterio>=1.3.3",
     "numpy~=1.15",
-    "morecantile>=4.0,<5.0",
-    "pydantic~=1.0",
+    "morecantile>=5.0,<6.0",
+    "pydantic~=2.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "cogdumper",
```

### Comparing `rio_cogeo-4.0.1/rio_cogeo/cogeo.py` & `rio_cogeo-5.0.0/rio_cogeo/cogeo.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/rio_cogeo/profiles.py` & `rio_cogeo-5.0.0/rio_cogeo/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/rio_cogeo/scripts/cli.py` & `rio_cogeo-5.0.0/rio_cogeo/scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
     help="GDAL configuration options.",
 )
 def info(input, to_json, config):  # noqa: C901
     """Dataset info."""
     metadata = cog_info(input, config=config)
 
     if to_json:
-        click.echo(metadata.json(exclude_none=True, by_alias=True))
+        click.echo(metadata.model_dump_json(exclude_none=True, by_alias=True))
     else:
 
         sep = 25
         click.echo(
             f"""{click.style('Driver:', bold=True)} {metadata.Driver}
 {click.style('File:', bold=True)} {metadata.Path}
 {click.style('COG:', bold=True)} {metadata.COG}
```

### Comparing `rio_cogeo-4.0.1/rio_cogeo/utils.py` & `rio_cogeo-5.0.0/rio_cogeo/utils.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-4.0.1/PKG-INFO` & `rio_cogeo-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-cogeo
-Version: 4.0.1
+Version: 5.0.0
 Summary: Cloud Optimized GeoTIFF (COGEO) creation plugin for rasterio
 Keywords: COGEO,CloudOptimized Geotiff,rasterio
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: click>=7.0
 Requires-Dist: rasterio>=1.3.3
 Requires-Dist: numpy~=1.15
-Requires-Dist: morecantile>=4.0,<5.0
-Requires-Dist: pydantic~=1.0
+Requires-Dist: morecantile>=5.0,<6.0
+Requires-Dist: pydantic~=2.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: cogdumper ; extra == "test"
 Project-URL: Documentation, https://cogeotiff.github.io/rio-cogeo/
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: rio-cogeo Version: 4.0.1 Summary: Cloud Optimized
+Metadata-Version: 2.1 Name: rio-cogeo Version: 5.0.0 Summary: Cloud Optimized
 GeoTIFF (COGEO) creation plugin for rasterio Keywords: COGEO,CloudOptimized
 Geotiff,rasterio Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: click>=7.0 Requires-Dist:
-rasterio>=1.3.3 Requires-Dist: numpy~=1.15 Requires-Dist: morecantile>=4.0,<5.0
-Requires-Dist: pydantic~=1.0 Requires-Dist: pre-commit ; extra == "dev"
+rasterio>=1.3.3 Requires-Dist: numpy~=1.15 Requires-Dist: morecantile>=5.0,<6.0
+Requires-Dist: pydantic~=2.0 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-material ; extra
 == "docs" Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ;
 extra == "test" Requires-Dist: cogdumper ; extra == "test" Project-URL:
 Documentation, https://cogeotiff.github.io/rio-cogeo/ Project-URL: Source,
 https://github.com/cogeotiff/rio-cogeo Provides-Extra: dev Provides-Extra: docs
 Provides-Extra: test # rio-cogeo
                                      [COG]
```

