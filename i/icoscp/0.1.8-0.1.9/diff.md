# Comparing `tmp/icoscp-0.1.8.tar.gz` & `tmp/icoscp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoscp-0.1.8.tar", last modified: Thu Sep 23 12:34:10 2021, max compression
+gzip compressed data, was "icoscp-0.1.9.tar", last modified: Mon Oct 11 15:48:48 2021, max compression
```

## Comparing `icoscp-0.1.8.tar` & `icoscp-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:10.635106 icoscp-0.1.8/
--rw-rw-rw-   0        0        0     3410 2021-09-23 12:34:10.632108 icoscp-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1991 2021-09-23 12:29:00.000000 icoscp-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:09.475857 icoscp-0.1.8/icoscp/
--rw-rw-rw-   0        0        0     1094 2021-08-27 14:55:12.000000 icoscp-0.1.8/icoscp/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:09.661747 icoscp-0.1.8/icoscp/collection/
--rw-rw-rw-   0        0        0      149 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/collection/__init__.py
--rw-rw-rw-   0        0        0     9134 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/collection/collection.py
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:10.344279 icoscp-0.1.8/icoscp/cpb/
--rw-rw-rw-   0        0        0      416 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/cpb/__init__.py
--rw-rw-rw-   0        0        0    19187 2021-09-23 12:17:17.000000 icoscp-0.1.8/icoscp/cpb/dobj.py
--rw-rw-rw-   0        0        0     3547 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/cpb/dtype_dict.py
--rw-rw-rw-   0        0        0     1217 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/cpb/get_size.py
--rw-rw-rw-   0        0        0     1403 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/cpb/logfile.py
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:10.560156 icoscp-0.1.8/icoscp/sparql/
--rw-rw-rw-   0        0        0      461 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/sparql/__init__.py
--rw-rw-rw-   0        0        0     5419 2021-08-18 07:35:38.000000 icoscp-0.1.8/icoscp/sparql/runsparql.py
--rw-rw-rw-   0        0        0    42178 2021-09-22 10:57:10.000000 icoscp-0.1.8/icoscp/sparql/sparqls.py
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:10.625112 icoscp-0.1.8/icoscp/station/
--rw-rw-rw-   0        0        0      149 2021-09-17 11:50:34.000000 icoscp-0.1.8/icoscp/station/__init__.py
--rw-rw-rw-   0        0        0    24001 2021-09-23 12:23:56.000000 icoscp-0.1.8/icoscp/station/station.py
-drwxrwxrwx   0        0        0        0 2021-09-23 12:34:09.601783 icoscp-0.1.8/icoscp.egg-info/
--rw-rw-rw-   0        0        0     3410 2021-09-23 12:34:08.000000 icoscp-0.1.8/icoscp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2021-09-23 12:34:08.000000 icoscp-0.1.8/icoscp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-23 12:34:08.000000 icoscp-0.1.8/icoscp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2021-09-23 12:34:08.000000 icoscp-0.1.8/icoscp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-09-23 12:34:08.000000 icoscp-0.1.8/icoscp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-23 12:34:10.635106 icoscp-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1737 2021-09-23 12:25:49.000000 icoscp-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.607086 icoscp-0.1.9/
+-rw-rw-rw-   0        0        0     3352 2021-10-11 15:48:48.607086 icoscp-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1933 2021-10-11 13:36:33.000000 icoscp-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.538079 icoscp-0.1.9/icoscp/
+-rw-rw-rw-   0        0        0     1094 2021-10-11 13:35:20.000000 icoscp-0.1.9/icoscp/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.569327 icoscp-0.1.9/icoscp/collection/
+-rw-rw-rw-   0        0        0      149 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/collection/__init__.py
+-rw-rw-rw-   0        0        0     9134 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/collection/collection.py
+-rw-rw-rw-   0        0        0      628 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/const.py
+-rw-rw-rw-   0        0        0     4813 2021-10-06 11:59:55.000000 icoscp-0.1.9/icoscp/country.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.575832 icoscp-0.1.9/icoscp/cpb/
+-rw-rw-rw-   0        0        0      416 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/cpb/__init__.py
+-rw-rw-rw-   0        0        0    19187 2021-10-06 11:59:55.000000 icoscp-0.1.9/icoscp/cpb/dobj.py
+-rw-rw-rw-   0        0        0     3547 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/cpb/dtype_dict.py
+-rw-rw-rw-   0        0        0     1217 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/cpb/get_size.py
+-rw-rw-rw-   0        0        0     1403 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/cpb/logfile.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.575832 icoscp-0.1.9/icoscp/sparql/
+-rw-rw-rw-   0        0        0      461 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/sparql/__init__.py
+-rw-rw-rw-   0        0        0     5419 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/sparql/runsparql.py
+-rw-rw-rw-   0        0        0    42178 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/sparql/sparqls.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.591461 icoscp-0.1.9/icoscp/station/
+-rw-rw-rw-   0        0        0      149 2021-10-05 14:53:51.000000 icoscp-0.1.9/icoscp/station/__init__.py
+-rw-rw-rw-   0        0        0    15459 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/station/fmap.py
+-rw-rw-rw-   0        0        0    24964 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/station/station.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.607086 icoscp-0.1.9/icoscp/stilt/
+-rw-rw-rw-   0        0        0      162 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/__init__.py
+-rw-rw-rw-   0        0        0     3644 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/fmap.py
+-rw-rw-rw-   0        0        0     4049 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/geoinfo.py
+-rw-rw-rw-   0        0        0   580154 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/stations.json
+-rw-rw-rw-   0        0        0    14687 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/stiltobj.py
+-rw-rw-rw-   0        0        0    19080 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/stiltstation.py
+-rw-rw-rw-   0        0        0     6050 2021-10-11 13:15:25.000000 icoscp-0.1.9/icoscp/stilt/timefuncs.py
+drwxrwxrwx   0        0        0        0 2021-10-11 15:48:48.569327 icoscp-0.1.9/icoscp.egg-info/
+-rw-rw-rw-   0        0        0     3352 2021-10-11 15:48:48.000000 icoscp-0.1.9/icoscp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2021-10-11 15:48:48.000000 icoscp-0.1.9/icoscp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-11 15:48:48.000000 icoscp-0.1.9/icoscp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2021-10-11 15:48:48.000000 icoscp-0.1.9/icoscp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-10-11 15:48:48.000000 icoscp-0.1.9/icoscp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-10-11 15:48:48.607086 icoscp-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2021-10-11 15:14:31.000000 icoscp-0.1.9/setup.py
```

### Comparing `icoscp-0.1.8/PKG-INFO` & `icoscp-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoscp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Access to ICOS data objects hosted at https://data.icos-cp.eu
 Home-page: https://www.icos-cp.eu/
 Author: Claudio D'Onofrio, Zois Zogopoulos, ICOS Carbon Portal
 Author-email: claudio.donofrio@nateko.lu.se, zois.zogopoulos@nateko.lu.se, info@icos-cp.eu
 License: GPLv3+
 Project-URL: Source, https://github.com/ICOS-Carbon-Portal/pylib
 Project-URL: Documentation, https://icos-carbon-portal.github.io/pylib/
