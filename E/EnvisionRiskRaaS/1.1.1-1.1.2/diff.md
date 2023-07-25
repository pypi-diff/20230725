# Comparing `tmp/envisionriskraas-1.1.1.tar.gz` & `tmp/envisionriskraas-1.1.2.tar.gz`

## Comparing `envisionriskraas-1.1.1.tar` & `envisionriskraas-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86243 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0    86333 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/README.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 envisionriskraas-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    86243 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/README.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/PKG-INFO
```

### Comparing `envisionriskraas-1.1.1/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.1.2/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.1/LICENSE.txt` & `envisionriskraas-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.1/README.md` & `envisionriskraas-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.1/PKG-INFO` & `envisionriskraas-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.1.1
+Version: 1.1.2
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
 Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
 Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: datetime
-Requires-Dist: json
-Requires-Dist: os
-Requires-Dist: pandas
-Requires-Dist: queue
-Requires-Dist: requests
-Requires-Dist: typing
+Requires-Python: >=3.11
+Requires-Dist: pandas>=2.0.3; python_version < '3.11'
+Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
+Requires-Dist: requests>=2.31.0; python_version < '3.11'
+Requires-Dist: typing>=3.10.0.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <h1>EnvisionRiskRaaS</h1>
 <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.2 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-
 documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
 risk-management Project-URL: Homepage, https://www.envisionrisk.com/ Author-
 email: EnvisionRisk
 envisionrisk.com>, Coptolon
 brezina.dk> License-File: LICENSE.txt Keywords: Market risk,Quantitative
 finance,Risk-as-a-service Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Requires-Python: >=3.7 Requires-Dist: datetime Requires-Dist:
-json Requires-Dist: os Requires-Dist: pandas Requires-Dist: queue Requires-
-Dist: requests Requires-Dist: typing Description-Content-Type: text/markdown
+:: Python :: 3 Requires-Python: >=3.11 Requires-Dist: pandas>=2.0.3;
+python_version < '3.11' Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
+Requires-Dist: requests>=2.31.0; python_version < '3.11' Requires-Dist:
+typing>=3.10.0.0; python_version < '3.11' Description-Content-Type: text/
+markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
 without leaving your Python programming environment. Embrace this smarter,
```

