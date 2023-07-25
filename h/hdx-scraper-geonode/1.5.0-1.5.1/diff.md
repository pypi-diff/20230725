# Comparing `tmp/hdx_scraper_geonode-1.5.0.tar.gz` & `tmp/hdx_scraper_geonode-1.5.1.tar.gz`

## Comparing `hdx_scraper_geonode-1.5.0.tar` & `hdx_scraper_geonode-1.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4954 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/documentation/main.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/_version.py
--rwxr-xr-x   0        0        0    18256 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/geonodetohdx.py
--rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/hdx_geonode.yaml
--rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/tests/config/project_configuration.yml
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/tests/fixtures/hdx_geonode.yml
--rwxr-xr-x   0        0        0    43540 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/tests/hdx/scraper/geonode/test_geonodetohdx.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/LICENSE
--rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5290 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/main.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/_version.py
+-rwxr-xr-x   0        0        0    18251 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/geonodetohdx.py
+-rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/hdx_geonode.yaml
+-rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/config/project_configuration.yml
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/fixtures/hdx_geonode.yml
+-rwxr-xr-x   0        0        0    43552 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/hdx/scraper/geonode/test_geonodetohdx.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/LICENSE
+-rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/PKG-INFO
```

### Comparing `hdx_scraper_geonode-1.5.0/CONTRIBUTING.md` & `hdx_scraper_geonode-1.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/requirements.txt` & `hdx_scraper_geonode-1.5.1/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
+annotated-types==0.5.0
+    # via pydantic
+anyio==3.7.1
+    # via httpcore
 attrs==23.1.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
-certifi==2023.5.7
-    # via requests
+certifi==2023.7.22
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via frictionless
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 ckanapi==4.7
     # via hdx-python-api
-click==8.1.3
+click==8.1.6
     # via typer
 colorama==0.4.6
     # via typer
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.1
+cryptography==41.0.2
     # via pyopenssl
 decorator==5.1.1
     # via
     #   jsonpath-ng
     #   validators
 defopt==6.4.0
     # via hdx-python-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
 docutils==0.20.1
     # via defopt
 email-validator==2.0.0.post2
     # via hdx-python-api
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
-frictionless==5.13.1
+frictionless==5.15.10
     # via hdx-python-utilities
-hdx-python-api==6.0.4
+h11==0.14.0
+    # via httpcore
+hdx-python-api==6.0.6
     # via hdx-scraper-geonode (pyproject.toml)
 hdx-python-country==3.5.1
     # via hdx-python-api
 hdx-python-utilities==3.6.1
     # via hdx-python-country
-humanize==4.6.0
+httpcore==0.17.3
+    # via dnspython
+humanize==4.7.0
     # via frictionless
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
+    #   anyio
     #   email-validator
     #   requests
-ijson==3.2.2
+ijson==3.2.3
     # via hdx-python-utilities
-inflect==6.0.4
+inflect==7.0.0
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.2
     # via frictionless
@@ -81,15 +92,15 @@
     # via hdx-python-utilities
 jsonpath-ng==1.5.3
     # via libhxl
 jsonschema==4.17.3
     # via
     #   frictionless
     #   tableschema-to-template
-libhxl==5.0.1
+libhxl==5.0.2
     # via hdx-python-country
 loguru==0.7.0
     # via hdx-python-utilities
 makefun==1.15.1
     # via hdx-python-api
 markdown-it-py==3.0.0
     # via rich
@@ -107,15 +118,15 @@
     # via quantulum3
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.8.0
+platformdirs==3.9.1
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
@@ -125,18 +136,20 @@
     # via hdx-scraper-geonode (pyproject.toml)
 pyasn1==0.5.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pycparser==2.21
     # via cffi
-pydantic==1.10.9
+pydantic==2.0.3
     # via
     #   frictionless
     #   inflect
+pydantic-core==2.3.0
+    # via pydantic
 pygments==2.15.1
     # via rich
 pyopenssl==23.2.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pyphonetics==0.5.3
@@ -158,15 +171,15 @@
 python-io-wrapper==0.3.1
     # via libhxl
 python-slugify==8.0.1
     # via
     #   ckanapi
     #   frictionless
     #   hdx-scraper-geonode (pyproject.toml)
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 quantulum3==0.9.0
     # via hdx-python-api
 ratelimit==2.2.1
@@ -196,46 +209,53 @@
     #   ckanapi
     #   isodate
     #   jsonpath-ng
     #   pockets
     #   python-dateutil
     #   requests-file
     #   sphinxcontrib-napoleon
+sniffio==1.3.0
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 sphinxcontrib-napoleon==0.7
     # via defopt
 stringcase==1.2.0
     # via frictionless
 structlog==23.1.0
     # via libhxl
 tableschema-to-template==0.0.13
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
 typer[all]==0.9.0
     # via frictionless
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   frictionless
+    #   inflect
     #   pydantic
+    #   pydantic-core
     #   typer
 unidecode==1.3.6
     # via
     #   libhxl
     #   pyphonetics
