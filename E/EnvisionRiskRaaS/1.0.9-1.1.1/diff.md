# Comparing `tmp/envisionriskraas-1.0.9.tar.gz` & `tmp/envisionriskraas-1.1.1.tar.gz`

## Comparing `envisionriskraas-1.0.9.tar` & `envisionriskraas-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    86243 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0    86333 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/README.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/PKG-INFO
```

### Comparing `envisionriskraas-1.0.9/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.1.1/src/EnvisionRiskRaaS/RAAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #* the communication with the cloud server, and transform the JSON output
 #* from the API into Python data structures.
 
 import requests
 import json
 import os
 import datetime
-import maskpass
 import pandas as pd
 from typing import Dict
 from queue import Empty
 
 #******************************************************************************
 #### General API Functions - GET/POST                                      ####
 #******************************************************************************
```

### Comparing `envisionriskraas-1.0.9/LICENSE.txt` & `envisionriskraas-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.9/README.md` & `envisionriskraas-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.9/pyproject.toml` & `envisionriskraas-1.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.9"
-authors = [
-  { name="EnvisionRisk", email="support@envisionrisk.com" },
-]
+version = "1.1.1"
+authors = [{name="EnvisionRisk", email="support@envisionrisk.com" },{name="Coptolon",email="mark@brezina.dk"},]
+keywords = ["Risk-as-a-service","Market risk","Quantitative finance"]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [ "requests", "json", "os", "datetime", "pandas", "typing", "queue" ]
+
 [project.urls]
-"API webpage" = "https://www.linkedin.com/safety/go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D"
+"API webpage" = "https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management"
 "Homepage" = "https://www.envisionrisk.com/"
```

### Comparing `envisionriskraas-1.0.9/PKG-INFO` & `envisionriskraas-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.9
+Version: 1.1.1
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
-Project-URL: API webpage, https://www.linkedin.com/safety/go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D
+Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
-Author-email: EnvisionRisk <support@envisionrisk.com>
+Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
+Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: datetime
+Requires-Dist: json
+Requires-Dist: os
+Requires-Dist: pandas
+Requires-Dist: queue
+Requires-Dist: requests
+Requires-Dist: typing
 Description-Content-Type: text/markdown
 
 <h1>EnvisionRiskRaaS</h1>
 <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.1 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
-Project-URL: API webpage, https://www.linkedin.com/safety/
-go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-
-documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
-risk-management&trk=flagship-messaging-
-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-
-ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D
-Project-URL: Homepage, https://www.envisionrisk.com/ Author-email: EnvisionRisk
-envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
-Type: text/markdown
+Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-
+documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
+risk-management Project-URL: Homepage, https://www.envisionrisk.com/ Author-
+email: EnvisionRisk
+envisionrisk.com>, Coptolon
+brezina.dk> License-File: LICENSE.txt Keywords: Market risk,Quantitative
+finance,Risk-as-a-service Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Requires-Python: >=3.7 Requires-Dist: datetime Requires-Dist:
+json Requires-Dist: os Requires-Dist: pandas Requires-Dist: queue Requires-
+Dist: requests Requires-Dist: typing Description-Content-Type: text/markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
 without leaving your Python programming environment. Embrace this smarter,
```