@@ -36,15 +36,15 @@
 
 This package is under active development. Please be aware that changes to names of functions and classes are possible without further notice. Please do feedback any recommendations, issues, etc if you try it out.
 
 
 What is the package about?
 In essence this package allows you to have direct access to data objects from the ICOS CarbonPortal were a "Preview" is available. It is an easy access to data objects hosted at the ICOS Carbon Portal ( https://data.icos-cp.eu/ ). By using this library you can load data files directly into memory.
 
-Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://www.icos-cp.eu/data-services/about-data-portal/data-license" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
+Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://data.icos-cp.eu/licence" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
 
 We would encourage you to use a virtual environment for python to test this library.
 For example with mini-conda (https://docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 
 - `conda create -n icos python`
 - `activate icos`
 - `pip install icoscp`
@@ -54,13 +54,7 @@
 
 
 
 
 
 
 
-
-
-
-cd20200720
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icoscp Version: 0.1.8 Summary: Access to ICOS data
+Metadata-Version: 2.1 Name: icoscp Version: 0.1.9 Summary: Access to ICOS data
 objects hosted at https://data.icos-cp.eu Home-page: https://www.icos-cp.eu/
 Author: Claudio D'Onofrio, Zois Zogopoulos, ICOS Carbon Portal Author-email:
 claudio.donofrio@nateko.lu.se, zois.zogopoulos@nateko.lu.se, info@icos-cp.eu
 License: GPLv3+ Project-URL: Source, https://github.com/ICOS-Carbon-Portal/
 pylib Project-URL: Documentation, https://icos-carbon-portal.github.io/pylib/
 Project-URL: DataPortal, https://data.icos-cp.eu/portal/ Project-URL:
 SparqlEndpoint, https://meta.icos-cp.eu/sparqlclient/?type=CSV Platform:
@@ -36,8 +36,8 @@
 library, you agree and accept, that all ICOS data is provided under a CC_BY_4.0
 licence_[https://www.icos-cp.eu/sites/default/files/inline-images/
 creativecommons.png] We would encourage you to use a virtual environment for
 python to test this library. For example with mini-conda (https://
 docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 - `conda create -n icos python` - `activate icos` - `pip install icoscp`
 Documentation about the library and all the modules are available at https://
-icos-carbon-portal.github.io/pylib/ cd20200720
+icos-carbon-portal.github.io/pylib/
```

### Comparing `icoscp-0.1.8/README.md` & `icoscp-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 This package is under active development. Please be aware that changes to names of functions and classes are possible without further notice. Please do feedback any recommendations, issues, etc if you try it out.
 
 
 What is the package about?
 In essence this package allows you to have direct access to data objects from the ICOS CarbonPortal were a "Preview" is available. It is an easy access to data objects hosted at the ICOS Carbon Portal ( https://data.icos-cp.eu/ ). By using this library you can load data files directly into memory.
 
-Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://www.icos-cp.eu/data-services/about-data-portal/data-license" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
+Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://data.icos-cp.eu/licence" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
 
 We would encourage you to use a virtual environment for python to test this library.
 For example with mini-conda (https://docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 
 - `conda create -n icos python`
 - `activate icos`
 - `pip install icoscp`
@@ -23,13 +23,7 @@
 
 Documentation about the library and all the modules are available at https://icos-carbon-portal.github.io/pylib/
 
 
 
 
 
-
-
-
-
-
-cd20200720
```

#### html2text {}

```diff
@@ -18,8 +18,8 @@
 library, you agree and accept, that all ICOS data is provided under a CC_BY_4.0
 licence_[https://www.icos-cp.eu/sites/default/files/inline-images/
 creativecommons.png] We would encourage you to use a virtual environment for
 python to test this library. For example with mini-conda (https://
 docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 - `conda create -n icos python` - `activate icos` - `pip install icoscp`
 Documentation about the library and all the modules are available at https://
-icos-carbon-portal.github.io/pylib/ cd20200720
+icos-carbon-portal.github.io/pylib/
```

### Comparing `icoscp-0.1.8/icoscp/__init__.py` & `icoscp-0.1.9/icoscp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,13 @@
     you only need to store a list of pid's and your script to reproduce
     always the same result, regardless on which computer you run it.
     (as long as you have an internet connection)    
 """
 
 __credits__     = "ICOS Carbon Portal"
 __license__     = ['Software: GPL-3.0','ICSO Data accessed with this library CC BY 4.0']
-__version__     = "0.1.7"
+__version__     = "0.1.9"
 __maintainer__  = "ICOS Carbon Portal, elaborated products team"
 __email__       = ['info@icos-cp.eu', 'claudio.donofrio@nateko.lu.se']
-__status__      = "r1"
-__date__        = "2021-06-23"
-
-
+__status__      = "stable"
+__date__        = "2021-10-11"
```

### Comparing `icoscp-0.1.8/icoscp/collection/collection.py` & `icoscp-0.1.9/icoscp/collection/collection.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/cpb/dobj.py` & `icoscp-0.1.9/icoscp/cpb/dobj.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/cpb/dtype_dict.py` & `icoscp-0.1.9/icoscp/cpb/dtype_dict.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/cpb/get_size.py` & `icoscp-0.1.9/icoscp/cpb/get_size.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/cpb/logfile.py` & `icoscp-0.1.9/icoscp/cpb/logfile.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/sparql/runsparql.py` & `icoscp-0.1.9/icoscp/sparql/runsparql.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/sparql/sparqls.py` & `icoscp-0.1.9/icoscp/sparql/sparqls.py`

 * *Files identical despite different names*

### Comparing `icoscp-0.1.8/icoscp/station/station.py` & `icoscp-0.1.9/icoscp/station/station.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,33 @@
         
     from icoscp.station import station    
     station.getIdList() # returns a pandas data frame with all station Id's'
     myStation = station.get('StationId') # create a single statino object
     myList = station.getList('AS') #  returns a list of Atmospheric stations
 """
 
-__author__      = ["Claudio D'Onofrio"]
-__credits__     = "ICOS Carbon Portal"
-__license__     = "GPL-3.0"
-__version__     = "0.1.2"
-__maintainer__  = "ICOS Carbon Portal, elaborated products team"
-__email__       = ['info@icos-cp.eu', 'claudio.donofrio@nateko.lu.se']
-__status__      = "rc1"
-__date__        = "2020-11-05"
+__author__ = ["Claudio D'Onofrio", "Zois Zogopoulos"]
+__credits__ = "ICOS Carbon Portal"
+__license__ = "GPL-3.0"
+__version__ = "0.1.3"
+__maintainer__ = "ICOS Carbon Portal, elaborated products team"
+__email__ = ['info@icos-cp.eu', 'claudio.donofrio@nateko.lu.se', 'zois.zogopoulos@nateko.lu.se']
+__status__ = "rc1"
+__date__ = "2021-09-20"
 
 import json
+
 import pandas as pd
-from icoscp.sparql.runsparql import RunSparql
-from icoscp.sparql import sparqls
 from tqdm import tqdm
 
+from icoscp.sparql import sparqls
+from icoscp.sparql.runsparql import RunSparql
+import icoscp.station.fmap as fmap
+
+
 # ----------------------------------------------
 class Station():
     """ Create an ICOS Station object. This class intends to create 
         an instance of station, providing meta data including 
         stationId, Name, PI, Lat, Lon,  etc.
         Examples:
         import station
@@ -40,203 +44,216 @@
         myStation = station.get('HTM')
         
         station.info()
         
         # extract single attribute
         station.lat -> returns latitude as float
     """
-    
+
     def __init__(self):
         """
         Initialize your Station. If you have a list of attributes,
         call .setStation(attribList). 
       
         """
 
-        self._stationId = None      # shortName like HTM or SE-NOR   
-        self._valid = False         # if stationId is set and valid, return True            
-        self._name = None           # longName
-        self._theme = None          # AS | ES | OS
-        self._icosclass = None      # 1 | 2 
-        self._siteType = None       # description of site
-        
-        #locations
-        self._lat = None            # latitude
-        self._lon = None            # longitude
-        self._eas = None            # elevation above sea level
-        self._eag = None            # elevation above ground, height of tower
-        
-        #pi information
-        self._firstName = None      # Station PI first name
-        self._lastName = None       # Station PI last name
-        self._email = None          # Station PI email
-        
+        self._stationId = None  # shortName like HTM or SE-NOR
+        self._valid = False  # if stationId is set and valid, return True
+        self._name = None  # longName
+        self._theme = None  # AS | ES | OS
+        self._icosclass = None  # 1 | 2
+        self._siteType = None  # description of site
+
+        # locations
+        self._lat = None  # latitude
+        self._lon = None  # longitude
+        self._eas = None  # elevation above sea level
+        self._eag = None  # elevation above ground, height of tower
+
+        # pi information
+        self._firstName = None  # Station PI first name
+        self._lastName = None  # Station PI last name
+        self._email = None  # Station PI email
+
         # other information
         self._country = None
-        self._project = None        # list, project affiliation, 
-        self._uri = None            # list, links to ressources, landing pages
-        
+        self._project = None  # list, project affiliation,
+        self._uri = None  # list, links to ressources, landing pages
+
         # data and products
-        self._datacheck = False    # check if data and products have been asked for already
-        self._data = None           # list of associated dataobjects
-        self._products = None       # list of available products
-        
-            
-    #super().__init__() # for subclasses
-    #-------------------------------------
+        self._datacheck = False  # check if data and products have been asked for already
+        self._data = None  # list of associated dataobjects
+        self._products = None  # list of available products
+
+    # super().__init__() # for subclasses
+    # -------------------------------------
     @property
     def stationId(self):
         return self._stationId
-    
+
     @stationId.setter
     def stationId(self, stationId):
         self._stationId = stationId
-    #-------------------------------------
+
+    # -------------------------------------
     @property
     def valid(self):
         return self._valid
-    
+
     @valid.setter
     def valid(self, valid):
         self._valid = valid
-    #-------------------------------------
+
+    # -------------------------------------
     @property
     def theme(self):
         return self._theme
-    
+
     @theme.setter
     def theme(self, theme):
         self._theme = theme
-     #-------------------------------------
+
+    # -------------------------------------
     @property
     def icosclass(self):
         return self._icosclass
-    
+
     @icosclass.setter
     def icosclass(self, icosclass):
         self._icosclass = icosclass
-     #-------------------------------------    
+
+    # -------------------------------------
     @property
     def name(self):
         return self._name
-    
+
     @name.setter
     def name(self, name):
-        self._name = name    
-    #-------------------------------------
+        self._name = name
+        # -------------------------------------
+
     @property
     def lat(self):
         return self._lat
-    
+
     @lat.setter
     def lat(self, lat):
-        self._lat = lat    
-    #-------------------------------------
+        self._lat = lat
+        # -------------------------------------
+
     @property
     def lon(self):
         return self._lon
-    
+
     @lon.setter
     def lon(self, lon):
-        self._lon = lon    
-    #-------------------------------------
+        self._lon = lon
+        # -------------------------------------
+
     @property
     def eas(self):
         return self._eas
-    
+
     @eas.setter
     def eas(self, eas):
-        self._eas = eas    
-    #-------------------------------------
+        self._eas = eas
+        # -------------------------------------
+
     @property
     def eag(self):
         return self._eag
-    
+
     @eag.setter
     def eag(self, eag):
-        self._eag = eag    
-    #-------------------------------------
+        self._eag = eag
+        # -------------------------------------
+
     @property
     def firstName(self):
         return self._firstName
-    
+
     @firstName.setter
     def firstName(self, firstName):
-        self._firstName = firstName    
-    #-------------------------------------
+        self._firstName = firstName
+        # -------------------------------------
+
     @property
     def lastName(self):
         return self._lastName
-    
+
     @lastName.setter
     def lastName(self, lastName):
         self._lastName = lastName
-    #-------------------------------------
+
+    # -------------------------------------
     @property
     def email(self):
         return self._email
-    
+
     @email.setter
     def email(self, email):
         self._email = email
-    #-------------------------------------     
+
+    # -------------------------------------
     @property
     def country(self):
         return self._country
-    
+
     @country.setter
     def country(self, country):
         self._country = country
-    #-------------------------------------
+
+    # -------------------------------------
     @property
     def project(self):
         return self._project
-    
+
     @project.setter
     def project(self, project):
         self._project = project
-    #-------------------------------------
+
+    # -------------------------------------
     @property
     def uri(self):
         return self._uri
-    
+
     @uri.setter
     def uri(self, uri):
         self._uri = uri
-    #-------------------------------------
 
-    def __str__(self):          
+    # -------------------------------------
+
+    def __str__(self):
         return self.info('json')
-       
-        
+
     def data(self, level=None):
         """
         return a list of digital objects for the station
         parameter: level [str | int] default None
         provide filter to dataobjects
             1 = raw data
             2 = QAQC data
             3 = elaborated products
         """
         # check if data has already been asked for
         if not self._datacheck:
             self._setData()
             self._datacheck = True
-            
+
         if not isinstance(self._data, pd.DataFrame):
             # _data is not a dataframe but contains a string...
             return self._data
 
         if level:
             # if level is provided, filter pandas data frame
-            return self._data[self._data['datalevel']==str(level)]
+            return self._data[self._data['datalevel'] == str(level)]
         else:
             # return complete pandas data fram
             return self._data
-    
+
     def products(self, fmt='pandas'):
         """
         Parameters
         ----------
         fmt : str,  optional ['pandas', 'dict']
                     Return a pandas dataframe of unique data products for
                     the station. The default is 'pandas'.
@@ -247,24 +264,23 @@
             uniqe list of data products.
 
         """
         # check if data has already bee asked for
         if not self._datacheck:
             self._setData()
             self._datacheck = True
-        
+
         if not isinstance(self._products, pd.DataFrame):
             return self._products
-        
+
         if fmt == 'dict':
             return self._products.to_dict()
         else:
             return self._products
-    
-    
+
     def setStation(self, attrib=None):
         """
         You can set attributes for the station by providing a dictionary        
         Parameters.      
         project & uri must be a list
         lat, lon, eas, eag, must be convertible to float
         everything else is a string.
@@ -286,164 +302,163 @@
         - email (PI email)    
         - country                    
         
         Returns
         -------
         None
         """
-        
-        if not isinstance(attrib, dict):            
+
+        if not isinstance(attrib, dict):
             return
-        
+
         # minimal sanity check
-        checkFloat = ['lat','lon','eag','eas']
+        checkFloat = ['lat', 'lon', 'eag', 'eas']
         checkList = ['project', 'uri']
-                                
-        #create 'keys' without the underscore
-        keys = [k.strip('_') for k in list(self.__dict__)]        
+
+        # create 'keys' without the underscore
+        keys = [k.strip('_') for k in list(self.__dict__)]
         for a in attrib:
             a = a.strip('_')
             if a in keys and a in checkFloat:
                 try:
-                    self.__setattr__('_'+a, float(attrib[a]))
+                    self.__setattr__('_' + a, float(attrib[a]))
                 except:
                     continue
             elif a in keys and a in checkList:
                 try:
-                    self.__setattr__('_'+a, list(attrib[a]))
+                    self.__setattr__('_' + a, list(attrib[a]))
                 except:
                     continue
             else:
                 self.__setattr__('_' + a, attrib[a])
-                
 
-
-    def info(self, fmt = 'dict'):
+    def info(self, fmt='dict'):
         """
         Parameters
         ----------
         fmt : str ['dict' | 'json' | 'list' | 'pandas' | 'html']
             You can choose a return format by providing fmt.
             The default is 'dict'.
             
 
         Returns
         -------
         All attributes for the Station
 
         """
-        #create new 'keys' without the underscore
+        # create new 'keys' without the underscore
         newKeys = [k.strip('_') for k in list(self.__dict__)]
-        values =  self.__dict__.values()
-        dictionary = dict(zip(newKeys,values))
-        
+        values = self.__dict__.values()
+        dictionary = dict(zip(newKeys, values))
+
         # remove some of the __dictionary__ keys to get a shorter
         # summary of information about the station
-        
+
         remove = ['data', 'products', 'valid', 'datacheck']
         dictionary = {key: value for key, value in dictionary.items() if key not in remove}
-        
-        
+
         if fmt == 'dict':
             return dictionary
-        
+
         if fmt == 'json':
             return json.dumps(dictionary, indent=4)
-                        
+
         if fmt == 'list':
             return (list(dictionary.keys()), list(dictionary.values()))
-        
-        if fmt == 'pandas':            
+
+        if fmt == 'pandas':
             return pd.DataFrame(dictionary, index=[0])
-        
+
         if fmt == 'html':
-	    
-	    #Create and initialize variable to store station info in html table:            
+
+            # Create and initialize variable to store station info in html table:
             html_table = """<meta content="text/html; charset=UTF-8">
                             <style>td{padding: 3px;}</style><table>"""
 
-            #Loop through all keys of station dictionary:
+            # Loop through all keys of station dictionary:
             for k in dictionary.keys():
 
-                #Check if current dict key holds the the long name of the station and
-                #if the key to the URL of the station landing page is included:
-                if((k=='name') & ('uri' in dictionary.keys())):
-                    
-                    #Create table row and add link with URL to station landing page:
-                    html_table = html_table+'<tr><td>'+k+'</td><td><b><a href="'+str(dictionary['uri'][0])+'"target="_blank">'+str(dictionary[k])+'</a></b></td></tr>'           
-                
-                #Skip creating table row for 'uri' key:
-                elif(k=='uri'):
+                # Check if current dict key holds the the long name of the station and
+                # if the key to the URL of the station landing page is included:
+                if ((k == 'name') & ('uri' in dictionary.keys())):
+
+                    # Create table row and add link with URL to station landing page:
+                    html_table = html_table + '<tr><td>' + k + '</td><td><b><a href="' + str(
+                        dictionary['uri'][0]) + '"target="_blank">' + str(
+                        dictionary[k]) + '</a></b></td></tr>'
+
+                    # Skip creating table row for 'uri' key:
+                elif (k == 'uri'):
                     continue
-                
-                #Dict key 'project' returns a list. Print all comma-sep items as string.
-                elif(k=='project'):
+
+                # Dict key 'project' returns a list. Print all comma-sep items as string.
+                elif (k == 'project'):
 
                     project_str = ', '.join(dictionary[k])
-                    html_table = html_table+'<tr><td>'+k+'</td><td><b>'+project_str+'</b></td></tr>'
-                
-                #Add table row with station info for current key:
+                    html_table = html_table + '<tr><td>' + k + '</td><td><b>' + project_str + '</b></td></tr>'
+
+                # Add table row with station info for current key:
                 else:
-                    html_table = html_table+'<tr><td>'+k+'</td><td><b>'+str(dictionary[k])+'</b></td></tr>'
-            
-            #Add html closing tag for table:
-            html_table = html_table +'</table>'
-            
-            #Return station info as html table:
+                    html_table = html_table + '<tr><td>' + k + '</td><td><b>' + str(
+                        dictionary[k]) + '</b></td></tr>'
+
+            # Add html closing tag for table:
+            html_table = html_table + '</table>'
+
+            # Return station info as html table:
             return html_table
-        
+
     def _setData(self):
-        
+
         """
         Query the sparql endpoint for data products submitted by this station
         adjust latitude and longitude and store a list of data specifications
         and data objects (PID's)
         """
-        
+
         if not self.stationId:
             return
         """      
         # get the ressource url and adjust lat and lon from data portal
         query = sparqls.stationResource(self.stationId)
         key, val = RunSparql(query, 'array').run()
         if val:            
             self.url = val[0][0]
             self.lat = float(val[0][2])
             self.lon = float(val[0][3])
-        """            
-        
+        """
+
         # it is possible, that a station id has multiple URI
         # ask for all URI
-        query = sparqls.stationData(self.uri,'all')
+        query = sparqls.stationData(self.uri, 'all')
         data = RunSparql(query, 'pandas').run()
-        
+
         if not data.empty:
-            self._data = data            
+            self._data = data
         else:
-             self._data = 'no data available'            
-         
-         # check if data is available and extract the 'unique' data products        
+            self._data = 'no data available'
+
+            # check if data is available and extract the 'unique' data products
         if isinstance(self._data, pd.DataFrame):
-             p = self._data['specLabel'].unique()            
-             self._products = pd.DataFrame(p)
-             
-             # replace samplingheight=None with empty string
-             self._data.samplingheight.replace(to_replace=[None], value="", inplace=True)
+            p = self._data['specLabel'].unique()
+            self._products = pd.DataFrame(p)
+
+            # replace samplingheight=None with empty string
+            self._data.samplingheight.replace(to_replace=[None], value="", inplace=True)
         else:
-             self._products = 'no data available'
+            self._products = 'no data available'
 
-            
-    def sh(self, product = None):
+    def sh(self, product=None):
         """        
         This function is a short cut to return the getSamplingHeight()        
         for documentation, please refer to .getSamplingHeight()
         """
         return self.getSamplingHeight(product)
-    
-    def getSamplingHeight(self, product = None):
+
+    def getSamplingHeight(self, product=None):
         """        
         a list of unique values for sampling heights for the specified data product
         in case of no sampling hights or the product is not found for this
         station, an empty list is returned.
         A short-cut function is defined .sh() which calls this function.
         
         Parameters
@@ -453,37 +468,37 @@
         Returns
         -------
         list, empty if sampling height for product is not found.
         
         """
         # default return empty list
         sh = ['']
-        
+
         # check if product is availabe for station
         if not product in self._data.values:
             return sh
-        
+
         # if product is available but no sampling height is defined, return
         # count returns zero, if no sampling heights found
         if not self._data['samplingheight'][self._data.specLabel.str.match(product)].count():
             return sh
-        
+
         # finally get all sampling heights and create a unique list        
-        sh = self._data.samplingheight[self._data.specLabel == product].unique()        
+        sh = self._data.samplingheight[self._data.specLabel == product].unique()
         sh = list(filter(None, sh))
         if not sh:
-            return['']
-        
+            return ['']
+
         # at this point we have to assume we have an unsorted list of
         # samplingheights as strings. cast to float and sort.
         sh = [float(s) for s in sh]
         sh.sort()
         return sh
-        
-        
+
+
 # --EOF Station Class-----------------------------------------            
 # ------------------------------------------------------------
 def get(stationId):
     """
     Parameters
     ----------
     stationId : str StationId as you can extract with getIdList. Example 'NOR'
@@ -491,117 +506,151 @@
     example :  get('NOR')
             
     Returns
     -------
     station : object Returns a station object (if stationId is found)
 
     """
-    
+
     # create the station instance
-    myStn = Station()  
-    
-    query = sparqls.getStations(stationId)    
-    stn = RunSparql(query,'pandas').run()
-    
+    myStn = Station()
+
+    query = sparqls.getStations(stationId)
+    stn = RunSparql(query, 'pandas').run()
+
     if not isinstance(stn, pd.DataFrame) or stn.empty:
         myStn.stationId = stationId
-        myStn.valid = False        
+        myStn.valid = False
         return myStn
     else:
-        stn['project'] = stn.apply(lambda x : __project(x['uri']), axis=1)
+        stn['project'] = stn.apply(lambda x: __project(x['uri']), axis=1)
 
     # we have found a valid id
     myStn.stationId = stn.id.values[0]
     myStn.valid = True
-    
+
     # it is possible that more than one station has the same id
     # we will give precedence to the icos project
     # but provide a list of URI and projects affiliations
-    
+
     # get lat, lon, eas from icos entry
     if not stn[stn.project.str.upper() == "ICOS"].empty:
         if stn.lat.any():
             myStn.lat = float(stn.lat[stn.project.str.upper() == 'ICOS'])
         if stn.lat.any():
             myStn.lon = float(stn.lon[stn.project.str.upper() == 'ICOS'])
         if stn.elevation.any():
             myStn.eas = float(stn.elevation[stn.project.str.upper() == 'ICOS'])
-    else: 
+    else:
         if stn.lat.any():
             myStn.lat = float(stn.lat.values[0])
         if stn.lon.any():
             myStn.lon = float(stn.lon.values[0])
         if stn.elevation.any():
             myStn.eas = float(stn.elevation.values[0])
-        
-    
+
     myStn.name = stn.name.iloc[0]
     myStn.country = stn.country.iloc[0]
     myStn.project = stn.project.tolist()
     myStn.uri = stn.uri.tolist()
-        
-    
+
     # if the station belongs to ICOS
     # add information from the labeling app.
     # this is an interim step and should be removed after the full meta data
     # flow from the thematic centres is achieved.        
-    
-    if 'ICOS' in myStn.project:            
+
+    if 'ICOS' in myStn.project:
         query = sparqls.stations_with_pi(stationId)
-        lstn = RunSparql(query,'pandas').run()
+        lstn = RunSparql(query, 'pandas').run()
         if not lstn.empty:
             myStn.theme = lstn['stationTheme'].values[0]
             myStn.icosclass = lstn['class'].values[0]
             myStn.icosclass = lstn['class'].values[0]
             myStn.firstName = lstn['firstName'].values[0]
             myStn.lastName = lstn['lastName'].values[0]
             myStn.email = lstn['email'].values[0]
             myStn.siteType = lstn['siteType'].values[0]
             myStn.eag = lstn['eag'].values[0]
 
-    #myStn._setData()        
+    # myStn._setData()
     return myStn
 
-    
-def getIdList(project='ICOS', sort='name'):
-    """
-    Returns a list with all station id's. By default only only ICOS stations
-    will be returned. If filter is set to 'all',  all known station id's are retured.
-    Please be aware, that the usage of data associated with non-ICOS station
-    might be different then the CCBY 4.0 Licence at ICOS.
+
+def getIdList(project='ICOS', sort='name', outfmt='pandas'):
+    """Retrieves a list of stations using a specific format.
+
+    Returns a list with all station id's. By default only ICOS stations
+    will be returned. If `project` is set to 'all', all known station
+    id's are returned. Please be aware, that the usage of data
+    associated with non-ICOS stations might be different than the
+    CCBY 4.0 Licence at ICOS.
 
     Parameters
     ----------
-    project : str, optional. The default is 'ICOS'. If you provide the
-                set project to "all" for all known stations
-                or provide a project name (see getIdList.project)                
-                             
-    sort : str, optional. The default is 'name'.
-    
+    project : str, optional
+        The default is 'ICOS'. If you set `project` to 'all', all known
+        stations are returned.
+
+    sort : str, optional
+        The default is 'name'. A user can `sort` by any of the
+        dataframe's columns: uri, id, name, country, lat, lon,
+        elevation, project, theme.
+
+    outfmt: str, optional
+        The default is 'pandas'. If you provide 'map' to the `outfmt`
+        argument a folium map is created with all known stations that
+        have valid longitude and latitude values. Be advised that in
+        this case, stations without a fixed location (like measurements
+        that belong to stations collected from instrumented Ships of
+        Opportunity) will not be included.
+
     Returns
     -------
-    Pandas data frame with station id's, name and country.
-    """    
-    
-    project = project.upper()
-    
-    query = sparqls.getStations()    
-    stn = RunSparql(query,'pandas').run()
+    queried_stations : pandas.Dataframe
+        `queried_stations` dataframe includes station id's, name,
+        country, and landing page (or uri) among others.
+
+    stations_map : folium.Map
+        `stations_map` is an interactive folium map with the available
+        stations provided by `project` argument.
+
+    Examples
+    --------
+    >>> stations_dataframe = getIdList(project='ICOS').head()
+    >>> print(stations_dataframe)
+            uri 	 id 	name 	...   elevation   project	theme
+    40 	http...  SE-Sto  Abis... 	... 	351.893      ICOS 	   ES
+    35 	http...  IT-Noe  Arca... 	... 	25.0 	     ICOS 	   ES
+    102 http...  UK-AMo  Auch... 	... 	270.0 	     ICOS 	   ES
+    48 	http...  FR-Aur  Aura...	... 	250.0 	     ICOS 	   ES
+    127 http...  1199 	 BE-F... 	... 	None 	     ICOS 	   OS
 
-    stn['project'] = stn.apply(lambda x : __project(x['uri']), axis=1)
-    stn['theme'] = stn.apply(lambda x: x['uri'].split('/')[-1].split('_')[0], axis=1)
-    
+    """
+
+    project = project.upper()
+    query = sparqls.getStations()
+    queried_stations = RunSparql(query, 'pandas').run()
+    queried_stations['project'] = queried_stations.apply(lambda x: __project(x['uri']), axis=1)
+    queried_stations['theme'] = queried_stations.apply(lambda x: x['uri'].
+                                                       split('/')[-1].split('_')[0], axis=1)
     if not project == 'ALL':
-        stn = stn[stn.project == project.upper()]
-    # we may have double entries....drop 
-    stn.drop
-    stn.sort_values(by=sort, inplace=True)
-    
-    return stn
-    
+        queried_stations = queried_stations[queried_stations.project == project.upper()]
+    # Drop any existing double entries.
+    queried_stations.drop
+    # Sort queried stations by the given sort argument if any.
+    queried_stations.sort_values(by=sort, inplace=True)
+
+    if outfmt == 'map' and not queried_stations.empty:
+        stations_folium_map = fmap.get(queried_stations, project)
+        return stations_folium_map
+
+    else:
+        return queried_stations
+
+
 def __project(uri):
     """
     internal use, do not call directly. Lambda function
     to apply on dataframe to get a column for 'project'
 
     Parameters
     ----------
@@ -610,28 +659,29 @@
     Returns 
     -------
     project : str, from predefined dict
 
     """
     uri = uri.lower().split('/')[-1].split('_')[0]
     project = {
-        'as' : "ICOS",
-        'es' : "ICOS",
-        'os' : "ICOS", 
-        'neon' : 'NEON', 
-        'ingos' : 'INGOS' ,   
-        'fluxnet' : 'FLUXNET'
-        }
-    
+        'as': "ICOS",
+        'es': "ICOS",
+        'os': "ICOS",
+        'neon': 'NEON',
+        'ingos': 'INGOS',
+        'fluxnet': 'FLUXNET'
+    }
+
     if uri in project:
         return project.get(uri)
     else:
         return 'other'
-    
-def getList(theme=['AS','ES','OS'], ids=None):
+
+
+def getList(theme=['AS', 'ES', 'OS'], ids=None):
     """
     Query the SPARQL endpoint for stations, create an object for each Station
     and return the list of stations.
     By default all (Ocean, Ecosystem, Atmosphere) ICOS stations are returned
     which have been certified (Class 1 & 2). 
     NOTE: if you provide a station list, all other parameters are ignored.
     
@@ -655,48 +705,49 @@
     stationIds : str | [iterable object of strings]) 
     
     Returns
     -------
     stationList : list of station objects
     
     """
-    
+
     stationList = []
-    
+
     # if a list of id's is provided, ignore theme and class.    
     if ids:
         for s in tqdm(ids):
             stationList.append(get(s))
-            
+
         return stationList
-    
-    defaulttheme=['AS','ES','OS']    
-    
+
+    defaulttheme = ['AS', 'ES', 'OS']
+
     # make sure input is a list and in uppercase    
-    
+
     if isinstance(theme, str):
         theme = [theme.upper()]
     elif isinstance(theme, list):
         theme = [x.upper() for x in theme]
     if not isinstance(theme, list) or not (set(defaulttheme) & set(theme)):
         # looks like input is not a theme.
         # Revert to default values, return all certified stations.
-        theme=defaulttheme
-    
+        theme = defaulttheme
+
     # get station list, by default returns all icos stations
     stations = getIdList()
     # filter by theme
     stations = stations[stations.theme.isin(theme)]
-    
-    
+
     stationList = []
     for s in tqdm(stations.id):
         stationList.append(get(s))
-            
+
     return stationList
+
+
 # ------------------------------------------------------------    
 if __name__ == "__main__":
     """
     execute only if run as a script
     get a full list from the CarbonPortal SPARQL endpoint
     and create a list of station objects    
     """
@@ -712,8 +763,9 @@
     myStation = station.get('NOR') 
     
     # return a list of station objects for all Ocean ICOS stations.
     stationList = station.getList(['OS']) 
     """
     print(msg)
 
+
 # ------------------------------------------------------------
```

### Comparing `icoscp-0.1.8/icoscp.egg-info/PKG-INFO` & `icoscp-0.1.9/icoscp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoscp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Access to ICOS data objects hosted at https://data.icos-cp.eu
 Home-page: https://www.icos-cp.eu/
 Author: Claudio D'Onofrio, Zois Zogopoulos, ICOS Carbon Portal
 Author-email: claudio.donofrio@nateko.lu.se, zois.zogopoulos@nateko.lu.se, info@icos-cp.eu
 License: GPLv3+
 Project-URL: Source, https://github.com/ICOS-Carbon-Portal/pylib
 Project-URL: Documentation, https://icos-carbon-portal.github.io/pylib/
@@ -36,15 +36,15 @@
 
 This package is under active development. Please be aware that changes to names of functions and classes are possible without further notice. Please do feedback any recommendations, issues, etc if you try it out.
 
 
 What is the package about?
 In essence this package allows you to have direct access to data objects from the ICOS CarbonPortal were a "Preview" is available. It is an easy access to data objects hosted at the ICOS Carbon Portal ( https://data.icos-cp.eu/ ). By using this library you can load data files directly into memory.
 
-Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://www.icos-cp.eu/data-services/about-data-portal/data-license" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
+Please be aware, that by either downloading data, or accessing data directly through this library, you agree and accept, that all ICOS data is provided under a <a href="https://data.icos-cp.eu/licence" target="_blank">CC BY 4.0 licence <img src="https://www.icos-cp.eu/sites/default/files/inline-images/creativecommons.png"></a>
 
 We would encourage you to use a virtual environment for python to test this library.
 For example with mini-conda (https://docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 
 - `conda create -n icos python`
 - `activate icos`
 - `pip install icoscp`
@@ -54,13 +54,7 @@
 
 
 
 
 
 
 
-
-
-
-cd20200720
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icoscp Version: 0.1.8 Summary: Access to ICOS data
+Metadata-Version: 2.1 Name: icoscp Version: 0.1.9 Summary: Access to ICOS data
 objects hosted at https://data.icos-cp.eu Home-page: https://www.icos-cp.eu/
 Author: Claudio D'Onofrio, Zois Zogopoulos, ICOS Carbon Portal Author-email:
 claudio.donofrio@nateko.lu.se, zois.zogopoulos@nateko.lu.se, info@icos-cp.eu
 License: GPLv3+ Project-URL: Source, https://github.com/ICOS-Carbon-Portal/
 pylib Project-URL: Documentation, https://icos-carbon-portal.github.io/pylib/
 Project-URL: DataPortal, https://data.icos-cp.eu/portal/ Project-URL:
 SparqlEndpoint, https://meta.icos-cp.eu/sparqlclient/?type=CSV Platform:
@@ -36,8 +36,8 @@
 library, you agree and accept, that all ICOS data is provided under a CC_BY_4.0
 licence_[https://www.icos-cp.eu/sites/default/files/inline-images/
 creativecommons.png] We would encourage you to use a virtual environment for
 python to test this library. For example with mini-conda (https://
 docs.conda.io/en/latest/miniconda.html) you can create a new environment with:
 - `conda create -n icos python` - `activate icos` - `pip install icoscp`
 Documentation about the library and all the modules are available at https://
-icos-carbon-portal.github.io/pylib/ cd20200720
+icos-carbon-portal.github.io/pylib/
```

### Comparing `icoscp-0.1.8/setup.py` & `icoscp-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
+
 def readme():
     try:
         with open('readme.md') as f:
             return f.read()
     except:
         pass
 
 setuptools.setup(
     name='icoscp',
-    version='0.1.8',
+    version='0.1.9',
 	license='GPLv3+',
     author="Claudio D'Onofrio, Zois Zogopoulos, ICOS Carbon Portal",
     author_email='claudio.donofrio@nateko.lu.se, zois.zogopoulos@nateko.lu.se, info@icos-cp.eu',
+    include_package_data=True,
     description='Access to ICOS data objects hosted at https://data.icos-cp.eu',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://www.icos-cp.eu/',
     project_urls={
             'Source':'https://github.com/ICOS-Carbon-Portal/pylib',
 			'Documentation':'https://icos-carbon-portal.github.io/pylib/',
```