-urllib3==2.0.3
+urllib3==2.0.4
     # via
     #   libhxl
     #   requests
 validators==0.20.0
     # via frictionless
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via pre-commit
-wheel==0.40.0
+wheel==0.41.0
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.1.2
     # via tableschema-to-template
```

### Comparing `hdx_scraper_geonode-1.5.0/.config/pre-commit-config.yaml` & `hdx_scraper_geonode-1.5.1/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/.github/workflows/publish.yaml` & `hdx_scraper_geonode-1.5.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/.github/workflows/run-python-tests.yaml` & `hdx_scraper_geonode-1.5.1/.github/workflows/run-python-tests.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This workflow will install Python dependencies, lint and run tests
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run tests
 
 on:
+  workflow_dispatch: # add run button in github
   push:
     branches-ignore:
       - gh-pages
   pull_request:
     branches-ignore:
       - gh-pages
```

### Comparing `hdx_scraper_geonode-1.5.0/documentation/main.md` & `hdx_scraper_geonode-1.5.1/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/documentation/pydoc-markdown.yaml` & `hdx_scraper_geonode-1.5.1/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/geonodetohdx.py` & `hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/geonodetohdx.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         else:
           - 'internally displaced persons - idp'
 
     Args:
         geonode_url (str): GeoNode server url
         downloader (Download): Download object from HDX Python Utilities
         hdx_geonode_config_yaml (Optional[str]): Configuration file for scraper
+
     """
 
     def __init__(
         self,
         geonode_url: str,
         downloader: Download,
         hdx_geonode_config_yaml: Optional[str] = None,
@@ -152,18 +153,17 @@
         Args:
             use_count (bool): Whether to use null count metadata to exclude countries. Defaults to True.
 
         Returns:
             List[Dict]: List of countries in form (iso3 code, name)
 
         """
-        response = self.downloader.download(
+        jsonresponse = self.downloader.download_json(
             f"{self.geonode_urls[0]}/api/regions"
         )
-        jsonresponse = response.json()
         countries = list()
         for location in jsonresponse["objects"]:
             loccode = location["code"]
             locname = location["name_en"]
             if use_count:
                 count = location.get("count")
                 if count is None:
@@ -195,18 +195,17 @@
         Returns:
             List[Dict]: List of layers
         """
         if countryiso is None:
             regionstr = ""
         else:
             regionstr = f"/?regions__code__in={countryiso}"
-        response = self.downloader.download(
+        jsonresponse = self.downloader.download_json(
             f"{self.geonode_urls[0]}/api/layers{regionstr}"
         )
-        jsonresponse = response.json()
         return jsonresponse["objects"]
 
     @staticmethod
     def get_orgname(metadata: Dict, orgclass: Type = Organization) -> str:
         """
         Get orgname from Dict if available or use orgid from Dict to look up organisation name
 
@@ -271,23 +270,23 @@
         logger.info(f"Creating dataset: {title}")
         detail_url = layer["detail_url"]
         supplemental_information = layer["supplemental_information"]
         if supplemental_information.lower()[:7] == "no info":
             dataset_notes = notes
         else:
             dataset_notes = f"{notes}\n\n{supplemental_information}"
-        reference_period = parse_date(layer["date"])
+        date = parse_date(layer["date"])
         if origtitle == title:
-            dataset.set_reference_period(reference_period)
+            dataset.set_reference_period(date)
         else:
             dataset_notes = (
                 f"{dataset_notes}\n\nOriginal dataset title: {origtitle}"
             )
             logger.info(
-                f"Using {ranges[0][0]}-{ranges[0][1]} instead of {reference_period} for reference period"
+                f"Using {ranges[0][0]}-{ranges[0][1]} instead of {date} for reference period"
             )
         slugified_name = slugify(
             f"{self.get_orgname(metadata)}_geonode_{title}"
         )
         slugified_name = process_dataset_name(slugified_name)
         slugified_name = slugified_name[:90]
         dataset["name"] = slugified_name
@@ -338,23 +337,25 @@
             {
                 "name": f"{title} shapefile",
                 "url": f"{geonode_url}/geoserver/wfs?format_options=charset:UTF-8&typename={typename}&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": f"Zipped Shapefile. {notes}",
             }
         )
         resource.set_file_type("zipped shapefile")
+        resource.set_date_data_updated(date)
         dataset.add_update_resource(resource)
         resource = Resource(
             {
                 "name": f"{title} geojson",
                 "url": f"{geonode_url}/geoserver/wfs?srsName={srid}&typename={typename}&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": f"GeoJSON file. {notes}",
             }
         )
         resource.set_file_type("GeoJSON")
