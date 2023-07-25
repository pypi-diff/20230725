# Comparing `tmp/wiserep_api-0.1.5.tar.gz` & `tmp/wiserep_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.5.tar", last modified: Thu May  4 13:30:27 2023, max compression
+gzip compressed data, was "wiserep_api-0.1.6.tar", last modified: Tue Jul 25 08:22:58 2023, max compression
```

## Comparing `wiserep_api-0.1.5.tar` & `wiserep_api-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.5/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.5/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2023-05-04 05:27:21.000000 wiserep_api-0.1.5/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.5/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.5/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.5/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.5/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      893 2023-05-04 12:28:16.000000 wiserep_api-0.1.5/tests/test_properties.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.5/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      283 2023-05-04 12:23:09.000000 wiserep_api-0.1.5/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-04 13:30:00.000000 wiserep_api-0.1.5/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2844 2023-05-04 07:21:49.000000 wiserep_api-0.1.5/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3748 2023-05-04 12:32:22.000000 wiserep_api-0.1.5/wiserep_api/properties.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.5/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:34:32.000000 wiserep_api-0.1.5/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5790 2023-05-04 07:19:34.000000 wiserep_api-0.1.5/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api/static/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.5/wiserep_api/static/spectral_types.json
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-04 13:30:27.746963 wiserep_api-0.1.5/wiserep_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4129 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      521 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-05-04 13:30:27.000000 wiserep_api-0.1.5/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-25 08:22:58.530428 wiserep_api-0.1.6/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.6/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.6/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5023 2023-07-25 08:22:58.526428 wiserep_api-0.1.6/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4536 2023-05-04 13:47:07.000000 wiserep_api-0.1.6/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-05-02 08:10:24.000000 wiserep_api-0.1.6/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-07-25 08:22:58.530428 wiserep_api-0.1.6/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.6/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-25 08:22:58.526428 wiserep_api-0.1.6/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.6/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2326 2023-05-04 07:16:40.000000 wiserep_api-0.1.6/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1268 2023-07-25 08:20:56.000000 wiserep_api-0.1.6/tests/test_properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.6/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-25 08:22:58.526428 wiserep_api-0.1.6/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      305 2023-07-07 11:18:07.000000 wiserep_api-0.1.6/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-07-25 08:21:56.000000 wiserep_api-0.1.6/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3688 2023-07-07 11:22:26.000000 wiserep_api-0.1.6/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3744 2023-07-07 11:22:33.000000 wiserep_api-0.1.6/wiserep_api/properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.6/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:34:32.000000 wiserep_api-0.1.6/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5534 2023-07-07 11:22:50.000000 wiserep_api-0.1.6/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-25 08:22:58.526428 wiserep_api-0.1.6/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.6/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-25 08:22:58.526428 wiserep_api-0.1.6/wiserep_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5023 2023-07-25 08:22:58.000000 wiserep_api-0.1.6/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      521 2023-07-25 08:22:58.000000 wiserep_api-0.1.6/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-07-25 08:22:58.000000 wiserep_api-0.1.6/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       30 2023-07-25 08:22:58.000000 wiserep_api-0.1.6/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2023-07-25 08:22:58.000000 wiserep_api-0.1.6/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.5/LICENSE` & `wiserep_api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/PKG-INFO` & `wiserep_api-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.5
+Version: 0.1.6
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,18 @@
 License-File: LICENSE
 
 # WiseRep API
 API to access WiserRep data from command lines
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
-[![Tests and Publish](https://github.com/temuller/wiserep_api/actions/workflows/main.yml/badge.svg)](https://github.com/temuller/wiserep_api/actions/workflows/main.yml)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
+[![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
+
 
 ## Installation
 
 It is recommended to install ``wiserep_api`` from pip:
 
 ```python
 pip install wiserep_api
@@ -85,17 +86,34 @@
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
     snid.run_snid(directory, command=snid_commmand)
 ```
 
-### Getting the classification
+### Getting object's properties  
+
+The properties of a given object can be easily obtained:
 
-The spectral type of a given target can also be retrived:
+```python
+from wiserep_api import get_target_property
+
+for prop in ['type', 'redshift', 'host', 'coords', 'coords_deg']:
+    value = get_target_property('2004eo', prop)
+    print(f'{prop}: {value}')
+```   
+```python
+type: SN Ia
+redshift: 0.015718
+host: NGC6928
+coords: 20:32:54.190 +09:55:42.71
+coords_deg: 308.22579 +9.92853
+```
+
+The spectral type of a given object can also be retrived with ``get_target_class``, which does a more "in-depth" search of the classification in case this is not found in the main properties:
 
 ```python
 from wiserep_api import get_target_class
 
 sn_type = get_target_class("2004eo")
 print(sn_type)
 ```
@@ -103,7 +121,24 @@
 'SN Ia'
 ```
 
 
 ## Contributing
 
 To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
+
+## Citing WiseRep API
+
+If you make use of this code, please cite it:
+
+```code
+@software{tomas_e_muller_bravo_2023_7896352,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/wiserep\_api: First Official Release!},
+  month        = may,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.5},
+  doi          = {10.5281/zenodo.7896352},
+  url          = {https://doi.org/10.5281/zenodo.7896352}
+}
+```
```

### Comparing `wiserep_api-0.1.5/README.md` & `wiserep_api-0.1.6/wiserep_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: wiserep-api
+Version: 0.1.6
+Summary: API to access WiserRep data from command lines
+Home-page: https://github.com/temuller/wiserep_api
+Author: Tomás Enrique Müller-Bravo
+Author-email: t.e.muller-bravo@ice.csic.es
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # WiseRep API
 API to access WiserRep data from command lines
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
-[![Tests and Publish](https://github.com/temuller/wiserep_api/actions/workflows/main.yml/badge.svg)](https://github.com/temuller/wiserep_api/actions/workflows/main.yml)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
+[![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
+
 
 ## Installation
 
 It is recommended to install ``wiserep_api`` from pip:
 
 ```python
 pip install wiserep_api
@@ -70,25 +86,59 @@
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
     snid.run_snid(directory, command=snid_commmand)
 ```
 
-### Getting the classification
+### Getting object's properties  
+
+The properties of a given object can be easily obtained:
+
+```python
+from wiserep_api import get_target_property
+
+for prop in ['type', 'redshift', 'host', 'coords', 'coords_deg']:
+    value = get_target_property('2004eo', prop)
+    print(f'{prop}: {value}')
+```   
+```python
+type: SN Ia
+redshift: 0.015718
+host: NGC6928
+coords: 20:32:54.190 +09:55:42.71
+coords_deg: 308.22579 +9.92853
+```
 
-The spectral type of a given target can also be retrived:
+The spectral type of a given object can also be retrived with ``get_target_class``, which does a more "in-depth" search of the classification in case this is not found in the main properties:
 
 ```python
 from wiserep_api import get_target_class
 
 sn_type = get_target_class("2004eo")
 print(sn_type)
 ```
 ```python
 'SN Ia'
 ```
 
 
 ## Contributing
 
-To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
+To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
+
+## Citing WiseRep API
+
+If you make use of this code, please cite it:
+
+```code
+@software{tomas_e_muller_bravo_2023_7896352,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/wiserep\_api: First Official Release!},
+  month        = may,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.5},
+  doi          = {10.5281/zenodo.7896352},
+  url          = {https://doi.org/10.5281/zenodo.7896352}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wiserep_api-0.1.5/setup.py` & `wiserep_api-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/tests/test_download_spectra.py` & `wiserep_api-0.1.6/tests/test_download_spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/tests/test_properties.py` & `wiserep_api-0.1.6/tests/test_properties.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,22 @@
                            'coords':'20:32:54.190 +09:55:42.71',
                            'coords_deg':'308.22579 +9.92853',
                           } 
         for prop, value in properties_dict.items():
             result = get_target_property(target, prop)
             np.testing.assert_string_equal(str(result), value)
 
+        # multiple properties at once
+        properties = list(properties_dict.keys())
+        values = get_target_property(target, properties)
+        expected_props = ['SN Ia', 0.015718, 'NGC6928', 
+                          '20:32:54.190 +09:55:42.71', '308.22579 +9.92853']
+
+        assert values==expected_props, "The values retrieved do not match the expected ones" 
+
 class TestClassification(unittest.TestCase):
     def test_classification(self):
         sn_type = get_target_class("2004eo")
         np.testing.assert_string_equal(sn_type, "SN Ia")
 
 
 if __name__ == "__main__":
```

### Comparing `wiserep_api-0.1.5/wiserep_api/search.py` & `wiserep_api-0.1.6/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/wiserep_api/snid.py` & `wiserep_api-0.1.6/wiserep_api/snid.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/wiserep_api/spectra.py` & `wiserep_api-0.1.6/wiserep_api/spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pandas as pd
 from astropy.io import fits
-from wiserep_api.api import get_response, get_object_id
+from wiserep_api.api import get_response, get_target_response
 
 
 def exclude_include(url, exclude=None, include=None):
     """Either includes or excludes the given URL according to the
     given patterns.
 
     Note: only one of the parameters ('exclude' or 'include') can be
@@ -61,36 +61,28 @@
     exclude: list, default 'None'
         Files with the given string patterns are excluded.
         Cannot be given together with 'include'.
     include: list, default 'None'
         Files with the given string patterns are inxcluded.
         Cannot be given together with 'exclude'.
     verbose: bool, default 'False'
-        If True, print some of the extra information
+        If 'True', print some of the extra information.
 
     Returns
     -------
     target_class: str
         The target's classification. Returns 'Unknown' if not found.
     """
     if os.path.isdir("spectra") is False:
         os.mkdir("spectra")
 
     assert file_type in [None, "ascii", "fits"], "not a valide file type"
 
-    # look for the target ID in the search webpage
-    obj_id = get_object_id(iau_name, verbose)
-    if (obj_id is None) or (obj_id == "Unknown"):
-        return obj_id
-
-    # target's webpage
-    target_url = f"https://www.wiserep.org/object/{obj_id}"
-    response = get_response(target_url)
-    if response is None:
-        return None
+    # target's url
+    response = get_target_response(iau_name, verbose)
 
     # search for spectra URLs
     # ASCII
     txt_urls = []
     split_text = response.text.split("asciifile=https%3A//")
     for st in split_text:
         url = st.split('"')[0]
```

### Comparing `wiserep_api-0.1.5/wiserep_api/static/spectral_types.json` & `wiserep_api-0.1.6/wiserep_api/static/spectral_types.json`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.5/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,16 @@
-Metadata-Version: 2.1
-Name: wiserep-api
-Version: 0.1.5
-Summary: API to access WiserRep data from command lines
-Home-page: https://github.com/temuller/wiserep_api
-Author: Tomás Enrique Müller-Bravo
-Author-email: t.e.muller-bravo@ice.csic.es
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # WiseRep API
 API to access WiserRep data from command lines
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
-[![Tests and Publish](https://github.com/temuller/wiserep_api/actions/workflows/main.yml/badge.svg)](https://github.com/temuller/wiserep_api/actions/workflows/main.yml)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
+[![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
+
 
 ## Installation
 
 It is recommended to install ``wiserep_api`` from pip:
 
 ```python
 pip install wiserep_api
@@ -85,17 +71,34 @@
 snid_commmand = 'snid inter=0 plot=0 aband=0 usetype=Ia-91T'
 
 for sn in sne_list:
     directory = os.path.join('spectra', sn)
     snid.run_snid(directory, command=snid_commmand)
 ```
 
-### Getting the classification
+### Getting object's properties  
+
+The properties of a given object can be easily obtained:
+
+```python
+from wiserep_api import get_target_property
+
+for prop in ['type', 'redshift', 'host', 'coords', 'coords_deg']:
+    value = get_target_property('2004eo', prop)
+    print(f'{prop}: {value}')
+```   
+```python
+type: SN Ia
+redshift: 0.015718
+host: NGC6928
+coords: 20:32:54.190 +09:55:42.71
+coords_deg: 308.22579 +9.92853
+```
 
-The spectral type of a given target can also be retrived:
+The spectral type of a given object can also be retrived with ``get_target_class``, which does a more "in-depth" search of the classification in case this is not found in the main properties:
 
 ```python
 from wiserep_api import get_target_class
 
 sn_type = get_target_class("2004eo")
 print(sn_type)
 ```
@@ -103,7 +106,24 @@
 'SN Ia'
 ```
 
 
 ## Contributing
 
 To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
+
+## Citing WiseRep API
+
+If you make use of this code, please cite it:
+
+```code
+@software{tomas_e_muller_bravo_2023_7896352,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/wiserep\_api: First Official Release!},
+  month        = may,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.5},
+  doi          = {10.5281/zenodo.7896352},
+  url          = {https://doi.org/10.5281/zenodo.7896352}
+}
+```
```

### Comparing `wiserep_api-0.1.5/wiserep_api.egg-info/SOURCES.txt` & `wiserep_api-0.1.6/wiserep_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