+        resource.set_date_data_updated(date)
         dataset.add_update_resource(resource)
 
         showcase = Showcase(
             {
                 "name": f"{slugified_name}-showcase",
                 "title": title,
                 "notes": notes,
```

### Comparing `hdx_scraper_geonode-1.5.0/src/hdx/scraper/geonode/hdx_geonode.yaml` & `hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/hdx_geonode.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/tests/hdx/scraper/geonode/test_geonodetohdx.py` & `hdx_scraper_geonode-1.5.1/tests/hdx/scraper/geonode/test_geonodetohdx.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,40 +230,44 @@
     wfpresources = [
         [
             {
                 "name": "ICA Sudan - Land Degradation shapefile",
                 "url": "http://xxx/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:sdn_ica_landdegradation_geonode_20180201&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. This layer contains...",
                 "format": "shp",
+                "last_modified": "2018-11-22T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "ICA Sudan - Land Degradation geojson",
                 "url": "http://xxx/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:sdn_ica_landdegradation_geonode_20180201&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. This layer contains...",
                 "format": "geojson",
+                "last_modified": "2018-11-22T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
         [
             {
                 "name": "ICA Sudan - Most Predominant Livelihood Zones shapefile",
                 "url": "https://ogcserver.gis.wfp.org/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:sdn_ica_predlhz_geonode_20180201&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. This layer contains...",
                 "format": "shp",
+                "last_modified": "2018-11-22T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "ICA Sudan - Most Predominant Livelihood Zones geojson",
                 "url": "https://ogcserver.gis.wfp.org/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:sdn_ica_predlhz_geonode_20180201&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. This layer contains...",
                 "format": "geojson",
+                "last_modified": "2018-11-22T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
     ]
 
     wfporganization = {
@@ -374,40 +378,44 @@
     mimuresources = [
         [
             {
                 "name": "Myanmar Town shapefile",
                 "url": "http://yyy/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:mmr_town_2019_july&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. Towns are urban areas divided into wards.",
                 "format": "shp",
+                "last_modified": "2019-08-05T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "Myanmar Town geojson",
                 "url": "http://yyy/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:mmr_town_2019_july&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. Towns are urban areas divided into wards.",
                 "format": "geojson",
+                "last_modified": "2019-08-05T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
         [
             {
                 "name": "Myanmar Forest Cover Change shapefile",
                 "url": "http://yyy/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:myan_lvl2_smoothed_dec2015_resamp&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. A Landsat-based classification of Myanmar’s forest cover",
                 "format": "shp",
+                "last_modified": "2019-02-12T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "Myanmar Forest Cover Change geojson",
                 "url": "http://yyy/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:myan_lvl2_smoothed_dec2015_resamp&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. A Landsat-based classification of Myanmar’s forest cover",
                 "format": "geojson",
+                "last_modified": "2019-02-12T00:00:00",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
     ]
 
     mimuorganization = {
@@ -621,53 +629,32 @@
         class Response:
             @staticmethod
             def json():
                 pass
 
         class Download:
             @staticmethod
-            def download(url):
-                response = Response()
+            def download_json(url):
                 if url == "http://xxx/api/regions":
-
-                    def fn():
-                        return {"objects": TestGeoNodeToHDX.wfplocationsdata}
-
-                    response.json = fn
+                    return {"objects": TestGeoNodeToHDX.wfplocationsdata}
                 elif url == "http://xxx/api/layers/?regions__code__in=SDN":
-
-                    def fn():
-                        return {"objects": TestGeoNodeToHDX.wfplayersdata}
-
-                    response.json = fn
+                    return {"objects": TestGeoNodeToHDX.wfplayersdata}
                 elif url == "http://yyy/api/layers":
-
-                    def fn():
-                        return {"objects": TestGeoNodeToHDX.mimulayersdata}
-
-                    response.json = fn
+                    return {"objects": TestGeoNodeToHDX.mimulayersdata}
                 elif url == "http://zzz/api/layers":
-
-                    def fn():
-                        return {
-                            "objects": TestGeoNodeToHDX.mimulayersdata
-                            + [TestGeoNodeToHDX.oldmimulayer]
-                        }
-
-                    response.json = fn
+                    return {
+                        "objects": TestGeoNodeToHDX.mimulayersdata
+                        + [TestGeoNodeToHDX.oldmimulayer]
+                    }
                 elif url == "http://aaa/api/layers":
-
-                    def fn():
-                        return {
-                            "objects": TestGeoNodeToHDX.mimulayersdata
-                            + [TestGeoNodeToHDX.mimulayersdata[0]]
-                        }
-
-                    response.json = fn
-                return response
+                    return {
+                        "objects": TestGeoNodeToHDX.mimulayersdata
+                        + [TestGeoNodeToHDX.mimulayersdata[0]]
+                    }
+                return None
 
         return Download()
 
     @pytest.fixture(scope="function")
     def yaml_config(self):
         return join("tests", "fixtures", "hdx_geonode.yml")
```

### Comparing `hdx_scraper_geonode-1.5.0/.gitignore` & `hdx_scraper_geonode-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/LICENSE` & `hdx_scraper_geonode-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/README.md` & `hdx_scraper_geonode-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.0/pyproject.toml` & `hdx_scraper_geonode-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-api >= 6.0.4",
+    "hdx-python-api >= 6.0.6",
     "python-slugify",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `hdx_scraper_geonode-1.5.0/PKG-INFO` & `hdx_scraper_geonode-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-scraper-geonode
-Version: 1.5.0
+Version: 1.5.1
 Summary: HDX Python generic geonode scraper
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-scraper-geonode
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,geonode,scraper
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: hdx-python-api>=6.0.4
+Requires-Dist: hdx-python-api>=6.0.6
 Requires-Dist: python-slugify
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

