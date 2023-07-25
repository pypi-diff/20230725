# Comparing `tmp/pyxecm-0.2.0.tar.gz` & `tmp/pyxecm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.2.0.tar", last modified: Fri Jul 21 13:57:32 2023, max compression
+gzip compressed data, was "pyxecm-0.3.0.tar", last modified: Tue Jul 25 06:37:51 2023, max compression
```

## Comparing `pyxecm-0.2.0.tar` & `pyxecm-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.891350 pyxecm-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-21 13:57:10.000000 pyxecm-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-21 13:57:32.891350 pyxecm-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-21 13:57:10.000000 pyxecm-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-21 13:57:22.000000 pyxecm-0.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.889351 pyxecm-0.2.0/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    59539 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/customizer.py
--rw-rw-rw-   0 root         (0) root         (0)    33679 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    77601 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256630 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   129336 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10227 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   289068 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5907 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/translate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.890350 pyxecm-0.2.0/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 13:57:32.891350 pyxecm-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-21 13:57:10.000000 pyxecm-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:37:51.396696 pyxecm-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-25 06:37:13.000000 pyxecm-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-25 06:37:51.395696 pyxecm-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-25 06:37:13.000000 pyxecm-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-07-25 06:37:38.000000 pyxecm-0.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:37:51.388696 pyxecm-0.3.0/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:37:51.394696 pyxecm-0.3.0/pyxecm/customizer/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    63588 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/customizer.py
+-rw-rw-rw-   0 root         (0) root         (0)    34896 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    79494 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)   289970 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/customizer/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:37:51.395696 pyxecm-0.3.0/pyxecm/helper/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/helper/assoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/helper/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    21847 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/helper/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)    11005 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   259638 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   133657 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-07-25 06:37:13.000000 pyxecm-0.3.0/pyxecm/otpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:37:51.390696 pyxecm-0.3.0/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-25 06:37:51.000000 pyxecm-0.3.0/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-25 06:37:51.000000 pyxecm-0.3.0/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 06:37:51.000000 pyxecm-0.3.0/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 06:37:51.000000 pyxecm-0.3.0/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-25 06:37:51.000000 pyxecm-0.3.0/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 06:37:51.396696 pyxecm-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-25 06:37:13.000000 pyxecm-0.3.0/setup.py
```

### Comparing `pyxecm-0.2.0/LICENSE` & `pyxecm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.2.0/PKG-INFO` & `pyxecm-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: customizer
 License-File: LICENSE
 
 # PYXECM
 
 A python library to interact with Opentext Extended ECM REST API. 
 API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
```

### Comparing `pyxecm-0.2.0/README.md` & `pyxecm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.2.0/pyproject.toml` & `pyxecm-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 
 [build-system]
   build-backend = "setuptools.build_meta"
   requires = ["setuptools >= 61.0"]
 
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
-  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "zipfile36", "suds"]
+  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "zipfile36", "suds", "python-hcl2", "lxml"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
   keywords = ["opentext", "extendedecm", "contentserver", "otds", "appworks", "archivecenter"]
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.2.0"
+  version = "0.3.0"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
     name = "Dr. Marc Diefenbruch"
 
+  [project.optional-dependencies]
+    customizer = ["python-hcl2", "lxml", "pyrfc"]
+
   [project.urls]
     Homepage = "https://ecm.glpages.otxlab.net/pyxecm/"
 
 [tool]
 
   [tool.setuptools]
-    packages = ["pyxecm"]
+    packages = ["pyxecm", "pyxecm.customizer", "pyxecm.helper"]
```

### Comparing `pyxecm-0.2.0/pyxecm/customizer.py` & `pyxecm-0.3.0/pyxecm/customizer/customizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,206 +25,229 @@
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import logging
 import os
 import sys
 import time
-from dataclasses import dataclass
+from dataclasses import dataclass, field, asdict
 from datetime import datetime
 
 import requests
+
 # OpenText specific modules:
 import yaml
-from pyxecm.k8s import K8s
-from pyxecm.m365 import M365
-from pyxecm.otac import OTAC
-from pyxecm.otcs import OTCS
-from pyxecm.otds import OTDS
-from pyxecm.otiv import OTIV
-from pyxecm.otpd import OTPD
+from pyxecm import OTAC, OTCS, OTDS, OTIV, OTPD
+from pyxecm.customizer.k8s import K8s
+from pyxecm.customizer.m365 import M365
+from pyxecm.customizer.payload import Payload
 
-logger = logging.getLogger("customizer")
+logger = logging.getLogger("pyxecm.customizer")
 
 
 @dataclass
 class CustomizerSettings:
     """Class to manage settings"""
 
-    placeholder_values = {}
-    stop_on_error = os.environ.get("LOGLEVEL", "INFO") == "DEBUG"
-    cust_log_file = "/tmp/customizing.log"
+    placeholder_values: dict = field(default_factory=dict)
+    stop_on_error: str = os.environ.get("LOGLEVEL", "INFO") == "DEBUG"
+    cust_log_file: str = "/tmp/customizing.log"
     customizer_start_time = customizer_end_time = datetime.now()
 
     # The following CUST artifacts are created by the main.tf in the python module:
-    cust_settings_dir = "/settings/"
-    cust_payload_dir = "/payload/"
-    cust_payload = cust_payload_dir + "payload.yaml"
-    cust_payload_external = "/payload-external/"
+    cust_settings_dir: str = "/settings/"
+    cust_payload_dir: str = "/payload/"
+    cust_payload: str = cust_payload_dir + "payload.yaml"
+    cust_payload_external: str = "/payload-external/"
 
-    cust_target_folder_nickname = (
+    cust_target_folder_nickname: str = (
         "deployment"  # nickname of folder to upload payload and log files
     )
     # CUST_RM_SETTINGS_DIR = "/opt/opentext/cs/appData/supportasset/Settings/"
     cust_rm_settings_dir = cust_settings_dir
 
 
 @dataclass
 class CustomizerSettingsOTDS:
     """Class for OTDS related settings"""
 
-    protocol = os.environ.get("OTDS_PROTOCOL", "http")
-    public_protocol = os.environ.get("OTDS_PUBLIC_PROTOCOL", "https")
-    hostname = os.environ.get("OTDS_HOSTNAME", "otds")
-    port = os.environ.get("OTDS_SERVICE_PORT_OTDS", 80)
-    admin = os.environ.get("OTDS_ADMIN", "admin")
-    admin_partition = "otds.admin"
-    public_url = os.environ.get("OTDS_PUBLIC_URL", "otds.xecm.dev")
-    password = os.environ.get("OTDS_PASSWORD", "Opentext1!")
+    protocol: str = os.environ.get("OTDS_PROTOCOL", "http")
+    public_protocol: str = os.environ.get("OTDS_PUBLIC_PROTOCOL", "https")
+    hostname: str = os.environ.get("OTDS_HOSTNAME", "otds")
+    port: int = os.environ.get("OTDS_SERVICE_PORT_OTDS", 80)
+    username: str = os.environ.get("OTDS_ADMIN", "admin")
+    admin_partition: str = "otds.admin"
+    public_url: str = os.environ.get("OTDS_PUBLIC_URL", "otds.xecm.dev")
+    password: str = os.environ.get("OTDS_PASSWORD", "Opentext1!")
 
 
 @dataclass
 class CustomizerSettingsOTCS:
     """Class for OTCS related settings"""
 
     # Content Server Constants:
-    protocol = os.environ.get("OTCS_PROTOCOL", "http")
-    public_protocol = os.environ.get("OTCS_PUBLIC_PROTOCOL", "https")
-    hostname = hostname_backend = os.environ.get("OTCS_HOSTNAME", "otcs-admin-0")
-    hostname_frontend = os.environ.get("OTCS_HOSTNAME_FRONTEND", "otcs-frontend")
-    public_url = os.environ.get("OTCS_PUBLIC_URL", "otcs.xecm.dev")
-    port = port_backend = os.environ.get("OTCS_SERVICE_PORT_OTCS", 8080)
-    port_frontend = 80
-    admin = os.environ.get("OTCS_ADMIN", "admin")
-    password = os.environ.get("OTCS_PASSWORD", "Opentext1!")
-    partition = os.environ.get("OTCS_PARTITION", "Content Server Members")
-    resource_name = "cs"
-    k8s_statefulset_frontend = "otcs-frontend"
-    k8s_statefulset_backend = "otcs-admin"
-    k8s_ingress = "otxecm-ingress"
-    maintenance_mode = os.environ.get("OTCS_MAINTENANCE_MODE", "true").lower() == "true"
-    license_feature = "X3"
+    protocol: str = os.environ.get("OTCS_PROTOCOL", "http")
+    public_protocol: str = os.environ.get("OTCS_PUBLIC_PROTOCOL", "https")
+    hostname: str = os.environ.get("OTCS_HOSTNAME", "otcs-admin-0")
+    hostname_backend: str = os.environ.get("OTCS_HOSTNAME", "otcs-admin-0")
+    hostname_frontend: str = os.environ.get("OTCS_HOSTNAME_FRONTEND", "otcs-frontend")
+    public_url: str = os.environ.get("OTCS_PUBLIC_URL", "otcs.xecm.dev")
+    port: int = os.environ.get("OTCS_SERVICE_PORT_OTCS", 8080)
+    port_backend: int = os.environ.get("OTCS_SERVICE_PORT_OTCS", 8080)
+    port_frontend: int = 80
+    admin: str = os.environ.get("OTCS_ADMIN", "admin")
+    password: str = os.environ.get("OTCS_PASSWORD", "Opentext1!")
+    partition: str = os.environ.get("OTCS_PARTITION", "Content Server Members")
+    resource_name: str = "cs"
+    k8s_statefulset_frontend: str = "otcs-frontend"
+    k8s_statefulset_backend: str = "otcs-admin"
+    k8s_ingress: str = "otxecm-ingress"
+    maintenance_mode: str = (
+        os.environ.get("OTCS_MAINTENANCE_MODE", "true").lower() == "true"
+    )
+    license_feature: str = "X3"
 
     # K8s service name for maintenance pod
-    maintenance_service_name = "maintenance"
-    mainteance_service_port = 80  # K8s service name for maintenance pod
+    maintenance_service_name: str = "maintenance"
+    mainteance_service_port: int = 80  # K8s service name for maintenance pod
 
     replicas_frontend = 0
     replicas_backend = 0
 
 
 @dataclass
 class CustomizerSettingsOTAC:
     """Class for OTAC related settings"""
 
-    enabled = os.environ.get("OTAC_ENABLED", True)
-    hostname = os.environ.get("OTAC_SERVICE_HOST", "otac-0")
-    port = os.environ.get("OTAC_SERVICE_PORT", 8080)
-    protocol = os.environ.get("OTAC_PROTOCOL", "http")
-    public_url = os.environ.get("OTAC_PUBLIC_URL", "otcs.xecm.dev")
-    admin = os.environ.get("OTAC_ADMIN", "dsadmin")
-    password = os.environ.get("OTAC_PASSWORD", "")
-    known_server = os.environ.get("OTAC_KNOWN_SERVER", "")
-    k8s_pod_name = "otac-0"
+    enabled: str = os.environ.get("OTAC_ENABLED", "true")
+    hostname: str = os.environ.get("OTAC_SERVICE_HOST", "otac-0")
+    port: int = os.environ.get("OTAC_SERVICE_PORT", 8080)
+    protocol: str = os.environ.get("OTAC_PROTOCOL", "http")
+    public_url: str = os.environ.get("OTAC_PUBLIC_URL", "otcs.xecm.dev")
+    admin: str = os.environ.get("OTAC_ADMIN", "dsadmin")
+    password: str = os.environ.get("OTAC_PASSWORD", "")
+    known_server: str = os.environ.get("OTAC_KNOWN_SERVER", "")
+    k8s_pod_name: str = "otac-0"
 
 
 @dataclass
 class CustomizerSettingsOTPD:
     """Class for OTPD related settings"""
 
-    enabled = os.environ.get("OTPD_ENABLED", False)
-    hostname = os.environ.get("OTPD_SERVICE_HOST", "otpd")
-    port = os.environ.get("OTPD_SERVICE_PORT", 8080)
-    protocol = os.environ.get("OTPD_PROTOCOL", "http")
-    db_importfile = os.environ.get(
+    enabled: str = os.environ.get("OTPD_ENABLED", "false")
+    hostname: str = os.environ.get("OTPD_SERVICE_HOST", "otpd")
+    port: int = os.environ.get("OTPD_SERVICE_PORT", 8080)
+    protocol: str = os.environ.get("OTPD_PROTOCOL", "http")
+    db_importfile: str = os.environ.get(
         "OTPD_DBIMPORTFILE", "URL://url.download.location/file.zip"
     )
-    tenant = os.environ.get("OTPD_TENANT", "Successfactors")
-    user = os.environ.get("OTPD_USER", "powerdocsapiuser")
-    password = os.environ.get("OTPD_PASSWORD", "Opentext1!")
-    k8s_pod_name = "otpd-0"
+    tenant: str = os.environ.get("OTPD_TENANT", "Successfactors")
+    user: str = os.environ.get("OTPD_USER", "powerdocsapiuser")
+    password: str = os.environ.get("OTPD_PASSWORD", "Opentext1!")
+    k8s_pod_name: str = "otpd-0"
 
 
 @dataclass
 class CustomizerSettingsOTIV:
     """Class for OTIV related settings"""
 
-    enabled = os.environ.get("OTIV_ENABLED", False)
-    license_file = "/payload/otiv-license.lic"
-    license_feature = "FULLTIME_USERS_REGULAR"
-    product_name = "Viewing"
-    product_description = "OpenText Intelligent Viewing"
-    resource_name = "iv"
+    enabled: str = os.environ.get("OTIV_ENABLED", "false")
+    license_file: str = "/payload/otiv-license.lic"
+    license_feature: str = "FULLTIME_USERS_REGULAR"
+    product_name: str = "Viewing"
+    product_description: str = "OpenText Intelligent Viewing"
+    resource_name: str = "iv"
+
+
+@dataclass
+class CustomizerSettingsK8S:
+    """Class for K8s related settings"""
+
+    enabled: bool = os.environ.get("K8S_ENABLED", "true").lower() == "true"
+    in_cluster: bool = True
+    kubeconfig_file: str = "~/.kube/config"
+    namespace: str = "default"
 
 
 @dataclass
 class CustomizerSettingsOTAWP:
     """Class for OTAWP related settings"""
 
-    enabled = os.environ.get("OTAWP_ENABLED", False)
-    resource_name = "awp"
-    access_role_name = "Access to " + resource_name
-    admin = os.environ.get("OTAWP_ADMIN", "sysadmin")
-    password = os.environ.get("OTAWP_PASSWORD", "Opentext1!")
-    public_protocol = os.environ.get("OTAWP_PROTOCOL", "https")
-    public_url = os.environ.get("OTAWP_PUBLIC_URL", "otawp.xecm.dev")
-    k8s_statefulset = "appworks"
-    k8s_configmap = "appworks-config-ymls"
+    enabled: str = os.environ.get("OTAWP_ENABLED", "false")
+    resource_name: str = "awp"
+    access_role_name: str = "Access to " + resource_name
+    admin: str = os.environ.get("OTAWP_ADMIN", "sysadmin")
+    password: str = os.environ.get("OTAWP_PASSWORD", "Opentext1!")
+    public_protocol: str = os.environ.get("OTAWP_PROTOCOL", "https")
+    public_url: str = os.environ.get("OTAWP_PUBLIC_URL", "otawp.xecm.dev")
+    k8s_statefulset: str = "appworks"
+    k8s_configmap: str = "appworks-config-ymls"
 
 
 @dataclass
-class CustomizerSettingsO365:
+class CustomizerSettingsM365:
     """Class for O365 related settings"""
 
-    enabled = os.environ.get("O365_ENABLED", False)
+    enabled: str = os.environ.get("O365_ENABLED", "false")
     """Enable/Disable the O365 Customization"""
-    tenant_id = os.environ.get("O365_TENANT_ID", "")
-    client_id = os.environ.get("O365_CLIENT_ID", "")
-    client_secret = os.environ.get("O365_CLIENT_SECRET", "")
-    user = os.environ.get("O365_USER", "")
-    password = os.environ.get("O365_PASSWORD", "")
-    domain = os.environ.get("O365_DOMAIN", "")
-    sku_id = os.environ.get("O365_SKU_ID", "c7df2760-2c81-4ef7-b578-5b5392b571df")
+    tenant_id: str = os.environ.get("O365_TENANT_ID", "")
+    client_id: str = os.environ.get("O365_CLIENT_ID", "")
+    client_secret: str = os.environ.get("O365_CLIENT_SECRET", "")
+    user: str = os.environ.get("O365_USER", "")
+    password: str = os.environ.get("O365_PASSWORD", "")
+    domain: str = os.environ.get("O365_DOMAIN", "")
+    sku_id: str = os.environ.get("O365_SKU_ID", "c7df2760-2c81-4ef7-b578-5b5392b571df")
     """Office 365 E5, used as default SKU for users (c7df2760-2c81-4ef7-b578-5b5392b571df)"""
-    teams_app_name = "OpenText Extended ECM"
+    teams_app_name: str = "OpenText Extended ECM"
     """Name of the Microsoft Teams App (OpenText Extended ECM)"""
 
 
 class Customizer:
     """Customizer Class to control the cusomization automation
 
     Args: None
     """
 
-    def __init__(self):
-        self.settings = CustomizerSettings()
+    def __init__(
+        self,
+        settings: CustomizerSettings = CustomizerSettings(),
+        otds: CustomizerSettingsOTDS = CustomizerSettingsOTDS(),
+        otcs: CustomizerSettingsOTCS = CustomizerSettingsOTCS(),
+        otac: CustomizerSettingsOTAC = CustomizerSettingsOTAC(),
+        otpd: CustomizerSettingsOTPD = CustomizerSettingsOTPD(),
+        otiv: CustomizerSettingsOTIV = CustomizerSettingsOTIV(),
+        k8s: CustomizerSettingsK8S = CustomizerSettingsK8S(),
+        otawp: CustomizerSettingsOTAWP = CustomizerSettingsOTAWP(),
+        m365: CustomizerSettingsM365 = CustomizerSettingsM365(),
+    ):
+        self.settings = settings
 
         # OTDS Constants:
-        self.otds = CustomizerSettingsOTDS()
+        self.otds_settings = otds
 
         # Content Server Constants:
-        self.otcs = CustomizerSettingsOTCS()
+        self.otcs_settings = otcs
 
         # Archive Center constants:
-        self.otac = CustomizerSettingsOTAC()
+        self.otac_settings = otac
 
         # PowerDocs constants:
-        self.otpd = CustomizerSettingsOTPD()
+        self.otpd_settings = otpd
 
         # Intelligent Viewing constants:
-        self.otiv = CustomizerSettingsOTIV()
+        self.otiv_settings = otiv
 
         # AppWorks Platform constants:
-        self.otawp = CustomizerSettingsOTAWP()
+        self.otawp_settings = otawp
 
         # K8s Mode
-        self.k8s_enabled = os.environ.get("K8S_ENABLED", "true").lower() == "true"
+        self.k8s_settings = k8s
 
         # Microsoft 365 Environment variables:
-        self.o365 = CustomizerSettingsO365()
+        self.m365_settings = m365
 
         # Initialize Objects for later assignment
         self.otds_object: OTDS
         self.otcs_object: OTCS
         self.otcs_backend_object: OTCS
         self.otcs_frontend_object: OTCS
         self.otpd_object: OTPD | None
@@ -239,104 +262,114 @@
         Args:
             None
         Returns:
             object: M365 object or None if the object couldn't be created or
                     the authentication fails.
         """
 
-        logger.info("Microsoft 365 Tenant ID             = %s", self.o365.tenant_id)
-        logger.info("Microsoft 365 Client ID             = %s", self.o365.client_id)
+        logger.info(
+            "Microsoft 365 Tenant ID             = %s", self.m365_settings.tenant_id
+        )
+        logger.info(
+            "Microsoft 365 Client ID             = %s", self.m365_settings.client_id
+        )
         logger.debug(
-            "Microsoft 365 Client Secret         = %s", self.o365.client_secret
+            "Microsoft 365 Client Secret         = %s", self.m365_settings.client_secret
         )
         logger.info(
             "Microsoft 365 User                  = %s",
-            (self.o365.user if self.o365.user != "" else "<not configured>"),
+            (
+                self.m365_settings.user
+                if self.m365_settings.user != ""
+                else "<not configured>"
+            ),
         )
         logger.debug(
             "Microsoft 365 Password              = %s",
-            (self.o365.password if self.o365.password != "" else "<not configured>"),
+            (
+                self.m365_settings.password
+                if self.m365_settings.password != ""
+                else "<not configured>"
+            ),
         )
-        logger.info("Microsoft 365 Domain                = %s", self.o365.domain)
-        logger.info("Microsoft 365 Default License SKU   = %s", self.o365.sku_id)
         logger.info(
-            "Microsoft 365 Teams App             = %s", self.o365.teams_app_name
+            "Microsoft 365 Domain                = %s", self.m365_settings.domain
         )
-
-        m365_object = M365(
-            self.o365.tenant_id,
-            self.o365.client_id,
-            self.o365.client_secret,
-            self.o365.domain,
-            self.o365.sku_id,
-            self.o365.teams_app_name,
+        logger.info(
+            "Microsoft 365 Default License SKU   = %s", self.m365_settings.sku_id
+        )
+        logger.info(
+            "Microsoft 365 Teams App             = %s",
+            self.m365_settings.teams_app_name,
         )
 
+        m365_object = M365(**asdict(self.m365_settings))
+
         if m365_object and m365_object.authenticate():
             logger.info("Connected to Microsoft Graph API.")
             return m365_object
         else:
             logger.error("Failed to connect to Microsoft Graph API.")
             return m365_object
 
         # end function definition
 
-    def init_k8s(self, in_cluster: bool = True) -> K8s:
+    def init_k8s(self, in_cluster: bool = True, **kwargs) -> K8s:
         """Initialize the Kubernetes object we use to talk to the Kubernetes API.
 
         Args:
             inCluster (boolean): controls wether the code runs inside a pod (inCluster = True)
                                 or locally (access via .kube / kubectl, inCluster = False)
         Return:
             K8s object
             The global variables otcs_replicas_frontend and otcs_replicas_backend are initialized
         """
 
         logger.info("Connect to Kubernetes, inCluster -> %s", in_cluster)
 
-        k8s_object = K8s(in_cluster)
+        k8s_object = K8s(in_cluster=in_cluster, **kwargs)
         if k8s_object:
             logger.info("Kubernetes API is ready now.")
         else:
             logger.error("Cannot establish connection to Kubernetes.")
 
         # Get number of replicas for frontend:
-        otcs_frontend_scale = k8s_object.getStatefulSetScale(
-            self.otcs.k8s_statefulset_frontend
+        otcs_frontend_scale = k8s_object.get_stateful_set_scale(
+            self.otcs_settings.k8s_statefulset_frontend
         )
         if not otcs_frontend_scale:
             logger.error(
                 "Cannot find Kubernetes Stateful Set for OTCS Frontends -> %s",
-                self.otcs.k8s_statefulset_frontend,
+                self.otcs_settings.k8s_statefulset_frontend,
             )
             sys.exit()
 
-        self.otcs.replicas_frontend = otcs_frontend_scale.spec.replicas  # type: ignore
+        self.otcs_settings.replicas_frontend = otcs_frontend_scale.spec.replicas  # type: ignore
         logger.info(
             "Stateful Set -> %s has -> %s replicas",
-            self.otcs.k8s_statefulset_frontend,
-            self.otcs.replicas_frontend,
+            self.otcs_settings.k8s_statefulset_frontend,
+            self.otcs_settings.replicas_frontend,
         )
 
         # Get number of replicas for backend:
-        otcs_backend_scale = k8s_object.getStatefulSetScale(
-            self.otcs.k8s_statefulset_backend
+        otcs_backend_scale = k8s_object.get_stateful_set_scale(
+            self.otcs_settings.k8s_statefulset_backend
         )
         if not otcs_backend_scale:
             logger.error(
                 "Cannot find Kubernetes Stateful Set for OTCS Backends -> %s",
-                self.otcs.k8s_statefulset_backend,
+                self.otcs_settings.k8s_statefulset_backend,
             )
             sys.exit()
 
-        self.otcs.replicas_backend = otcs_backend_scale.spec.replicas  # type: ignore
+        self.otcs_settings.replicas_backend = otcs_backend_scale.spec.replicas  # type: ignore
         logger.info(
             "Stateful Set -> %s has -> %s replicas",
-            self.otcs.k8s_statefulset_backend,
-            self.otcs.replicas_backend,
+            self.otcs_settings.k8s_statefulset_backend,
+            self.otcs_settings.replicas_backend,
         )
 
         return k8s_object
 
         # end function definition
 
     def init_otds(self) -> OTDS:
@@ -345,41 +378,35 @@
         Args:
             None
         Returns:
             object: OTDS object
         """
 
         logger.info("Connection parameters OTDS:")
-        logger.info("OTDS Protocol          = %s", self.otds.protocol)
-        logger.info("OTDS Public Protocol   = %s", self.otds.public_protocol)
-        logger.info("OTDS Hostname          = %s", self.otds.hostname)
-        logger.info("OTDS Public URL        = %s", self.otds.public_url)
-        logger.info("OTDS Port              = %s", str(self.otds.port))
-        logger.info("OTDS Admin User        = %s", self.otds.admin)
-        logger.debug("OTDS Admin Password   = %s", self.otds.password)
-        logger.info("OTDS Admin Partition   = %s", self.otds.admin_partition)
-
-        otds_object = OTDS(
-            self.otds.protocol,
-            self.otds.hostname,
-            int(self.otds.port),
-            self.otds.admin,
-            self.otds.password,
-        )
+        logger.info("OTDS Protocol          = %s", self.otds_settings.protocol)
+        logger.info("OTDS Public Protocol   = %s", self.otds_settings.public_protocol)
+        logger.info("OTDS Hostname          = %s", self.otds_settings.hostname)
+        logger.info("OTDS Public URL        = %s", self.otds_settings.public_url)
+        logger.info("OTDS Port              = %s", str(self.otds_settings.port))
+        logger.info("OTDS Admin User        = %s", self.otds_settings.username)
+        logger.debug("OTDS Admin Password   = %s", self.otds_settings.password)
+        logger.info("OTDS Admin Partition   = %s", self.otds_settings.admin_partition)
+
+        otds_object = OTDS(**asdict(self.otds_settings))
 
         logger.info("Authenticating to OTDS...")
         otds_cookie = otds_object.authenticate()
         while otds_cookie is None:
             logger.warning("Waiting 30 seconds for OTDS to become ready...")
             time.sleep(30)
             otds_cookie = otds_object.authenticate()
         logger.info("OTDS is ready now.")
 
         logger.info("Enable OTDS audit...")
-        otds_object.enableAudit()
+        otds_object.enable_audit()
 
         return otds_object
 
         # end function definition
 
     def init_otac(self) -> OTAC:
         """Initialize the OTAC object and parameters.
@@ -388,55 +415,55 @@
 
         Args: None
         Return:
             OTAC object
         """
 
         logger.info("Connection parameters OTAC:")
-        logger.info("OTAC Protocol          = %s", self.otac.protocol)
-        logger.info("OTAC Hostname          = %s", self.otac.hostname)
-        logger.info("OTAC Public URL        = %s", self.otac.public_url)
-        logger.info("OTAC Port              = %s", str(self.otac.port))
-        logger.info("OTAC Admin User        = %s", self.otac.admin)
-        logger.debug("OTAC Admin Password   = %s", self.otac.password)
+        logger.info("OTAC Protocol          = %s", self.otac_settings.protocol)
+        logger.info("OTAC Hostname          = %s", self.otac_settings.hostname)
+        logger.info("OTAC Public URL        = %s", self.otac_settings.public_url)
+        logger.info("OTAC Port              = %s", str(self.otac_settings.port))
+        logger.info("OTAC Admin User        = %s", self.otac_settings.admin)
+        logger.debug("OTAC Admin Password   = %s", self.otac_settings.password)
         logger.info(
             "OTAC Known Server      = %s",
             (
-                self.otac.known_server
-                if self.otac.known_server != ""
+                self.otac_settings.known_server
+                if self.otac_settings.known_server != ""
                 else "<not configured>"
             ),
         )
 
         otac_object = OTAC(
-            self.otac.protocol,
-            self.otac.hostname,
-            int(self.otac.port),
-            self.otac.admin,
-            self.otac.password,
-            self.otds.admin,
-            self.otds.password,
+            self.otac_settings.protocol,
+            self.otac_settings.hostname,
+            int(self.otac_settings.port),
+            self.otac_settings.admin,
+            self.otac_settings.password,
+            self.otds_settings.username,
+            self.otds_settings.password,
         )
 
         # is there a known server configured for Archive Center (to sync content with)
-        if otac_object and self.otac.known_server != "":
+        if otac_object and self.otac_settings.known_server != "":
             # wait until the OTAC pod is in ready state
             logger.info("Waiting for Archive Center to become ready...")
-            self.k8s_object.waitPodCondition(self.otac.k8s_pod_name, "Ready")
+            self.k8s_object.wait_pod_condition(self.otac_settings.k8s_pod_name, "Ready")
 
             logger.info("Configure known host for Archive Center...")
-            response = otac_object.execCommand(
-                f"cf_create_host {self.otac.known_server} 0 /archive 8080 8090"
+            response = otac_object.exec_command(
+                f"cf_create_host {self.otac_settings.known_server} 0 /archive 8080 8090"
             )
             if not response or not response.ok:
                 logger.error("Failed to configure known host for Archive Center!")
 
             logger.info("Configure host alias for Archive Center...")
-            response = otac_object.execCommand(
-                f"cf_set_variable MY_HOST_ALIASES {self.otac.k8s_pod_name},{self.otac.public_url},otac DS"
+            response = otac_object.exec_command(
+                f"cf_set_variable MY_HOST_ALIASES {self.otac_settings.k8s_pod_name},{self.otac_settings.public_url},otac DS"
             )
             if not response or not response.ok:
                 logger.error("Failed to configure host alias for Archive Center!")
 
             # Restart the spawner in Archive Center:
             logger.info("Restart Archive Center Spawner...")
             self.restart_otac_service()
@@ -464,129 +491,135 @@
             partition_name: name of OTDS Partition for Extended ECM users
             resource_name: name of OTDS resource for Extended ECM
         Returns:
             object: OTCS object
         """
 
         logger.info("Connection parameters OTCS (Extended ECM):")
-        logger.info("OTCS Protocol              = %s", self.otcs.protocol)
-        logger.info("OTCS Public Protocol       = %s", self.otcs.public_protocol)
+        logger.info("OTCS Protocol              = %s", self.otcs_settings.protocol)
+        logger.info(
+            "OTCS Public Protocol       = %s", self.otcs_settings.public_protocol
+        )
         logger.info("OTCS Hostname              = %s", hostname)
-        logger.info("OTCS Public URL            = %s", self.otcs.public_url)
+        logger.info("OTCS Public URL            = %s", self.otcs_settings.public_url)
         logger.info("OTCS Port                  = %s", str(port))
-        logger.info("OTCS Admin User            = %s", self.otcs.admin)
-        logger.debug("OTCS Admin Password       = %s", self.otcs.password)
+        logger.info("OTCS Admin User            = %s", self.otcs_settings.admin)
+        logger.debug("OTCS Admin Password       = %s", self.otcs_settings.password)
         logger.info("OTCS User Partition        = %s", partition_name)
         logger.info("OTCS Resource Name         = %s", resource_name)
-        logger.info("OTCS User Default License  = %s", self.otcs.license_feature)
         logger.info(
-            "OTCS K8s Frontend Pods     = %s", self.otcs.k8s_statefulset_frontend
+            "OTCS User Default License  = %s", self.otcs_settings.license_feature
+        )
+        logger.info(
+            "OTCS K8s Frontend Pods     = %s",
+            self.otcs_settings.k8s_statefulset_frontend,
         )
         logger.info(
-            "OTCS K8s Backend Pods      = %s", self.otcs.k8s_statefulset_backend
+            "OTCS K8s Backend Pods      = %s",
+            self.otcs_settings.k8s_statefulset_backend,
         )
 
         otcs_object = OTCS(
-            self.otcs.protocol,
+            self.otcs_settings.protocol,
             hostname,
             int(port),
-            self.otcs.admin,
-            self.otcs.password,
+            self.otcs_settings.admin,
+            self.otcs_settings.password,
             partition_name,
             resource_name,
         )
 
         # It is important to wait for OTCS to be configured - otherwise we
         # may interfere with the OTCS container automation and run into errors
         logger.info("Wait for OTCS to be configured...")
-        otcs_configured = otcs_object.isConfigured()
+        otcs_configured = otcs_object.is_configured()
         while not otcs_configured:
             logger.warning("OTCS is not configured yet. Waiting 30 seconds...")
             time.sleep(30)
-            otcs_configured = otcs_object.isConfigured()
+            otcs_configured = otcs_object.is_configured()
         logger.info("OTCS is configured now.")
 
         logger.info("Authenticating to OTCS...")
         otcs_cookie = otcs_object.authenticate()
         while otcs_cookie is None:
             logger.warning("Waiting 30 seconds for OTCS to become ready...")
             time.sleep(30)
             otcs_cookie = otcs_object.authenticate()
         logger.info("OTCS is ready now.")
 
         # Set first name and last name of Admin user (ID = 1000):
-        otcs_object.updateUser(1000, field="first_name", value="Terrarium")
-        otcs_object.updateUser(1000, field="last_name", value="Admin")
+        otcs_object.update_user(1000, field="first_name", value="Terrarium")
+        otcs_object.update_user(1000, field="last_name", value="Admin")
 
         if "OTCS_RESSOURCE_ID" not in self.settings.placeholder_values:
             self.settings.placeholder_values[
                 "OTCS_RESSOURCE_ID"
-            ] = self.otds_object.getResource(self.otcs.resource_name)["resourceID"]
+            ] = self.otds_object.get_resource(self.otcs_settings.resource_name)[
+                "resourceID"
+            ]
             logger.debug(
                 "Placeholder values after OTCS init = %s",
                 self.settings.placeholder_values,
             )
 
-        if self.otawp.enabled == "true":
-            otcs_resource = self.otds_object.getResource(self.otcs.resource_name)
+        if self.otawp_settings.enabled == "true":
+            otcs_resource = self.otds_object.get_resource(
+                self.otcs_settings.resource_name
+            )
             otcs_resource[
                 "logoutURL"
-            ] = f"{self.otawp.public_protocol}://{self.otawp.public_url}/home/system/wcp/sso/sso_logout.htm"
+            ] = f"{self.otawp_settings.public_protocol}://{self.otawp_settings.public_url}/home/system/wcp/sso/sso_logout.htm"
             otcs_resource["logoutMethod"] = "GET"
 
-            self.otds_object.updateResource(name="cs", resource=otcs_resource)
+            self.otds_object.update_resource(name="cs", resource=otcs_resource)
 
         # Allow impersonation of the resource for all users:
-        self.otds_object.impersonateResource(resource_name)
+        self.otds_object.impersonate_resource(resource_name)
 
         return otcs_object
 
         # end function definition
 
     def init_otiv(self) -> OTIV:
         """Initialize the OTIV (Intelligent Viewing) object and its OTDS settings.
 
         Args:
         Returns:
             objects: OTIV object
         """
 
         logger.info("Parameters for OTIV (Intelligent Viewing):")
-        logger.info("OTDS Resource Name       = %s", self.otiv.resource_name)
-        logger.info("OTIV License File        = %s", self.otiv.license_file)
-        logger.info("OTIV Product Name        = %s", self.otiv.product_name)
-        logger.info("OTIV Product Description = %s", self.otiv.product_description)
-        logger.info("OTIV License Feature     = %s", self.otiv.license_feature)
-
-        otiv_object = OTIV(
-            self.otiv.resource_name,
-            self.otiv.product_name,
-            self.otiv.product_description,
-            self.otiv.license_file,
-            self.otiv.license_feature,
+        logger.info("OTDS Resource Name       = %s", self.otiv_settings.resource_name)
+        logger.info("OTIV License File        = %s", self.otiv_settings.license_file)
+        logger.info("OTIV Product Name        = %s", self.otiv_settings.product_name)
+        logger.info(
+            "OTIV Product Description = %s", self.otiv_settings.product_description
         )
+        logger.info("OTIV License Feature     = %s", self.otiv_settings.license_feature)
+
+        otiv_object = OTIV(**asdict(self.otiv_settings))
 
-        otds_resource = self.otds_object.getResource(self.otiv.resource_name)
+        otds_resource = self.otds_object.get_resource(self.otiv_settings.resource_name)
         if not otds_resource:
             logger.error(
                 "OTDS Resource -> {} for Intelligent Viewing not found. OTIV may not be ready."
             )
             sys.exit()
 
-        otiv_license = self.otds_object.addLicenseToResource(
-            self.otiv.license_file,
-            self.otiv.product_name,
-            self.otiv.product_description,
+        otiv_license = self.otds_object.add_license_to_resource(
+            self.otiv_settings.license_file,
+            self.otiv_settings.product_name,
+            self.otiv_settings.product_description,
             otds_resource["resourceID"],
         )
         if not otiv_license:
             logger.info(
                 "Couldn't apply license -> %s for product -> %s. Intelligent Viewing may not be deployed!",
-                self.otiv.license_file,
-                self.otiv.product_name,
+                self.otiv_settings.license_file,
+                self.otiv_settings.product_name,
             )
             sys.exit()
 
         return otiv_object
 
         # end function definition
 
@@ -596,95 +629,97 @@
         Args:
             None
         Returns:
             object: OTPD (PowerDocs) object
         """
 
         logger.info("Connection parameters OTPD (PowerDocs):")
-        logger.info("OTPD Protocol             = %s", self.otpd.protocol)
-        logger.info("OTPD Hostname             = %s", self.otpd.hostname)
-        logger.info("OTPD Port                 = %s", str(self.otpd.port))
-        logger.info("OTPD API User             = %s", self.otpd.user)
-        logger.info("OTPD Tenant               = %s", self.otpd.tenant)
+        logger.info("OTPD Protocol             = %s", self.otpd_settings.protocol)
+        logger.info("OTPD Hostname             = %s", self.otpd_settings.hostname)
+        logger.info("OTPD Port                 = %s", str(self.otpd_settings.port))
+        logger.info("OTPD API User             = %s", self.otpd_settings.user)
+        logger.info("OTPD Tenant               = %s", self.otpd_settings.tenant)
         logger.info(
             "OTPD Database Import File = %s",
             (
-                self.otpd.db_importfile
-                if self.otpd.db_importfile != ""
+                self.otpd_settings.db_importfile
+                if self.otpd_settings.db_importfile != ""
                 else "<not configured>"
             ),
         )
-        logger.info("OTPD K8s Pod Name         = %s", self.otpd.k8s_pod_name)
+        logger.info("OTPD K8s Pod Name         = %s", self.otpd_settings.k8s_pod_name)
 
         otpd_object = OTPD(
-            self.otpd.protocol,
-            self.otpd.hostname,
-            int(self.otpd.port),
-            self.otpd.user,
-            self.otpd.password,
+            self.otpd_settings.protocol,
+            self.otpd_settings.hostname,
+            int(self.otpd_settings.port),
+            self.otpd_settings.user,
+            self.otpd_settings.password,
         )
 
         # wait until the OTPD pod is in ready state
-        self.k8s_object.waitPodCondition(self.otpd.k8s_pod_name, "Ready")
+        self.k8s_object.wait_pod_condition(self.otpd_settings.k8s_pod_name, "Ready")
 
         # Fix settings for local Kubernetes deployments.
         # Unclear why this is not the default.
         if otpd_object:
-            otpd_object.applySetting("LocalOtdsUrl", "http://otds/otdsws")
-            otpd_object.applySetting(
+            otpd_object.apply_setting("LocalOtdsUrl", "http://otds/otdsws")
+            otpd_object.apply_setting(
                 "LocalApplicationServerUrlForContentManager",
                 "http://localhost:8080/c4ApplicationServer",
-                self.otpd.tenant,
+                self.otpd_settings.tenant,
             )
 
         return otpd_object
 
         # end function definition
 
     def init_otawp(self):
         """Initialize OTDS for Appworks Platform
         Args:
         Return: None
         """
 
         logger.info("Connection parameters OTAWP:")
-        logger.info("OTAWP Enabled          = %s", self.otawp.enabled)
-        logger.info("OTAWP Resource         = %s", self.otawp.resource_name)
-        logger.info("OTAWP Access Role      = %s", self.otawp.access_role_name)
-        logger.info("OTAWP Admin User       = %s", self.otawp.admin)
-        logger.debug("OTAWP Password         = %s", self.otawp.password)
-        logger.info("OTAWP K8s Stateful Set = %s", self.otawp.k8s_statefulset)
-        logger.info("OTAWP K8s Config Map   = %s", self.otawp.k8s_configmap)
+        logger.info("OTAWP Enabled          = %s", self.otawp_settings.enabled)
+        logger.info("OTAWP Resource         = %s", self.otawp_settings.resource_name)
+        logger.info("OTAWP Access Role      = %s", self.otawp_settings.access_role_name)
+        logger.info("OTAWP Admin User       = %s", self.otawp_settings.admin)
+        logger.debug("OTAWP Password         = %s", self.otawp_settings.password)
+        logger.info("OTAWP K8s Stateful Set = %s", self.otawp_settings.k8s_statefulset)
+        logger.info("OTAWP K8s Config Map   = %s", self.otawp_settings.k8s_configmap)
 
         logger.info(
             "Wait for OTCS to create its OTDS resource with name -> %s...",
-            self.otcs.resource_name,
+            self.otcs_settings.resource_name,
         )
 
         # Loop to wait for OTCS to create its OTDS resource
         # (we need it to update the AppWorks K8s Config Map):
-        otcs_resource = self.otds_object.getResource(self.otcs.resource_name)
+        otcs_resource = self.otds_object.get_resource(self.otcs_settings.resource_name)
         while otcs_resource is None:
             logger.warning(
                 "OTDS resource for Content Server with name -> %s does not exist yet. Waiting...",
-                self.otcs.resource_name,
+                self.otcs_settings.resource_name,
             )
             time.sleep(30)
-            otcs_resource = self.otds_object.getResource(self.otcs.resource_name)
+            otcs_resource = self.otds_object.get_resource(
+                self.otcs_settings.resource_name
+            )
 
         otcs_resource_id = otcs_resource["resourceID"]
 
         logger.info("OTDS resource ID for Content Server -> %s", otcs_resource_id)
 
         # make sure code is idempotent and only try to add ressource if it doesn't exist already:
-        awp_resource = self.otds_object.getResource(self.otawp.resource_name)
+        awp_resource = self.otds_object.get_resource(self.otawp_settings.resource_name)
         if not awp_resource:
             logger.info(
                 "OTDS resource -> %s for AppWorks Platform does not yet exist. Creating...",
-                self.otawp.resource_name,
+                self.otawp_settings.resource_name,
             )
             # Create a Python dict with the special payload we need for AppWorks:
             additional_payload = {}
             additional_payload["connectorid"] = "rest"
             additional_payload["resourceType"] = "rest"
             user_attribute_mapping = [
                 {
@@ -883,126 +918,133 @@
             additional_payload["pcModifyPermissionAllowed"] = "true"
             additional_payload["pcDeletePermissionAllowed"] = "false"
             additional_payload["connectionParamInfo"] = [
                 {
                     "name": "fBaseURL",
                     "value": "http://appworks:8080/home/system/app/otdspush",
                 },
-                {"name": "fUsername", "value": self.otawp.admin},
-                {"name": "fPassword", "value": self.otawp.password},
+                {"name": "fUsername", "value": self.otawp_settings.admin},
+                {"name": "fPassword", "value": self.otawp_settings.password},
             ]
 
-            awp_resource = self.otds_object.addResource(
-                self.otawp.resource_name,
+            awp_resource = self.otds_object.add_resource(
+                self.otawp_settings.resource_name,
                 "AppWorks Platform",
                 "AppWorks Platform",
                 additional_payload,
             )
         else:
             logger.info(
                 "OTDS resource -> %s for AppWorks Platform does already exist.",
-                self.otawp.resource_name,
+                self.otawp_settings.resource_name,
             )
 
         awp_resource_id = awp_resource["resourceID"]
 
         logger.info("OTDS resource ID for AppWorks Platform -> %s", awp_resource_id)
 
         self.settings.placeholder_values["OTAWP_RESOURCE_ID"] = str(awp_resource_id)
 
         logger.debug(
             "Placeholder values after OTAWP init = %s", self.settings.placeholder_values
         )
 
         logger.info("Update AppWorks Kubernetes Config Map with OTDS resource IDs...")
 
-        config_map = self.k8s_object.getConfigMap(self.otawp.k8s_configmap)
+        config_map = self.k8s_object.get_config_map(self.otawp_settings.k8s_configmap)
         if not config_map:
             logger.error(
                 "Failed to retrieve AppWorks Kubernetes Config Map -> %s",
-                self.otawp.k8s_configmap,
+                self.otawp_settings.k8s_configmap,
             )
         else:
             solution = yaml.safe_load(config_map.data["solution.yaml"])  # type: ignore
 
             # Change values as required
             solution["platform"]["organizations"]["system"]["otds"][
                 "resourceId"
             ] = awp_resource_id
             solution["platform"]["content"]["ContentServer"][
                 "contentServerUrl"
-            ] = f"{self.otcs.public_protocol}://{self.otcs.public_url}/cs/cs"
+            ] = f"{self.otcs_settings.public_protocol}://{self.otcs_settings.public_url}/cs/cs"
             solution["platform"]["content"]["ContentServer"][
                 "contentServerSupportDirectoryUrl"
-            ] = f"{self.otcs.public_protocol}://{self.otcs.public_url}/cssupport"
+            ] = f"{self.otcs_settings.public_protocol}://{self.otcs_settings.public_url}/cssupport"
             solution["platform"]["content"]["ContentServer"][
                 "otdsResourceId"
             ] = otcs_resource_id
             solution["platform"]["authenticators"]["OTDS_auth"]["publicLoginUrl"] = (
-                self.otds.public_protocol
+                self.otds_settings.public_protocol
                 + "://"
-                + self.otds.public_url
+                + self.otds_settings.public_url
                 + "/otdsws/login"
             )
             solution["platform"]["security"]["contentSecurityPolicy"] = (
                 "frame-ancestors 'self' "
-                + self.otcs.public_protocol
+                + self.otcs_settings.public_protocol
                 + "://"
-                + self.otcs.public_url
+                + self.otcs_settings.public_url
             )
             data = {"solution.yaml": yaml.dump(solution)}
-            result = self.k8s_object.replaceConfigMap(self.otawp.k8s_configmap, data)
+            result = self.k8s_object.replace_config_map(
+                self.otawp_settings.k8s_configmap, data
+            )
             if result:
                 logger.info("Successfully updated AppWorks Solution YAML.")
             else:
                 logger.error("Failed to update AppWorks Solution YAML.")
             logger.debug("Solution YAML for AppWorks -> %s", solution)
 
         logger.info("Scale AppWorks Kubernetes Stateful Set to 1...")
-        self.k8s_object.scaleStatefulSet(sts_name=self.otawp.k8s_statefulset, scale=1)
+        self.k8s_object.scale_stateful_set(
+            sts_name=self.otawp_settings.k8s_statefulset, scale=1
+        )
 
         # Add the OTCS Admin user to the AppWorks Access Role in OTDS
-        self.otds_object.addUserToAccessRole(
-            "Access to " + self.otawp.resource_name, "otadmin@otds.admin"
+        self.otds_object.add_user_to_access_role(
+            "Access to " + self.otawp_settings.resource_name, "otadmin@otds.admin"
         )
 
         # Loop to wait for OTCS to create its OTDS user partition:
-        otcs_partition = self.otds_object.getPartition(self.otcs.partition)
+        otcs_partition = self.otds_object.get_partition(self.otcs_settings.partition)
         while otcs_partition is None:
             logger.warning(
                 "OTDS user partition for Content Server with name -> %s does not exist yet. Waiting...",
-                self.otcs.partition,
+                self.otcs_settings.partition,
             )
 
             time.sleep(30)
-            otcs_partition = self.otds_object.getPartition(self.otcs.partition)
+            otcs_partition = self.otds_object.get_partition(
+                self.otcs_settings.partition
+            )
 
         # Add the OTDS user partition for OTCS to the AppWorks Platform Access Role in OTDS.
         # This will effectvely sync all OTCS users with AppWorks Platform:
-        self.otds_object.addPartitionToAccessRole(
-            self.otawp.access_role_name, self.otcs.partition
+        self.otds_object.add_partition_to_access_role(
+            self.otawp_settings.access_role_name, self.otcs_settings.partition
         )
 
         # Add the OTDS admin partition to the AppWorks Platform Access Role in OTDS.
-        self.otds_object.addPartitionToAccessRole(
-            self.otawp.access_role_name, self.otds.admin_partition
+        self.otds_object.add_partition_to_access_role(
+            self.otawp_settings.access_role_name, self.otds_settings.admin_partition
         )
 
         # Set Group inclusion for Access Role for OTAWP to "True":
-        self.otds_object.updateAccessRoleAttributes(
-            self.otawp.access_role_name, [{"name": "pushAllGroups", "values": ["True"]}]
+        self.otds_object.update_access_role_attributes(
+            self.otawp_settings.access_role_name,
+            [{"name": "pushAllGroups", "values": ["True"]}],
         )
 
         # Add ResourceID User to OTDSAdmin to allow push
-        self.otds_object.addUserToGroup(
+        self.otds_object.add_user_to_group(
             user=str(awp_resource_id) + "@otds.admin", group="otdsadmins@otds.admin"
         )
 
         # Allow impersonation for all users:
-        self.otds_object.impersonateResource(self.otawp.resource_name)
+        self.otds_object.impersonate_resource(self.otawp_settings.resource_name)
 
         # end function definition
 
     def restart_otcs_service(self, otcs_object: OTCS):
         """Restart the Content Server service in all OTCS pods
 
         Args:
@@ -1010,67 +1052,67 @@
         Returns:
             None
         """
 
         logger.info("Restart OTCS frontend and backend pods...")
 
         # Restart all frontends:
-        for x in range(0, self.otcs.replicas_frontend):
-            pod_name = self.otcs.k8s_statefulset_frontend + "-" + str(x)
+        for x in range(0, self.otcs_settings.replicas_frontend):
+            pod_name = self.otcs_settings.k8s_statefulset_frontend + "-" + str(x)
 
             logger.info("Deactivate Liveness probe for pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "touch /tmp/keepalive"]
             )
             logger.info("Restarting pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "/opt/opentext/cs/stop_csserver"]
             )
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "/opt/opentext/cs/start_csserver"]
             )
 
         # Restart all backends:
-        for x in range(0, self.otcs.replicas_backend):
-            pod_name = self.otcs.k8s_statefulset_backend + "-" + str(x)
+        for x in range(0, self.otcs_settings.replicas_backend):
+            pod_name = self.otcs_settings.k8s_statefulset_backend + "-" + str(x)
 
             logger.info("Deactivate Liveness probe for pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "touch /tmp/keepalive"]
             )
             logger.info("Restarting pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "/opt/opentext/cs/stop_csserver"]
             )
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "/opt/opentext/cs/start_csserver"]
             )
 
         logger.info("Re-Authenticating to OTCS after restart of pods...")
         otcs_cookie = otcs_object.authenticate(revalidate=True)
         while otcs_cookie is None:
             logger.warning("Waiting 30 seconds for OTCS to become ready...")
             time.sleep(30)
             otcs_cookie = otcs_object.authenticate(revalidate=True)
         logger.info("OTCS is ready again.")
 
         # Reactivate Liveness probes in all pods:
-        for x in range(0, self.otcs.replicas_frontend):
-            pod_name = self.otcs.k8s_statefulset_frontend + "-" + str(x)
+        for x in range(0, self.otcs_settings.replicas_frontend):
+            pod_name = self.otcs_settings.k8s_statefulset_frontend + "-" + str(x)
 
             logger.info("Reactivate Liveness probe for pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "rm /tmp/keepalive"]
             )
 
-        for x in range(0, self.otcs.replicas_backend):
-            pod_name = self.otcs.k8s_statefulset_backend + "-" + str(x)
+        for x in range(0, self.otcs_settings.replicas_backend):
+            pod_name = self.otcs_settings.k8s_statefulset_backend + "-" + str(x)
 
             logger.info("Reactivate Liveness probe for pod -> %s", pod_name)
-            self.k8s_object.execPodCommand(
+            self.k8s_object.exec_pod_command(
                 pod_name, ["/bin/sh", "-c", "rm /tmp/keepalive"]
             )
 
         logger.info("Restart OTCS frontend and backend pods has been completed.")
 
         # end function definition
 
@@ -1078,26 +1120,26 @@
         """Restart the Archive Center spawner service in OTAC pod
 
         Args:
         Returns:
             boolean: True if restart was done, False if error occured
         """
 
-        if not self.otac.enabled:
+        if not self.otac_settings.enabled:
             return False
 
         logger.info(
             "Restarting spawner service in Archive Center pod -> %s",
-            self.otac.k8s_pod_name,
+            self.otac_settings.k8s_pod_name,
         )
         # The Archive Center Spawner needs to be run in "interactive" mode - otherwise the command will "hang":
         # The "-c" parameter is not required in this case
         # False is given as parameter as OTAC writes non-errors to stderr
-        response = self.k8s_object.execPodCommandInteractive(
-            self.otac.k8s_pod_name,
+        response = self.k8s_object.exec_pod_command_interactive(
+            self.otac_settings.k8s_pod_name,
             ["/bin/sh", "/etc/init.d/spawner restart"],
             60,
             False,
         )
 
         if response:
             return True
@@ -1110,102 +1152,106 @@
         """Delete the AppWorks Platform Pod to make Kubernetes restart it.
 
         Args:
         Returns:
             None
         """
 
-        self.k8s_object.deletePod(self.otawp.k8s_statefulset + "-0")
+        self.k8s_object.delete_pod(self.otawp_settings.k8s_statefulset + "-0")
 
         # end function definition
 
     def consolidate_otds(self):
         """Consolidate OTDS resources
         Args:
         Return: None
         """
 
-        self.otds_object.consolidate(self.otcs.resource_name)
+        self.otds_object.consolidate(self.otcs_settings.resource_name)
 
-        if self.otawp.enabled == "true":  # is AppWorks Platform deployed?
-            self.otds_object.consolidate(self.otawp.resource_name)
+        if self.otawp_settings.enabled == "true":  # is AppWorks Platform deployed?
+            self.otds_object.consolidate(self.otawp_settings.resource_name)
 
         # end function definition
 
     def import_powerdocs_configuration(self, otpd_object: OTPD):
         """Import a database export (zip file) into the PowerDocs database
 
         Args:
             otpd_object (object): PowerDocs object
         """
 
-        if self.otpd.db_importfile.startswith("http"):
+        if self.otpd_settings.db_importfile.startswith("http"):
             # Download file from remote location specified by the OTPD_DBIMPORTFILE
             # this must be a public place without authentication:
             logger.info(
                 "Download PowerDocs database file from URL -> %s",
-                self.otpd.db_importfile,
+                self.otpd_settings.db_importfile,
             )
 
             try:
-                package = requests.get(self.otpd.db_importfile, timeout=60)
+                package = requests.get(self.otpd_settings.db_importfile, timeout=60)
                 package.raise_for_status()
                 logger.info(
                     "Successfully downloaded PowerDocs database file -> %s; status code -> %s",
-                    self.otpd.db_importfile,
+                    self.otpd_settings.db_importfile,
                     package.status_code,
                 )
                 filename = "/tmp/otpd_db_import.zip"
                 with open(filename, mode="wb") as localfile:
                     localfile.write(package.content)
 
                 logger.info(
                     "Starting import on %s://%s:%s of %s",
-                    self.otpd.protocol,
-                    self.otpd.hostname,
-                    self.otpd.port,
-                    self.otpd.db_importfile,
+                    self.otpd_settings.protocol,
+                    self.otpd_settings.hostname,
+                    self.otpd_settings.port,
+                    self.otpd_settings.db_importfile,
                 )
-                response = otpd_object.importDatabase(filename=filename)
+                response = otpd_object.import_database(filename=filename)
                 logger.info("Response -> %s", response)
 
             except requests.exceptions.HTTPError as err:
                 logger.error("Request error -> %s", err)
 
         # end function definition
 
     def set_maintenance_mode(self, enable: bool = True):
         """Enable or Disable Maintenance Mode
 
         Args:
             enable (bool, optional): _description_. Defaults to True.
         """
-        if enable:
+        if enable and self.k8s_settings.enabled:
             logger.info("========== Enable Maintenance Mode ==========")
             logger.info(
                 "Put OTCS frontends in Maitenance Mode by changing the Kubernetes Ingress backend service..."
             )
-            self.k8s_object.updateIngressBackendServices(
-                self.otcs.k8s_ingress,
+            self.k8s_object.update_ingress_backend_services(
+                self.otcs_settings.k8s_ingress,
                 "otcs",
-                self.otcs.maintenance_service_name,
-                self.otcs.mainteance_service_port,
+                self.otcs_settings.maintenance_service_name,
+                self.otcs_settings.mainteance_service_port,
             )
             logger.info("OTCS frontend is now in Maintenance Mode!")
-
+        elif not self.k8s_settings.enabled:
+            logger.warning(
+                "Kubernetes Integration disabled - Cannot Enable/Disable Maintenance Mode"
+            )
+            self.k8s_object = None
         else:
             # Changing the Ingress backend service to OTCS frontend service:
             logger.info(
                 "Put OTCS frontend back in Production Mode by changing the Kubernetes Ingress backend service..."
             )
-            self.k8s_object.updateIngressBackendServices(
-                self.otcs.k8s_ingress,
+            self.k8s_object.update_ingress_backend_services(
+                self.otcs_settings.k8s_ingress,
                 "otcs",
-                self.otcs.hostname_frontend,
-                self.otcs.port_frontend,
+                self.otcs_settings.hostname_frontend,
+                self.otcs_settings.port_frontend,
             )
             logger.info("OTCS frontend is now back in Production Mode!")
 
     def customization_run(self):
         """Central function to initiate the customization"""
         # Set Timer for duration calculation
         self.settings.customizer_start_time = (
@@ -1220,128 +1266,132 @@
         self.otds_object = self.init_otds()
         if not self.otds_object:
             logger.error("Failed to initialize OTDS - exiting...")
             sys.exit()
 
         # Establish in-cluster Kubernetes connection
         logger.info("========== Initialize Kubernetes ============")
-        if self.k8s_enabled:
-            self.k8s_object = self.init_k8s(in_cluster=True)
+        if self.k8s_settings.enabled:
+            self.k8s_object = self.init_k8s(**asdict(self.k8s_settings))
 
             if not self.k8s_object:
                 logger.error("Failed to initialize Kubernetes - exiting...")
                 sys.exit()
 
         # Put Frontend in Maintenance mode to make sure nobody interferes
         # during customization:
-        if self.otcs.maintenance_mode:
+        if self.otcs_settings.maintenance_mode:
             self.set_maintenance_mode(True)
 
-        if self.otawp.enabled == "true":  # is AppWorks Platform deployed?
+        if self.otawp_settings.enabled == "true":  # is AppWorks Platform deployed?
             logger.info("========== Initialize OTAWP =============")
 
             # Configure required OTDS resources as AppWorks doesn't do this on its own:
             self.init_otawp()
         else:
             self.settings.placeholder_values["OTAWP_RESOURCE_ID"] = ""
 
         logger.info("========== Initialize OTCS backend ======")
         self.otcs_backend_object = self.init_otcs(
-            self.otcs.hostname_backend,
-            int(self.otcs.port_backend),
-            self.otcs.partition,
-            self.otcs.resource_name,
+            self.otcs_settings.hostname_backend,
+            int(self.otcs_settings.port_backend),
+            self.otcs_settings.partition,
+            self.otcs_settings.resource_name,
         )
         if not self.otcs_backend_object:
             logger.error("Failed to initialize OTCS backend - exiting...")
             sys.exit()
 
         logger.info("========== Initialize OTCS frontend =====")
         self.otcs_frontend_object = self.init_otcs(
-            self.otcs.hostname_frontend,
-            int(self.otcs.port_frontend),
-            self.otcs.partition,
-            self.otcs.resource_name,
+            self.otcs_settings.hostname_frontend,
+            int(self.otcs_settings.port_frontend),
+            self.otcs_settings.partition,
+            self.otcs_settings.resource_name,
         )
         if not self.otcs_frontend_object:
             logger.error("Failed to initialize OTCS frontend - exiting...")
             sys.exit()
 
-        if self.otac.enabled == "true":  # is Archive Center deployed?
+        if self.otac_settings.enabled == "true":  # is Archive Center deployed?
             logger.info("========== Initialize OTAC ==============")
 
             self.otac_object = self.init_otac()
             if not self.otac_object:
                 logger.error("Failed to initialize OTAC - exiting...")
                 sys.exit()
         else:
             self.otac_object = None
 
-        if self.otiv.enabled == "true":  # is PowerDocs deployed?
+        if self.otiv_settings.enabled == "true":  # is PowerDocs deployed?
             logger.info("========== Initialize OTIV ==============")
 
             self.otiv_object = self.init_otiv()
+        else:
+            self.otiv_object = None
 
-        if self.otpd.enabled == "true":  # is PowerDocs deployed?
+        if self.otpd_settings.enabled == "true":  # is PowerDocs deployed?
             logger.info("========== Initialize OTPD ==============")
 
             self.otpd_object = self.init_otpd()
             if not self.otpd_object:
                 logger.error("Failed to initialize OTPD - exiting...")
                 sys.exit()
         else:
             self.otpd_object = None
 
         if (
-            self.o365.enabled == "true"
-            and self.o365.user != ""
-            and self.o365.password != ""
+            self.m365_settings.enabled == "true"
+            and self.m365_settings.user != ""
+            and self.m365_settings.password != ""
         ):  # is M365 enabled?
             logger.info("======== Initialize MS Graph API ========")
 
             # Initialize the M365 object and connection to M365 Graph API:
             self.m365_object = self.init_m365()
 
             logger.info("======== Upload MS Teams App ============")
 
             # Download MS Teams App from OTCS (this has with 23.2 a nasty side-effect
             # of unsetting 2 checkboxes on that config page - we reset these checkboxes
             # with the settings file "O365Settings.xml"):
-            response = self.otcs_frontend_object.downloadConfigFile(
+            response = self.otcs_frontend_object.download_config_file(
                 "/cs/cs?func=officegroups.DownloadTeamsPackage",
                 "/tmp/ot.xecm.teams.zip",
             )
-            self.m365_object.authenticateUser(self.o365.user, self.o365.password)
+            self.m365_object.authenticate_user(
+                self.m365_settings.user, self.m365_settings.password
+            )
 
             # Check if the app is already installed:
-            response = self.m365_object.getTeamsApps(
-                f"contains(displayName, '{self.o365.teams_app_name}')"
+            response = self.m365_object.get_teams_apps(
+                f"contains(displayName, '{self.m365_settings.teams_app_name}')"
             )
-            if self.m365_object.existResultItem(
-                response, "displayName", self.o365.teams_app_name
+            if self.m365_object.exist_result_item(
+                response, "displayName", self.m365_settings.teams_app_name
             ):
                 logger.info(
                     "Extended ECM Teams App is already in app catalog. Trying to install an update (may give a warning if it is not a new version)..."
                 )
-                app_id = self.m365_object.getResultValue(
+                app_id = self.m365_object.get_result_value(
                     response, "id", 0
                 )  # 0 = Index = first item
                 logger.info(
                     "Extended ECM Teams App is already in app catalog (app ID -> %s). Updating existing app...",
                     app_id,
                 )
-                response = self.m365_object.uploadTeamsApp(
+                response = self.m365_object.upload_teams_app(
                     "/tmp/ot.xecm.teams.zip", update_existing_app=True, app_id=app_id
                 )
             else:
                 # this upload will be done with the user credentials - this is required:
                 logger.info(
                     "Extended Teams ECM App is not yet in app catalog. Installing as new app..."
                 )
-                response = self.m365_object.uploadTeamsApp("/tmp/ot.xecm.teams.zip")
+                response = self.m365_object.upload_teams_app("/tmp/ot.xecm.teams.zip")
         else:
             self.m365_object = None
 
         logger.info("========== Processing Payload ===========")
 
         cust_payload_list = [self.settings.cust_payload]
 
@@ -1359,15 +1409,15 @@
         for cust_payload in cust_payload_list:
             # Open the payload file. If this fails we bail out:
             logger.info("Starting processing of payload -> %s", cust_payload)
 
             # Set startTime for duration calculation
             start_time = datetime.now()
 
-            payload_object = payload.Payload(
+            payload_object = Payload(
                 payload_source=cust_payload,
                 custom_settings_dir=self.settings.cust_settings_dir,
                 k8s_object=self.k8s_object,
                 otds_object=self.otds_object,
                 otac_object=self.otac_object,
                 otcs_backend_object=self.otcs_backend_object,
                 otcs_frontend_object=self.otcs_frontend_object,
@@ -1388,62 +1438,66 @@
             payload_object.processPayload()
 
             logger.info("========== Consolidate OTDS Resources ==================")
             self.consolidate_otds()
 
             # Upload payload file for later review to Enterprise Workspace
             logger.info("========== Upload Payload file to Extended ECM =========")
-            response = self.otcs_backend_object.getNodeFromNickname(
+            response = self.otcs_backend_object.get_node_from_nickname(
                 self.settings.cust_target_folder_nickname
             )
-            target_folder_id = self.otcs_backend_object.getResultValue(response, "id")
+            target_folder_id = self.otcs_backend_object.get_result_value(response, "id")
             if not target_folder_id:
                 target_folder_id = 2000  # use Enterprise Workspace as fallback
             # Write YAML file with upadated payload (including IDs, etc.).
             # We need to write to /tmp as initial location is read-only:
             cust_payload = "/tmp/" + os.path.basename(cust_payload)
             with open(cust_payload, "w", encoding="utf-8") as file:
                 yaml.dump(payload_object.getPayload(), file)
 
             # Check if the payload file has been uploaded before.
             # This can happen if we re-run the python container.
             # In this case we add a version to the existing document:
-            response = self.otcs_backend_object.getNodeByParentAndName(
+            response = self.otcs_backend_object.get_node_by_parent_and_name(
                 int(target_folder_id), os.path.basename(cust_payload)
             )
-            target_document_id = self.otcs_backend_object.getResultValue(response, "id")
+            target_document_id = self.otcs_backend_object.get_result_value(
+                response, "id"
+            )
             if target_document_id:
-                response = self.otcs_backend_object.addDocumentVersion(
+                response = self.otcs_backend_object.add_document_version(
                     int(target_document_id),
                     cust_payload,
                     os.path.basename(cust_payload),
                     "text/plain",
                     "Updated payload file after re-run of customization",
                 )
             else:
-                response = self.otcs_backend_object.uploadFileToParent(
+                response = self.otcs_backend_object.upload_file_to_parent(
                     cust_payload,
                     os.path.basename(cust_payload),
                     "text/plain",
                     int(target_folder_id),
                 )
 
             duration = datetime.now() - start_time
             logger.info(
                 "========== Payload -> %s completed execution in %s ===",
                 cust_payload,
                 duration,
             )
 
-        if self.otcs.maintenance_mode:
+        if self.otcs_settings.maintenance_mode:
             self.set_maintenance_mode(False)
 
         # Restart AppWorksPlatform pod if it is deployed (to make settings effective):
-        if self.otawp.enabled == "true":  # is AppWorks Platform deployed?
-            otawp_resource = self.otds_object.getResource(self.otawp.resource_name)
+        if self.otawp_settings.enabled == "true":  # is AppWorks Platform deployed?
+            otawp_resource = self.otds_object.get_resource(
+                self.otawp_settings.resource_name
+            )
             if (
                 not "allowImpersonation" in otawp_resource
                 or not otawp_resource["allowImpersonation"]
             ):
                 # Allow impersonation for all users:
                 logger.warning(
                     "OTAWP impersonation is not correct in OTDS before OTAWP pod restart!"
@@ -1452,51 +1506,55 @@
                 logger.info(
                     "OTAWP impersonation is correct in OTDS before OTAWP pod restart!"
                 )
             logger.info("Restart OTAWP pod...")
             self.restart_otawp_pod()
             # For some reason we need to double-check that the impersonation for OTAWP has been set correctly
             # and if not set it again:
-            otawp_resource = self.otds_object.getResource(self.otawp.resource_name)
+            otawp_resource = self.otds_object.get_resource(
+                self.otawp_settings.resource_name
+            )
             if (
                 not "allowImpersonation" in otawp_resource
                 or not otawp_resource["allowImpersonation"]
             ):
                 # Allow impersonation for all users:
                 logger.warning(
                     "OTAWP impersonation is not correct in OTDS - set it once more..."
                 )
-                self.otds_object.impersonateResource(self.otawp.resource_name)
+                self.otds_object.impersonate_resource(self.otawp_settings.resource_name)
 
         # Upload log file for later review to "Deployment" folder in "Administration" folder
         if os.path.exists(self.settings.cust_log_file):
             logger.info("========== Upload log file to Extended ECM =============")
-            response = self.otcs_backend_object.getNodeFromNickname(
+            response = self.otcs_backend_object.get_node_from_nickname(
                 self.settings.cust_target_folder_nickname
             )
-            target_folder_id = self.otcs_backend_object.getResultValue(response, "id")
+            target_folder_id = self.otcs_backend_object.get_result_value(response, "id")
             if not target_folder_id:
                 target_folder_id = 2000  # use Enterprise Workspace as fallback
             # Check if the log file has been uploaded before.
             # This can happen if we re-run the python container:
             # In this case we add a version to the existing document:
-            response = self.otcs_backend_object.getNodeByParentAndName(
+            response = self.otcs_backend_object.get_node_by_parent_and_name(
                 int(target_folder_id), os.path.basename(self.settings.cust_log_file)
             )
-            target_document_id = self.otcs_backend_object.getResultValue(response, "id")
+            target_document_id = self.otcs_backend_object.get_result_value(
+                response, "id"
+            )
             if target_document_id:
-                response = self.otcs_backend_object.addDocumentVersion(
+                response = self.otcs_backend_object.add_document_version(
                     int(target_document_id),
                     self.settings.cust_log_file,
                     os.path.basename(self.settings.cust_log_file),
                     "text/plain",
                     "Updated Python Log after re-run of customization",
                 )
             else:
-                response = self.otcs_backend_object.uploadFileToParent(
+                response = self.otcs_backend_object.upload_file_to_parent(
                     self.settings.cust_log_file,
                     os.path.basename(self.settings.cust_log_file),
                     "text/plain",
                     int(target_folder_id),
                 )
 
         self.settings.customizer_end_time = datetime.now()
@@ -1506,15 +1564,28 @@
         )
 
 
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
         datefmt="%d-%b-%Y %H:%M:%S",
-        level=logging.DEBUG,
+        level=logging.INFO,
         handlers=[
             logging.StreamHandler(sys.stdout),
         ],
     )
 
-    my_customizer = Customizer()
+    my_customizer = Customizer(
+        otcs=CustomizerSettingsOTCS(
+            hostname="otcs.eng.terrarium.cloud",
+            hostname_backend="otcs.eng.terrarium.cloud",
+            hostname_frontend="otcs.eng.terrarium.cloud",
+            protocol="https",
+            port_backend=443,
+        ),
+        otds=CustomizerSettingsOTDS(hostname="otds.eng.terrarium.cloud"),
+        otpd=CustomizerSettingsOTPD(enabled=False),
+        k8s=CustomizerSettingsK8S(enabled=False),
+        otiv=CustomizerSettingsOTIV(enabled="true"),
+    )
+
     my_customizer.customization_run()
```

### Comparing `pyxecm-0.2.0/pyxecm/k8s.py` & `pyxecm-0.3.0/pyxecm/customizer/k8s.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,133 +6,156 @@
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
 https://github.com/kubernetes-client/python/tree/master/examples
 
 Class: K8s
 Methods:
 
 __init__ : class initializer
-getCoreV1Api: Get Kubernetes API object for Core APIs
-getAppsV1Api: Get Kubernetes API object for Applications (e.g. Stateful Sets)
-getNetworkingV1Api: Get Kubernetes API object for Networking (e.g. Ingress)
-getNamespace: Get the Kubernetes namespace the K8s object is configured for
-
-getPod: Get a Kubernetes Pod based on its name
-listPods: Get a list of Kubernetes pods based on field and label selectors
-execPodCommand: Execute a list of commands in a Kubernetes Pod
-execPodCommendInteractive: Write commands to stdin and wait for response
-deletePod: Delete a running pod (e.g. to make Kubernetes restart it)
-
-getConfigMap: Get a Kubernetes Config Map based on its name
-listConfigMaps: Get a list of Kubernetes Config Maps based on field and label selectors
-findConfigMap: Find a Kubernetes Config Map based on its name
-replaceConfigMap: Replace the data body of a Kubernetes Config Map
-
-getStatefulSet: Gets a Kubernetes Stateful Set based on its name
-getStatefulSetScale: Gets the number of replicas for a Kubernetes Stateful Set
-patchStatefulSet: Updates the specification of a Kubernetes Stateful Set
-scaleStatefulSet: Changes number of replicas for a Kubernetes Stateful Set
-
-getService: Get a Kubernetes Service based on its name
-listServices: Get a list of Kubernetes Services based on field and label selectors
-patchService: Update the specification of a Kubernetes Service
-
-getIngress: Get a Kubernetes Ingress based on its name
-patchIngress: Update the specification of a Kubernetes Ingress
-updateIngressBackendServices: Replace the backend service and port for an ingress host
+get_core_v1_api: Get Kubernetes API object for Core APIs
+get_apps_v1_api: Get Kubernetes API object for Applications (e.g. Stateful Sets)
+get_networking_v1_api: Get Kubernetes API object for Networking (e.g. Ingress)
+get_namespace: Get the Kubernetes namespace the K8s object is configured for
+
+get_pod: Get a Kubernetes Pod based on its name
+list_pods: Get a list of Kubernetes pods based on field and label selectors
+exec_pod_command: Execute a list of commands in a Kubernetes Pod
+exec_pod_command_interactive: Write commands to stdin and wait for response
+delete_pod: Delete a running pod (e.g. to make Kubernetes restart it)
+
+get_config_map: Get a Kubernetes Config Map based on its name
+list_config_maps: Get a list of Kubernetes Config Maps based on field and label selectors
+find_config_map: Find a Kubernetes Config Map based on its name
+replace_config_map: Replace the data body of a Kubernetes Config Map
+
+get_stateful_set: Gets a Kubernetes Stateful Set based on its name
+get_stateful_set_scale: Gets the number of replicas for a Kubernetes Stateful Set
+patch_stateful_set: Updates the specification of a Kubernetes Stateful Set
+scale_stateful_set: Changes number of replicas for a Kubernetes Stateful Set
+
+get_service: Get a Kubernetes Service based on its name
+list_services: Get a list of Kubernetes Services based on field and label selectors
+patch_service: Update the specification of a Kubernetes Service
+
+get_ingress: Get a Kubernetes Ingress based on its name
+patch_ingress: Update the specification of a Kubernetes Ingress
+update_ingress_backend_services: Replace the backend service and port for an ingress host
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
-import os
 import logging
 import time
 from kubernetes import client, config
 from kubernetes.stream import stream
 from kubernetes.client.exceptions import ApiException
 
 # Configure Kubernetes API authentication to use pod serviceAccount
 # config.load_incluster_config()
 
-logger = logging.getLogger("pyxecm.k8s")
+logger = logging.getLogger("pyxecm.customizer.k8s")
 
-class K8s(object):
+
+class K8s:
     """Used to automate stettings in Kubernetes."""
 
     _core_v1_api = None
     _apps_v1_api = None
     _networking_v1_api = None
     _namespace = None
 
-    def __init__(self, inCluster: bool = True, namespace: str = ""):
+    def __init__(self, in_cluster: bool = True, **kwargs):
         """Initialize the Kubernetes object."""
 
         # Configure Kubernetes API authentication to use pod serviceAccount
-        if inCluster:
+        if in_cluster:
             config.load_incluster_config()
         else:
-            config.load_kube_config()
+            config.load_kube_config(config_file=kwargs["kubeconfig_file"])
 
         self._core_v1_api = client.CoreV1Api()
         self._apps_v1_api = client.AppsV1Api()
         self._networking_v1_api = client.NetworkingV1Api()
-        if namespace:
-            self._namespace = namespace
+        if "namespace" in kwargs and not in_cluster:
+            self._namespace = kwargs["namespace"]
         else:
             # Read current namespace
             with open(
-                "/var/run/secrets/kubernetes.io/serviceaccount/namespace", "r"
-            ) as f:
-                self._namespace = f.read()
+                "/var/run/secrets/kubernetes.io/serviceaccount/namespace",
+                "r",
+                encoding="utf-8",
+            ) as namespace_file:
+                self._namespace = namespace_file.read()
+
+    def get_core_v1_api(self):
+        """Returns Kubernetes Core V1 API object
 
-    def getCoreV1Api(self):
+        Returns:
+            object: Kubernetes API object
+        """
         return self._core_v1_api
 
-    def getAppsV1Api(self):
+    def get_apps_v1_api(self):
+        """Returns Kubernetes Apps V1 API object
+
+        Returns:
+            object: Kubernetes API object
+        """
         return self._apps_v1_api
 
-    def getNetworkingV1Api(self):
+    def get_networking_v1_api(self):
+        """Returns Kubernetes Networking V1 API object
+
+        Returns:
+            object: Kubernetes API object
+        """
         return self._networking_v1_api
 
-    def getNamespace(self):
+    def get_namespace(self):
+        """Returns Kubernetes Namespace
+
+        Returns:
+            str: Kubernetes namespace
+        """
         return self._namespace
 
-    def getPod(self, pod_name: str):
-        """Get a pod in the configured namespace (the namespace is defined in the class constructor).
+    def get_pod(self, pod_name: str):
+        """Get a pod in the configured namespace (the namespace is defined
+            in the class constructor).
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#read_namespaced_pod
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
         Returns:
             V1Pod (object) or None if the call fails.
             - api_version='v1',
             - kind='Pod',
             - metadata=V1ObjectMeta(...),
             - spec=V1PodSpec(...),
             - status=V1PodStatus(...)
         """
 
         try:
-            response = self.getCoreV1Api().read_namespaced_pod(
-                name=pod_name, namespace=self.getNamespace()
+            response = self.get_core_v1_api().read_namespaced_pod(
+                name=pod_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to get Pod -> {}; error -> {}".format(pod_name, str(e))
+                "Failed to get Pod -> %s; error -> %s", pod_name, str(exception)
             )
             return None
 
         return response
 
     # end method definition
 
-    def listPods(self, field_selector: str = "", label_selector: str = ""):
+    def list_pods(self, field_selector: str = "", label_selector: str = ""):
         """List all Kubernetes pods in a given namespace. The list can be further restricted
             by specifying a field or label selector.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_pod
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
         Returns:
@@ -143,123 +166,125 @@
                     V1Pod object using dot notation, for example, pod.metadata.name to access the name of the pod
             - kind: The Kubernetes object kind, which is always "PodList".
             - metadata: Additional metadata about the pod list, such as the resource version.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1PodList.md
         """
 
         try:
-            response = self.getCoreV1Api().list_namespaced_pod(
+            response = self.get_core_v1_api().list_namespaced_pod(
                 field_selector=field_selector,
                 label_selector=label_selector,
-                namespace=self.getNamespace(),
+                namespace=self.get_namespace(),
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to list Pods with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    field_selector, label_selector, str(e)
-                )
+                "Failed to list Pods with field_selector -> %s and label_selector -> %s; error -> %s",
+                field_selector,
+                label_selector,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def waitPodCondition(self, pod_name: str, condition_name: str):
+    def wait_pod_condition(self, pod_name: str, condition_name: str):
         """Wait for the pod to reach a defined condition (e.g. "Ready").
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             condition_name (string): name of the condition, e.g. "Ready"
         Returns:
             True once the pod reaches the condition - otherwise wait forever
         """
 
         ready = False
         while not ready:
             try:
-                pod_status = self.getCoreV1Api().read_namespaced_pod_status(
-                    pod_name, self.getNamespace()
+                pod_status = self.get_core_v1_api().read_namespaced_pod_status(
+                    pod_name, self.get_namespace()
                 )
 
                 # Check if the pod has reached the defined condition:
                 for cond in pod_status.status.conditions:
                     if cond.type == condition_name and cond.status == "True":
                         logger.info(
-                            "Pod -> {} is in state -> {}!".format(
-                                pod_name, condition_name
-                            )
+                            "Pod -> %s is in state -> %s!", pod_name, condition_name
                         )
                         ready = True
                         break
                 else:
                     logger.info(
-                        "Pod -> {} is not yet in state -> {}. Waiting...".format(
-                            pod_name, condition_name
-                        )
+                        "Pod -> %s is not yet in state -> %s. Waiting...",
+                        pod_name,
+                        condition_name,
                     )
                     time.sleep(30)
                     continue
 
-            except ApiException as e:
+            except ApiException as exception:
                 logger.error(
-                    "Failed to wait for pod -> {}; error -> {}".format(pod_name, str(e))
+                    "Failed to wait for pod -> %s; error -> %s",
+                    pod_name,
+                    str(exception),
                 )
 
     # end method definition
 
-    def execPodCommand(self, pod_name: str, command: list):
+    def exec_pod_command(self, pod_name: str, command: list):
         """Execute a command inside a Kubernetes Pod (similar to kubectl exec on command line).
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#connect_get_namespaced_pod_exec
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             command (list): list of command and its parameters, e.g. ["/bin/bash", "-c", "pwd"]
                             The "-c" is required to make the shell executing the command.
         Returns:
             Response of the command or None if the call fails
         """
 
-        pod = self.getPod(pod_name)
+        pod = self.get_pod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(pod_name))
+            logger.error("Pod -> %s does not exist", pod_name)
 
-        logger.info("Execute command -> {} in pod -> {}".format(command, pod_name))
+        logger.info("Execute command -> %s in pod -> %s", command, pod_name)
 
         try:
             response = stream(
-                self.getCoreV1Api().connect_get_namespaced_pod_exec,
+                self.get_core_v1_api().connect_get_namespaced_pod_exec,
                 pod_name,
-                self.getNamespace(),
+                self.get_namespace(),
                 command=command,
                 stderr=True,
                 stdin=False,
                 stdout=True,
                 tty=False,
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to execute command -> {} in pod -> {}; error -> {}".format(
-                    command, pod_name, str(e)
-                )
+                "Failed to execute command -> %s in pod -> %s; error -> %s",
+                command,
+                pod_name,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
     # Some commands like the OTAC spawner need to run interactive - otherwise the command "hangs"
-    def execPodCommandInteractive(
+    def exec_pod_command_interactive(
         self,
         pod_name: str,
         commands: list,
         timeout: int = 30,
         write_stderr_to_error_log: bool = True,
     ):
         """Execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
-            Other than execPodCommand() method above this is an interactive execution using
+            Other than exec_pod_command() method above this is an interactive execution using
             stdin and reading the output from stdout and stderr. This is required for longer
             running commands. It is currently used for restarting the spawner of Archive Center.
             The output of the command is pushed into the logging.
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             commands (list): list of command and its parameters, e.g. ["/bin/bash", "/etc/init.d/spawner restart"]
                              Here we should NOT have a "-c" parameter!
@@ -268,41 +293,42 @@
                                to make sure we get the full output of the command.
             write_stderr_to_error_log (boolean): flag to control if output in stderr should be written to info or error log stream.
                                                  Default is write to error log (True)
         Returns:
             Response of the command (string) or None if the call fails
         """
 
-        pod = self.getPod(pod_name)
+        pod = self.get_pod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(pod_name))
+            logger.error("Pod -> %s does not exist", pod_name)
 
         if not commands:
             return None
 
         # Get first command - this should be the shell:
         command = commands.pop(0)
 
         try:
             response = stream(
-                self.getCoreV1Api().connect_get_namespaced_pod_exec,
+                self.get_core_v1_api().connect_get_namespaced_pod_exec,
                 pod_name,
-                self.getNamespace(),
+                self.get_namespace(),
                 command=command,
                 stderr=True,
                 stdin=True,  # This is important!
                 stdout=True,
                 tty=False,
                 _preload_content=False,  # This is important!
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to execute command -> {} in pod -> {}; error -> {}".format(
-                    command, pod_name, str(e)
-                )
+                "Failed to execute command -> %s in pod -> %s; error -> %s",
+                command,
+                pod_name,
+                str(exception),
             )
             return None
 
         while response.is_open():
             got_response = False
             response.update(timeout=timeout)
             if response.peek_stdout():
@@ -312,30 +338,28 @@
                 if write_stderr_to_error_log:
                     logger.error(response.read_stderr().replace("\n", " "))
                 else:
                     logger.info(response.read_stderr().replace("\n", " "))
                 got_response = True
             if commands:
                 command = commands.pop(0)
-                logger.info(
-                    "Execute command -> {} in pod -> {}".format(command, pod_name)
-                )
+                logger.info("Execute command -> %s in pod -> %s", command, pod_name)
                 response.write_stdin(command + "\n")
             else:
                 # We continue as long as we get some response during timeout period
                 if not got_response:
                     break
 
         response.close()
 
         return response
 
     # end method definition
 
-    def deletePod(self, pod_name: str):
+    def delete_pod(self, pod_name: str):
         """Delete a pod in the configured namespace (the namespace is defined in the class constructor).
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#delete_namespaced_pod
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
         Return:
             V1Status (object) or None if the call fails.
             - api_version: The Kubernetes API version.
@@ -344,33 +368,33 @@
             - status: The status of the operation, which is either "Success" or an error status.
             - message: A human-readable message explaining the status.
             - reason: A short string that describes the reason for the status.
             - code: An HTTP status code that corresponds to the status.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Status.md
         """
 
-        pod = self.getPod(pod_name)
+        pod = self.get_pod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(pod_name))
+            logger.error("Pod -> %s does not exist", pod_name)
 
         try:
-            response = self.getCoreV1Api().delete_namespaced_pod(
-                pod_name, namespace=self.getNamespace()
+            response = self.get_core_v1_api().delete_namespaced_pod(
+                pod_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to delete Pod -> {}; error -> {}".format(pod_name, str(e))
+                "Failed to delete Pod -> %s; error -> %s", pod_name, str(exception)
             )
             return None
 
         return response
 
     # end method definition
 
-    def getConfigMap(self, config_map_name: str):
+    def get_config_map(self, config_map_name: str):
         """Get a config map in the configured namespace (the namespace is defined in the class constructor).
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#read_namespaced_config_map
         Args:
             config_map_name (string): name of the Kubernetes config map in the current namespace
         Returns:
             V1ConfigMap (object) that includes these fields:
             - api_version: The Kubernetes API version.
@@ -382,26 +406,30 @@
             - binary_data: A dictionary containing the binary data stored in the ConfigMap,
                            where the keys represent the keys of the binary data items and the values
                            represent the values of the binary data items. Binary data is encoded as base64
                            strings in the dictionary values.
         """
 
         try:
-            response = self.getCoreV1Api().read_namespaced_config_map(
-                name=config_map_name, namespace=self.getNamespace()
+            response = self.get_core_v1_api().read_namespaced_config_map(
+                name=config_map_name, namespace=self.get_namespace()
+            )
+        except ApiException as exception:
+            logger.error(
+                "Failed to get Config Map -> %s; error -> %s",
+                config_map_name,
+                str(exception),
             )
-        except ApiException as e:
-            logger.error("Failed to get Config Map -> {}; error -> {}".format(str(e)))
             return None
 
         return response
 
     # end method definition
 
-    def listConfigMaps(self, field_selector: str = "", label_selector: str = ""):
+    def list_config_maps(self, field_selector: str = "", label_selector: str = ""):
         """List all Kubernetes Config Maps in the current namespace.
             The list can be filtered by providing field selectors and label selectors.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_config_map
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
         Returns:
@@ -412,346 +440,360 @@
                      V1Pod object using dot notation, for example, cm.metadata.name to access the name of the config map
             - kind: The Kubernetes object kind, which is always "ConfigMapList".
             - metadata: Additional metadata about the config map list, such as the resource version.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ConfigMapList.md
         """
 
         try:
-            response = self.getCoreV1Api().list_namespaced_config_map(
+            response = self.get_core_v1_api().list_namespaced_config_map(
                 field_selector=field_selector,
                 label_selector=label_selector,
-                namespace=self.getNamespace(),
+                namespace=self.get_namespace(),
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to list Config Maps with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    field_selector, label_selector, str(e)
-                )
+                "Failed to list Config Maps with field_selector -> %s and label_selector -> %s; error -> %s",
+                field_selector,
+                label_selector,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def findConfigMap(self, config_map_name: str):
+    def find_config_map(self, config_map_name: str):
         """Find a Kubernetes Config Map based on its name.
-           This is just a wrapper method for listConfigMaps()
+           This is just a wrapper method for list_config_maps()
            that uses the name as a field selector.
 
         Args:
             config_map_name (string): name of the Config Map
         Returns:
             object: V1ConfigMapList (object) or None if the call fails
         """
 
         try:
-            response = self.listConfigMaps(
+            response = self.list_config_maps(
                 field_selector="metadata.name={}".format(config_map_name)
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to find Config Map -> {}; error -> {}".format(
-                    config_map_name, str(e)
-                )
+                "Failed to find Config Map -> %s; error -> %s",
+                config_map_name,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def replaceConfigMap(self, config_map_name: str, config_map_data: dict):
+    def replace_config_map(self, config_map_name: str, config_map_data: dict):
         """Replace a Config Map with a new specification.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#replace_namespaced_config_map
 
         Args:
             config_map_name (string): name of the Kubernetes Config Map
             config_map_data (dictionary): new specification of the Config Map
         Returns:
             V1ConfigMap (object) or None if the call fails.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ConfigMap.md
         """
 
         try:
-            response = self.getCoreV1Api().replace_namespaced_config_map(
+            response = self.get_core_v1_api().replace_namespaced_config_map(
                 name=config_map_name,
-                namespace=self.getNamespace(),
+                namespace=self.get_namespace(),
                 body=client.V1ConfigMap(
                     metadata=client.V1ObjectMeta(
                         name=config_map_name,
                     ),
                     data=config_map_data,
                 ),
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to replace Config Map -> {}; error -> {}".format(
-                    config_map_name, str(e)
-                )
+                "Failed to replace Config Map -> %s; error -> %s",
+                config_map_name,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def getStatefulSet(self, sts_name: str):
+    def get_stateful_set(self, sts_name: str):
         """Get a Kubernetes Stateful Set based on its name.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#read_namespaced_stateful_set
 
         Args:
             sts_name (string): name of the Kubernetes stateful set
         Returns:
             V1StatefulSet (object) or None if the call fails.
             See : https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
-            response = self.getAppsV1Api().read_namespaced_stateful_set(
-                name=sts_name, namespace=self.getNamespace()
+            response = self.get_apps_v1_api().read_namespaced_stateful_set(
+                name=sts_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to get Stateful Set -> {}; error -> {}".format(sts_name, str(e))
+                "Failed to get Stateful Set -> %s; error -> %s",
+                sts_name,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def getStatefulSetScale(self, sts_name: str):
+    def get_stateful_set_scale(self, sts_name: str):
         """Get the number of replicas for a Kubernetes Stateful Set.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#read_namespaced_stateful_set_scale
 
         Args:
             sts_name (string): name of the Kubernetes Stateful Set
         Returns:
             V1Scale (object) or None if the call fails.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Scale.md
         """
 
         try:
-            response = self.getAppsV1Api().read_namespaced_stateful_set_scale(
-                name=sts_name, namespace=self.getNamespace()
+            response = self.get_apps_v1_api().read_namespaced_stateful_set_scale(
+                name=sts_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to get scaling (replicas) of Stateful Set -> {}; error -> {}".format(
-                    sts_name, str(e)
-                )
+                "Failed to get scaling (replicas) of Stateful Set -> %s; error -> %s",
+                sts_name,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchStatefulSet(self, sts_name: str, sts_body: dict):
+    def patch_stateful_set(self, sts_name: str, sts_body: dict):
         """Patch a Stateful set with new values.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#patch_namespaced_stateful_set
 
         Args:
             sts_name (string): name of the Kubernetes stateful set in the current namespace
             sts_body (string): patch string
         Returns:
             V1StatefulSet (object) or None if the call fails.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
-            response = self.getAppsV1Api().patch_namespaced_stateful_set(
-                name=sts_name, namespace=self.getNamespace(), body=sts_body
+            response = self.get_apps_v1_api().patch_namespaced_stateful_set(
+                name=sts_name, namespace=self.get_namespace(), body=sts_body
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to patch Stateful Set -> {} with -> {}; error -> {}".format(
-                    sts_name, sts_body, str(e)
-                )
+                "Failed to patch Stateful Set -> %s with -> %s; error -> %s",
+                sts_name,
+                sts_body,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def scaleStatefulSet(self, sts_name: str, scale: int):
-        """Scale a stateful set to a specific number of replicas. It uses the class method patchStatefulSet() above.
+    def scale_stateful_set(self, sts_name: str, scale: int):
+        """Scale a stateful set to a specific number of replicas.
+           It uses the class method patch_stateful_set() above.
 
         Args:
             sts_name (string): name of the Kubernetes stateful set in the current namespace
         Returns:
             V1StatefulSet (object) or None if the call fails.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
-            response = self.patchStatefulSet(
+            response = self.patch_stateful_set(
                 sts_name, sts_body={"spec": {"replicas": scale}}
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to scale Stateful Set -> {} to -> {} replicas; error -> {}".format(
-                    sts_name, scale, str(e)
-                )
+                "Failed to scale Stateful Set -> %s to -> %s replicas; error -> %s",
+                sts_name,
+                scale,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def getService(self, service_name: str):
+    def get_service(self, service_name: str):
         """Get a Kubernetes Service with a defined name in the current namespace
 
         Args:
             service_name (string): name of the Kubernetes Service in the current namespace
         Returns:
             V1Service (object) or None if the call fails
             This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Service.md
         """
 
         try:
-            response = self.getCoreV1Api().read_namespaced_service(
-                name=service_name, namespace=self.getNamespace()
+            response = self.get_core_v1_api().read_namespaced_service(
+                name=service_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to get Service -> {}; error -> {}".format(service_name, str(e))
+                "Failed to get Service -> %s; error -> %s", service_name, str(exception)
             )
             return None
 
         return response
 
     # end method definition
 
-    def listServices(self, field_selector: str = "", label_selector: str = ""):
+    def list_services(self, field_selector: str = "", label_selector: str = ""):
         """List all Kubernetes Service in the current namespace.
             The list can be filtered by providing field selectors and label selectors.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_service
 
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
         Returns:
             V1ServiceList (object) or None if the call fails
             Properties can be accessed with the "." notation (this is an object not a dict!):
             - api_version: The Kubernetes API version.
-            - items: A list of V1Service objects, each representing a service. You can access the fields of a
-                     V1Service object using dot notation, for example, service.metadata.name to access the name of the service
+            - items: A list of V1Service objects, each representing a service.
+                     You can access the fields of a V1Service object using dot notation,
+                     for example, service.metadata.name to access the name of the service
             - kind: The Kubernetes object kind, which is always "ServiceList".
             - metadata: Additional metadata about the pod list, such as the resource version.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ServiceList.md
         """
 
         try:
-            response = self.getCoreV1Api().list_namespaced_service(
+            response = self.get_core_v1_api().list_namespaced_service(
                 field_selector=field_selector,
                 label_selector=label_selector,
-                namespace=self.getNamespace(),
+                namespace=self.get_namespace(),
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to list Services with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    field_selector, label_selector, str(e)
-                )
+                "Failed to list Services with field_selector -> %s and label_selector -> %s; error -> %s",
+                field_selector,
+                label_selector,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchService(self, service_name: str, service_body: dict):
+    def patch_service(self, service_name: str, service_body: dict):
         """Patches a Kubernetes Service with an updated spec
 
         Args:
             service_name (string): name of the Kubernetes Ingress in the current namespace
-            service_body (dict): new / updated Service body spec (will be merged with existing values)
+            service_body (dict): new / updated Service body spec
+                                 (will be merged with existing values)
         Returns:
             V1Service object or None if the call fails
-            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            This is NOT a dict but an object - you have to use the "." syntax
+            to access to returned elements
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Service.md
         """
 
         try:
-            response = self.getCoreV1Api().patch_namespaced_service(
-                name=service_name, namespace=self.getNamespace(), body=service_body
+            response = self.get_core_v1_api().patch_namespaced_service(
+                name=service_name, namespace=self.get_namespace(), body=service_body
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to patch Service -> {} with -> {}; error -> {}".format(
-                    service_name, service_body, str(e)
-                )
+                "Failed to patch Service -> %s with -> %s; error -> %s",
+                service_name,
+                service_body,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def getIngress(self, ingress_name: str):
+    def get_ingress(self, ingress_name: str):
         """Get a Kubernetes Ingress with a defined name in the current namespace
 
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
         Returns:
             V1Ingress object or None if the call fails
             This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
         try:
-            response = self.getNetworkingV1Api().read_namespaced_ingress(
-                name=ingress_name, namespace=self.getNamespace()
+            response = self.get_networking_v1_api().read_namespaced_ingress(
+                name=ingress_name, namespace=self.get_namespace()
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to get Ingress -> {}; error -> {}".format(ingress_name, str(e))
+                "Failed to get Ingress -> %s; error -> %s", ingress_name, str(exception)
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchIngress(self, ingress_name: str, ingress_body: dict):
+    def patch_ingress(self, ingress_name: str, ingress_body: dict):
         """Patch a Kubernetes Ingress with a updated spec.
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/NetworkingV1Api.md#patch_namespaced_ingress
 
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
-            ingress_body (dict): new / updated ingress body spec (will be merged with existing values)
+            ingress_body (dict): new / updated ingress body spec
+                                 (will be merged with existing values)
         Returns:
             V1Ingress object or None if the call fails
-            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            This is NOT a dict but an object - you have to use the
+            "." syntax to access to returned elements
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
         try:
-            response = self.getNetworkingV1Api().patch_namespaced_ingress(
+            response = self.get_networking_v1_api().patch_namespaced_ingress(
                 name=ingress_name,
-                namespace=self.getNamespace(),
+                namespace=self.get_namespace(),
                 body=ingress_body,
             )
-        except ApiException as e:
+        except ApiException as exception:
             logger.error(
-                "Failed to patch Ingress -> {} with -> {}; error -> {}".format(
-                    ingress_name, ingress_body, str(e)
-                )
+                "Failed to patch Ingress -> %s with -> %s; error -> %s",
+                ingress_name,
+                ingress_body,
+                str(exception),
             )
             return None
 
         return response
 
     # end method definition
 
-    def updateIngressBackendServices(
+    def update_ingress_backend_services(
         self, ingress_name: str, hostname: str, service_name: str, service_port: int
     ):
         """Updates a backend service and port of an Kubernetes Ingress
 
         "spec": {
             "rules": [
                 {
@@ -780,36 +822,39 @@
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
             hostname (string): hostname that should get an updated backend service / port
             service_name (string): new backend service name
             service_port (integer): new backend service port
         Returns:
             V1Ingress Object or None if the call fails
-            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            This is NOT a dict but an object - you have to use the "." syntax
+            to access to returned elements
             See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
-        ingress = self.getIngress(ingress_name)
+        ingress = self.get_ingress(ingress_name)
         if not ingress:
             return None
 
         host = ""
         rules = ingress.spec.rules
         rule_index = 0
         for rule in rules:
             if hostname in rule.host:
                 host = rule.host
                 path = rule.http.paths[0]
                 backend = path.backend
                 service = backend.service
 
                 logger.info(
-                    "Replace backend service -> {} ({}) with new backend service -> {} ({})".format(
-                        service.name, service.port.number, service_name, service_port
-                    )
+                    "Replace backend service -> %s (%s) with new backend service -> %s (%s)",
+                    service.name,
+                    service.port.number,
+                    service_name,
+                    service_port,
                 )
 
                 service.name = service_name
                 service.port.number = service_port
                 break
             else:
                 rule_index += 1
@@ -831,10 +876,10 @@
                 "path": "/spec/rules/{}/http/paths/0/backend/service/port/number".format(
                     rule_index
                 ),
                 "value": service_port,
             },
         ]
 
-        return self.patchIngress(ingress_name, body)
+        return self.patch_ingress(ingress_name, body)
 
     # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/m365.py` & `pyxecm-0.3.0/pyxecm/customizer/m365.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,53 +4,52 @@
 
 Class: M365
 Methods:
 
 __init__ : class initializer
 config : returns config data set
 credentials: returns the token data
-requestHeader: request header for MS Graph API calls
-parseRequestResponse: process result into Json
-existResultItem: check if an dict item is in the response
-                 of the Graph REST API call
-getResultValue: check if a defined value (based on a key) is in the Graph API response
-parseRequestResponse: parse the REST API responses and convert
-                      them to Python dict in a safe way
+request_header: request header for MS Graph API calls
+parse_request_response: parse the REST API responses and convert
+                        them to Python dict in a safe way
+exist_result_item: check if an dict item is in the response
+                   of the Graph REST API call
+get_result_value: check if a defined value (based on a key) is in the Graph API response
 
 authenticate : authenticates at M365 Graph API
 
-getUsers: Get list all all users in M365 tenant 
-getUser: Get a M365 User based on its email
-getGroups: Get list all all groups in M365 tenant
-getGroup: Get a M365 Group based on its name
-addGroup: Add a M365 Group
-addUser: Add a M365 User
-hasTeam: Check if a M365 Group has a M365 Team connected or not
-addTeam: Add a M365 Team (based on an existing group)
-deleteTeams: Delete MS teams with a given name
-getUserLicenses: Get the assigned license SKUs of a user
-assignLicenseToUser: Add an M365 license to a user (e.g. to use Office 365)
-getUserPhoto: Retriev the photo of a M365 user
-updateUserPhoto: Update a user with a profile photo (which must be in local file system)
-getGroupMembers: Get members (users and groups) of the specified group
-getGroupOwners: Get owners (users) of the specified group
-addGroupMember: Add a user or group to a target group
-isMember: Check whether a M365 user is already in a M365 group
-addGroupOwner: Add a user as owner to a group
-purgeDeletedItems: Purge all deleted users and groups in the organization
-purgeDeletedItem: Help function that purges a single user or group
-getTeamsApps: Get a list of MS Teams apps in catalog that match a given filter criterium
-uploadTeamsApp: Upload a new app package to the catalog of MS Teams apps
-removeTeamsApp: Remove MS Teams App for the app catalog
-assignTeamsAppToUser: Assign (add) a MS teams app to a M365 user.
-upgradeTeamsAppOfUser: Upgrade a MS teams app for a user.
-addSensitivityLabel: Assign a existing sensitivity label to a user.
-                     THIS IS CURRENTLY NOT WORKING!
-assignSensitivityLabelToUser: Create a new sensitivity label in M365
-                              THIS IS CURRENTLY NOT WORKING!
+get_users: Get list all all users in M365 tenant 
+get_user: Get a M365 User based on its email
+get_groups: Get list all all groups in M365 tenant
+get_group: Get a M365 Group based on its name
+add_group: Add a M365 Group
+add_user: Add a M365 User
+has_team: Check if a M365 Group has a M365 Team connected or not
+add_team: Add a M365 Team (based on an existing group)
+delete_teams: Delete MS teams with a given name
+get_user_licenses: Get the assigned license SKUs of a user
+assign_license_to_user: Add an M365 license to a user (e.g. to use Office 365)
+get_user_photo: Retriev the photo of a M365 user
+update_user_photo: Update a user with a profile photo (which must be in local file system)
+get_group_members: Get members (users and groups) of the specified group
+get_group_owners: Get owners (users) of the specified group
+add_group_member: Add a user or group to a target group
+is_member: Check whether a M365 user is already in a M365 group
+add_group_owner: Add a user as owner to a group
+purge_deleted_items: Purge all deleted users and groups in the organization
+purge_deleted_item: Help function that purges a single user or group
+get_teams_apps: Get a list of MS Teams apps in catalog that match a given filter criterium
+upload_teams_app: Upload a new app package to the catalog of MS Teams apps
+remove_teams_app: Remove MS Teams App for the app catalog
+assign_teams_app_to_user: Assign (add) a MS teams app to a M365 user.
+upgrade_teams_app_of_user: Upgrade a MS teams app for a user.
+add_sensitivity_label: Assign a existing sensitivity label to a user.
+                       THIS IS CURRENTLY NOT WORKING!
+assign_sensitivity_label_to_user: Create a new sensitivity label in M365
+                                  THIS IS CURRENTLY NOT WORKING!
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
@@ -61,17 +60,17 @@
 import re
 import urllib.parse
 import zipfile
 from urllib.parse import quote
 
 import requests
 
-logger = logging.getLogger("customizer.m365")
+logger = logging.getLogger("pyxecm.customizer.m365")
 
-requestLoginHeaders = {
+request_login_headers = {
     "Content-Type": "application/x-www-form-urlencoded",
     "Accept": "application/json",
 }
 
 
 class M365(object):
     """Used to automate stettings in Microsoft 365 via the Graph API."""
@@ -84,67 +83,79 @@
         self,
         tenant_id: str,
         client_id: str,
         client_secret: str,
         domain: str,
         sku_id: str,
         teams_app_name: str,
+        **kwargs,
     ):
         """Initialize the M365 object
 
         Args:
             tenant_id (string): M365 Tenant ID
             client_id (string): M365 Client ID
             client_secret (string): M365 Client Secret
             domain (string): M365 domain
             sku_id (string): License SKU for M365 users
             teams_app_name (string): name of the Extended ECM app for MS Teams
+            kwargs
         """
 
-        m365Config = {}
+        m365_config = {}
 
         # Set the authentication endpoints and credentials
-        m365Config["tenantId"] = tenant_id
-        m365Config["clientId"] = client_id
-        m365Config["clientSecret"] = client_secret
-        m365Config["domain"] = domain
-        m365Config["skuId"] = sku_id
-        m365Config["teamsAppName"] = teams_app_name
-        m365Config[
+        m365_config["tenantId"] = tenant_id
+        m365_config["clientId"] = client_id
+        m365_config["clientSecret"] = client_secret
+        m365_config["domain"] = domain
+        m365_config["skuId"] = sku_id
+        m365_config["teamsAppName"] = teams_app_name
+        m365_config[
             "authenticationUrl"
         ] = "https://login.microsoftonline.com/{}/oauth2/v2.0/token".format(tenant_id)
-        m365Config["graphUrl"] = "https://graph.microsoft.com/v1.0/"
-        m365Config["betaUrl"] = "https://graph.microsoft.com/beta/"
-        m365Config["directoryObjects"] = m365Config["graphUrl"] + "directoryObjects"
+        m365_config["graphUrl"] = "https://graph.microsoft.com/v1.0/"
+        m365_config["betaUrl"] = "https://graph.microsoft.com/beta/"
+        m365_config["directoryObjects"] = m365_config["graphUrl"] + "directoryObjects"
 
         # Set the data for the token request
-        m365Config["tokenData"] = {
+        m365_config["tokenData"] = {
             "client_id": client_id,
             "scope": "https://graph.microsoft.com/.default",
             "client_secret": client_secret,
             "grant_type": "client_credentials",
         }
 
-        m365Config["groupsUrl"] = m365Config["graphUrl"] + "groups"
-        m365Config["usersUrl"] = m365Config["graphUrl"] + "users"
-        m365Config["teamsUrl"] = m365Config["graphUrl"] + "teams"
-        m365Config["teamsTemplatesUrl"] = m365Config["graphUrl"] + "teamsTemplates"
-        m365Config["teamsAppsUrl"] = m365Config["graphUrl"] + "appCatalogs/teamsApps"
-        m365Config["directoryUrl"] = m365Config["graphUrl"] + "directory"
-        m365Config["securityUrl"] = m365Config["betaUrl"] + "security"
+        m365_config["groupsUrl"] = m365_config["graphUrl"] + "groups"
+        m365_config["usersUrl"] = m365_config["graphUrl"] + "users"
+        m365_config["teamsUrl"] = m365_config["graphUrl"] + "teams"
+        m365_config["teamsTemplatesUrl"] = m365_config["graphUrl"] + "teamsTemplates"
+        m365_config["teamsAppsUrl"] = m365_config["graphUrl"] + "appCatalogs/teamsApps"
+        m365_config["directoryUrl"] = m365_config["graphUrl"] + "directory"
+        m365_config["securityUrl"] = m365_config["betaUrl"] + "security"
 
-        self._config = m365Config
+        self._config = m365_config
 
-    def config(self):
+    def config(self) -> dict:
+        """Returns the configuration dictionary
+
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
-    def credentials(self):
+    def credentials(self) -> dict:
+        """Return the login credentials
+
+        Returns:
+            dict: dictionary with login credentials for M365
+        """
         return self.config()["tokenData"]
 
-    def credentialsUser(self, username: str, password: str) -> dict:
+    def credentials_user(self, username: str, password: str) -> dict:
         """In some cases MS Graph APIs cannot be called via
             application permissions (client_id, client_secret)
             but requires a token of a user authenticated
             with username + password. This is e.g. the case
             to upload a MS teams app to the catalog.
             See https://learn.microsoft.com/en-us/graph/api/teamsapp-publish
 
@@ -163,38 +174,56 @@
             "username": username,
             "password": password,
         }
         return credentials
 
     # end method definition
 
-    def requestHeader(self, content_type: str = "application/json") -> dict:
+    def request_header(self, content_type: str = "application/json") -> dict:
+        """Deliver the request header used for Application calls.
+           Consists of Bearer access token and Content Type
+
+        Args:
+            None.
+        Return:
+            dictionary: request header values
+        """
+
         request_header = {
             "Authorization": "Bearer {}".format(self._access_token),
             "Content-Type": content_type,
         }
         return request_header
 
     # end method definition
 
-    def requestHeaderUser(self, content_type: str = "application/json") -> dict:
+    def request_header_user(self, content_type: str = "application/json") -> dict:
+        """Deliver the request header used for user specific calls.
+           Consists of Bearer access token and Content Type
+
+        Args:
+            None.
+        Return:
+            dictionary: request header values
+        """
+
         request_header = {
             "Authorization": "Bearer {}".format(self._user_access_token),
             "Content-Type": content_type,
         }
         return request_header
 
     # end method definition
 
-    def parseRequestResponse(
+    def parse_request_response(
         self,
         response_object: requests.Response,
         additional_error_message: str = "",
         show_error: bool = True,
-    ) -> dict:
+    ) -> dict | None:
         """Converts the request response (JSon) to a Python dict in a safe way
            that also handles exceptions. It first tries to load the response.text
            via json.loads() that produces a dict output. Only if response.text is
            not set or is empty it just converts the response_object to a dict using
            the vars() built-in method.
 
         Args:
@@ -204,39 +233,41 @@
             show_error (boolean): True: write an error to the log file
                                   False: write a warning to the log file
         Returns:
             dictionary: response information or None in case of an error
         """
 
         if not response_object:
-            return {}
+            return None
 
         try:
             if response_object.text:
                 dict_object = json.loads(response_object.text)
             else:
                 dict_object = vars(response_object)
-        except json.JSONDecodeError as e:
+        except json.JSONDecodeError as exception:
             if additional_error_message:
                 message = "Cannot decode response as JSon. {}; error -> {}".format(
-                    additional_error_message, e
+                    additional_error_message, exception
                 )
             else:
-                message = "Cannot decode response as JSon; error -> {}".format(e)
+                message = "Cannot decode response as JSon; error -> {}".format(
+                    exception
+                )
             if show_error:
                 logger.error(message)
             else:
                 logger.warning(message)
-            return {}
+            return None
         else:
             return dict_object
 
     # end method definition
 
-    def existResultItem(
+    def exist_result_item(
         self, response: dict, key: str, value: str, sub_dict_name: str = ""
     ) -> bool:
         """Check existence of key / value pair in the response properties of an MS Graph API call.
 
         Args:
             response (dictionary): REST response from an MS Graph REST Call
             key (string): property name (key)
@@ -268,76 +299,78 @@
                     return False
                 if value == item[sub_dict_name][key]:
                     return True
         return False
 
     # end method definition
 
-    def getResultValue(self, response: dict, key: str, index: int = 0) -> str:
+    def get_result_value(self, response: dict, key: str, index: int = 0) -> str | None:
         """Get value of a result property with a given key of an MS Graph API call.
 
         Args:
             response (dictionary): REST response from an MS Graph REST Call
             key (string): property name (key)
             index (integer, optional): Index to use (1st element has index  0).
                                        Defaults to 0.
         Returns:
             string: value for the key, None otherwise
         """
 
         if not response:
-            return ""
+            return None
         if not "value" in response:
-            return ""
+            return None
 
         values = response["value"]
         if not values or not isinstance(values, list) or len(values) - 1 < index:
-            return ""
+            return None
 
         return values[index][key]
 
     # end method definition
 
-    def authenticate(self, revalidate: bool = False):
+    def authenticate(self, revalidate: bool = False) -> str | None:
         """Authenticate at M365 Graph API with client ID and client secret.
 
         Args:
             revalidate (boolean, optional): determinse if a re-athentication is enforced
                                             (e.g. if session has timed out with 401 error)
         Returns:
             Access token. Also stores access token in self._access_token
         """
 
         # Already authenticated and session still valid?
         if self._access_token and not revalidate:
             return self._access_token
 
         request_url = self.config()["authenticationUrl"]
-        request_header = requestLoginHeaders
+        request_header = request_login_headers
 
         logger.info("Requesting M365 Access Token from -> %s", request_url)
 
         authenticate_post_body = self.credentials()
         authenticate_response = None
 
         try:
             authenticate_response = requests.post(
                 request_url,
                 data=authenticate_post_body,
                 headers=request_header,
                 timeout=60,
             )
-        except requests.exceptions.ConnectionError as e:
+        except requests.exceptions.ConnectionError as exception:
             logger.warning(
-                "Unable to connect to -> %s : %s", self.config()["authenticationUrl"], e
+                "Unable to connect to -> %s : %s",
+                self.config()["authenticationUrl"],
+                exception,
             )
             return None
 
         if authenticate_response.ok:
-            authenticate_dict = self.parseRequestResponse(authenticate_response)
+            authenticate_dict = self.parse_request_response(authenticate_response)
             if not authenticate_dict:
                 return None
             else:
                 access_token = authenticate_dict["access_token"]
                 logger.debug("Access Token -> %s", access_token)
         else:
             logger.error(
@@ -348,34 +381,34 @@
 
         # Store authentication access_token:
         self._access_token = access_token
         return self._access_token
 
     # end method definition
 
-    def authenticateUser(self, username: str, password: str):
+    def authenticate_user(self, username: str, password: str) -> str | None:
         """Authenticate at M365 Graph API with username and password.
 
         Args:
             username (string): name (emails) of the M365 user
             password (string): password of the M365 user
         Returns:
             Access token. Also stores access token in self._access_token
         """
 
         request_url = self.config()["authenticationUrl"]
-        request_header = requestLoginHeaders
+        request_header = request_login_headers
 
         logger.info(
             "Requesting M365 Access Token for user -> %s from -> %s",
             username,
             request_url,
         )
 
-        authenticate_post_body = self.credentialsUser(username, password)
+        authenticate_post_body = self.credentials_user(username, password)
         authenticate_response = None
 
         try:
             authenticate_response = requests.post(
                 request_url,
                 data=authenticate_post_body,
                 headers=request_header,
@@ -387,15 +420,15 @@
                 self.config()["authenticationUrl"],
                 username,
                 e,
             )
             return None
 
         if authenticate_response.ok:
-            authenticate_dict = self.parseRequestResponse(authenticate_response)
+            authenticate_dict = self.parse_request_response(authenticate_response)
             if not authenticate_dict:
                 return None
             else:
                 access_token = authenticate_dict["access_token"]
                 logger.debug("User Access Token -> %s", access_token)
         else:
             logger.error(
@@ -407,54 +440,55 @@
 
         # Store authentication access_token:
         self._user_access_token = access_token
         return self._user_access_token
 
     # end method definition
 
-    def getUsers(self):
+    def get_users(self) -> dict | None:
         """Get list all all users in M365 tenant
 
         Returns:
             List of all users.
         """
 
         request_url = self.config()["usersUrl"]
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info("Get list of all users; calling -> %s", request_url)
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of users; status -> %s; error -> %s",
                     response.status_code,
                     response.text,
                 )
                 return None
 
     # end method definition
 
-    def getUser(self, user_email: str, show_error: bool = False):
+    def get_user(self, user_email: str, show_error: bool = False) -> dict | None:
         """Get a M365 User based on its email
 
         Args:
             user_email (string): M365 user email
         Returns:
-            User information (json) or None if the user couldn't be retrieved (e.g. because it doesn't exist).
+            dict: User information or None if the user couldn't be retrieved (e.g. because it doesn't exist
+                  or if there is a permission problem).
             Example Output:
             {
                 '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#users/$entity',
                 'businessPhones': [],
                 'displayName': 'Bob Davis',
                 'givenName': 'Bob',
                 'id': '72c80809-094f-4e6e-98d4-25a736385d10',
@@ -465,91 +499,91 @@
                 'preferredLanguage': None,
                 'surname': 'Davis',
                 'userPrincipalName': 'bdavis@M365x61936377.onmicrosoft.com'
             }
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_email
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
-        logger.info("Get user -> %s; calling -> %s", user_email, request_url)
+        logger.info("Get M365 user -> %s; calling -> %s", user_email, request_url)
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 if show_error:
                     logger.error(
-                        "Failed to get user -> %s; status -> %s; error -> %s",
+                        "Failed to get M365 user -> %s; status -> %s; error -> %s",
                         user_email,
                         response.status_code,
                         response.text,
                     )
                 else:
-                    logger.info("User -> %s not found.", user_email)
+                    logger.info("M365 User -> %s not found.", user_email)
                 return None
 
     # end method definition
 
-    def getGroups(self, max_number: int = 250) -> dict:
+    def get_groups(self, max_number: int = 250) -> dict | None:
         """Get list all all groups in M365 tenant
 
         Args:
-            None
+            max_number (int): maximum result values (limit)
         Returns:
-            List of all groups.
+            List of all groups or None in case of an error.
         """
 
         request_url = self.config()["groupsUrl"]
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
-        logger.info("Get list of all groups; calling -> %s", request_url)
+        logger.info("Get list of all M365 groups; calling -> %s", request_url)
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
                 headers=request_header,
                 params={"$top": str(max_number)},
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get list of groups; status -> %s; error -> %s",
+                    "Failed to get list of M365 groups; status -> %s; error -> %s",
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def getGroup(self, group_name: str, show_error: bool = False) -> dict:
+    def get_group(self, group_name: str, show_error: bool = False) -> dict | None:
         """Get a M365 Group based on its name
 
         Args:
             group_name (string): M365 Group name
             show_error (boolean): should an error be logged if group is not found.
         Returns:
-            dictionary: Group information or None if the group couldn't be created (e.g. because it exisits already).
+            dictionary: Group information or None if the group doesn't exist.
             Example Output:
             {
                 '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#groups',
                 'value': [
                     {
                         'id': 'b65f7dba-3ed1-49df-91bf-2bf99affcc8d',
                         'deletedDateTime': None,
@@ -592,46 +626,46 @@
             }
         """
 
         query = {"$filter": "displayName eq '" + group_name + "'"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = self.config()["groupsUrl"] + "?" + encoded_query
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
-        logger.info("Get group -> %s; calling -> %s", group_name, request_url)
+        logger.info("Get M365 group -> %s; calling -> %s", group_name, request_url)
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 if show_error:
                     logger.error(
-                        "Failed to get group -> %s; status -> %s; error -> %s",
+                        "Failed to get M365 group -> %s; status -> %s; error -> %s",
                         group_name,
                         response.status_code,
                         response.text,
                     )
                 else:
-                    logger.info("Group -> %s not found.", group_name)
-                return {}
+                    logger.info("M365 Group -> %s not found.", group_name)
+                return None
 
     # end method definition
 
-    def addGroup(
+    def add_group(
         self, name: str, security_enabled: bool = False, mail_enabled: bool = True
-    ):
+    ) -> dict | None:
         """Add a M365 Group.
 
         Args:
             name (string): name of the group
             security_enabled (boolean, optional): whether or not this group is used for permission management
             mail_enabled (boolean, optional): whether or not this group is email enabled
         Returns:
@@ -679,66 +713,67 @@
             "mailEnabled": mail_enabled,
             "mailNickname": name.replace(" ", ""),
             "securityEnabled": security_enabled,
             "groupTypes": ["Unified"],
         }
 
         request_url = self.config()["groupsUrl"]
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info("Adding M365 group -> %s; calling -> %s", name, request_url)
         logger.debug("M365 group attributes -> %s", group_post_body)
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(group_post_body),
                 headers=request_header,
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add M365 group -> %s; status -> %s; error -> %s",
                     name,
                     response.status_code,
                     response.text,
                 )
                 return None
 
     # end method definition
 
-    def addUser(
+    def add_user(
         self,
         email: str,
         password: str,
         first_name: str,
         last_name: str,
         location: str = "US",
         department: str = "",
-    ) -> dict:
+    ) -> dict | None:
         """Add a M365 user.
 
         Args:
             email (string): email address of the user. This is also the unique identifier
             password (string): password of the user
             first_name (string): first name of the user
             last_name (string): last name of the user
             location (string, optional): country ISO 3166-1 alpha-2 format (e.g. US, CA, FR, DE, CN, ...)
             department (string, optional): department of the user
         Returns:
-            dictionary: User information or None if the user couldn't be created (e.g. because it exisits already).
+            dictionary: User information or None if the user couldn't be created (e.g. because it exisits already
+                        or if a permission problem occurs).
         """
 
         user_post_body = {
             "accountEnabled": True,
             "displayName": first_name + " " + last_name,
             "givenName": first_name,
             "surname": last_name,
@@ -750,62 +785,62 @@
             },
             "usageLocation": location,
         }
         if department:
             user_post_body["department"] = department
 
         request_url = self.config()["usersUrl"]
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info("Adding M365 user -> %s; calling -> %s", email, request_url)
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(user_post_body),
                 headers=request_header,
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add M365 user -> %s; status -> %s; error -> %s",
                     email,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def hasTeam(self, group_name: str) -> bool:
+    def has_team(self, group_name: str) -> bool:
         """Check if a M365 Group has a M365 Team connected or not
 
         Args:
             group_name (str): name of the M365 group
         Returns:
             boolean: Returns True if a Team is assigned and False otherwise
         """
 
-        response = self.getGroup(group_name)
+        response = self.get_group(group_name)
         if response is None or not "value" in response or not response["value"]:
             logger.error("M365 group -> %s not found.", group_name)
             return False
         group_id = response["value"][0]["id"]
 
         request_url = self.config()["groupsUrl"] + "/" + group_id + "/team"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
             "Check if group -> %s has a M365 Team connected; calling -> %s",
             group_name,
             request_url,
         )
 
@@ -818,47 +853,47 @@
                 return True
             elif response.status_code == 404:  # Group does not have a Team assigned!
                 logger.info("Group -> %s has has no M365 team connected.", group_name)
                 return False
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to check if group -> %s has a Team connected; status -> %s; error -> %s",
                     group_name,
                     response.status_code,
                     response.text,
                 )
                 return False
 
     # end method definition
 
-    def addTeam(self, name: str, template_name: str = "standard"):
+    def add_team(self, name: str, template_name: str = "standard") -> dict | None:
         """Add M365 Team based on an existing M365 Group.
 
         Args:
             name (string): name of the team. It is assumed that a group with the same name does already exist!
             template_name (string, optional): name of the team template. "standard" is the default value.
         Returns:
             Team information (json - empty text!) or None if the team couldn't be created (e.g. because it exisits already).
         """
 
-        response = self.getGroup(name)
+        response = self.get_group(name)
         if response is None or not "value" in response or not response["value"]:
             logger.error(
                 "M365 group -> %s not found. It is required for creating a corresponding M365 Team.",
                 name,
             )
             return None
         group_id = response["value"][0]["id"]
 
-        response = self.getGroupOwners(name)
+        response = self.get_group_owners(name)
         if response is None or not "value" in response or not response["value"]:
             logger.warning(
                 "M365 group -> %s has no owners. This is required for creating a corresponding M365 Team.",
                 name,
             )
             return None
 
@@ -866,47 +901,47 @@
             "template@odata.bind": "{}('{}')".format(
                 self.config()["teamsTemplatesUrl"], template_name
             ),
             "group@odata.bind": "{}('{}')".format(self.config()["groupsUrl"], group_id),
         }
 
         request_url = self.config()["teamsUrl"]
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info("Adding team -> %s; calling -> %s", name, request_url)
         logger.debug("Team Attributes -> %s", team_post_body)
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(team_post_body),
                 headers=request_header,
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add team -> %s; status -> %s; error -> %s",
                     name,
                     response.status_code,
                     response.text,
                 )
                 return None
 
     # end method definition
 
-    def deleteTeams(self, name: str) -> bool:
+    def delete_teams(self, name: str) -> bool:
         """Delete Microsoft 365 Teams with a specific name. Microsoft 365 allows
             to have multiple teams with the same name. So this method may delete
             multiple teams if the have the same name. The Graph API we use here
             is the M365 Group API as deleting the group also deletes the associated team.
 
         Args:
             name (string): name of the Microsoft 365 Team
@@ -917,33 +952,33 @@
         # We need a special handling of team names with single quotes:
         escaped_group_name = name.replace("'", "''")
         encoded_group_name = quote(escaped_group_name, safe="")
         request_url = self.config()[
             "groupsUrl"
         ] + "?$filter=displayName eq '{}'".format(encoded_group_name)
 
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
             "Delete all Microsoft 365 Teams with name -> %s; calling -> %s",
             name,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                existing_teams = self.parseRequestResponse(response)
+                existing_teams = self.parse_request_response(response)
                 break
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of groups; status -> %s; error -> %s",
                     response.status_code,
                     response.text,
                 )
@@ -977,30 +1012,30 @@
                 return False
         else:
             logger.error("Failed to retrieve teams with name -> %s", name)
             return False
 
     # end method definition
 
-    def deleteAllTeams(self, exception_list: list, pattern_list: list) -> bool:
+    def delete_all_teams(self, exception_list: list, pattern_list: list) -> bool:
         """Delete all teams (groups) that are NOT on the exception list AND
            that are matching at least one of the patterns in the provided pattern list.
            This method is used for general cleanup of teams. Be aware that deleted teams
            are still listed under https://admin.microsoft.com/#/deletedgroups
 
         Args:
             exception_list (list): list of group names that should not be deleted
             pattern_list (list): list of patterns for group names to be deleted
                                  (regular expression)
         Returns:
             boolean: True if teams have been deleted, False otherwise.
         """
 
         # Get list of all existing M365 groups/teams:
-        response = self.getGroups(max_number=500)
+        response = self.get_groups(max_number=500)
         if not "value" in response or not response["value"]:
             return False
         groups = response["value"]
         logger.info(
             "Found -> %s existing M365 groups. Checking which ones should be deleted...",
             len(groups),
         )
@@ -1020,26 +1055,26 @@
                 result = re.search(pattern, group_name)
                 if result:
                     logger.info(
                         "Group name -> %s is matching pattern -> %s. Delete it now...",
                         group_name,
                         pattern,
                     )
-                    self.deleteTeams(group_name)
+                    self.delete_teams(group_name)
                     break
             else:
                 logger.info(
                     "Group name -> %s is not matching any delete pattern. Skipping.",
                     group_name,
                 )
         return True
 
     # end method definition
 
-    def getUserLicenses(self, user_id: str) -> dict:
+    def get_user_licenses(self, user_id: str) -> dict | None:
         """Get the assigned license SKUs of a user
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
         Returns:
             dictionary: List of user licenses or None if request fails.
             Example Output:
@@ -1053,124 +1088,124 @@
                         'servicePlans': [{...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, ...]
                     }
                 ]
             }
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_id + "/licenseDetails"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get licenses of user -> %s; status -> %s; error -> %s",
+                    "Failed to get M365 licenses of user -> %s; status -> %s; error -> %s",
                     user_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def assignLicenseToUser(self, user_id: str, sku_id: str) -> dict:
+    def assign_license_to_user(self, user_id: str, sku_id: str) -> dict | None:
         """Add an M365 license to a user (e.g. to use Office 365)
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             sku_id (string): M365 GUID of the SKU
                             (e.g. c7df2760-2c81-4ef7-b578-5b5392b571df for E5 and
                                   6fd2c87f-b296-42f0-b197-1e91e994b900 for E3)
 
         Returns:
             dictionary: response or None if request fails
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_id + "/assignLicense"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         # Construct the request body for assigning the E5 license
         license_post_body = {
             "addLicenses": [
                 {
                     "disabledPlans": [],
                     "skuId": sku_id,  # "c42b9cae-ea4f-4a69-9ca5-c53bd8779c42"
                 }
             ],
             "removeLicenses": [],
         }
 
         logger.info(
-            "Assign license -> %s to user -> %s; calling -> %s",
+            "Assign M365 license -> %s to M365 user -> %s; calling -> %s",
             sku_id,
             user_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url, json=license_post_body, headers=request_header, timeout=60
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add license -> %s to user -> %s; status -> %s; error -> %s",
+                    "Failed to add M365 license -> %s to M365 user -> %s; status -> %s; error -> %s",
                     sku_id,
                     user_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def getUserPhoto(self, user_id: str, show_error: bool = True):
+    def get_user_photo(self, user_id: str, show_error: bool = True):
         """Get the photo of a M365 user
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             show_error (boolean): whether or not an error should be logged if the user
                                   does not have a photo in M365
         Returns:
             string: Image of the user photo or None if the user photo couldn't be retrieved.
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_id + "/photo/$value"
         # Set image as content type:
-        request_header = self.requestHeader("image/*")
+        request_header = self.request_header("image/*")
 
         logger.info("Get photo of user -> %s; calling -> %s", user_id, request_url)
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
                 return response.content  # this is the actual image - not json!
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get photo of user -> %s; status -> %s; error -> %s",
                         user_id,
                         response.status_code,
@@ -1178,198 +1213,198 @@
                     )
                 else:
                     logger.info("User -> %s does not yet have a photo.", user_id)
                 return None
 
     # end method definition
 
-    def updateUserPhoto(self, user_id: str, photo_path: str) -> dict:
+    def update_user_photo(self, user_id: str, photo_path: str) -> dict | None:
         """Update the M365 user photo
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             photo_path (string): file system path with the location of the photo
         Returns:
             dictionary: Response of Graph REST API or None if the user photo couldn't be updated.
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_id + "/photo/$value"
         # Set image as content type:
-        request_header = self.requestHeader("image/*")
+        request_header = self.request_header("image/*")
 
         # Check if the photo file exists
         if not os.path.isfile(photo_path):
             logger.error("Photo file -> %s not found!", photo_path)
-            return {}
+            return None
 
         try:
             # Read the photo file as binary data
             with open(photo_path, "rb") as image_file:
                 photo_data = image_file.read()
         except OSError as e:
             # Handle any errors that occurred while reading the photo file
             logger.error("Error reading photo file -> %s; error -> %s", photo_path, e)
-            return {}
+            return None
 
         data = photo_data
 
         logger.info(
-            "Update user -> %s with photo -> %s; calling -> %s",
+            "Update M365 user -> %s with photo -> %s; calling -> %s",
             user_id,
             photo_path,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.put(
                 request_url, headers=request_header, data=data, timeout=60
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user -> %s with photo -> %s; status -> %s; error -> %s",
                     user_id,
                     photo_path,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def getGroupMembers(self, group_name: str) -> dict:
+    def get_group_members(self, group_name: str) -> dict | None:
         """Get members (users and groups) of the specified group.
 
         Args:
             group_name (string): name of the group
         Returns:
             dictionary: Response of Graph REST API or None if the REST call fails.
         """
 
-        response = self.getGroup(group_name)
+        response = self.get_group(group_name)
         if not response or not "value" in response or not response["value"]:
             logger.error(
                 "Group -> %s does not exist! Cannot retrieve group members.", group_name
             )
-            return {}
+            return None
         group_id = response["value"][0]["id"]
 
         query = {"$select": "id,displayName,mail,userPrincipalName"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = (
             self.config()["groupsUrl"] + "/" + group_id + "/members?" + encoded_query
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
-            "Get members of group -> %s (%s); calling -> %s",
+            "Get members of M365 group -> %s (%s); calling -> %s",
             group_name,
             group_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get members of group -> %s (%s); status -> %s; error -> %s",
+                    "Failed to get members of M365 group -> %s (%s); status -> %s; error -> %s",
                     group_name,
                     group_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def getGroupOwners(self, group_name: str) -> dict:
+    def get_group_owners(self, group_name: str) -> dict | None:
         """Get owners (users) of the specified group.
 
         Args:
             group_name (string): name of the group
         Returns:
             dictionary: Response of Graph REST API or None if the REST call fails.
         """
 
-        response = self.getGroup(group_name)
+        response = self.get_group(group_name)
         if not response or not "value" in response or not response["value"]:
             logger.error(
                 "Group -> %s does not exist! Cannot retrieve group owners.", group_name
             )
-            return {}
+            return None
         group_id = response["value"][0]["id"]
 
         query = {"$select": "id,displayName,mail,userPrincipalName"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = (
             self.config()["groupsUrl"] + "/" + group_id + "/owners?" + encoded_query
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
-            "Get owners of group -> %s (%s); calling -> %s",
+            "Get owners of M365 group -> %s (%s); calling -> %s",
             group_name,
             group_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get owners of group -> %s (%s); status -> %s; error -> %s",
+                    "Failed to get owners of M365 group -> %s (%s); status -> %s; error -> %s",
                     group_name,
                     group_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def addGroupMember(self, group_id: str, member_id: str) -> dict:
+    def add_group_member(self, group_id: str, member_id: str) -> dict | None:
         """Add a member (user or group) to a (parent) group
 
         Args:
             group_id (string): M365 GUID of the group
             member_id (string): M365 GUID of the new member
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
 
         request_url = self.config()["groupsUrl"] + "/" + group_id + "/members/$ref"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         group_member_post_body = {
             "@odata.id": self.config()["directoryObjects"] + "/" + member_id
         }
 
         logger.info(
             "Adding member -> %s to group -> %s; calling -> %s",
@@ -1383,35 +1418,35 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=json.dumps(group_member_post_body),
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
 
             # Check if Session has expired - then re-authenticate and try once more
             if response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add member -> %s to group -> %s; status -> %s; error -> %s",
+                    "Failed to add member -> %s to M365 group -> %s; status -> %s; error -> %s",
                     member_id,
                     group_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def isMember(self, group_id: str, member_id: str, show_error: bool = True) -> bool:
+    def is_member(self, group_id: str, member_id: str, show_error: bool = True) -> bool:
         """Checks whether a M365 user is already in a M365 group
 
         Args:
             group_id (string): M365 GUID of the group
             member_id (string): M365 GUID of the user (member)
             show_error (boolean): whether or not an error should be logged if the user
                                   is not a member of the group
@@ -1420,36 +1455,36 @@
         """
 
         # don't encode this URL - this has not been working!!
         request_url = (
             self.config()["groupsUrl"]
             + f"/{group_id}/members?$filter=id eq '{member_id}'"
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
             "Check if user -> %s is in group -> %s; calling -> %s",
             member_id,
             group_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                response = self.parseRequestResponse(response)
+                response = self.parse_request_response(response)
                 if not "value" in response or len(response["value"]) == 0:
                     return False
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 # MS Graph API returns an error if the member is not in the
                 # group. This is typically not what we want. We just return False.
                 if show_error:
                     logger.error(
                         "Failed to check if user -> %s is in group -> %s; status -> %s; error -> %s",
@@ -1458,135 +1493,135 @@
                         response.status_code,
                         response.text,
                     )
                 return False
 
     # end method definition
 
-    def addGroupOwner(self, group_id: str, owner_id: str) -> dict:
+    def add_group_owner(self, group_id: str, owner_id: str) -> dict | None:
         """Add an owner (user) to a group
 
         Args:
             group_id (string): M365 GUID of the group
             owner_id (string): M365 GUID of the new member
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
 
         request_url = self.config()["groupsUrl"] + "/" + group_id + "/owners/$ref"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         group_member_post_body = {
             "@odata.id": self.config()["directoryObjects"] + "/" + owner_id
         }
 
         logger.info(
-            "Adding owner -> %s to group -> %s; calling -> %s",
+            "Adding owner -> %s to M365 group -> %s; calling -> %s",
             owner_id,
             group_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=json.dumps(group_member_post_body),
                 timeout=60,
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add owner -> %s to group -> %s; status -> %s; error -> %s",
+                    "Failed to add owner -> %s to M365 group -> %s; status -> %s; error -> %s",
                     owner_id,
                     group_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def purgeDeletedItems(self):
+    def purge_deleted_items(self):
         """Purge all deleted users and groups.
         Purging users and groups requires administrative rights that typically
         are not provided in Contoso example org.
         """
 
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         request_url = (
             self.config()["directoryUrl"] + "/deletedItems/microsoft.graph.group"
         )
         response = requests.get(request_url, headers=request_header, timeout=60)
-        deleted_groups = self.parseRequestResponse(response)
+        deleted_groups = self.parse_request_response(response)
 
         for group in deleted_groups["value"]:
             group_id = group["id"]
-            response = self.purgeDeletedItem(group_id)
+            response = self.purge_deleted_item(group_id)
 
         request_url = (
             self.config()["directoryUrl"] + "/deletedItems/microsoft.graph.user"
         )
         response = requests.get(request_url, headers=request_header, timeout=60)
-        deleted_users = self.parseRequestResponse(response)
+        deleted_users = self.parse_request_response(response)
 
         for user in deleted_users["value"]:
             user_id = user["id"]
-            response = self.purgeDeletedItem(user_id)
+            response = self.purge_deleted_item(user_id)
 
     # end method definition
 
-    def purgeDeletedItem(self, item_id: str):
+    def purge_deleted_item(self, item_id: str) -> dict | None:
         """Helper method to purge a single deleted user or group.
            This requires elevated permissions that are typically
            not available via Graph API.
 
         Args:
             item_id (string): M365 GUID of the user or group to purge
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
 
         request_url = self.config()["directoryUrl"] + "/deletedItems/" + item_id
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info("Purging deleted item -> %s; calling -> %s", item_id, request_url)
 
         retries = 0
         while True:
             response = requests.delete(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
                     "Failed to purge deleted item -> %s; status -> %s; error -> %s",
                     item_id,
                     response.status_code,
                     response.text,
                 )
                 return None
 
     # end method definition
 
-    def getTeamsApps(self, filter_expression: str = "") -> dict:
+    def get_teams_apps(self, filter_expression: str = "") -> dict | None:
         """Get a list of MS Teams apps in catalog that match a given filter criterium
 
         Args:
             filter_expression (string, optional): filter string see https://learn.microsoft.com/en-us/graph/filter-query-parameter
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
@@ -1600,38 +1635,40 @@
                 filter_expression,
                 request_url,
             )
         else:
             request_url = self.config()["teamsAppsUrl"]
             logger.info("Get list of all MS Teams Apps; calling -> %s", request_url)
 
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get list of MS Teams apps; status -> %s; error -> %s",
+                    "Failed to get list of M365 Teams apps; status -> %s; error -> %s",
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def getTeamsAppsOfUser(self, user_id: str, filter_expression: str = "") -> dict:
+    def get_teams_apps_of_user(
+        self, user_id: str, filter_expression: str = ""
+    ) -> dict | None:
         """Get a list of MS Teams apps of a user that match a given filter criterium
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             filter_expression (string, optional): filter string see https://learn.microsoft.com/en-us/graph/filter-query-parameter
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
@@ -1646,47 +1683,47 @@
             self.config()["usersUrl"]
             + "/"
             + user_id
             + "/teamwork/installedApps?"
             + encoded_query
         )
         logger.info(
-            "Get list of MS Teams Apps for user -> %s using query -> %s; calling -> %s",
+            "Get list of M365 Teams Apps for user -> %s using query -> %s; calling -> %s",
             user_id,
             query,
             request_url,
         )
 
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get list of MS Teams for user -> %s; status -> %s; error -> %s",
+                    "Failed to get list of M365 Teams for user -> %s; status -> %s; error -> %s",
                     user_id,
                     response.status_code,
                     response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def uploadTeamsApp(
+    def upload_teams_app(
         self, app_path: str, update_existing_app: bool = False, app_id: str = ""
-    ) -> dict:
+    ) -> dict | None:
         """Upload a new app package to the catalog of MS Teams apps.
             This is not possible with client secret credentials
             but requires a token of a user authenticated
             with username + password.
             See https://learn.microsoft.com/en-us/graph/api/teamsapp-publish
             (permissions table on that page)
 
@@ -1694,231 +1731,239 @@
             app_path (string): file path (with directory) to the app package to upload
         Returns:
             dictionary: Response of the MS GRAPH API REST call or None if the request fails
         """
 
         if update_existing_app and not app_id:
             logger.error(
-                "To update an existing app you need to provide the existing App ID!"
+                "To update an existing M365 app you need to provide the existing App ID!"
             )
-            return {}
+            return None
 
         if not os.path.exists(app_path):
-            logger.error("Teams App file -> {} does not exist!")
-            return {}
+            logger.error("M365 Teams App file -> {} does not exist!")
+            return None
 
         # Ensure that the app file is a zip file
         if not app_path.endswith(".zip"):
-            logger.error("Teams App file -> {} must be a zip file!")
-            return {}
+            logger.error("M365 Teams App file -> {} must be a zip file!")
+            return None
 
         request_url = self.config()["teamsAppsUrl"]
         if update_existing_app:
             request_url += "/" + app_id + "/appDefinitions"
         # Here we need the credentials of an authenticated user!
         # (not the application credentials (client_id, client_secret))
-        request_header = self.requestHeaderUser("application/zip")
+        request_header = self.request_header_user("application/zip")
 
         # upload_files = {'file': open(app_path, 'rb')}
 
         with open(app_path, "rb") as f:
             app_data = f.read()
 
         with zipfile.ZipFile(app_path) as z:
             # Ensure that the app file contains a manifest.json file
             if "manifest.json" not in z.namelist():
                 logger.error(
-                    "Teams App file -> {} does not contain a manifest.json file!"
+                    "M365 Teams App file -> {} does not contain a manifest.json file!"
                 )
-                return {}
+                return None
 
         logger.info(
             "Upload Teams App -> %s to the MS Teams catalog; calling -> %s",
             app_path,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url, headers=request_header, data=app_data, timeout=60
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
 
             # Check if Session has expired - then re-authenticate and try once more
             if response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 if update_existing_app:
                     logger.warning(
-                        "Failed to update existing MS teams app -> %s (may be because it is not a new version); status -> %s; error -> %s",
+                        "Failed to update existing M365 teams app -> %s (may be because it is not a new version); status -> %s; error -> %s",
                         app_path,
                         response.status_code,
                         response.text,
                     )
 
                 else:
                     logger.error(
-                        "Failed to upload new MS teams app -> %s; status -> %s; error -> %s",
+                        "Failed to upload new M365 teams app -> %s; status -> %s; error -> %s",
                         app_path,
                         response.status_code,
                         response.text,
                     )
-                return {}
+                return None
 
     # end method definition
 
-    def removeTeamsApp(self, app_id: str):
+    def remove_teams_app(self, app_id: str):
         """Remove MS Teams App for the app catalog
 
         Args:
             app_id (string): Microsoft 365 GUID of the MS Teams app
         """
 
         request_url = self.config()["teamsAppsUrl"] + "/" + app_id
         # Here we need the credentials of an authenticated user!
         # (not the application credentials (client_id, client_secret))
-        request_header = self.requestHeaderUser()
+        request_header = self.request_header_user()
 
         # Make the DELETE request to remove the app from the app catalog
         response = requests.delete(request_url, headers=request_header, timeout=60)
 
         # Check the status code of the response
         if response.status_code == 204:
             logger.info(
-                "The app with ID -> %s has been successfully removed from the app catalog.",
+                "The M365 app with ID -> %s has been successfully removed from the app catalog.",
                 app_id,
             )
         else:
             logger.error(
-                "An error occurred while removing the app from the app catalog. Status code -> %s. Error message -> %s",
+                "An error occurred while removing the M365 app from the M365 app catalog. Status code -> %s. Error message -> %s",
                 response.status_code,
                 response.text,
             )
 
     # end method definition
 
-    def assignTeamsAppToUser(self, user_id: str, app_name: str) -> dict:
-        """Assigns (adds) a MS teams app to a M365 user.
+    def assign_teams_app_to_user(self, user_id: str, app_name: str) -> dict | None:
+        """Assigns (adds) a M365 teams app to a M365 user.
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             app_name (string): exact name of the app
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
 
-        app = self.getTeamsApps(f"contains(displayName, '{app_name}')")
+        app = self.get_teams_apps(f"contains(displayName, '{app_name}')")
         if not app or not app["value"]:
-            logger.error("App -> %s not found!", app_name)
-            return {}
-        app_id = self.getResultValue(app, "id", 0)
+            logger.error("M365 App -> %s not found!", app_name)
+            return None
+        app_id = self.get_result_value(app, "id", 0)
 
         request_url = (
             self.config()["usersUrl"] + "/" + user_id + "/teamwork/installedApps"
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         post_body = {
             "teamsApp@odata.bind": self.config()["teamsAppsUrl"] + "/" + app_id
         }
 
         logger.info(
-            "Assign teams app -> %s (%s) to user -> %s; calling -> %s",
+            "Assign M365 teams app -> %s (%s) to M365 user -> %s; calling -> %s",
             app_name,
             app_id,
             user_id,
             request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url, json=post_body, headers=request_header, timeout=60
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to assign teams app -> {} ({}) to user -> {}; status -> {}; error -> {}".format(
-                        app_name, app_id, user_id, response.status_code, response.text
-                    )
+                    "Failed to assign M365 teams app -> %s (%s) to M365 user -> %s; status -> %s; error -> %s",
+                    app_name,
+                    app_id,
+                    user_id,
+                    response.status_code,
+                    response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def upgradeTeamsAppOfUser(self, user_id: str, app_name: str) -> dict:
+    def upgrade_teams_app_of_user(self, user_id: str, app_name: str) -> dict | None:
         """Upgrade a MS teams app for a user. The call will fail if the user does not
             already have the app assigned. So this needs to be checked before
             calling this method.
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             app_name (string): exact name of the app
         Returns:
             dictionary: response of the MS Graph API call or None if the call fails.
         """
 
-        app = self.getTeamsAppsOfUser(
+        app = self.get_teams_apps_of_user(
             user_id, "contains(teamsAppDefinition/displayName, '{}')".format(app_name)
         )
         if not app or not app["value"]:
-            logger.error("App -> {} not found!".format(app_name))
-            return {}
-        app_id = self.getResultValue(app, "id", 0)
+            logger.error("App -> %s not found!", app_name)
+            return None
+        app_id = self.get_result_value(app, "id", 0)
 
         request_url = (
             self.config()["usersUrl"]
             + "/"
             + user_id
             + "/teamwork/installedApps/"
             + app_id
             + "/upgrade"
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
-            "Upgrade teams app -> {} ({}) of user -> {}; calling -> {}".format(
-                app_name, app_id, user_id, request_url
-            )
+            "Upgrade M365 teams app -> %s (%s) of user -> %s; calling -> %s",
+            app_name,
+            app_id,
+            user_id,
+            request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(request_url, headers=request_header, timeout=60)
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to upgrade teams app -> {} ({}) of user -> {}; status -> {}; error -> {}".format(
-                        app_name, app_id, user_id, response.status_code, response.text
-                    )
+                    "Failed to upgrade M365 teams app -> %s (%s) of user -> %s; status -> %s; error -> %s",
+                    app_name,
+                    app_id,
+                    user_id,
+                    response.status_code,
+                    response.text,
                 )
-                return {}
+                return None
 
     # end method definition
 
-    def addSensitivityLabel(
+    def add_sensitivity_label(
         self,
         name: str,
         display_name: str,
         description: str = "",
         color: str = "red",
         enabled: bool = True,
         admin_description: str = "",
@@ -1953,40 +1998,40 @@
             "adminDescription": admin_description,
             "userDescription": user_description,
             "encryptContent": enable_encryption,
             "contentMarking": enable_marking,
         }
 
         request_url = self.config()["securityUrl"] + "/sensitivityLabels"
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
-            "Create sensitivity label -> {}; calling -> {}".format(name, request_url)
+            "Create M365 sensitivity label -> %s; calling -> %s", name, request_url
         )
 
         # Send the POST request to create the label
         response = requests.post(
             request_url, headers=request_header, data=json.dumps(payload), timeout=60
         )
 
         # Check the response status code
         if response.status_code == 201:
-            logger.info("Label -> {} has been created successfully!".format(name))
+            logger.info("Label -> %s has been created successfully!", name)
             return response
         else:
             logger.error(
-                "Failed to create the label -> {}! Response status code: {}".format(
-                    name, response.status_code
-                )
+                "Failed to create the M365 label -> %s! Response status code -> %s",
+                name,
+                response.status_code,
             )
             return None
 
     # end method definition
 
-    def assignSensitivityLabelToUser(self, user_email: str, label_name: str):
+    def assign_sensitivity_label_to_user(self, user_email: str, label_name: str):
         """Assigns a existing sensitivity label to a user.
             THIS IS CURRENTLY NOT WORKING!
 
         Args:
             user_email (string): email address of the user (as unique identifier)
             label_name (string): name of the label (need to exist)
 
@@ -1996,37 +2041,40 @@
 
         # Set up the request body with the label name
         body = {"labelName": label_name}
 
         request_url = (
             self.config()["usersUrl"] + "/" + user_email + "/assignSensitivityLabels"
         )
-        request_header = self.requestHeader()
+        request_header = self.request_header()
 
         logger.info(
-            "Assign label -> {} to user -> {}; calling -> {}".format(
-                label_name, user_email, request_url
-            )
+            "Assign label -> %s to user -> %s; calling -> %s",
+            label_name,
+            user_email,
+            request_url,
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url, headers=request_header, json=body, timeout=60
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
-                request_header = self.requestHeader()
+                request_header = self.request_header()
                 retries += 1
             else:
                 logger.error(
-                    "Failed to assign label -> {} to user -> {}; status -> {}; error -> {}".format(
-                        label_name, user_email, response.status_code, response.text
-                    )
+                    "Failed to assign label -> %s to M365 user -> %s; status -> %s; error -> %s",
+                    label_name,
+                    user_email,
+                    response.status_code,
+                    response.text,
                 )
                 return None
 
     # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/otac.py` & `pyxecm-0.3.0/pyxecm/otac.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 OTAC Module to implement functions to apply Archive Center settings
 
 Class: OTAC
 Methods:
 
 __init__ : class initializer
 config : returns config data set
-execCommand: exec a command on Archive Center
+hostname: returns the Archive Center hostname
+set_hostname: sets the Archive Center hostname
+exec_command: exec a command on Archive Center
+put_cert: put Certificate on Archive Center
+enable_cert: enables Certitificate on Archive Center
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
-import requests
-import os
 import logging
+import os
 import base64
+import requests
 
 from suds.client import Client
 
 logger = logging.getLogger("pyxecm.otac")
 
 requestHeaders = {"Content-Type": "application/x-www-form-urlencoded"}
 
@@ -39,89 +43,114 @@
         protocol: str,
         hostname: str,
         port: int,
         ds_username: str,
         ds_password: str,
         admin_username: str,
         admin_password: str,
+        **kwargs
     ):
         """Initialize the OTAC object
 
         Args:
             protocol (string): Either http or https.
             hostname (string): The hostname of the Archive Center  to communicate with.
             port (integer): The port number used to talk to the Archive Center .
             ds_username (string): The admin user name of Archive Center (dsadmin).
             ds_password (string): The admin password of Archive Center (dsadmin).
             admin_username (string): The admin user name of Archive Center (otadmin@otds.admin).
             admin_password (string): The admin password of Archive Center (otadmin@otds.admin).
+            **kwargs
         """
 
-        otacConfig = {}
+        otac_config = {}
 
         if hostname:
-            otacConfig["hostname"] = hostname
+            otac_config["hostname"] = hostname
         else:
-            otacConfig["hostname"] = ""
+            otac_config["hostname"] = ""
 
         if protocol:
-            otacConfig["protocol"] = protocol
+            otac_config["protocol"] = protocol
         else:
-            otacConfig["protocol"] = "http"
+            otac_config["protocol"] = "http"
 
         if port:
-            otacConfig["port"] = port
+            otac_config["port"] = port
         else:
-            otacConfig["port"] = 80
+            otac_config["port"] = 80
 
         if ds_username:
-            otacConfig["ds_username"] = ds_username
+            otac_config["ds_username"] = ds_username
         else:
-            otacConfig["ds_username"] = "dsadmin"
+            otac_config["ds_username"] = "dsadmin"
 
         if ds_password:
-            otacConfig["ds_password"] = ds_password
+            otac_config["ds_password"] = ds_password
         else:
-            otacConfig["ds_password"] = ""
+            otac_config["ds_password"] = ""
 
         if admin_username:
-            otacConfig["admin_username"] = admin_username
+            otac_config["admin_username"] = admin_username
         else:
-            otacConfig["admin_username"] = "admin"
+            otac_config["admin_username"] = "admin"
 
         if admin_password:
-            otacConfig["admin_password"] = admin_password
+            otac_config["admin_password"] = admin_password
         else:
-            otacConfig["admin_password"] = ""
+            otac_config["admin_password"] = ""
 
-        otacBaseUrl = protocol + "://" + otacConfig["hostname"]
+        otac_base_url = protocol + "://" + otac_config["hostname"]
         if str(port) not in ["80", "443"]:
-            otacBaseUrl += ":{}".format(port)
-        otacExecUrl = otacBaseUrl + "/archive/admin/exec"
-        otacConfig["execUrl"] = otacExecUrl
-        otacConfig["baseUrl"] = otacBaseUrl
+            otac_base_url += ":{}".format(port)
+        otac_exec_url = otac_base_url + "/archive/admin/exec"
+        otac_config["execUrl"] = otac_exec_url
+        otac_config["baseUrl"] = otac_base_url
 
-        self._config = otacConfig
+        self._config = otac_config
 
-    def config(self):
+    def config(self) -> dict:
+        """Returns the configuration dictionary
+
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
-    def hostname(self):
+    def hostname(self) -> str:
+        """Returns the Archive Center hostname
+
+        Returns:
+            str: Archive Center hostname
+        """
         return self.config()["hostname"]
 
-    def setHostname(self, hostname: str):
+    def set_hostname(self, hostname: str):
+        """Sets the Archive Center hostname
+
+        Args:
+            hostname (str): new Archive Center hostname
+        """
         self.config()["hostname"] = hostname
 
-    def setCredentials(
+    def set_credentials(
         self,
         ds_username: str = "",
         ds_password: str = "",
         admin_username: str = "",
         admin_password: str = "",
     ):
+        """Set the credentials for Archive Center for the "ds" and "admin" users.
+
+        Args:
+            ds_username (str, optional): non-default user name of the "ds" user. Defaults to "".
+            ds_password (str, optional): non-default password of the "ds" user. Defaults to "".
+            admin_username (str, optional): non-default user name of the "admin" user. Defaults to "".
+            admin_password (str, optional): non-default password of the "admin" user. Defaults to "".
+        """
         if ds_username:
             self.config()["ds_username"] = ds_username
         else:
             self.config()["ds_username"] = "dsadmin"
 
         if ds_password:
             self.config()["ds_password"] = ds_password
@@ -134,164 +163,176 @@
             self.config()["admin_username"] = "admin"
 
         if admin_password:
             self.config()["admin_password"] = admin_password
         else:
             self.config()["admin_password"] = ""
 
-    def baseUrl(self):
+    def base_url(self) -> str:
+        """Returns the Archive Center base URL
+
+        Returns:
+            str: Archive Center base URL
+        """
         return self.config()["baseUrl"]
 
-    def execUrl(self):
+    def exec_url(self) -> str:
+        """Returns the Archive Center URL to execute commandss
+
+        Returns:
+            str: Archive Center exec URL
+        """
         return self.config()["execUrl"]
 
-    def _soapLogin(self):
+    def _soap_login(self):
         """Authenticate via SOAP with admin User
 
         Args:
             None
         Returns:
             string: soap_token
         """
 
-        url = self.baseUrl() + "/archive/services/Authentication?wsdl"
+        url = self.base_url() + "/archive/services/Authentication?wsdl"
         client = Client(url)
         self._soap_token = client.service.Authenticate(
             username=self.config()["admin_username"],
             password=self.config()["admin_password"],
         )
 
         return self._soap_token
 
     # end method definition
 
-    def execCommand(self, command: str):
+    def exec_command(self, command: str):
         """Execute a command on Archive Center
 
         Args:
             command (string): command to execute
         Returns:
             _type_: _description_
         """
 
         payload = {
             "command": command,
             "user": self.config()["ds_username"],
             "passwd": self.config()["ds_password"],
         }
 
-        request_url = self.execUrl()
+        request_url = self.exec_url()
         logger.info(
-            "Execute command -> {} on Archive Center (user -> {}); calling -> {}".format(
-                command, payload["user"], request_url
-            )
+            "Execute command -> %s on Archive Center (user -> %s); calling -> %s",
+            command,
+            payload["user"],
+            request_url,
         )
         response = requests.post(request_url, data=payload, headers=requestHeaders)
         if not response.ok:
             logger.error(
-                "Failed to execute command -> {} on Archive Center; error -> {}".format(
-                    command, response.text.replace("\n", " ")
-                )
+                "Failed to execute command -> %s on Archive Center; error -> %s",
+                command,
+                response.text.replace("\n", " "),
             )
 
         return response
 
     # end method definition
 
-    def putCert(
+    def put_cert(
         self,
         auth_id: str,
         logical_archive: str,
         cert_path: str,
         permissions: str = "rcud",
     ):
         """Put Certificate on Archive Center
 
         Args:
             auth_id (string): ID of Certification
             logical_archive (string): Archive ID
-            certPath (string): local path to certificate (base64)
-            permissions (string, optional): Permissions. Defaults to "rcud" (read-create-update-delete).
+            cert_path (string): local path to certificate (base64)
+            permissions (string, optional): Permissions of the certificate.
+                                            Defaults to "rcud" (read-create-update-delete).
         Returns:
             response or None if the request fails
         """
 
         # Check if the photo file exists
         if not os.path.isfile(cert_path):
-            logger.error("Certificate file -> {} not found!".format(cert_path))
+            logger.error("Certificate file -> %s not found!", cert_path)
             return None
 
-        with open(cert_path, "r") as file:
-            cert_content = file.read().strip()
+        with open(cert_path, "r") as cert_file:
+            cert_content = cert_file.read().strip()
 
-        # Check that we have the pem certificate file - this is what OTAC expects. If the file content is
-        # base64 encoded we will decode it
+        # Check that we have the pem certificate file - this is what OTAC expects.
+        # If the file content is base64 encoded we will decode it
         if "BEGIN CERTIFICATE" in cert_content:
-            logger.info("Certificate file -> {} is not base64 encoded".format(cert_path))
+            logger.info("Certificate file -> %s is not base64 encoded", cert_path)
         elif "BEGIN CERTIFICATE" in base64.b64decode(
             cert_content, validate=True
         ).decode("utf-8"):
-            logger.info("Certificate file -> {} is base64 encoded".format(cert_path))
+            logger.info("Certificate file -> %s is base64 encoded", cert_path)
             cert_content = base64.b64decode(cert_content, validate=True).decode("utf-8")
         else:
-            logger.error(
-                "Cerfificate file -> {} is not in the right format".format(cert_path)
-            )
+            logger.error("Certificate file -> %s is not in the right format", cert_path)
             return None
 
         request_url = (
-            self.baseUrl()
+            self.base_url()
             + "/archive?putCert&pVersion=0046&authId="
             + auth_id
             + "&contRep="
             + logical_archive
             + "&permissions="
             + permissions
         )
         logger.info(
-            "Putting certificate -> {} on Archive -> {}; calling -> {}".format(
-                cert_path, logical_archive, request_url
-            )
+            "Putting certificate -> %s on Archive -> %s; calling -> %s",
+            cert_path,
+            logical_archive,
+            request_url,
         )
         response = requests.put(request_url, data=cert_content, headers=requestHeaders)
 
         if not response.ok:
             message = response.text.split(
                 '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN'
             )[0]
             logger.error(
-                "Failed to put certificate -> {} on Archive -> {}; error -> {}".format(
-                    cert_path, logical_archive, message
-                )
+                "Failed to put certificate -> %s on Archive -> %s; error -> %s",
+                cert_path,
+                logical_archive,
+                message,
             )
 
         return response
 
     # end method definition
 
-    def enableCert(self, auth_id: str, logical_archive: str, enable: bool = True):
-        """Enable Certitificate
+    def enable_cert(self, auth_id: str, logical_archive: str, enable: bool = True):
+        """Enables Certitificate on Archive Center
 
         Args:
             auth_id (string): Client ID
             logical_archive (string): Archive ID
             enable (boolean, optional): Enable or Disable certificate. Defaults to True.
         Returns:
             response or None if request fails.
         """
 
-        if self._soap_token == "":
-            self._soapLogin()
+        if not self._soap_token:
+            self._soap_login()
 
-        if enable == True:
+        if enable:
             enabled: int = 1
         else:
             enabled: int = 0
 
-        url = self.baseUrl() + "/ot-admin/services/ArchiveAdministration?wsdl"
+        url = self.base_url() + "/ot-admin/services/ArchiveAdministration?wsdl"
         client = Client(url)
 
         token_header = client.factory.create("ns0:OTAuthentication")
         token_header.AuthenticationToken = self._soap_token
         client.set_options(soapheaders=token_header)
 
         try:
@@ -301,17 +342,18 @@
                     {"key": "CERT_TYPE", "data": "@{}".format(logical_archive)},
                     {"key": "CERT_NAME", "data": auth_id},
                     {"key": "CERT_FLAGS", "data": enabled},
                 ],
             )
             return response
 
-        except Exception as e:
+        except Exception as exception:
             logger.error(
-                "Failed to execute SetCertificateFlags for Client -> {} on Archive -> {}; error -> {}".format(
-                    auth_id, logical_archive, e
-                )
+                "Failed to execute SetCertificateFlags for Client -> %s on Archive -> %s; error -> %s",
+                auth_id,
+                logical_archive,
+                exception,
             )
             return None
 
 
 # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/otcs.py` & `pyxecm-0.3.0/pyxecm/otcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,172 +5,173 @@
 Class: OTCS
 Methods:
 
 __init__ : class initializer
 config : returns config data set
 cookie : returns cookie information
 credentials: Get credentials (username and password)
-setCredentials: Set new credentials
+set_credentials: Set new credentials
 hostname: Get the configured OTCS hostname
-setHostname: Set the hostname of OTCS
-baseUrl : Get OTCS base URL
-csUrl: Get the Extended ECM (OTCS) URL
-restUrl : Get OTCS REST base URL
-
-requestFormHeader: Deliver the request header used for the CRUD REST API calls.
-requestJsonHeader: Deliver the request header for REST calls that require content type application/json.
-requestDownloadHeader: Deliver the request header used for download REST API calls. These calls accept application/octet-stream.
-
-parseRequestResponse: Converts the text property of a request response object to a Python dict in a safe way
-lookupResultValue: Lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call
-existResultItem: Check existence of key / value pair in the response properties of an Extended ECM REST API call.
-getResultValue: Read an item value from the REST API response. This is considering the most typical structures delivered by V2 REST API of Extended ECM
+set_hostname: Set the hostname of OTCS
+base_url : Get OTCS base URL
+cs_url: Get the Extended ECM (OTCS) URL
+rest_url : Get OTCS REST base URL
+
+request_form_header: Deliver the request header used for the CRUD REST API calls.
+request_json_header: Deliver the request header for REST calls that require content type application/json.
+request_download_header: Deliver the request header used for download REST API calls. These calls accept application/octet-stream.
+
+parse_request_response: Converts the text property of a request response object
+                        to a Python dict in a safe way
+lookup_result_value: Lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call
+exist_result_item: Check existence of key / value pair in the response properties of an Extended ECM REST API call.
+get_result_value: Read an item value from the REST API response. This is considering the most typical structures delivered by V2 REST API of Extended ECM
 
-isConfigured: returns true if the OTCS pod is ready to serve requests
+is_configured: returns true if the OTCS pod is ready to serve requests
 authenticate : Authenticates at Content Server and retrieve OTCS Ticket.
 
-applyConfig: Apply Content Server administration settings from XML file
+apply_config: Apply Content Server administration settings from XML file
 
-getUser: Lookup Content Server user
-addUser: Add Content Server user
-searchUser: Find a user based on search criteria
-updateUser: Update a defined field for a user
-updateUserProfile: Update a defined field for a user profile
-updateUserPhoto: Update a user with a profile photo (which must be an existing node)
-isProxy: Check if a user (login name) is a proxy of the current user
-getUserProxies: Get the list of proxy users for the current user
-updateUserProxy: Add a proxy to the current (authenticated) user
-addFavorite: Add a favorite for the current (authenticated) user
-
-getGroup: Lookup Content Server group
-addGroup: Add Content Server group
-getGroupMembers: Get Content Server group members
-addGroupMember: Add a user or group to a target group
-
-getNode: Get a node based on the node ID
-getNodeByParentAndName: Get a node based on the parent ID and name
-getNodeByWorkspaceAndPath: Get a node based on the workspace ID and path (list of folder names)
-getNodeByVolumeAndPath: Get a node based on the volume ID and path
-getNodeFromNickname: Get a node based on the nickname
-getSubnodes: get children nodes of a parent node
-renameNode: Change the name and description of a node
-getVolumes: Get all Volumes
-getVolume: Get Volume information based on the volume type ID
-checkNodeName: Check if a a node name in a parent location has a name collision
-uploadFileToVolume: Fetch a file from a URL or local filesystem and upload
+get_user: Lookup Content Server user
+add_user: Add Content Server user
+search_user: Find a user based on search criteria
+update_user: Update a defined field for a user
+update_user_profile: Update a defined field for a user profile
+update_user_photo: Update a user with a profile photo (which must be an existing node)
+is_proxy: Check if a user (login name) is a proxy of the current user
+get_user_proxies: Get the list of proxy users for the current user
+update_user_proxy: Add a proxy to the current (authenticated) user
+add_favorite: Add a favorite for the current (authenticated) user
+
+get_group: Lookup Content Server group
+add_group: Add Content Server group
+get_group_members: Get Content Server group members
+add_group_member: Add a user or group to a target group
+
+get_node: Get a node based on the node ID
+get_node_by_parent_and_name: Get a node based on the parent ID and name
+get_node_by_workspace_and_path: Get a node based on the workspace ID and path (list of folder names)
+get_node_by_volume_and_path: Get a node based on the volume ID and path
+get_node_from_nickname: Get a node based on the nickname
+get_subnodes: get children nodes of a parent node
+rename_node: Change the name and description of a node
+get_volumes: Get all Volumes
+get_volume: Get Volume information based on the volume type ID
+check_node_name: Check if a a node name in a parent location has a name collision
+upload_file_to_volume: Fetch a file from a URL or local filesystem and upload
                     it to a Extended ECM volume
-uploadFileToParent: Upload a document to a parent folder
-addDocumentVersion: Add a version to an Extended ECM document
-getLatestDocumentVersion: Get latest version of a document node based on the node ID.
-downloadDocument: Download a document
-downloadConfigFile: Download a config file from a given OTCS URL. This is NOT for downloading documents from within the OTCS repository
+upload_file_to_parent: Upload a document to a parent folder
+add_document_version: Add a version to an Extended ECM document
+get_latest_document_version: Get latest version of a document node based on the node ID.
+download_document: Download a document
+download_config_file: Download a config file from a given OTCS URL. This is NOT for downloading documents from within the OTCS repository
 
 search: search for a search term using Extended ECM search engine
 
-getExternalSystemConnection: Get Extended ECM external system connection
-addExternalSystemConnection: Add Extended ECM external system connection
+get_external_system_connection: Get Extended ECM external system connection
+add_external_system_connection: Add Extended ECM external system connection
 
-createTransportWorkbench: Create a Workbench in the Transport Volume
-unpackTransportPackage: Unpack an existing Transport Package into an existing Workbench
-deployWorkbench: Deploy an existing Workbench
-deployTransport: Main method to deploy a transport. This uses subfunctions to upload,
+create_transport_workbench: Create a Workbench in the Transport Volume
+unpack_transport_package: Unpack an existing Transport Package into an existing Workbench
+deploy_workbench: Deploy an existing Workbench
+deploy_transport: Main method to deploy a transport. This uses subfunctions to upload,
                  unpackage and deploy the transport, and creates the required workbench
-replaceTransportPlaceholders: Search and replace strings in the XML files of the transport packlage
+replace_transport_placeholders: Search and replace strings in the XML files of the transport packlage
 
-getWorkspaceTypes: Get all workspace types configured in Extended ECM
-getBusinessObjectType: Get information for a specific business object type
-getWorkspaceCreateForm: Get the Workspace create form
-getWorkspace: Get a workspace node
-getWorkspaceInstances: Get all instances of a given workspace type 
-getWorkspaceByTypeAndName: Lookup workspace based on workspace type name and workspace name 
-createWorkspace: Create a new business workspace
-createWorkspaceRelationship: Create a relationship between two workspaces
-getWorkspaceRelationships: get a list of related workspaces
-getWorkspaceRoles: Get the Workspace roles
-addMemberToWorkspace: Add member to workspace role. Check that the user is not yet a member
-removeMemberFromWorkspace: Remove member from workspace role
-assignWorkspacePermissions: Update workspace permissions for a given role
-updateWorkspaceIcon: Update a workspace with a with a new icon (which is uploaded)
-
-createItem: Create an item in Extended ECM (e.g. folder or URL item)
-updateItem: Update an item in Extended ECM (e.g. folder or URL item)
-getDocumentTemplates: Get all document templates for a given target location
-createDocumentFromTemplate: Create a document based on a document template
-
-getWebReportParameters: Get parameters of a Web Report
-runWebReport: Run a Web Report that is identified by its nick name
-
-installCSApplication: Install a CS Application (based on WebReports)
-
-assignItemToUserGroup: Assign an item (e.g. Workspace or document) to a list of users or groups
-
-convertPermissionStringToPermissionValue: Convert a list of permission names to a permission value
-convertPermissionValueToPermissionString: Convert a permission value to a list of permission strings
-assignPermission: Assign permissions to an item for a defined user or group
-
-getNodeCategories: Get categories assigned to a node
-getNodeCategory: Get a specific category assigned to a node
-getNodeCategoryIds: Get list of all category definition IDs that are assign to the node.
-getNodeCategoryDefinition: Get category definition (category id and attribute IDs and types)
-assignCategory: Assign a category to a node
-setCategoryValue: Set a value for a specific category attribute to a node
-
-assignClassification: Assign a classification to an item
-assignRMClassification: Assign a Records management classification to an item
-
-registerWorkspaceTemplate: Register a workspace template for Extended ECM for Engineering
-
-getRecordsManagementRSIs: Get the ist of RSIs together with their RSI schedules
-getRecordsManagementCodes: Get Records Management Codes
-updateRecordsManagementCodes: Update the Records Management Codes
-createRecordsManagementRSI: Create a new Records Management RSI item
-createRecordsManagementRSISchedule: Create a schedule for an existing RSI item
-createRecordsManagementHold: Create a Records Management Hold
-getRecordsManagementHolds: Get a list of all Records Management Holds in the system.
-importRecordsManagementCodes: Import RM codes from a config file
-importRecordsManagementRSIs: Import RM RSIs from a config file
-importRecordsManagementSettings: Import Records Management settings from a config file
-importPhysicalObjectsCodes: Import Physical Objects codes from a config file
-importPhysicalObjectsSettings: Import Physical Objects settings from a config file
-importPhysicalObjectsLocators: Import Physical Objects locators from a config file
-importSecurityClearanceCodes: Import Securioty Clearance codes from a config file
+get_workspace_types: Get all workspace types configured in Extended ECM
+get_business_object_type: Get information for a specific business object type
+get_workspace_create_form: Get the Workspace create form
+get_workspace: Get a workspace node
+get_workspace_instances: Get all instances of a given workspace type 
+get_workspace_by_type_and_name: Lookup workspace based on workspace type name and workspace name 
+create_workspace: Create a new business workspace
+create_workspace_relationship: Create a relationship between two workspaces
+get_workspace_relationships: get a list of related workspaces
+get_workspace_roles: Get the Workspace roles
+add_member_to_workspace: Add member to workspace role. Check that the user is not yet a member
+remove_member_from_workspace: Remove member from workspace role
+assign_workspace_permissions: Update workspace permissions for a given role
+update_workspace_icon: Update a workspace with a with a new icon (which is uploaded)
+
+create_item: Create an item in Extended ECM (e.g. folder or URL item)
+update_item: Update an item in Extended ECM (e.g. folder or URL item)
+get_document_templates: Get all document templates for a given target location
+create_document_from_template: Create a document based on a document template
+
+get_web_report_parameters: Get parameters of a Web Report
+run_web_report: Run a Web Report that is identified by its nick name
+
+install_cs_application: Install a CS Application (based on WebReports)
+
+assign_item_to_user_group: Assign an item (e.g. Workspace or document) to a list of users or groups
+
+convert_permission_string_to_permission_value: Convert a list of permission names to a permission value
+convert_permission_value_to_permission_string: Convert a permission value to a list of permission strings
+assign_permission: Assign permissions to an item for a defined user or group
+
+get_node_categories: Get categories assigned to a node
+get_node_category: Get a specific category assigned to a node
+get_node_category_ids: Get list of all category definition IDs that are assign to the node.
+get_node_category_definition: Get category definition (category id and attribute IDs and types)
+assign_category: Assign a category to a node
+set_category_value: Set a value for a specific category attribute to a node
+
+assign_classification: Assign a classification to an item
+assign_rm_classification: Assign a Records management classification to an item
+
+register_workspace_template: Register a workspace template for Extended ECM for Engineering
+
+get_records_management_rsis: Get the ist of RSIs together with their RSI schedules
+get_records_management_codes: Get Records Management Codes
+update_records_management_codes: Update the Records Management Codes
+create_records_management_rsi: Create a new Records Management RSI item
+create_records_management_rsi_schedule: Create a schedule for an existing RSI item
+create_records_management_hold: Create a Records Management Hold
+get_records_management_holds: Get a list of all Records Management Holds in the system.
+import_records_management_codes: Import RM codes from a config file
+import_records_management_rsis: Import RM RSIs from a config file
+import_records_management_settings: Import Records Management settings from a config file
+import_physical_objects_codes: Import Physical Objects codes from a config file
+import_physical_objects_settings: Import Physical Objects settings from a config file
+import_physical_objects_locators: Import Physical Objects locators from a config file
+import_security_clearance_codes: Import Securioty Clearance codes from a config file
 
-assignUserSecurityClearance: Assign a Security Clearance level to a user
-assignUserSupplementalMarkings: Assign a list of Supplemental Markings to a user
+assign_user_security_clearance: Assign a Security Clearance level to a user
+assign_user_supplemental_markings: Assign a list of Supplemental Markings to a user
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
-import requests
 import json
 import urllib.parse
 from datetime import datetime
 import zipfile
+import requests
 from pyxecm.helper.xml import XML
 
 logger = logging.getLogger("pyxecm.otcs")
 
-requestJsonHeaders = {
+REQUEST_JSON_HEADERS = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
-requestFormHeaders = {
+REQUEST_FORM_HEADERS = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/x-www-form-urlencoded",
 }
 
-requestDownloadHeaders = {
+REQUEST_DOWNLOAD_HEADERS = {
     "accept": "application/octet-stream",
     "Content-Type": "application/json",
 }
 
 
 class OTCS:
     """Used to automate stettings in OpenText Extended ECM."""
@@ -184,226 +185,268 @@
         hostname: str,
         port: int,
         username: str,
         password: str,
         user_partition: str = "Content Server Members",
         resource_name: str = "cs",
         default_license: str = "X3",
+        **kwargs,
     ):
         """Initialize the OTCS object
 
         Args:
             protocol (string): Either http or https.
             hostname (string): The hostname of Extended ECM server to communicate with.
             port (integer): The port number used to talk to the Extended ECM server.
             username (string): The admin user name of Extended ECM.
             password (string): The admin password of Extended ECM.
             user_partition (string): Name of the OTDS partition for OTCS users. Default is "Content Server Members".
             resource_name (string, optional): Name of the OTDS resource for OTCS. Dault is "cs".
             default_license (string, optional): name of the default user license. Default is "X3".
+            **kwargs
         """
 
-        # Initialize otcsConfig as an empty dictionary
-        otcsConfig = {}
+        # Initialize otcs_config as an empty dictionary
+        otcs_config = {}
 
         if hostname:
-            otcsConfig["hostname"] = hostname
+            otcs_config["hostname"] = hostname
         else:
-            otcsConfig["hostname"] = "otcs-admin-0"
+            otcs_config["hostname"] = "otcs-admin-0"
 
         if protocol:
-            otcsConfig["protocol"] = protocol
+            otcs_config["protocol"] = protocol
         else:
-            otcsConfig["protocol"] = "http"
+            otcs_config["protocol"] = "http"
 
         if port:
-            otcsConfig["port"] = port
+            otcs_config["port"] = port
         else:
-            otcsConfig["port"] = 8080
+            otcs_config["port"] = 8080
 
         if username:
-            otcsConfig["username"] = username
+            otcs_config["username"] = username
         else:
-            otcsConfig["username"] = "admin"
+            otcs_config["username"] = "admin"
 
         if password:
-            otcsConfig["password"] = password
+            otcs_config["password"] = password
         else:
-            otcsConfig["password"] = ""
+            otcs_config["password"] = ""
 
         if user_partition:
-            otcsConfig["partition"] = user_partition
+            otcs_config["partition"] = user_partition
         else:
-            otcsConfig["partition"] = ""
+            otcs_config["partition"] = ""
 
         if resource_name:
-            otcsConfig["resource"] = resource_name
+            otcs_config["resource"] = resource_name
         else:
-            otcsConfig["resource"] = ""
+            otcs_config["resource"] = ""
 
         if default_license:
-            otcsConfig["license"] = default_license
+            otcs_config["license"] = default_license
         else:
-            otcsConfig["license"] = ""
+            otcs_config["license"] = ""
 
-        otcsBaseUrl = protocol + "://" + otcsConfig["hostname"]
+        otcsBaseUrl = protocol + "://" + otcs_config["hostname"]
         if str(port) not in ["80", "443"]:
             otcsBaseUrl += ":{}".format(port)
-        otcsConfig["baseUrl"] = otcsBaseUrl
+        otcs_config["baseUrl"] = otcsBaseUrl
 
-        otcsConfig["configuredUrl"] = otcsBaseUrl + "/cssupport/csconfigured"
+        otcs_config["configuredUrl"] = otcsBaseUrl + "/cssupport/csconfigured"
 
         otcsUrl = otcsBaseUrl + "/cs/cs"
-        otcsConfig["csUrl"] = otcsUrl
+        otcs_config["csUrl"] = otcsUrl
 
         otcsRestUrl = otcsUrl + "/api"
-        otcsConfig["restUrl"] = otcsRestUrl
+        otcs_config["restUrl"] = otcsRestUrl
 
-        otcsConfig["authenticationUrl"] = otcsRestUrl + "/v1/auth"
-        otcsConfig["usersUrl"] = otcsRestUrl + "/v1/members"
-        otcsConfig["groupsUrl"] = otcsRestUrl + "/v1/members"
-        otcsConfig["membersUrl"] = otcsRestUrl + "/v2/members"
-        otcsConfig["nodesUrl"] = otcsRestUrl + "/v1/nodes"
-        otcsConfig["nodesUrlv2"] = otcsRestUrl + "/v2/nodes"
-        otcsConfig["doctemplatesUrl"] = otcsRestUrl + "/v2/doctemplates"
-        otcsConfig["nicknameUrl"] = otcsRestUrl + "/v2/nicknames"
-        otcsConfig["importSettingsUrl"] = otcsRestUrl + "/v2/import/settings/admin"
-        otcsConfig["searchUrl"] = otcsRestUrl + "/v2/search"
-        otcsConfig["volumeUrl"] = otcsRestUrl + "/v2/volumes"
-        otcsConfig["externalSystem"] = otcsRestUrl + "/v2/externalsystems"
-        otcsConfig["businessworkspacetypes"] = (
+        otcs_config["authenticationUrl"] = otcsRestUrl + "/v1/auth"
+        otcs_config["usersUrl"] = otcsRestUrl + "/v1/members"
+        otcs_config["groupsUrl"] = otcsRestUrl + "/v1/members"
+        otcs_config["membersUrl"] = otcsRestUrl + "/v2/members"
+        otcs_config["nodesUrl"] = otcsRestUrl + "/v1/nodes"
+        otcs_config["nodesUrlv2"] = otcsRestUrl + "/v2/nodes"
+        otcs_config["doctemplatesUrl"] = otcsRestUrl + "/v2/doctemplates"
+        otcs_config["nicknameUrl"] = otcsRestUrl + "/v2/nicknames"
+        otcs_config["importSettingsUrl"] = otcsRestUrl + "/v2/import/settings/admin"
+        otcs_config["searchUrl"] = otcsRestUrl + "/v2/search"
+        otcs_config["volumeUrl"] = otcsRestUrl + "/v2/volumes"
+        otcs_config["externalSystem"] = otcsRestUrl + "/v2/externalsystems"
+        otcs_config["businessworkspacetypes"] = (
             otcsRestUrl + "/v2/businessworkspacetypes"
         )
-        otcsConfig["businessworkspacecreateform"] = (
+        otcs_config["businessworkspacecreateform"] = (
             otcsRestUrl + "/v2/forms/businessworkspaces/create"
         )
-        otcsConfig["businessworkspaces"] = otcsRestUrl + "/v2/businessworkspaces"
-        otcsConfig["favoritesUrl"] = otcsRestUrl + "/v2/members/favorites"
-        otcsConfig["webReportsUrl"] = otcsRestUrl + "/v1/webreports"
-        otcsConfig["csApplicationsUrl"] = otcsRestUrl + "/v2/csapplications"
-        otcsConfig["xEngProjectTemplateUrl"] = (
+        otcs_config["businessworkspaces"] = otcsRestUrl + "/v2/businessworkspaces"
+        otcs_config["favoritesUrl"] = otcsRestUrl + "/v2/members/favorites"
+        otcs_config["webReportsUrl"] = otcsRestUrl + "/v1/webreports"
+        otcs_config["csApplicationsUrl"] = otcsRestUrl + "/v2/csapplications"
+        otcs_config["xEngProjectTemplateUrl"] = (
             otcsRestUrl + "/v2/xengcrt/projecttemplate"
         )
-        otcsConfig["rsisUrl"] = otcsRestUrl + "/v2/rsis"
-        otcsConfig["rsiSchedulesUrl"] = otcsRestUrl + "/v2/rsischedules"
-        otcsConfig["recordsManagementUrl"] = otcsRestUrl + "/v1/recordsmanagement"
-        otcsConfig["recordsManagementUrlv2"] = otcsRestUrl + "/v2/recordsmanagement"
-        otcsConfig["userSecurityUrl"] = otcsRestUrl + "/v2/members/usersecurity"
-        otcsConfig["physicalObjectsUrl"] = otcsRestUrl + "/v1/physicalobjects"
-        otcsConfig["securityClearancesUrl"] = otcsRestUrl + "/v1/securityclearances"
-        otcsConfig["holdsUrl"] = otcsRestUrl + "/v1/holds"
-        otcsConfig["holdsUrlv2"] = otcsRestUrl + "/v2/holds"
-        otcsConfig["validationUrl"] = otcsRestUrl + "/v1/validation/nodes/names"
+        otcs_config["rsisUrl"] = otcsRestUrl + "/v2/rsis"
+        otcs_config["rsiSchedulesUrl"] = otcsRestUrl + "/v2/rsischedules"
+        otcs_config["recordsManagementUrl"] = otcsRestUrl + "/v1/recordsmanagement"
+        otcs_config["recordsManagementUrlv2"] = otcsRestUrl + "/v2/recordsmanagement"
+        otcs_config["userSecurityUrl"] = otcsRestUrl + "/v2/members/usersecurity"
+        otcs_config["physicalObjectsUrl"] = otcsRestUrl + "/v1/physicalobjects"
+        otcs_config["securityClearancesUrl"] = otcsRestUrl + "/v1/securityclearances"
+        otcs_config["holdsUrl"] = otcsRestUrl + "/v1/holds"
+        otcs_config["holdsUrlv2"] = otcsRestUrl + "/v2/holds"
+        otcs_config["validationUrl"] = otcsRestUrl + "/v1/validation/nodes/names"
+
+        self._config = otcs_config
 
-        self._config = otcsConfig
+    def config(self) -> dict:
+        """Returns the configuration dictionary
 
-    def config(self):
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
-    def cookie(self):
+    def cookie(self) -> dict:
+        """Returns the login cookie of Extended ECM.
+           This is set by the authenticate() method
+
+        Returns:
+            dict: Estended ECM cookie
+        """
         return self._cookie
 
-    def credentials(self):
+    def credentials(self) -> dict:
+        """Get credentials (username + password)
+
+        Returns:
+            dict: dictionary with username and password
+        """
         return {
             "username": self.config()["username"],
             "password": self.config()["password"],
         }
 
-    def setCredentials(self, username: str = "", password: str = ""):
-        if username:
-            self.config()["username"] = username
-        else:
-            self.config()["username"] = "admin"
+    def set_credentials(self, username: str = "admin", password: str = ""):
+        """Set the credentials for Extended ECM for the based on user name and password.
 
-        if password:
-            self.config()["password"] = password
-        else:
-            self.config()["password"] = ""
+        Args:
+            username (str, optional): Username. Defaults to "admin".
+            password (str, optional): Password of the user. Defaults to "".
+        """
+        self.config()["username"] = username
+        self.config()["password"] = password
+
+    def hostname(self) -> str:
+        """Returns the hostname of Extended ECM (e.g. "otcs")
 
-    def hostname(self):
+        Returns:
+            string: hostname
+        """
         return self.config()["hostname"]
 
-    def setHostname(self, hostname: str):
+    def set_hostname(self, hostname: str):
+        """Sets the hostname of Extended ECM
+
+        Args:
+            hostname (str): new hostname
+        """
         self.config()["hostname"] = hostname
 
-    def baseUrl(self):
+    def base_url(self) -> str:
+        """Returns the base URL of Extended ECM
+
+        Returns:
+            string: base URL
+        """
         return self.config()["baseUrl"]
 
-    def csUrl(self):
+    def cs_url(self) -> str:
+        """Returns the Extended ECM URL
+
+        Returns:
+            string: Extended ECM URL
+        """
         return self.config()["csUrl"]
 
-    def restUrl(self):
+    def rest_url(self) -> str:
+        """Returns the REST URL of Extended ECM
+
+        Returns:
+            string: REST URL
+        """
         return self.config()["restUrl"]
 
-    def requestFormHeader(self) -> dict:
+    def request_form_header(self) -> dict:
         """Deliver the request header used for the CRUD REST API calls.
            Consists of Cookie + Form Headers (see global variable)
 
         Args:
             None.
         Return:
             dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
-        request_header.update(requestFormHeaders)
+        request_header.update(REQUEST_FORM_HEADERS)
 
         return request_header
 
     # end method definition
 
-    def requestJsonHeader(self) -> dict:
+    def request_json_header(self) -> dict:
         """Deliver the request header for REST calls that require content type application/json.
            Consists of Cookie + Json Headers (see global variable)
 
         Args:
             None.
         Return:
             dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
-        request_header.update(requestJsonHeaders)
+        request_header.update(REQUEST_JSON_HEADERS)
 
         return request_header
 
     # end method definition
 
-    def requestDownloadHeader(self) -> dict:
+    def request_download_header(self) -> dict:
         """Deliver the request header used for the CRUD REST API calls.
            Consists of Cookie + Form Headers (see global vasriable)
 
         Args:
             None.
         Return:
             dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
-        request_header.update(requestDownloadHeaders)
+        request_header.update(REQUEST_DOWNLOAD_HEADERS)
 
         return request_header
 
     # end method definition
 
-    def parseRequestResponse(
+    def parse_request_response(
         self,
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
-    ) -> dict:
+    ) -> dict | None:
         """Converts the text property of a request response object to a Python dict in a safe way
             that also handles exceptions.
 
             Content Server may produce corrupt response when it gets restarted
             or hitting resource limits. So we try to avoid a fatal error and bail
             out more gracefully.
 
@@ -434,18 +477,19 @@
                 logger.warning(message)
             return None
         else:
             return dict_object
 
     # end method definition
 
-    def lookupResultValue(
+    def lookup_result_value(
         self, response: dict, key: str, value: str, return_key: str
     ) -> str:
-        """Lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call.
+        """Lookup a property value based on a provided key / value pair in the
+           response properties of an Extended ECM REST API call.
 
         Args:
             response (dictionary): REST response from an OTCS REST Call
             key (string): property name (key)
             value (string): value to find in the item with the matching key
             return_key (string): determines which value to return based on the name of the dict key
         Returns:
@@ -454,15 +498,16 @@
 
         if not response:
             return None
         if not "results" in response:
             return None
 
         results = response["results"]
-        # check if results is a list or a dict (both is possible - dependent on the actual REST API):
+        # check if results is a list or a dict (both is possible -
+        # dependent on the actual REST API):
         if isinstance(results, dict):
             # result is a dict - we don't need index value:
             data = results["data"]
             if isinstance(data, dict):
                 # data is a dict - we don't need index value:
                 properties = data["properties"]
                 if (
@@ -482,15 +527,15 @@
                         and properties[key] == value
                         and return_key in properties
                     ):
                         return properties[return_key]
                 return None
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                    "Data needs to be a list or dict but it is -> %s", str(type(data))
                 )
                 return None
         elif isinstance(results, list):
             # result is a list - we need index value
             for result in results:
                 data = result["data"]
                 if isinstance(data, dict):
@@ -510,31 +555,28 @@
                             key in properties
                             and properties[key] == value
                             and return_key in properties
                         ):
                             return properties[return_key]
                 else:
                     logger.error(
-                        "Data needs to be a list or dict but it is -> {}".format(
-                            type(data)
-                        )
+                        "Data needs to be a list or dict but it is -> %s",
+                        str(type(data)),
                     )
                     return None
             return None
         else:
             logger.error(
-                "Result needs to be a list or dict but it is -> {}".format(
-                    type(results)
-                )
+                "Result needs to be a list or dict but it is -> %s", str(type(results))
             )
             return None
 
     # end method definition
 
-    def existResultItem(
+    def exist_result_item(
         self, response: dict, key: str, value: str, property_name: str = "properties"
     ) -> bool:
         """Check existence of key / value pair in the response properties of an Extended ECM REST API call.
 
         Args:
             response (dictionary): REST response from an OTCS REST Call
             key (string): property name (key)
@@ -567,29 +609,28 @@
                 elif isinstance(properties, list):
                     # properties is a list we iterate through the list and try to find the key:
                     for item in properties:
                         if key in item and item[key] == value:
                             return True
                 else:
                     logger.error(
-                        "Properties needs to be a list or dict but it is -> {}".format(
-                            type(properties)
-                        )
+                        "Properties needs to be a list or dict but it is -> %s",
+                        str(type(properties)),
                     )
                     return False
             elif isinstance(data, list):
                 # data is a list - this has typically just one item, so we use 0 as index
                 for item in data:
                     properties = item[property_name]
                     if key in properties and properties[key] == value:
                         return True
                 return False
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                    "Data needs to be a list or dict but it is -> %s", str(type(data))
                 )
                 return False
         elif isinstance(results, list):
             # result is a list - we need index value
             for result in results:
                 if not "data" in result:
                     continue
@@ -603,31 +644,28 @@
                     # data is a list we iterate through the list and try to find the key:
                     for item in data:
                         properties = item[property_name]
                         if key in properties and properties[key] == value:
                             return True
                 else:
                     logger.error(
-                        "Data needs to be a list or dict but it is -> {}".format(
-                            type(data)
-                        )
+                        "Data needs to be a list or dict but it is -> %s",
+                        str(type(data)),
                     )
                     return False
             return False
         else:
             logger.error(
-                "Result needs to be a list or dict but it is -> {}".format(
-                    type(results)
-                )
+                "Result needs to be a list or dict but it is -> %s", str(type(results))
             )
             return False
 
     # end method definition
 
-    def getResultValue(
+    def get_result_value(
         self,
         response: dict,
         key: str,
         index: int = 0,
         property_name: str = "properties",
     ) -> int:
         """Read an item value from the REST API response. This is considering
@@ -739,44 +777,44 @@
                     type(results)
                 )
             )
             return None
 
     # end method definition
 
-    def isConfigured(self) -> bool:
+    def is_configured(self) -> bool:
         """Checks if the Content Server pod is ready to receive requests.
 
         Args:
             None.
         Returns:
             boolean: True if pod is ready. False if pod is not yet ready.
         """
 
         request_url = self.config()["configuredUrl"]
 
         logger.info("Trying to retrieve OTCS url -> {}".format(request_url))
 
         try:
             checkcsConfiguredResponse = requests.get(
-                request_url, headers=requestJsonHeaders
+                request_url, headers=REQUEST_JSON_HEADERS
             )
         except Exception as e:
             logger.warning("Unable to connect to -> {} : {}".format(request_url, e))
             logger.warning("OTCS service may not be ready yet.")
             return False
 
         if checkcsConfiguredResponse.ok:
             return True
         else:
             return False
 
     # end method definition
 
-    def authenticate(self, revalidate: bool = False) -> dict:
+    def authenticate(self, revalidate: bool = False) -> dict | None:
         """Authenticates at Content Server and retrieve OTCS Ticket.
 
         Args:
             revalidate (boolean): determinse if a re-athentication is enforced
                                   (e.g. if session has timed out with 401 error)
         Returns:
             dictionary: Cookie information of None in case of an error.
@@ -796,27 +834,27 @@
         )
 
         response = None
         try:
             response = requests.post(
                 self.config()["authenticationUrl"],
                 data=self.credentials(),
-                headers=requestFormHeaders,
+                headers=REQUEST_FORM_HEADERS,
             )
         except Exception as e:
             logger.warning(
                 "Unable to connect to -> {} : {}".format(
                     self.config()["authenticationUrl"], e
                 )
             )
             logger.warning("OTCS service may not be ready yet.")
             return None
 
         if response.ok:
-            authenticate_dict = self.parseRequestResponse(
+            authenticate_dict = self.parse_request_response(
                 response, "This can be normal during restart", False
             )
             if not authenticate_dict:
                 return None
             else:
                 otcs_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otcs_ticket))
@@ -829,15 +867,15 @@
         # Store authentication ticket:
         self._cookie = {"otcsticket": otcs_ticket, "LLCookie": otcs_ticket}
         self.otcsticket = otcs_ticket
         return self._cookie
 
     # end method definition
 
-    def applyConfig(self, xmlfilepath: str) -> dict:
+    def apply_config(self, xmlfilepath: str) -> dict:
         """Apply Content Server administration settings from XML file
 
         Args:
             xmlfilepath (string): name + path of the XML settings file
         Returns:
             dictionary: Import response or None if the import fails.
                         response["results"]["data"]["restart"] indicates if the settings
@@ -868,15 +906,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 logger.debug(
                     "Admin settings in file -> {} have been applied".format(xmlfilepath)
                 )
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -884,15 +922,15 @@
                         xmlfilepath, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getUser(self, name: str, show_error: bool = False) -> dict:
+    def get_user(self, name: str, show_error: bool = False) -> dict:
         """Lookup Content Server user based on the name.
 
         Args:
             name (string): name of the user
             show_error (boolean): treat as error if user is not found
         Returns:
             dictionary: User information or None if the user is not found.
@@ -910,25 +948,25 @@
             ]
             To access the (login) name of the first user found use ["data"][0]["name"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         # type = 0 ==> User
         request_url = self.config()["usersUrl"] + "?where_type=0&query={}".format(name)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info("Get user with name -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -939,15 +977,15 @@
                     )
                 else:
                     logger.info("User -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def addUser(
+    def add_user(
         self,
         name: str,
         password: str,
         first_name: str,
         last_name: str,
         email: str,
         base_group: int,
@@ -984,28 +1022,28 @@
             "privilege_modify_groups": ("Modify Groups" in privileges),
             "privilege_user_admin_rights": ("User Admin Rights" in privileges),
             "privilege_grant_discovery": ("Grant Discovery" in privileges),
             "privilege_system_admin_rights": ("System Admin Rights" in privileges),
         }
 
         request_url = self.config()["usersUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info("Adding user -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=userPostBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1013,15 +1051,15 @@
                         name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def searchUser(self, value: str, field: str = "where_name") -> dict:
+    def search_user(self, value: str, field: str = "where_name") -> dict:
         """Find a user based on search criteria.
 
         Args:
             value (string): field value
             field (string): user field to search with (where_name, where_first_name, where_last_name)
         Returns:
             dictionary: User information or None if the user couldn't be found (e.g. because it doesn't exist).
@@ -1063,29 +1101,29 @@
                         }
                     }
                 ]
             }
         """
 
         request_url = self.config()["membersUrl"] + "?" + field + "=" + value
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Searching user by field -> {}, value -> {}; calling -> {}".format(
                 field, value, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1093,29 +1131,29 @@
                         field, value, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUser(self, user_id: int, field: str, value: str) -> dict:
+    def update_user(self, user_id: int, field: str, value: str) -> dict:
         """Update a defined field for a user.
 
         Args:
             user_id (integer): ID of the user
             value (string): field value
             field (string): user field
         Returns:
             dictionary: User information or None if the user couldn't be updated (e.g. because it doesn't exist).
         """
 
         userPutBody = {field: value}
 
         request_url = self.config()["membersUrl"] + "/" + str(user_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Updating user with ID -> {}, field -> {}, value -> {}; calling -> {}".format(
                 user_id, field, value, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userPutBody))
@@ -1125,15 +1163,15 @@
             response = requests.put(
                 request_url,
                 data=userPutBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1141,30 +1179,30 @@
                         user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUserProfile(self, field: str, value) -> dict:
+    def update_user_profile(self, field: str, value) -> dict:
         """Update a defined field for a user profile.
            IMPORTANT: this method needs to be called by the authenticated user
 
         Args:
             value (string): field value
             field (string): user field
         Returns:
             dictionary: User information or None if the user couldn't be updated
                         (e.g. because it doesn't exist).
         """
 
         userProfilePutBody = {"SmartUI": {field: value}}
 
         request_url = self.config()["membersUrl"] + "/preferences"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Updating profile for current user, field -> {}, value -> {}; calling -> {}".format(
                 field, value, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userProfilePutBody))
@@ -1175,15 +1213,15 @@
             response = requests.put(
                 request_url,
                 data={"body": json.dumps(userProfilePutBody)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1191,28 +1229,28 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUserPhoto(self, user_id: int, photo_id: int):
+    def update_user_photo(self, user_id: int, photo_id: int) -> dict | None:
         """Update a user with a profile photo (which must be an existing node).
 
         Args:
             user_id (integer): ID of the user
             photo_id (integer): Node ID of the photo
         Returns:
             dictionary: Node information or None if photo node is not found.
         """
 
         updateUserPutBody = {"photo_id": photo_id}
 
         request_url = self.config()["usersUrl"] + "/" + str(user_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Update user ID -> {} with photo ID -> {}; calling -> {}".format(
                 user_id, photo_id, request_url
             )
         )
 
@@ -1221,15 +1259,15 @@
             response = requests.put(
                 request_url,
                 data=updateUserPutBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1237,61 +1275,61 @@
                         user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def isProxy(self, user_name: str) -> bool:
+    def is_proxy(self, user_name: str) -> bool:
         """Check if a user is defined as proxy of the current user
 
         Args:
             user_name (string): user  to test (login name)
         Returns:
             boolean: True is user is proxy of current user. False if not.
         """
 
-        response = self.getUserProxies()
+        response = self.get_user_proxies()
         if not response or not "proxies" in response:
             return False
         proxies = response["proxies"]
 
         for proxy in proxies:
             if proxy["name"] == user_name:
                 return True
         return False
 
     # end method definition
 
-    def getUserProxies(self) -> dict:
+    def get_user_proxies(self) -> dict | None:
         """Get list of user proxies.
            This method needs to be called as the user the proxy is acting for.
         Args:
             None
         Returns:
             dictionary: Node information or None if REST call fails.
         """
 
         request_url = self.config()["usersUrl"] + "/proxies"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get proxy users for current user; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
             response = requests.get(
                 request_url,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1299,17 +1337,17 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUserProxy(
+    def update_user_proxy(
         self, proxy_user_id: int, from_date: str = None, to_date: str = None
-    ) -> dict:
+    ) -> dict | None:
         """Update a user with a proxy user (which must be an existing user).
            IMPORTANT: This method needs to be called as the user the proxy is acting for.
            Optional this method can be provided with a time span the proxy should be active.
 
            Example payload for proxy user 19340 without time span:
            add_proxy:  {"19340":{}}
 
@@ -1328,15 +1366,15 @@
         if from_date and to_date:
             post_dict["from_date"] = from_date
             post_dict["to_date"] = to_date
 
         proxyPostBody = {str(proxy_user_id): post_dict}
 
         request_url = self.config()["usersUrl"] + "/proxies"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign proxy user with ID -> {} to current user; calling -> {}".format(
                 proxy_user_id, request_url
             )
         )
 
@@ -1346,15 +1384,15 @@
             response = requests.post(
                 request_url,
                 data={"add_proxy": json.dumps(proxyPostBody)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1362,39 +1400,39 @@
                         proxy_user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addFavorite(self, node_id: int) -> dict:
+    def add_favorite(self, node_id: int) -> dict | None:
         """Add a favorite for the current (authenticated) user.
 
         Args:
-            nodeid (integer): ID of the node.
+            node_id (integer): ID of the node.
         Returns:
             dictionary: Request response or None if the favorite creation has failed.
         """
 
         request_url = self.config()["favoritesUrl"] + "/" + str(node_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Adding favorite for node ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1404,20 +1442,20 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroup(self, name: str, show_error: bool = False) -> dict:
+    def get_group(self, name: str, show_error: bool = False) -> dict | None:
         """Lookup Content Server group.
 
         Args:
             name (string): name of the group
-            showError (boolean): if True, treat as error if group is not found
+            show_error (boolean): if True, treat as error if group is not found
         Returns:
             dictionary: Group information or None if the group is not found.
             The returned information has a structure like this:
             "data": [
                 {
                     "id": 0,
                     "name": "string",
@@ -1426,27 +1464,27 @@
             ]
             To access the id of the first group found use ["data"][0]["id"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         # type = 1 ==> Group
         request_url = self.config()["groupsUrl"] + "?where_type=1&query={}".format(name)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get group with name -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -1457,41 +1495,41 @@
                     )
                 else:
                     logger.info("Group -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def addGroup(self, name: str) -> dict:
+    def add_group(self, name: str) -> dict | None:
         """Add Content Server group.
 
         Args:
             name (string): name of the group
         Returns:
             dictionary: Group information or None if the group couldn't be created (e.g. because it exisits already).
         """
 
         groupPostBody = {"type": 1, "name": name}
 
         request_url = self.config()["groupsUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info("Adding group -> {}; calling -> {}".format(name, request_url))
         logger.debug("Group Attributes -> {}".format(groupPostBody))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=groupPostBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1499,15 +1537,17 @@
                         name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroupMembers(self, group: int, member_type: int, limit: int = 100) -> dict:
+    def get_group_members(
+        self, group: int, member_type: int, limit: int = 100
+    ) -> dict | None:
         """Get Content Server group members.
 
         Args:
             group (integer): ID of the group.
             member_type (integer): users = 0, groups = 1
             limit (integer, optional): max number of results (internal default is 25)
         Returns:
@@ -1521,27 +1561,27 @@
             + "/"
             + str(group)
             + "/members?where_type="
             + str(member_type)
             + "&limit="
             + str(limit)
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Getting members of group -> {}; calling -> {}".format(group, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1551,28 +1591,28 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def addGroupMember(self, member: int, group: int) -> dict:
+    def add_group_member(self, member: int, group: int) -> dict | None:
         """Add a user or group to a target group.
 
         Args:
             member (integer): ID of the user or group to add.
             group (integer): ID of the target group.
         Returns:
             dictionary: Response or None if adding a the member fails.
         """
 
         groupMemberPostBody = {"member_id": member}
 
         request_url = self.config()["membersUrl"] + "/" + str(group) + "/members"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Adding member -> {} to group -> {}; calling -> {}".format(
                 member, group, request_url
             )
         )
 
@@ -1581,15 +1621,15 @@
             response = requests.post(
                 request_url,
                 data=groupMemberPostBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1600,15 +1640,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNode(self, node_id: int) -> dict:
+    def get_node(self, node_id: int) -> dict | None:
         """Get a node based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the node
         Returns:
             dictionary: Node information or None if no node with this ID is found.
             "results": [
@@ -1671,27 +1711,27 @@
                         }
                     ]
                 }
             ]
         """
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get node with ID -> {}; calling -> {}".format(node_id, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1699,21 +1739,21 @@
                         node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNodeByParentAndName(
+    def get_node_by_parent_and_name(
         self,
         parent_id: int,
         name: str,
         fields: str = "properties",
         show_error: bool = False,
-    ) -> dict:
+    ) -> dict | None:
         """Get a node based on the parent ID and name. This method does basically
            a query with "where_name" and the "result" is a list.
 
         Args:
             parent_id (integer) is the node Id of the parent node
             name (string) is the name of the node to get
             fields (string): which fields to retrieve. This can have a big impact on performance!
@@ -1731,29 +1771,29 @@
 
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_id)
             + "/nodes?{}".format(encoded_query)
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get node with name -> {} and parent ID -> {}; calling -> {}".format(
                 name, parent_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -1771,17 +1811,17 @@
                             name, parent_id
                         )
                     )
                 return None
 
     # end method definition
 
-    def getNodeByWorkspaceAndPath(
+    def get_node_by_workspace_and_path(
         self, workspace_id: int, path: list, show_error: bool = False
-    ) -> dict:
+    ) -> dict | None:
         """Get a node based on the workspace ID (= node ID) and path (list of folder names).
 
         Args:
             workspace_id (integer): node ID of the workspace
             path (list): list of container items (top down), last item is name of to be retrieved item.
                          If path is empty the node of the volume is returned.
             show_error (boolean, optional): treat as error if node is not found
@@ -1789,19 +1829,19 @@
             dictionary: Node information or None if no node with this path is found.
         """
 
         current_item_id = workspace_id
 
         # in case the path is an empty list
         # we will have the node of the workspace:
-        node = self.getNode(current_item_id)
+        node = self.get_node(current_item_id)
 
         for path_element in path:
-            node = self.getNodeByParentAndName(current_item_id, path_element)
-            current_item_id = self.getResultValue(node, "id")
+            node = self.get_node_by_parent_and_name(current_item_id, path_element)
+            current_item_id = self.get_result_value(node, "id")
             if not current_item_id:
                 if show_error:
                     logger.error("Cannot find path element -> {}!".format(path_element))
                 else:
                     logger.info("Cannot find path element -> {}.".format(path_element))
                 return None
             logger.debug(
@@ -1810,15 +1850,15 @@
                 )
             )
 
         return node
 
     # end method definition
 
-    def getNodeByVolumeAndPath(self, volume_type: int, path: list = []) -> dict:
+    def get_node_by_volume_and_path(self, volume_type: int, path: list = []) -> dict | None:
         """Get a node based on the volume and path (list of container items).
 
         Args:
             volume_type (integer): Volume type ID (default is 141 = Enterprise Workspace)
                 "Records Management"                = 550
                 "Content Server Document Templates" = 20541
                 "O365 Office Online Volume"         = 1296
@@ -1840,68 +1880,68 @@
             path (list): list of container items (top down), last item is name of to be retrieved item.
                          If path is empty the node of the volume is returned.
         Returns:
             dictionary: Node information or None if no node with this path is found.
         """
 
         # Preparation: get volume IDs for Transport Warehouse (root volume and Transport Packages)
-        response = self.getVolume(volume_type)
+        response = self.get_volume(volume_type)
         if not response:
             logger.error("Volume Type -> {} not found!".format(volume_type))
             return None
 
-        volume_id = self.getResultValue(response, "id")
+        volume_id = self.get_result_value(response, "id")
         logger.info("Volume ID -> {}".format(volume_id))
 
         current_item_id = volume_id
 
         # in case the path is an empty list
         # we will have the node of the volume:
-        node = self.getNode(current_item_id)
+        node = self.get_node(current_item_id)
 
         for path_element in path:
-            node = self.getNodeByParentAndName(current_item_id, path_element)
-            current_item_id = self.getResultValue(node, "id")
+            node = self.get_node_by_parent_and_name(current_item_id, path_element)
+            current_item_id = self.get_result_value(node, "id")
             if not current_item_id:
                 logger.error(
                     "Cannot find path element -> {} in container with ID -> {}.".format(
                         path_element, current_item_id
                     )
                 )
                 return None
             logger.debug("Traversing path element -> {}".format(current_item_id))
 
         return node
 
     # end method definition
 
-    def getNodeFromNickname(self, nickname: str, show_error: bool = False) -> dict:
+    def get_node_from_nickname(self, nickname: str, show_error: bool = False) -> dict | None:
         """Get a node based on the nickname.
 
         Args:
             nickname (string): Nickname of the node.
             show_error (boolean): treat as error if node is not found
         Returns:
             dictionary: Node information or None if no node with this nickname is found.
         """
 
         request_url = self.config()["nicknameUrl"] + "/" + nickname + "/nodes"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get node with nickname -> {}; calling -> {}".format(nickname, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -1912,24 +1952,24 @@
                     )
                 else:
                     logger.info("Node with nickname -> {} not found.".format(nickname))
                 return None
 
     # end method definition
 
-    def getSubnodes(
+    def get_subnodes(
         self,
         parent_node_id: int,
         filter_node_types: int = -2,
         filter_name: str = "",
         show_hidden: bool = False,
         limit: int = 100,
         page: int = 1,
         fields: str = "properties",  # per default we just get the most important information
-    ) -> dict:
+    ) -> dict | None:
         """Get a subnodes of a parent node ID.
 
         Args:
             parent_node_id (integer) is the node Id of the node
             filter_node_types (integer, optional):
                 -1 get all containers
                 -2 get all searchable objects (default)
@@ -1962,29 +2002,29 @@
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_node_id)
             + "/nodes"
             + "?{}".format(encodedQuery)
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get subnodes of parent node with ID -> {}; calling -> {}".format(
                 parent_node_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1994,26 +2034,26 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def renameNode(
+    def rename_node(
         self,
         node_id: int,
         name: str,
         description: str,
         name_multilingual: dict = {},
         description_multilingual: dict = {},
-    ) -> dict:
+    ) -> dict | None:
         """Change the name and description of a node.
 
         Args:
-            node_id (integer): ID of the node. You can use the getVolume() function below to
+            node_id (integer): ID of the node. You can use the get_volume() function below to
                                to the node id for a volume.
             name (string): New name of the node.
             description (string): New description of the node.
             name_multilingual (dictionary, optional): multi-lingual node names
             description_multilingual (dictionary, optional): multi-lingual description
         Returns:
             dictionary: Request response or None if the renaming fails.
@@ -2023,15 +2063,15 @@
 
         if name_multilingual:
             renameNodePutBody["name_multilingual"] = name_multilingual
         if description_multilingual:
             renameNodePutBody["description_multilingual"] = description_multilingual
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Renaming node -> {} to -> {}; calling -> {}".format(
                 node_id, name, request_url
             )
         )
 
@@ -2040,15 +2080,15 @@
             response = requests.put(
                 request_url,
                 data={"body": json.dumps(renameNodePutBody)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2059,15 +2099,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getVolumes(self) -> dict:
+    def get_volumes(self) -> dict | None:
         """Get all Volumes.
 
         Args:
             None
         Returns:
             dictionary: Volume Details or None if an error occured.
             {
@@ -2110,25 +2150,25 @@
                 ]
             }
             Example:
             ["results"][0]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
         request_url = self.config()["volumeUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info("Get volumes; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2136,38 +2176,38 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getVolume(self, volume_type: int) -> dict:
+    def get_volume(self, volume_type: int) -> dict | None:
         """Get Volume information based on the volume type ID.
 
         Args:
             volume_type (integer): ID of the volume type
         Returns:
             dictionary: Volume Details or None if volume is not found.
             ["results"]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
         request_url = self.config()["volumeUrl"] + "/" + str(volume_type)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get volume type -> {}; calling -> {}".format(volume_type, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2177,25 +2217,25 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def checkNodeName(self, parent_id: int, node_name: str) -> dict:
+    def check_node_name(self, parent_id: int, node_name: str) -> dict | None:
         """Get Volume information based on the volume type ID.
 
         Args:
             parent_id (integer): ID of the parent location
             node_name (string): name of the new node
         Returns:
         """
 
         request_url = self.config()["validationUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Check if node with name -> {} can be created in parent with ID -> {}; calling -> {}".format(
                 node_name, parent_id, request_url
             )
         )
 
@@ -2206,15 +2246,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data={"body": json.dumps(checkNodeNamePostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2225,17 +2265,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def uploadFileToVolume(
+    def upload_file_to_volume(
         self, package_url: str, file_name: str, mime_type: str, volume_type: int
-    ) -> dict:
+    ) -> dict | None:
         """Fetch a file from a URL or local filesystem and upload it to a Content Server volume.
 
         Args:
             package_url (string): URL to download file
             file_name (string): name of the file
             mime_type (string): mimeType of the file
             volume_type (integer): type (ID) of the volume
@@ -2299,15 +2339,15 @@
                 request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2318,17 +2358,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def uploadFileToParent(
+    def upload_file_to_parent(
         self, file_url: str, file_name: str, mime_type: str, parent_id: int
-    ) -> dict:
+    ) -> dict | None:
         """Fetch a file from a URL or local filesystem and upload it to a Content Server parent (folder).
 
         Args:
             file_url (string): URL to download file or local file
             file_name (string): name of the file
             mime_type (string): mimeType of the file
             parent_id (integer): parent (ID) of the file to upload
@@ -2396,15 +2436,15 @@
                 request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2415,22 +2455,22 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def addDocumentVersion(
+    def add_document_version(
         self,
         node_id: int,
         file_url: str,
         file_name: str,
         mime_type: str = "text/plain",
         description: str = "",
-    ) -> dict:
+    ) -> dict | None:
         """Fetch a file from a URL or local filesystem and upload it as a new document version.
 
         Args:
             node_id (integer): ID of the document to add add version to
             file_url (string): URL to download file or local file
             file_name (string): name of the file
             mime_type (string, optional): mimeType of the file (default = text/plain)
@@ -2495,15 +2535,15 @@
                 request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2514,41 +2554,41 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getLatestDocumentVersion(self, node_id: int) -> dict:
+    def get_latest_document_version(self, node_id: int) -> dict | None:
         """Get latest version of a document node based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the node
         Returns:
             dictionary: Node information or None if no node with this ID is found.
         """
 
         request_url = (
             self.config()["nodesUrl"] + "/" + str(node_id) + "/versions/latest"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get latest version of document with node ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2556,15 +2596,15 @@
                         node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def downloadDocument(
+    def download_document(
         self, node_id: int, file_path: str, version_number: str = ""
     ) -> bool:
         """Download a document from Extended ECM to local file system.
 
         Args:
             node_id (integer): node ID of the document to download
             file_path (string): local file path (directory)
@@ -2578,15 +2618,15 @@
 
         directory = os.path.dirname(file_path)
         if not os.path.exists(directory):
             logger.error("Directory -> {} does not exist".format(directory))
             return False
 
         if not version_number:
-            response = self.getLatestDocumentVersion(node_id)
+            response = self.get_latest_document_version(node_id)
             if not response:
                 logger.error(
                     "Cannot get latest version of document with ID -> {}".format(
                         node_id
                     )
                 )
             version_number = response["data"]["version_number"]
@@ -2595,15 +2635,15 @@
             self.config()["nodesUrlv2"]
             + "/"
             + str(node_id)
             + "/versions/"
             + str(version_number)
             + "/content"
         )
-        request_header = self.requestDownloadHeader()
+        request_header = self.request_download_header()
 
         logger.info(
             "Download document with node ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
         )
 
@@ -2635,15 +2675,15 @@
             # Write the content to the file
             file.write(content)
 
         return True
 
         # end method definition
 
-    def downloadConfigFile(self, otcs_url_suffix: str, file_path: str) -> bool:
+    def download_config_file(self, otcs_url_suffix: str, file_path: str) -> bool:
         """Download a config file from a given OTCS URL. This is NOT
             for downloading documents from within the OTCS repository
             but for configuration files such as app packages for MS Teams.
 
         Args:
             otcs_url_suffix (string): OTCS URL suffix starting typically starting
                                       with /cs/cs?func=,
@@ -2651,15 +2691,15 @@
             file_path (string): local path to save the file (direcotry + filename)
         Returns:
             boolean: True if the download succeeds, False otherwise
         """
 
         request_url = self.config()["baseUrl"] + otcs_url_suffix
         # request_header = self.cookie()
-        request_header = self.requestDownloadHeader()
+        request_header = self.request_download_header()
 
         logger.info("Download config file from URL -> {}".format(request_url))
 
         try:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
@@ -2700,15 +2740,15 @@
         look_for: str = "complexQuery",
         modifier: str = "",
         slice_id: int = 0,
         query_id: int = 0,
         template_id: int = 0,
         limit: int = 100,
         page: int = 1,
-    ) -> dict:
+    ) -> dict | None:
         """Search for a search term.
 
         Args:
             search_term (string), e.g. "test or OTSubType: 189"
             look_for (string, optional): 'allwords', 'anywords', 'exactphrase', and 'complexquery'.
                                          If not specified, it defaults to 'complexQuery'.
             modifier (string, optional): 'synonymsof', 'relatedto', 'soundslike', 'wordbeginswith',
@@ -2737,30 +2777,30 @@
             searchPostBody["slice_id"] = slice_id
         if query_id > 0:
             searchPostBody["query_id"] = query_id
         if template_id > 0:
             searchPostBody["template_id"] = template_id
 
         request_url = self.config()["searchUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Serarch for term -> {}; calling -> {}".format(search_term, request_url)
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=searchPostBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2770,17 +2810,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getExternalSystemConnection(
+    def get_external_system_connection(
         self, connection_name: str, show_error: bool = False
-    ) -> dict:
+    ) -> dict | None:
         """Get Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
 
         Args:
             connection_name (string): Name of the connection
             show_error (boolean): treat as error if node is not found
         Returns:
             dictionary: External system Details or None if the REST call fails.
@@ -2799,15 +2839,15 @@
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -2822,26 +2862,26 @@
                     logger.info(
                         "External system -> {} not found.".format(connection_name)
                     )
                 return None
 
     # end method definition
 
-    def addExternalSystemConnection(
+    def add_external_system_connection(
         self,
         connection_name: str,
         connection_type: str,
         as_url: str,
         base_url: str,
         username: str,
         password: str,
         authentication_method: str = "BASIC",  # either BASIC or OAUTH
         client_id: str = None,
         client_secret: str = None,
-    ) -> dict:
+    ) -> dict | None:
         """Add Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
 
         Args:
             connection_name (string): Name of the connection
             connection_type (string): Type of the connection (HTTP, SF, SFInstance)
             as_url (string)
             base_url (string)
@@ -2882,15 +2922,15 @@
             response = requests.post(
                 request_url,
                 data=externalSystemPostBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2900,27 +2940,27 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def createTransportWorkbench(self, workbench_name: str) -> dict:
+    def create_transport_workbench(self, workbench_name: str) -> dict | None:
         """Create a Workbench in the Transport Volume.
 
         Args:
             workbench_name (string): name of the workbench to be created
         Returns:
             dictionary: Create response or None if the creation fails.
         """
 
         createWorbenchPostData = {"type": "528", "name": workbench_name}
 
         request_url = self.config()["nodesUrlv2"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create transport workbench -> {}; calling -> {}".format(
                 workbench_name, request_url
             )
         )
         retries = 0
@@ -2928,15 +2968,15 @@
             response = requests.post(
                 request_url,
                 data=createWorbenchPostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2944,28 +2984,28 @@
                         workbench_name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def unpackTransportPackage(self, package_id: int, workbench_id: int) -> dict:
+    def unpack_transport_package(self, package_id: int, workbench_id: int) -> dict | None:
         """Unpack an existing Transport Package into an existing Workbench.
 
         Args:
             package_iD (integer): ID of package to be unpacked
             workbench_iD (integer): ID of target workbench
         Returns:
             dictionary: Unpack response or None if the unpacking fails.
         """
 
         unpackPackagePostData = {"workbench_id": workbench_id}
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(package_id) + "/unpack"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Unpack transport package with ID -> {} into workbench with ID -> {}; calling -> {}".format(
                 package_id, workbench_id, request_url
             )
         )
 
@@ -2974,15 +3014,15 @@
             response = requests.post(
                 request_url,
                 data=unpackPackagePostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2993,25 +3033,25 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def deployWorkbench(self, workbench_id: int) -> dict:
+    def deploy_workbench(self, workbench_id: int) -> dict | None:
         """Deploy an existing Workbench.
 
         Args:
             workbench_iD (integer): ID of the workbench to be deployed
         Returns:
             dictionary: Deploy response or None if the deployment fails.
         """
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(workbench_id) + "/deploy"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Deploy workbench with ID -> {}; calling -> {}".format(
                 workbench_id, request_url
             )
         )
 
@@ -3026,15 +3066,15 @@
                 logger.error(
                     "Error deploying workbench -> {} : error -> {}".format(
                         workbench_id, e
                     )
                 )
                 return None
             if response.ok:
-                response_dict = self.parseRequestResponse(response)
+                response_dict = self.parse_request_response(response)
                 if not response_dict:
                     logger.error("Error deploying workbench -> {}".format(workbench_id))
                     return None
                 return response_dict
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -3046,21 +3086,21 @@
                         workbench_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def deployTransport(
+    def deploy_transport(
         self,
         package_url: str,
         package_name: str,
         package_description: str = "",
         replacements: list = [],
-    ) -> dict:
+    ) -> dict | None:
         """Main method to deploy a transport. This uses subfunctions to upload,
            unpackage and deploy the transport, and creates the required workbench.
 
         Args:
             package_url (string): URL to download the transport package.
             package_name (string): name of the transport package ZIP file
             package_description (string): description of the transport package
@@ -3070,40 +3110,40 @@
                                           - placeholder: text to replace
                                           - value: text to replace with
         Returns:
             dictionary: Deploy response or None if the deployment fails.
         """
 
         # Preparation: get volume IDs for Transport Warehouse (root volume and Transport Packages)
-        response = self.getVolume(525)
-        transport_root_volume_id = self.getResultValue(response, "id")
+        response = self.get_volume(525)
+        transport_root_volume_id = self.get_result_value(response, "id")
         if not transport_root_volume_id:
             logger.error("Failed to retrieve transport root volume")
             return None
         logger.info("Transport root volume ID -> {}".format(transport_root_volume_id))
 
-        response = self.getNodeByParentAndName(
+        response = self.get_node_by_parent_and_name(
             transport_root_volume_id, "Transport Packages"
         )
-        transport_package_volume_id = self.getResultValue(response, "id")
+        transport_package_volume_id = self.get_result_value(response, "id")
         if not transport_package_volume_id:
             logger.error("Failed to retrieve transport package volume")
             return None
         logger.info(
             "Transport package volume ID -> {}".format(transport_package_volume_id)
         )
 
         # Step 1: Upload Transport Package
         logger.info(
             "Check if transport package -> {} already exists...".format(package_name)
         )
-        response = self.getNodeByParentAndName(
+        response = self.get_node_by_parent_and_name(
             transport_package_volume_id, package_name
         )
-        package_id = self.getResultValue(response, "id")
+        package_id = self.get_result_value(response, "id")
         if package_id:
             logger.info(
                 "Transport package -> {} does already exist; existing package ID -> {}".format(
                     package_name, package_id
                 )
             )
         else:
@@ -3115,22 +3155,22 @@
             # If we have string replacements configured execute them now:
             if replacements:
                 logger.info(
                     "Transport -> {} has replacements -> {}".format(
                         package_name, replacements
                     )
                 )
-                self.replaceTransportPlaceholders(package_url, replacements)
+                self.replace_transport_placeholders(package_url, replacements)
             else:
                 logger.info("Transport -> {} has no replacements!".format(package_name))
             # Upload package to Extended ECM:
-            response = self.uploadFileToVolume(
+            response = self.upload_file_to_volume(
                 package_url, package_name, "application/zip", 531
             )
-            package_id = self.getResultValue(response, "id")
+            package_id = self.get_result_value(response, "id")
             if not package_id:
                 logger.error(
                     "Failed to upload transport package -> {}".format(package_url)
                 )
                 return None
             logger.info(
                 "Successfully uploaded transport package -> {}; new package ID -> {}".format(
@@ -3141,43 +3181,43 @@
         # Step 2: Create Transport Workbench (if not yet exist)
         workbench_name = package_name.split(".")[0]
         logger.info(
             "Check if workbench -> {} is already deployed...".format(workbench_name)
         )
         # check if the package name has the suffix "(deployed)" - this indicates it is alreadey
         # successfully deployed (see renaming at the end of this method)
-        response = self.getNodeByParentAndName(
+        response = self.get_node_by_parent_and_name(
             transport_root_volume_id, workbench_name + " (deployed)"
         )
-        workbench_id = self.getResultValue(response, "id")
+        workbench_id = self.get_result_value(response, "id")
         if workbench_id:
             logger.info(
                 "Workbench -> {} has already been deployed successfully; existing workbench ID -> {}; skipping transport".format(
                     workbench_name, workbench_id
                 )
             )
             # we return and skip this transport...
             return response
         else:
             logger.info(
                 "Check if workbench -> {} already exists...".format(workbench_name)
             )
-            response = self.getNodeByParentAndName(
+            response = self.get_node_by_parent_and_name(
                 transport_root_volume_id, workbench_name
             )
-            workbench_id = self.getResultValue(response, "id")
+            workbench_id = self.get_result_value(response, "id")
             if workbench_id:
                 logger.info(
                     "Workbench -> {} does already exist but is not successfully deployed; existing workbench ID -> {}".format(
                         workbench_name, workbench_id
                     )
                 )
             else:
-                response = self.createTransportWorkbench(workbench_name)
-                workbench_id = self.getResultValue(response, "id")
+                response = self.create_transport_workbench(workbench_name)
+                workbench_id = self.get_result_value(response, "id")
                 if not workbench_id:
                     logger.error(
                         "Failed to create workbench -> {}".format(workbench_name)
                     )
                     return None
                 logger.info(
                     "Successfully created workbench -> {}; new workbench ID -> {}".format(
@@ -3187,49 +3227,49 @@
 
         # Step 3: Unpack Transport Package to Workbench
         logger.info(
             "Unpack transport package -> {} ({}) to workbench -> {} ({})".format(
                 package_name, package_id, workbench_name, workbench_id
             )
         )
-        response = self.unpackTransportPackage(package_id, workbench_id)
-        if response == None:
+        response = self.unpack_transport_package(package_id, workbench_id)
+        if not response:
             logger.error(
                 "Failed to unpack the transport package -> {}".format(package_name)
             )
             return None
         logger.info(
             "Successfully unpackaged to workbench -> {} ({})".format(
                 workbench_name, workbench_id
             )
         )
 
         # Step 4: Deploy Workbench
         logger.info("Deploy workbench -> {} ({})".format(workbench_name, workbench_id))
-        response = self.deployWorkbench(workbench_id)
-        if response == None:
+        response = self.deploy_workbench(workbench_id)
+        if not response:
             logger.error("Failed to deploy workbench -> {}".format(workbench_name))
             return None
 
         logger.info(
             "Successfully deployed workbench -> {} ({})".format(
                 workbench_name, workbench_id
             )
         )
-        self.renameNode(
+        self.rename_node(
             workbench_id,
             workbench_name + " (deployed)",
             package_description,
         )
 
         return response
 
     # end method definition
 
-    def replaceTransportPlaceholders(
+    def replace_transport_placeholders(
         self, zip_file_path: str, replacements: list
     ) -> bool:
         """Search and replace strings in the XML files of the transport packlage
 
         Args:
             zip_file_path (string): path to transport zip file
             replacements (list of dicts): list of replacement values; dict needs to have two values:
@@ -3371,38 +3411,38 @@
         os.rename(new_zip_file_path, zip_file_path)
 
         # Return the path to the new zip file
         return True
 
         # end method definition
 
-    def getWorkspaceTypes(self) -> dict:
+    def get_workspace_types(self) -> dict | None:
         """Get all workspace types configured in Extended ECM.
 
         Args:
             None
         Returns:
             dictionary: Workspace Types or None if the request fails.
         """
 
         request_url = (
             self.config()["businessworkspacetypes"]
             + "?expand_templates=true&expand_wksp_info=true"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info("Get workspace types; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3410,15 +3450,15 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getBusinessObjectType(self, external_system_id: str, type_name: str) -> dict:
+    def get_business_object_type(self, external_system_id: str, type_name: str) -> dict | None:
         """Get business object type information.
 
         Args:
             external_system_id (string): external system Id (such as "TM6")
             type_name (string): type name (such as "SAP Customer")
         Returns:
             dictionary: Workspace Type information or None if the request fails.
@@ -3427,29 +3467,29 @@
         request_url = (
             self.config()["externalSystem"]
             + "/"
             + str(external_system_id)
             + "/botypes/"
             + str(type_name)
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get business object type -> {} for external system -> {}; calling -> {}".format(
                 type_name, external_system_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3459,22 +3499,22 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceCreateForm(
+    def get_workspace_create_form(
         self,
         template_id: int,
         external_system_id: int = None,
         bo_type: int = None,
         bo_id: int = None,
         parent_id: int = None,
-    ) -> dict:
+    ) -> dict | None:
         """Get the Workspace create form.
 
         Args:
             template_id (integer): ID of the workspace template
             external_system_id (string): identifier of the external system (None if no external system)
             bo_type (string, optional): business object type (None if no external system)
             bo_id (string, optional): business object identifier / key (None if no external system)
@@ -3497,29 +3537,29 @@
             request_url += "&bo_type={}".format(bo_type)
             request_url += "&bo_id={}".format(bo_id)
             logger.info(
                 "Use business object connection -> ({}, {}, {}) for workspace template -> {}".format(
                     external_system_id, bo_type, bo_id, template_id
                 )
             )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get workspace create form for template -> {}; calling -> {}".format(
                 template_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3529,37 +3569,37 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspace(self, node_id: int) -> dict:
+    def get_workspace(self, node_id: int) -> dict | None:
         """Get a workspace based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the workspace
         Returns:
             dictionary: Workspace node information or None if no node with this ID is found.
         """
 
         request_url = self.config()["businessworkspaces"] + "/" + str(node_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get workspace with ID -> {}; calling -> {}".format(node_id, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3569,37 +3609,37 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceInstances(self, type_name: str, expanded_view: bool = True):
+    def get_workspace_instances(self, type_name: str, expanded_view: bool = True):
         """Get all workspace instances of a given type. This is a convenience
-           wrapper method for getWorkspaceByTypeAndName()
+           wrapper method for get_workspace_by_type_and_name()
 
         Args:
             type_name (string): name of the workspace type
             expanded_view (boolean, optional): if 'False' then just search in recently
                                                accessed business workspace for this name and type
                                                if 'True' (this is the default) then search in all
                                                workspaces for this name and type
         Returns:
             dictionary: Workspace information or None if the workspace is not found.
         """
 
-        return self.getWorkspaceByTypeAndName(
+        return self.get_workspace_by_type_and_name(
             type_name, name="", expanded_view=expanded_view
         )
 
     # end method definition
 
-    def getWorkspaceByTypeAndName(
+    def get_workspace_by_type_and_name(
         self, type_name: str, name: str = "", expanded_view: bool = True
-    ) -> dict:
+    ) -> dict | None:
         """Lookup workspace based on workspace type and workspace name.
 
         Args:
             type_name (string): name of the workspace type
             name (string, optional): name of the workspace, if "" then deliver all instances
                                      of the given workspace type
             expanded_view (boolean, optional): if 'False' then just search in recently
@@ -3618,15 +3658,15 @@
         }
         if name:
             query["where_name"] = name
 
         encodedQuery = urllib.parse.urlencode(query, doseq=True)
 
         request_url = self.config()["businessworkspaces"] + "?{}".format(encodedQuery)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         if name:
             logger.info(
                 "Get workspace with name -> {} and type -> {}; calling -> {}".format(
                     name, type_name, request_url
                 )
             )
@@ -3639,15 +3679,15 @@
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if name:
@@ -3667,26 +3707,26 @@
                             response.text,
                         )
                     )
                 return None
 
     # end method definition
 
-    def createWorkspace(
+    def create_workspace(
         self,
         workspace_template_id: int,
         workspace_name: str,
         workspace_description: str,
         workspace_type: int,
         category_data: dict = {},
         external_system_id: int = None,
         bo_type: int = None,
         bo_id: int = None,
         parent_id: int = None,
-    ) -> dict:
+    ) -> dict | None:
         """Create a new business workspace.
 
         Args:
             workspace_template_id (integer): ID of the workspace template
             workspace_name (string): name of the workspace
             workspace_description (string): description of the workspace
             workspace_type (integer): type ID of the workspace
@@ -3719,15 +3759,15 @@
                 "Use business object connection -> ({}, {}, {}) for workspace -> {}".format(
                     external_system_id, bo_type, bo_id, workspace_name
                 )
             )
 
         # If workspace creation location cannot be derived from the workspace type
         # there may be an optional parent parameter passed to this method. This can
-        # also be the case if workspaces are nested into eachother:
+        # also be the case if workspaces are nested into each other:
         if parent_id is not None:
             createWorkspacePostData["parent_id"] = parent_id
             logger.info(
                 "Use specified location -> {} for workspace -> {}".format(
                     parent_id, workspace_name
                 )
             )
@@ -3735,15 +3775,15 @@
             logger.info(
                 "Determine location of workspace -> {} via workspace type -> {}".format(
                     workspace_name, workspace_type
                 )
             )
 
         request_url = self.config()["businessworkspaces"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create workspace -> {} with type -> {} from template -> {}; calling -> {}".format(
                 workspace_name, workspace_type, workspace_template_id, request_url
             )
         )
 
@@ -3754,15 +3794,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data={"body": json.dumps(createWorkspacePostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3773,20 +3813,20 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def createWorkspaceRelationship(
+    def create_workspace_relationship(
         self,
         workspace_id: int,
         related_workspace_id: int,
         relationship_type: str = "child",
-    ) -> dict:
+    ) -> dict | None:
         """Create a relationship between two workspaces.
 
         Args:
             workspace_id (integer): ID of the workspace
             related_workspace_id (integer): ID of the related workspace
             relationship_type (string, optional): "parent" or "child" - "child" is default if omitted
         Returns:
@@ -3797,15 +3837,15 @@
             "rel_bw_id": str(related_workspace_id),
             "rel_type": relationship_type,
         }
 
         request_url = self.config()["businessworkspaces"] + "/{}/relateditems".format(
             workspace_id
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create workspace relationship between -> {} and -> {}; calling -> {}".format(
                 workspace_id, related_workspace_id, request_url
             )
         )
 
@@ -3814,15 +3854,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=createWorkspaceRelationshipPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3833,44 +3873,44 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceRelationships(self, workspace_id: int) -> dict:
+    def get_workspace_relationships(self, workspace_id: int) -> dict | None:
         """Get the Workspace relationships to other workspaces.
 
         Args:
             workspace_id (integer): ID of the workspace template
         Returns:
             dictionary: Workspace relationships or None if the request fails.
         """
 
         request_url = (
             self.config()["businessworkspaces"]
             + "/"
             + str(workspace_id)
             + "/relateditems"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get related workspaces for workspace -> {}; calling -> {}".format(
                 workspace_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3880,41 +3920,41 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceRoles(self, workspace_id: int) -> dict:
+    def get_workspace_roles(self, workspace_id: int) -> dict | None:
         """Get the Workspace roles.
 
         Args:
             workspace_id (integer): ID of the workspace template
         Returns:
             dictionary: Workspace Roles data or None if the request fails.
         """
 
         request_url = (
             self.config()["businessworkspaces"] + "/" + str(workspace_id) + "/roles"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get workspace roles of workspace -> {}; calling -> {}".format(
                 workspace_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3924,17 +3964,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def addMemberToWorkspace(
+    def add_member_to_workspace(
         self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True
-    ) -> dict:
+    ) -> dict | None:
         """Add member to a workspace role. Check that the user is not yet a member.
 
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             member_id (integer): User or Group Id
             show_warning (boolean, optional): if True shows a warning if member is already in role
@@ -3943,15 +3983,15 @@
         """
 
         addMemberToWorkspacePostData = {"id": str(member_id)}
 
         request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Check if user/group -> {} is already in role -> {} of workspace -> {}; calling -> {}".format(
                 member_id, role_id, workspace_id, request_url
             )
         )
 
@@ -3963,17 +4003,17 @@
                 "Failed to get workspace members; status -> {}; error -> {}".format(
                     response.status_code,
                     response.text,
                 )
             )
             return None
 
-        workspace_members = self.parseRequestResponse(response)
+        workspace_members = self.parse_request_response(response)
 
-        if self.existResultItem(workspace_members, "id", member_id):
+        if self.exist_result_item(workspace_members, "id", member_id):
             if show_warning:
                 logger.warning(
                     "User -> {} is already a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
                 )
             return workspace_members
@@ -3988,47 +4028,47 @@
             request_url,
             headers=request_header,
             data=addMemberToWorkspacePostData,
             cookies=self.cookie(),
         )
 
         if response.ok:
-            return self.parseRequestResponse(response)
+            return self.parse_request_response(response)
         else:
             logger.error(
                 "Failed to add user/group -> {} to role -> {} of workspace -> {}; status -> {}; error -> {}".format(
                     member_id,
                     role_id,
                     workspace_id,
                     response.status_code,
                     response.text,
                 )
             )
             return None
 
     # end method definition
 
-    def removeMemberFromWorkspace(
+    def remove_member_from_workspace(
         self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True
-    ) -> dict:
+    ) -> dict | None:
         """Remove a member from a workspace role. Check that the user is currently a member.
 
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             member_id (integer): User or Group Id
             show_warning (boolean, optional): if True shows a warning if member is not in role
         Returns:
             dictionary: Workspace Role Membership or None if the request fails.
         """
 
         request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Check if user/group -> {} is in role -> {} of workspace -> {}; calling -> {}".format(
                 member_id, role_id, workspace_id, request_url
             )
         )
 
@@ -4040,17 +4080,17 @@
                 "Failed to get workspace members; status -> {}; error -> {}".format(
                     workspaceMembershipResponse.status_code,
                     workspaceMembershipResponse.text,
                 )
             )
             return None
 
-        workspace_members = self.parseRequestResponse(workspaceMembershipResponse)
+        workspace_members = self.parse_request_response(workspaceMembershipResponse)
 
-        if not self.existResultItem(workspace_members, "id", member_id):
+        if not self.exist_result_item(workspace_members, "id", member_id):
             if show_warning:
                 logger.warning(
                     "User -> {} is not a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
                 )
             return None
@@ -4068,32 +4108,32 @@
         workspaceMembershipResponse = requests.delete(
             request_url,
             headers=request_header,
             cookies=self.cookie(),
         )
 
         if workspaceMembershipResponse.ok:
-            return self.parseRequestResponse(workspaceMembershipResponse)
+            return self.parse_request_response(workspaceMembershipResponse)
         else:
             logger.error(
                 "Failed to remove user/group -> {} to role -> {} of workspace -> {}; status -> {}; error -> {}".format(
                     member_id,
                     role_id,
                     workspace_id,
                     workspaceMembershipResponse.status_code,
                     workspaceMembershipResponse.text,
                 )
             )
             return None
 
     # end method definition
 
-    def assignWorkspacePermissions(
+    def assign_workspace_permissions(
         self, workspace_id: int, role_id: int, permissions: list, apply_to: int = 2
-    ) -> dict:
+    ) -> dict | None:
         """Update permissions of a workspace role
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             permissions (list): list of permissions - potential elements:
                                 "see"
                                 "see_contents"
@@ -4113,15 +4153,15 @@
             dictionary: Workspace Role Membership or None if the request fails.
         """
 
         request_url = self.config()["businessworkspaces"] + "/{}/roles/{}".format(
             workspace_id, role_id
         )
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Updating Permissions of role -> {} of workspace -> {} with permissions -> {}; calling -> {}".format(
                 role_id, workspace_id, permissions, request_url
             )
         )
 
@@ -4135,15 +4175,15 @@
             response = requests.put(
                 request_url,
                 headers=request_header,
                 data={"body": json.dumps(permissionPostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4154,15 +4194,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateWorkspaceIcon(
+    def update_workspace_icon(
         self, workspace_id: int, file_path: str, file_mimetype: str = "image/*"
     ):
         """Update a workspace with a with a new icon (which is uploaded).
 
         Args:
             workspace_id (integer): ID of the workspace
             file_path (string): path + filename of icon file
@@ -4181,15 +4221,15 @@
             "file_filename": os.path.basename(file_path),
             "file": file_path,  # icon_file
         }
 
         request_url = (
             self.config()["businessworkspaces"] + "/" + str(workspace_id) + "/icons"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Update icon for workspace ID -> {} with icon file -> {}; calling -> {}".format(
                 workspace_id, file_path, request_url
             )
         )
 
@@ -4198,15 +4238,15 @@
             response = requests.post(
                 request_url,
                 data=updateWorkspaceIconPutBody,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4214,23 +4254,23 @@
                         workspace_id, file_path, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def createItem(
+    def create_item(
         self,
         parent_id: int,
         item_type: str,
         item_name: str,
         item_description: str = "",
         url: str = "",
         original_id: int = 0,
-    ) -> dict:
+    ) -> dict | None:
         """Create an Extended ECM item. This REST call is somewhat limited. It cannot set favortie (featured item) or hidden item.
            It does also not accept owner group information.
 
         Args:
             parent_id (integer): node ID of the parent
             item_type (string): type of the item (e.g. 0 = foler, 140 = URL)
             item_name (string): name of the item
@@ -4250,15 +4290,15 @@
 
         if url:
             createItemPostData["url"] = url
         if original_id > 0:
             createItemPostData["original_id"] = original_id
 
         request_url = self.config()["nodesUrlv2"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create item -> {} (type -> {}) under parent -> {}; calling -> {}".format(
                 item_name, item_type, parent_id, request_url
             )
         )
 
@@ -4268,15 +4308,15 @@
             response = requests.post(
                 request_url,
                 data={"body": json.dumps(createItemPostData)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4286,21 +4326,21 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateItem(
+    def update_item(
         self,
         node_id: int,
         parent_id: int = 0,
         item_name: str = "",
         item_description: str = "",
-    ) -> dict:
+    ) -> dict | None:
         """Update an Extended ECM item (parent, name, description). Changing the parent ID is
            a move operation. If parent ID = 0 the item will not be moved.
 
         Args:
             node_id (integer): ID of the node
             parent_id (integer): node ID of the new parent (move operation)
             item_name (string): new name of the item
@@ -4315,15 +4355,15 @@
         }
 
         if parent_id:
             # this is a move operation
             updateItemPutData["parent_id"] = parent_id
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Update item -> {} with data -> {}; calling -> {}".format(
                 item_name, updateItemPutData, request_url
             )
         )
 
@@ -4333,15 +4373,15 @@
             response = requests.put(
                 request_url,
                 data={"body": json.dumps(updateItemPutData)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4351,15 +4391,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getDocumentTemplates(self, parent_id: int):
+    def get_document_templates(self, parent_id: int):
         """Get all document templates for a given target location.
 
         Args:
             parent_id (integer): node ID of target location (e.g. a folder)
 
         Returns:
             dictionary: response of the REST call (converted to a Python dictionary)
@@ -4392,15 +4432,15 @@
 
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_id)
             + "/doctemplates?subtypes={144}&sidepanel_subtypes={144}"
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get document templates for target location -> {} (parent); calling -> {}".format(
                 parent_id, request_url
             )
         )
 
@@ -4409,15 +4449,15 @@
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
             response = requests.get(
                 request_url,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4427,15 +4467,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def createDocumentFromTemplate(
+    def create_document_from_template(
         self,
         template_id: int,
         parent_id: int,
         classification_id: int,
         category_data: dict,
         doc_name: str,
         doc_desciption: str = "",
@@ -4473,15 +4513,15 @@
             "roles": {
                 "categories": category_data,
                 "classifications": {"create_id": [classification_id], "id": []},
             },
         }
 
         request_url = self.config()["doctemplatesUrl"]
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create document -> {} from template -> {} in target location -> {} (parent); calling -> {}".format(
                 doc_name, template_id, parent_id, request_url
             )
         )
 
@@ -4493,15 +4533,15 @@
                 # this seems to only work with a "body" tag and is different form the documentation
                 # on developer.opentext.com
                 data={"body": json.dumps(createDocumentPostData)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4511,15 +4551,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWebReportParameters(self, nickname: str):
+    def get_web_report_parameters(self, nickname: str):
         """Get parameters of a Web Report in Extended ECM. These are defined on the Web Report node
             (Properties --> Parameters)
 
         Args:
             nickname (string): nickname of the Web Reports node.
         Returns:
             Response: list of Web Report parameters. Each list item is a dict describing the parameter.
@@ -4534,29 +4574,29 @@
                 "description": "string",
                 "mandatory": true
             }
             None if the REST call has failed.
         """
 
         request_url = self.config()["webReportsUrl"] + "/" + nickname + "/parameters"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Retrieving parameters of Web Report with nickname -> {}; calling -> {}".format(
                 nickname, request_url
             )
         )
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 # Return the "data" element which is a list of dict items:
-                result_dict = self.parseRequestResponse(response)
+                result_dict = self.parse_request_response(response)
                 logger.debug("Web Report parameters result -> {}".format(result_dict))
                 if not result_dict.get("data"):
                     return None
                 return result_dict["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -4570,26 +4610,26 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def runWebReport(self, nickname: str, web_report_parameters: dict = {}) -> dict:
+    def run_web_report(self, nickname: str, web_report_parameters: dict = {}) -> dict | None:
         """Run a Web Report that is identified by its nick name.
 
         Args:
             nickname (string): nickname of the Web Reports node.
             web_report_parameters (dictionary): Parameters of the Web Report (names + value pairs)
         Returns:
             dictionary: Response of the run Web Report request or None if the Web Report execution has failed.
         """
 
         request_url = self.config()["webReportsUrl"] + "/" + nickname
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Running Web Report with nickname -> {}; calling -> {}".format(
                 nickname, request_url
             )
         )
 
@@ -4598,15 +4638,15 @@
             response = requests.post(
                 request_url,
                 data=web_report_parameters,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4616,27 +4656,27 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def installCSApplication(self, application_name: str) -> dict:
+    def install_cs_application(self, application_name: str) -> dict | None:
         """Install a CS Application (based on WebReports)
 
         Args:
             application_name (string): name of the application (e.g. OTPOReports, OTRMReports, OTRMSecReports)
         Returns:
             dictionary: Response or None if the installation of the CS Application has failed.
         """
 
         installCSApplicationPostData = {"appName": application_name}
 
         request_url = self.config()["csApplicationsUrl"] + "/install"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Install CS Application -> {}; calling -> {}".format(
                 application_name, request_url
             )
         )
 
@@ -4645,15 +4685,15 @@
             response = requests.post(
                 request_url,
                 data=installCSApplicationPostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4663,17 +4703,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def assignItemToUserGroup(
+    def assign_item_to_user_group(
         self, node_id: int, subject: str, instruction: str, assignees: list
-    ) -> dict:
+    ) -> dict | None:
         """Assign an Extended ECM item to users and groups. This is a function used by
            Extended ECM for Government.
 
         Args:
             node_id (integer): node ID of the Extended ECM item (e.g. a workspace or a document)
             subject (string): title / subject of the assignment
             instructions (string): more detailed description or instructions for the assignment
@@ -4688,15 +4728,15 @@
             "assignees": assignees,
         }
 
         request_url = (
             self.config()["nodesUrlv2"] + "/" + str(node_id) + "/xgovassignments"
         )
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign item with ID -> {} to assignees -> {} (subject -> {}); calling -> {}".format(
                 node_id, assignees, subject, request_url
             )
         )
 
@@ -4706,15 +4746,15 @@
             response = requests.post(
                 request_url,
                 data={"add_assignment": json.dumps(assignmentPostData)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4726,15 +4766,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def convertPermissionStringToPermissionValue(self, permissions: list) -> int:
+    def convert_permission_string_to_permission_value(self, permissions: list) -> int:
         """Converts a list of permission names (strongs) to a bit-mask.
 
         Args:
             permissions (list): List of permission names - see conversion variable below.
         Returns:
             integer: bit-encoded permission value
         """
@@ -4760,15 +4800,17 @@
                 return 0
             permission_value += conversion[permission]
 
         return permission_value
 
     # end method definition
 
-    def convertPermissionValueToPermissionString(self, permission_value: int) -> list:
+    def convert_permission_value_to_permission_string(
+        self, permission_value: int
+    ) -> list:
         """Converts a bit-encoded permission value to a list of permission names (strings).
 
         Args:
             permission_value (integer): bit-encoded permission value
         Returns:
             list: list of permission names
         """
@@ -4792,22 +4834,22 @@
             if permission_value & value:  # binary and
                 permissions.append(key)
 
         return permissions
 
     # end method definition
 
-    def assignPermission(
+    def assign_permission(
         self,
         node_id: int,
         assignee_type: str,
         assignee: int,
         permissions: list,
         apply_to: int = 0,
-    ) -> dict:
+    ) -> dict | None:
         """Assign permissions for Extended ECM item to a user or group.
 
         Args:
             node_id (integer): node ID of the Extended ECM item
             assignee_type (string): this can be either "owner", "group" (for owner group),
                                     "public", or "custom" (assigned access)
             assignee (integer): ID of user or group ("right ID"). If 0 and assigneeType
@@ -4861,15 +4903,15 @@
             self.config()["nodesUrlv2"]
             + "/"
             + str(node_id)
             + "/permissions/"
             + assignee_type
         )
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign permissions -> {} to item with ID -> {}; assignee type -> {}; calling -> {}".format(
                 permissions, node_id, assignee_type, request_url
             )
         )
 
@@ -4890,15 +4932,15 @@
                 response = requests.put(
                     request_url,
                     data={"body": json.dumps(permissionPostData)},
                     headers=request_header,
                     cookies=self.cookie(),
                 )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4909,42 +4951,42 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNodeCategories(self, node_id: int, metadata: bool = True):
+    def get_node_categories(self, node_id: int, metadata: bool = True):
         """Get categories assigned to a node.
 
         Args:
             node_id (integer): ID of the node to get the categories for.
             metadata (boolean, optional): expand the attribute definitions of the category. Default is True
         Returns:
             dictionary: category response or None if the call to the REST API fails.
         """
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id) + "/categories"
         if metadata:
             request_url += "?metadata"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get categories of node with ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -4952,15 +4994,15 @@
                         node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNodeCategory(self, node_id: int, category_id: int, metadata: bool = True):
+    def get_node_category(self, node_id: int, category_id: int, metadata: bool = True):
         """Get a specific category assigned to a node.
 
         Args:
             node_id (integer): ID of the node to get the categories for.
             category_id (integer): ID of the category definition ID (in category volume)
             metadata (boolean, optional): expand the attribute definitions of the category. Default is True
         Returns:
@@ -4972,29 +5014,29 @@
             + "/"
             + str(node_id)
             + "/categories/"
             + str(category_id)
         )
         if metadata:
             request_url += "?metadata"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get category with ID -> {} on node with ID -> {}; calling -> {}".format(
                 category_id, node_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5002,39 +5044,39 @@
                         category_id, node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNodeCategoryIds(self, node_id: int) -> list:
+    def get_node_category_ids(self, node_id: int) -> list:
         """Get list of all category definition IDs that are assign to the node.
 
         Args:
             node_id (integer): ID of the node to get the categories for.
         Returns:
             list: list of category IDs (all categories assigned to the node)
         """
 
-        categories = self.getNodeCategories(node_id)
+        categories = self.get_node_categories(node_id)
         if not categories or not categories["results"]:
             return None
 
         category_id_list = []
 
         for category in categories["results"]:
             category_id_list += [
                 int(i) for i in category["metadata_order"]["categories"]
             ]
 
         return category_id_list
 
     # end method definition
 
-    def getNodeCategoryDefinition(self, node_id: int, category_name: str):
+    def get_node_category_definition(self, node_id: int, category_name: str):
         """Get category definition (category id and attribute IDs and types)
 
         Args:
             node_id (integer): node to read the category definition from
                                (e.g. a workspace template or a document template or a target folder)
                                This should NOT be the category definition object!
             category_name (string): name of the category
@@ -5051,15 +5093,15 @@
                                 'id': '12532_3',
                                 'type': 'user'
                             },
                             ...
                         }
         """
 
-        response = self.getNodeCategories(node_id)
+        response = self.get_node_categories(node_id)
         if response and response["results"]:
             attribute_definitions = {}
             for categories in response["results"]:
                 keys = categories["metadata"]["categories"].keys()
                 cat_id = next((key for key in keys if "_" not in key), -1)
                 cat_name = categories["metadata"]["categories"][cat_id]["name"]
                 if cat_name != category_name:
@@ -5076,15 +5118,15 @@
                     else:
                         att_type = categories["metadata"]["categories"][att_id][
                             "type_name"
                         ]
                     attribute_definitions[att_name] = {"id": att_id, "type": att_type}
         return cat_id, attribute_definitions
 
-    def assignCategory(
+    def assign_category(
         self,
         node_id: int,
         category_id: list,
         inheritance: bool = False,
         apply_to_sub_items: bool = False,
         apply_action: str = "add_upgrade",
         add_version: bool = False,
@@ -5108,21 +5150,21 @@
             add_version (boolean, optional): if a document version should be added for the category change (default = False)
             clear_existing_categories (boolean, optional): whether or not existing (other) categories should be removed (default = False)
         Returns:
             boolean: True = success, False = error
         """
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id) + "/categories"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         #
         # 1. Assign Category to Node if not yet assigned:
         #
 
-        existing_category_ids = self.getNodeCategoryIds(node_id)
+        existing_category_ids = self.get_node_category_ids(node_id)
         if not category_id in existing_category_ids:
             logger.info(
                 "Category with ID -> {} is not yet assigned to node ID -> {}. Assigning it now...".format(
                     category_id, node_id
                 )
             )
             categoryPostData = {
@@ -5232,15 +5274,15 @@
                         )
                     )
                     return False
         return True
 
     # end method definition
 
-    def setCategoryValue(
+    def set_category_value(
         self,
         node_id: int,
         value,
         category_id: int,
         attribute_id: int,
         set_id: int = 0,
         set_row: int = 1,
@@ -5263,15 +5305,15 @@
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(node_id)
             + "/categories/"
             + str(category_id)
         )
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         if set_id:
             logger.info(
                 "Assign value -> {} to category -> {}, set -> {}, row -> {}, attribute -> {} on node -> {}; calling -> {}".format(
                     value,
                     category_id,
                     set_id,
@@ -5301,15 +5343,15 @@
             response = requests.put(
                 request_url,
                 data=categoryPutData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5322,17 +5364,17 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def assignClassification(
+    def assign_classification(
         self, node_id: int, classifications: list, apply_to_sub_items: bool = False
-    ) -> dict:
+    ) -> dict | None:
         """Assign one or multiple classifications to an Extended ECM item
         Args:
             node_id (integer): node ID of the Extended ECM item
             classifications (list): list of classification item IDs
             apply_to_sub_items (boolean, optional): if True the classification is applied to
                                                     the item and all its sub-items
                                                     if False the classification is only applied
@@ -5351,15 +5393,15 @@
             "apply_to_sub_items": apply_to_sub_items,
         }
 
         request_url = (
             self.config()["nodesUrl"] + "/" + str(node_id) + "/classifications"
         )
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign classifications with IDs -> {} to item with ID -> {}; calling -> {}".format(
                 classifications, node_id, request_url
             )
         )
 
@@ -5368,15 +5410,15 @@
             response = requests.post(
                 request_url,
                 data=classificationPostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5387,17 +5429,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def assignRMClassification(
+    def assign_rm_classification(
         self, node_id: int, rm_classification: int, apply_to_sub_items: bool = False
-    ) -> dict:
+    ) -> dict | None:
         """Assign a RM classification to an Extended ECM item
         Args:
             node_id (integer): node ID of the Extended ECM item
             rm_classification (integer): Records Management classification ID
             apply_to_sub_items (boolean, optional): if True the RM classification is applied to
                                                     the item and all its sub-items
                                                     if False the RM classification is only applied
@@ -5411,15 +5453,15 @@
             "apply_to_sub_items": apply_to_sub_items,
         }
 
         request_url = (
             self.config()["nodesUrl"] + "/" + str(node_id) + "/rmclassifications"
         )
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign RM classifications with ID -> {} to item with ID -> {}; calling -> {}".format(
                 rm_classification, node_id, request_url
             )
         )
 
@@ -5428,15 +5470,15 @@
             response = requests.post(
                 request_url,
                 data=rmClassificationPostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5447,27 +5489,27 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def registerWorkspaceTemplate(self, node_id: int) -> dict:
+    def register_workspace_template(self, node_id: int) -> dict | None:
         """Register a workspace template as project template for Extended ECM for Engineering
         Args:
             node_id (integer): node ID of the Extended ECM workspace template
         Returns:
             dictionary: Response of request or None if the registration of the workspace template has failed.
         """
 
         registrationPostData = {"ids": "{{ {} }}".format(node_id)}
 
         request_url = self.config()["xEngProjectTemplateUrl"]
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Register workspace template with ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
         )
 
@@ -5476,15 +5518,15 @@
             response = requests.post(
                 request_url,
                 data=registrationPostData,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5494,15 +5536,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getRecordsManagementRSIs(self, limit: int = 100):
+    def get_records_management_rsis(self, limit: int = 100):
         """Get all Records management RSIs togther with their RSI Schedules.
 
         Args:
             limit (integer, optional): max elements to return (default = 100)
         Returns:
             list: list of Records Management RSIs or None if the request fails.
             Each RSI list element is a dict with this structure:
@@ -5543,27 +5585,27 @@
                 "ApprovalFlag": 0,
                 "MaximumRet": 0,
                 "ObjectType": "LIV"
             }
         """
 
         request_url = self.config()["rsisUrl"] + "?limit=" + str(limit)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get list of Records Management RSIs; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                rsi_dict = self.parseRequestResponse(response)
+                rsi_dict = self.parse_request_response(response)
                 return rsi_dict["results"]["data"]["rsis"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
@@ -5572,39 +5614,39 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getRecordsManagementCodes(self):
+    def get_records_management_codes(self):
         """Get Records Management Codes. These are the most basic data types of
            the Records Management configuration and required to create RSIs and
            other higher-level Records Management configurations
 
         Args:
             None
         Returns:
             RSI data (json) or None if the request fails.
         """
 
         request_url = self.config()["recordsManagementUrlv2"] + "/rmcodes"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get list of Records Management codes; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                rm_codes_dict = self.parseRequestResponse(response)
+                rm_codes_dict = self.parse_request_response(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
@@ -5614,44 +5656,44 @@
                     )
                 )
                 return None
 
     # end method definition
 
     # This is not yet working. REST API endpoint seems not to be in 22.4. Retest with 23.1
-    def updateRecordsManagementCodes(self, rm_codes: dict):
+    def update_records_management_codes(self, rm_codes: dict):
         """Update Records Management Codes. These are the most basic data types of
            the Records Management configuration and required to create RSIs and
            other higher-level Records Management configurations
 
         Args:
             rm_codes: dict with the updated codes
         Returns:
             RSI data (json) or None if the request fails.
         """
 
         updateRMCodesPostData = {}
 
         request_url = self.config()["recordsManagementUrl"] + "/rmcodes"
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Update Records Management codes; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=updateRMCodesPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                rm_codes_dict = self.parseRequestResponse(response)
+                rm_codes_dict = self.parse_request_response(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
@@ -5660,24 +5702,24 @@
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def createRecordsManagementRSI(
+    def create_records_management_rsi(
         self,
         name: str,
         status: str,
         status_date: str,
         description: str,
         subject: str,
         title: str,
         dispcontrol: bool,
-    ) -> dict:
+    ) -> dict | None:
         """Create a new Records Management RSI.
 
         Args:
             name (string): name of the RSI
             status (string): status of the RSI
             status_date (string): statusDate of the RSI YYYY-MM-DDTHH:mm:ss
             description (string): description of the RSI
@@ -5700,15 +5742,15 @@
             "subject": subject,
             "title": title,
             "dispcontrol": dispcontrol,
         }
 
         request_url = self.config()["rsiSchedulesUrl"]
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create Records Management RSI -> {}; calling -> {}".format(
                 name, request_url
             )
         )
 
@@ -5717,15 +5759,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=createRSIPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5735,15 +5777,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def createRecordsManagementRSISchedule(
+    def create_records_management_rsi_schedule(
         self,
         rsi_id: int,
         stage: str,
         event_type: int = 1,
         object_type: str = "LIV",
         rule_code: str = "",
         rule_comment: str = "",
@@ -5764,15 +5806,15 @@
         action_code: int = 0,
         description: str = "",
         new_status: str = "",
         min_num_versions_to_keep: int = 1,
         purge_superseded: bool = False,
         purge_majors: bool = False,
         mark_official_rendition: bool = False,
-    ) -> dict:
+    ) -> dict | None:
         """Create a new Records Management RSI Schedule for an existing RSI.
 
         Args:
             rsi_id (integer): ID of an existing RSI the schedule should be created for
             object_type (string): either "LIV" - Classified Objects (default) or "LRM" - RM Classifications
             stage (string): retention stage - this is the key parameter to define multiple stages (stages are basically schedules)
             event_type (integer): 1 Calculated Date, 2 Calendar Calculation, 3 Event Based, 4 Fixed Date, 5 Permanent
@@ -5834,15 +5876,15 @@
             "purgeSuperseded": purge_superseded,
             "purgeMajors": purge_majors,
             "markOfficialRendition": mark_official_rendition,
         }
 
         request_url = self.config()["rsiSchedulesUrl"] + "/" + str(rsi_id) + "/stages"
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create Records Management RSI Schedule -> {} for RSI -> {}; calling -> {}".format(
                 stage, rsi_id, request_url
             )
         )
 
@@ -5851,15 +5893,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=createRSISchedulePostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5869,24 +5911,24 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def createRecordsManagementHold(
+    def create_records_management_hold(
         self,
         hold_type: str,
         name: str,
         comment: str,
         alternate_id: str = "",
         parent_id: int = 0,
         date_applied: str = "",
         date_to_remove: str = "",
-    ) -> dict:
+    ) -> dict | None:
         """Create a new Records Management Hold.
 
         Args:
             hold_type (string): type of the Hold
             name (string): name of the RSI
             comment (string): comment
             alternate_id (string): alternate hold ID
@@ -5911,15 +5953,15 @@
         }
 
         if parent_id > 0:
             createHoldPostData["parent_id"] = parent_id
 
         request_url = self.config()["holdsUrl"]
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Create Records Management Hold -> {}; calling -> {}".format(
                 name, request_url
             )
         )
 
@@ -5928,15 +5970,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=createHoldPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -5946,18 +5988,18 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getRecordsManagementHolds(self) -> dict:
+    def get_records_management_holds(self) -> dict | None:
         """Get a list of all Records Management Holds in the system. Even though there are folders
         in the holds management area in RM these are not real folders - they cannot be retrieved
-        with getNodeByParentAndName() thus we need this method to get them all.
+        with get_node_by_parent_and_name() thus we need this method to get them all.
 
         Args:
             None
         Returns:
             dictionary: Response with list of holds:
             "results": {
                 "data": {
@@ -5983,29 +6025,29 @@
                     ]
                 }
             }
         """
 
         request_url = self.config()["holdsUrlv2"]
 
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Get list of Records Management Holds; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -6014,15 +6056,15 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def importRecordsManagementSettings(self, file_path: str) -> bool:
+    def import_records_management_settings(self, file_path: str) -> bool:
         """Import Records Management settings from a file that is uploaded from the python pod
 
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Returns:
             boolean: True if if the REST call succeeds or False otherwise.
         """
@@ -6072,15 +6114,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importRecordsManagementCodes(
+    def import_records_management_codes(
         self, file_path: str, update_existing_codes: bool = True
     ) -> bool:
         """Import RM Codes from a file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of settings file in Python container filesystem
             update_existing_codes (boolean): Flag that controls whether existing table maintenance codes
                                              should be updated.
@@ -6136,15 +6178,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importRecordsManagementRSIs(
+    def import_records_management_rsis(
         self,
         file_path: str,
         update_existing_rsis: bool = True,
         delete_schedules: bool = False,
     ) -> bool:
         """Import RM RSIs from a config file that is uploaded from the Python pod
         Args:
@@ -6206,15 +6248,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importPhysicalObjectsSettings(self, file_path: str) -> bool:
+    def import_physical_objects_settings(self, file_path: str) -> bool:
         """Import Physical Objects settings from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Returns:
             boolean: True if if the REST call succeeds or False otherwise.
         """
 
@@ -6263,15 +6305,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importPhysicalObjectsCodes(
+    def import_physical_objects_codes(
         self, file_path: str, update_existing_codes: bool = True
     ) -> bool:
         """Import Physical Objects codes from a config file that is uploaded from the Python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             update_existing_codes (boolean): whether or not existing codes should be updated (default = True)
         Returns:
@@ -6326,15 +6368,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importPhysicalObjectsLocators(self, file_path: str) -> bool:
+    def import_physical_objects_locators(self, file_path: str) -> bool:
         """Import Physical Objects locators from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Returns:
             boolean: True if if the REST call succeeds or False otherwise.
         """
 
@@ -6383,15 +6425,15 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importSecurityClearanceCodes(
+    def import_security_clearance_codes(
         self, file_path: str, include_users: bool = False
     ) -> bool:
         """Import Security Clearance codes from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             include_users (boolean): defines if users should be included or not
         Returns:
@@ -6446,17 +6488,17 @@
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def assignUserSecurityClearance(
+    def assign_user_security_clearance(
         self, user_id: int, security_clearance: int
-    ) -> dict:
+    ) -> dict | None:
         """Assign a Security Clearance level to an Extended ECM user
 
         Args:
             user_id (integer): ID of the user
             security_clearance (integer): security clearance level to be set
         Returns:
             dictionary: REST response or None if the REST call fails.
@@ -6465,15 +6507,15 @@
         assignUserSecurityClearancePostData = {
             "securityLevel": security_clearance,
         }
 
         request_url = self.config()[
             "userSecurityUrl"
         ] + "/{}/securityclearancelevel".format(user_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign security clearance -> {} to user ID -> {}; calling -> {}".format(
                 security_clearance, user_id, request_url
             )
         )
 
@@ -6482,15 +6524,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=assignUserSecurityClearancePostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -6501,17 +6543,17 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def assignUserSupplementalMarkings(
+    def assign_user_supplemental_markings(
         self, user_id: int, supplemental_markings: list
-    ) -> dict:
+    ) -> dict | None:
         """Assign a list of Supplemental Markings to a user
 
         Args:
             user_id (integer): ID of the user
             supplemental_markings (list of strings): list of Supplemental Markings to be set
         Returns:
             dictionary: REST response or None if the REST call fails.
@@ -6520,15 +6562,15 @@
         assignUserSupplementalMarkingsPostData = {
             "suppMarks": supplemental_markings,
         }
 
         request_url = self.config()[
             "userSecurityUrl"
         ] + "/{}/supplementalmarkings".format(user_id)
-        request_header = self.requestFormHeader()
+        request_header = self.request_form_header()
 
         logger.info(
             "Assign supplemental markings -> {} to user ID -> {}; calling -> {}".format(
                 supplemental_markings, user_id, request_url
             )
         )
 
@@ -6537,15 +6579,15 @@
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=assignUserSupplementalMarkingsPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -6559,22 +6601,32 @@
                 return None
 
     # end method definition
 
     def volumeTranslator(
         self, current_node_id: int, translator: object, languages: list
     ):
+        """Experimental code to translate the item names and item descriptions in a given hierarchy.
+           The actual translation is done by a tranlator object. This recursive method just
+           traverses the hierarchy and calls the translate() method of the translator object.
+
+        Args:
+            current_node_id (int): current node ID to translate
+            translator (object): this object needs to be created based on the "Translator" class
+                                 and passed to this method
+            languages (list): list of target languages
+        """
         # Get current node based on the ID:
-        current_node = self.getNode(current_node_id)
-        current_node_id = self.getResultValue(current_node, "id")
+        current_node = self.get_node(current_node_id)
+        current_node_id = self.get_result_value(current_node, "id")
 
-        name = self.getResultValue(current_node, "name")
-        description = self.getResultValue(current_node, "description")
-        names_multilingual = self.getResultValue(current_node, "name_multilingual")
-        descriptions_multilingual = self.getResultValue(
+        name = self.get_result_value(current_node, "name")
+        description = self.get_result_value(current_node, "description")
+        names_multilingual = self.get_result_value(current_node, "name_multilingual")
+        descriptions_multilingual = self.get_result_value(
             current_node, "description_multilingual"
         )
 
         for language in languages:
             if language == "en":
                 continue
             # Does the language not exist as metadata language or is it already translated?
@@ -6593,24 +6645,25 @@
                 and not descriptions_multilingual[language]
             ):
                 descriptions_multilingual[language] = translator.translate(
                     "en", language, descriptions_multilingual["en"]
                 )
 
         # Rename node multi-lingual:
-        response = self.renameNode(
+        response = self.rename_node(
             current_node_id,
             name,
             description,
             names_multilingual,
             descriptions_multilingual,
         )
 
         # Get children nodes of the current node:
-        results = self.getSubnodes(current_node_id, limit=200)["results"]
+        results = self.get_subnodes(current_node_id, limit=200)["results"]
 
+        # Recursive call of all subnodes:
         for result in results:
             self.volumeTranslator(
                 result["data"]["properties"]["id"], translator, languages
             )
 
     # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/otds.py` & `pyxecm-0.3.0/pyxecm/otds.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,242 +8,341 @@
 Methods:
 
 __init__ : class initializer
 config : returns config data set
 cookie : returns cookie information
 credentials: returns set of username and password
 
-baseUrl : returns OTDS base URL
-restUrl : returns OTDS REST base URL
-credentialUrl : returns the OTDS Credentials REST URL
-authHandlerUrl : returns the OTDS Authentication Handler REST URL
-partitionUrl : returns OTDS Partition REST URL
-accessRoleUrl : returns OTDS Access Role REST URL
-oauthClientUrl : returns OTDS OAuth Client REST URL
-resourceUrl : returns OTDS Resource REST URL
-licenseUrl : returns OTDS License REST URL
-tokenUrl : returns OTDS Token REST URL
-usersUrl : returns OTDS Users REST URL
-groupsUrl : returns OTDS Groups REST URL
-systemConfigUrl : returns OTDS System Config REST URL
+base_url : returns OTDS base URL
+rest_url : returns OTDS REST base URL
+credential_url : returns the OTDS Credentials REST URL
+authHandler_url : returns the OTDS Authentication Handler REST URL
+partition_url : returns OTDS Partition REST URL
+access_role_url : returns OTDS Access Role REST URL
+oauth_client_url : returns OTDS OAuth Client REST URL
+resource_url : returns OTDS Resource REST URL
+license_url : returns OTDS License REST URL
+token_url : returns OTDS Token REST URL
+users_url : returns OTDS Users REST URL
+groups_url : returns OTDS Groups REST URL
+system_config_url : returns OTDS System Config REST URL
+consolidation_url: returns OTDS consolidation URL
 
 authenticate : authenticates at OTDS server
 
-addLicenseToResource : Add (or update) a product license to OTDS
-getLicensesForResource : Get list of licenses for a resource
-deleteLicenseFromResource : Delete a license from a resource
-assignUserToLicense : Assign an OTDS user to a product license (feature) in OTDS.
-assignPartitionToLicense: Assign an OTDS user partition to a license (feature) in OTDS.
-getLicensedObjects: Return the licensed objects (users, groups, partitions) an OTDS for a
-                    license + license feature associated with an OTDS resource (like "cs").
-isUserLicensed: Check if a user is licensed for a license and license feature associated
-                with a particular OTDS resource.
-isPartitionLicensed: Check if a user partition is licensed for a license and license feature
-                     associated with a particular OTDS resource.
-
-addPartition : Add an OTDS partition
-getPartition : Get a partition with a specific name
-addUser : Add a user to a partion
-getUser : Get a user with a specific user ID (= login name @ partition)
-updateUser : Update attributes of on OTDS user
-deleteUser : Delete a user with a specific ID in a specific partition
-resetUserPassword : Reset a password of a specific user ID
-addGroup: Add an OTDS group
-getGroup: Get a OTDS group by its name
-addUserToGroup : Add an OTDS user to a OTDS group
-addGroupToParentGroup : Add on OTDS group to a parent group
-
-addResource : Add a new resource to OTDS
-getResource : Get an OTDS resource with a specific name
-activateResource : Activate an OTDS resource
-
-getAccessRoles : Get all OTDS Access Roles
-getAccessRole: Get an OTDS Access Role with a specific name
-addPartitionToAccessRole : Add an OTDS Partition to to an OTDS Access Role
-addUserToAccessRole : Add an OTDS user to to an OTDS Access Role
-addGroupToAccessRole : Add an OTDS group to to an OTDS Access Role
-updateAccessRoleAttributes: Update attributes of an existing access role
-
-addSystemAttribute : Add an OTDS System Attribute
-
-getTrustedSites : Get OTDS Trusted Sites
-addTrustedSite : Add a new trusted site to OTDS
-
-addOauthClient : Add a new OAuth client to OTDS
-getOauthClient : Get an OAuth client with a specific client ID
-updateOauthClient : Update an OAuth client
-addOauthClientsToAccessRole : Add an OTDS OAuth Client to an OTDS Access Role
-getAccessToken : Get an OTDS Access Token
-
-addAuthHandlerSAML: Add an authentication handler for SAML (e.g. for SuccessFactors)
-addAuthHandlerSAP: Add an authentication handler for SAP
-addAuthHandlerOAuth: Add an authentication handler for OAuth (used for Salesforce)
+add_license_to_resource : Add (or update) a product license to OTDS
+get_license_for_resource : Get list of licenses for a resource
+delete_license_from_resource : Delete a license from a resource
+assign_user_to_license : Assign an OTDS user to a product license (feature) in OTDS.
+assign_partition_to_license: Assign an OTDS user partition to a license (feature) in OTDS.
+get_licensed_objects: Return the licensed objects (users, groups, partitions) an OTDS for a
+                      license + license feature associated with an OTDS resource (like "cs").
+is_user_licensed: Check if a user is licensed for a license and license feature associated
+                  with a particular OTDS resource.
+is_group_licensed: Check if a group is licensed for a license and license feature associated
+                   with a particular OTDS resource.
+is_partition_licensed: Check if a user partition is licensed for a license and license feature
+                       associated with a particular OTDS resource.
+
+add_partition : Add an OTDS partition
+get_partition : Get a partition with a specific name
+add_user : Add a user to a partion
+get_user : Get a user with a specific user ID (= login name @ partition)
+update_user : Update attributes of on OTDS user
+delete_user : Delete a user with a specific ID in a specific partition
+reset_user_password : Reset a password of a specific user ID
+add_group: Add an OTDS group
+get_group: Get a OTDS group by its name
+add_user_to_group : Add an OTDS user to a OTDS group
+add_group_to_parent_group : Add on OTDS group to a parent group
+
+add_resource : Add a new resource to OTDS
+get_resource : Get an OTDS resource with a specific name
+update_resource: Update an existing OTDS resource
+activate_resource : Activate an OTDS resource
+
+get_access_roles : Get all OTDS Access Roles
+get_access_role: Get an OTDS Access Role with a specific name
+add_partition_to_access_role : Add an OTDS Partition to to an OTDS Access Role
+add_user_to_access_role : Add an OTDS user to to an OTDS Access Role
+add_group_to_access_role : Add an OTDS group to to an OTDS Access Role
+update_access_role_attributes: Update attributes of an existing access role
+
+add_system_attribute : Add an OTDS System Attribute
+
+get_trusted_sites : Get OTDS Trusted Sites
+add_trusted_site : Add a new trusted site to OTDS
+
+enable_audit: enable OTDS audit
+
+add_oauth_client : Add a new OAuth client to OTDS
+get_oauth_client : Get an OAuth client with a specific client ID
+update_oauth_client : Update an OAuth client
+add_oauth_clients_to_access_role : Add an OTDS OAuth Client to an OTDS Access Role
+get_access_token : Get an OTDS Access Token
+
+add_auth_handler_saml: Add an authentication handler for SAML (e.g. for SuccessFactors)
+add_auth_handler_sap: Add an authentication handler for SAP
+add_auth_handler_oauth: Add an authentication handler for OAuth (used for Salesforce)
 
 consolidate: Consolidate an OTDS resource
-impersonateResource: Configure impersonation for an OTDS resource
-impersonateOauth: Configure impersonation for an OTDS OAuth Client
+impersonate_resource: Configure impersonation for an OTDS resource
+impersonate_oauth_client: Configure impersonation for an OTDS OAuth Client
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler", "Jim Bennett"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
-import requests
 import json
 import base64
+import requests
 
-logger = logging.getLogger("pyxecm.otpd")
+logger = logging.getLogger("pyxecm.otds")
 
-requestHeaders = {
+REQUEST_HEADERS = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
-requestFormHeaders = {
+REQUEST_FORM_HEADERS = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/x-www-form-urlencoded",
 }
 
 
 class OTDS:
     """Used to automate stettings in OpenText Directory Services (OTDS)."""
 
     _config = None
     _cookie = None
 
     def __init__(
-        self, protocol: str, hostname: str, port: int, username: str, password: str
+        self,
+        protocol: str,
+        hostname: str,
+        port: int,
+        username: str,
+        password: str,
+        **kwargs,
     ):
         """Initialize the OTDS object
 
         Args:
             protocol (string): either http or https
             hostname (string): hostname of otds
             port (integer): port number - typically 80 or 443
             username (type): otds user name
             password (type): otds password
+            **kwargs
         """
 
         # Initialize otdsConfig as an empty dictionary
-        otdsConfig = {}
+        otds_config = {}
 
         if hostname:
-            otdsConfig["publicHostname"] = hostname
+            otds_config["publicHostname"] = hostname
         else:
-            otdsConfig["publicHostname"] = "otds"
+            otds_config["publicHostname"] = "otds"
 
         if protocol:
-            otdsConfig["protocol"] = protocol
+            otds_config["protocol"] = protocol
         else:
-            otdsConfig["protocol"] = "http"
+            otds_config["protocol"] = "http"
 
         if port:
-            otdsConfig["port"] = port
+            otds_config["port"] = port
         else:
-            otdsConfig["port"] = 80
+            otds_config["port"] = 80
 
         if username:
-            otdsConfig["username"] = username
+            otds_config["username"] = username
         else:
-            otdsConfig["username"] = "admin"
+            otds_config["username"] = "admin"
 
         if password:
-            otdsConfig["password"] = password
+            otds_config["password"] = password
         else:
-            otdsConfig["password"] = ""
+            otds_config["password"] = ""
 
-        otdsBaseUrl = protocol + "://" + otdsConfig["publicHostname"]
+        otdsBaseUrl = protocol + "://" + otds_config["publicHostname"]
         if str(port) not in ["80", "443"]:
             otdsBaseUrl += ":{}".format(port)
         otdsBaseUrl += "/otdsws"
-        otdsConfig["baseUrl"] = otdsBaseUrl
+        otds_config["baseUrl"] = otdsBaseUrl
 
         otdsRestUrl = otdsBaseUrl + "/rest"
-        otdsConfig["restUrl"] = otdsRestUrl
+        otds_config["restUrl"] = otdsRestUrl
 
-        otdsConfig["partitionUrl"] = otdsRestUrl + "/partitions"
-        otdsConfig["accessRoleUrl"] = otdsRestUrl + "/accessroles"
-        otdsConfig["credentialUrl"] = otdsRestUrl + "/authentication/credentials"
-        otdsConfig["oauthClientUrl"] = otdsRestUrl + "/oauthclients"
-        otdsConfig["tokenUrl"] = otdsBaseUrl + "/oauth2/token"
-        otdsConfig["resourceUrl"] = otdsRestUrl + "/resources"
-        otdsConfig["licenseUrl"] = otdsRestUrl + "/licensemanagement/licenses"
-        otdsConfig["usersUrl"] = otdsRestUrl + "/users"
-        otdsConfig["groupsUrl"] = otdsRestUrl + "/groups"
-        otdsConfig["systemConfigUrl"] = otdsRestUrl + "/systemconfig"
-        otdsConfig["authHandlerUrl"] = otdsRestUrl + "/authhandlers"
-        otdsConfig["consolidationUrl"] = otdsRestUrl + "/consolidation"
+        otds_config["partitionUrl"] = otdsRestUrl + "/partitions"
+        otds_config["accessRoleUrl"] = otdsRestUrl + "/accessroles"
+        otds_config["credentialUrl"] = otdsRestUrl + "/authentication/credentials"
+        otds_config["oauthClientUrl"] = otdsRestUrl + "/oauthclients"
+        otds_config["tokenUrl"] = otdsBaseUrl + "/oauth2/token"
+        otds_config["resourceUrl"] = otdsRestUrl + "/resources"
+        otds_config["licenseUrl"] = otdsRestUrl + "/licensemanagement/licenses"
+        otds_config["usersUrl"] = otdsRestUrl + "/users"
+        otds_config["groupsUrl"] = otdsRestUrl + "/groups"
+        otds_config["systemConfigUrl"] = otdsRestUrl + "/systemconfig"
+        otds_config["authHandlerUrl"] = otdsRestUrl + "/authhandlers"
+        otds_config["consolidationUrl"] = otdsRestUrl + "/consolidation"
 
-        self._config = otdsConfig
+        self._config = otds_config
 
-    def config(self):
+    def config(self) -> dict:
+        """Returns the configuration dictionary
+
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
-    def cookie(self):
+    def cookie(self) -> dict:
+        """Returns the login cookie of OTDS.
+           This is set by the authenticate() method
+
+        Returns:
+            dict: OTDS cookie
+        """
         return self._cookie
 
-    def credentials(self):
+    def credentials(self) -> dict:
+        """Returns the credentials (username + password)
+
+        Returns:
+            dict: dictionary with username and password
+        """
         return {
             "userName": self.config()["username"],
             "password": self.config()["password"],
         }
 
-    def baseUrl(self):
+    def base_url(self) -> str:
+        """Returns the base URL of OTDS
+
+        Returns:
+            string: base URL
+        """
         return self.config()["baseUrl"]
 
-    def restUrl(self):
+    def rest_url(self) -> str:
+        """Returns the REST URL of OTDS
+
+        Returns:
+            string: REST URL
+        """
         return self.config()["restUrl"]
 
-    def credentialUrl(self):
+    def credential_url(self) -> str:
+        """Returns the Credentials URL of OTDS
+
+        Returns:
+            string: Credentials URL
+        """
         return self.config()["credentialUrl"]
 
-    def authHandlerUrl(self):
+    def auth_handler_url(self) -> str:
+        """Returns the Auth Handler URL of OTDS
+
+        Returns:
+            string: Auth Handler URL
+        """
         return self.config()["authHandlerUrl"]
 
-    def partitionUrl(self):
+    def partition_url(self) -> str:
+        """Returns the Partition URL of OTDS
+
+        Returns:
+            string: Partition URL
+        """
         return self.config()["partitionUrl"]
 
-    def accessRoleUrl(self):
+    def access_role_url(self) -> str:
+        """Returns the Access Role URL of OTDS
+
+        Returns:
+            string: Access Role URL
+        """
         return self.config()["accessRoleUrl"]
 
-    def oauthClientUrl(self):
+    def oauth_client_url(self) -> str:
+        """Returns the OAuth Client URL of OTDS
+
+        Returns:
+            string: OAuth Client URL
+        """
         return self.config()["oauthClientUrl"]
 
-    def resourceUrl(self):
+    def resource_url(self) -> str:
+        """Returns the Resource URL of OTDS
+
+        Returns:
+            string: Resource URL
+        """
         return self.config()["resourceUrl"]
 
-    def licenseUrl(self):
+    def license_url(self) -> str:
+        """Returns the License URL of OTDS
+
+        Returns:
+            string: License URL
+        """
         return self.config()["licenseUrl"]
 
-    def tokenUrl(self):
+    def token_url(self) -> str:
+        """Returns the Token URL of OTDS
+
+        Returns:
+            string: Token URL
+        """
         return self.config()["tokenUrl"]
 
-    def usersUrl(self):
+    def users_url(self) -> str:
+        """Returns the Users URL of OTDS
+
+        Returns:
+            string: Users URL
+        """
         return self.config()["usersUrl"]
 
-    def groupsUrl(self):
+    def groups_url(self) -> str:
+        """Returns the Groups URL of OTDS
+
+        Returns:
+            string: Groups URL
+        """
         return self.config()["groupsUrl"]
 
-    def systemConfigUrl(self):
+    def system_config_url(self) -> str:
+        """Returns the System Config URL of OTDS
+
+        Returns:
+            string: System Config URL
+        """
         return self.config()["systemConfigUrl"]
 
-    def consolidationUrl(self):
+    def consolidation_url(self) -> str:
+        """Returns the Consolidation URL of OTDS
+
+        Returns:
+            string: Consolidation URL
+        """
         return self.config()["consolidationUrl"]
 
-    def parseRequestResponse(
+    def parse_request_response(
         self,
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
-    ) -> dict:
+    ) -> dict | None:
         """Converts the request response to a Python dict in a safe way
            that also handles exceptions.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
             additional_error_message (string): print a custom error message
             show_error (boolean): if True log an error, if False log a warning
@@ -269,15 +368,15 @@
                 logger.warning(message)
             return None
         else:
             return dict_object
 
     # end method definition
 
-    def authenticate(self, revalidate: bool = False) -> dict:
+    def authenticate(self, revalidate: bool = False) -> dict | None:
         """Authenticate at Directory Services and retrieve OTCS Ticket.
 
         Args:
             revalidate (boolean, optional): determine if a re-athentication is enforced
                                             (e.g. if session has timed out with 401 error)
         Returns:
             dictionary: Cookie information. Also stores cookie information in self._cookie
@@ -285,30 +384,30 @@
 
         # Already authenticated and session still valid?
         if self._cookie and not revalidate:
             return self._cookie
 
         otds_ticket = "NotSet"
 
-        logger.info("Requesting OTDS ticket from -> {}".format(self.credentialUrl()))
+        logger.info("Requesting OTDS ticket from -> {}".format(self.credential_url()))
 
         response = None
         try:
             response = requests.post(
-                self.credentialUrl(), json=self.credentials(), headers=requestHeaders
+                self.credential_url(), json=self.credentials(), headers=REQUEST_HEADERS
             )
         except Exception as e:
             logger.warning(
-                "Unable to connect to -> {} : {}".format(self.credentialUrl(), e)
+                "Unable to connect to -> {} : {}".format(self.credential_url(), e)
             )
             logger.warning("OTDS service may not be ready yet.")
             return None
 
         if response.ok:
-            authenticate_dict = self.parseRequestResponse(response)
+            authenticate_dict = self.parse_request_response(response)
             if not authenticate_dict:
                 return None
             else:
                 otds_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otds_ticket))
         else:
             logger.error(
@@ -317,22 +416,22 @@
             return None
 
         self._cookie = {"OTDSTicket": otds_ticket}
         return self._cookie
 
     # end method definition
 
-    def addLicenseToResource(
+    def add_license_to_resource(
         self,
         path_to_license_file: str,
         product_name: str,
         product_description: str,
         resource_id: str,
         update: bool = True,
-    ) -> dict:
+    ) -> dict | None:
         """Add a product license to an OTDS resource.
 
         Args:
             path_to_license_file (string): fully qualified filename of the license file
             product_name (string): product name
             product_description (string): product description
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
@@ -359,18 +458,18 @@
             "values": [
                 {"name": "oTLicenseFile", "values": license_content},
                 {"name": "oTLicenseResource", "values": resource_id},
                 {"name": "oTLicenseFingerprintGenerator", "values": [None]},
             ],
         }
 
-        request_url = self.licenseUrl()
+        request_url = self.license_url()
         # Check if we want to update an existing license:
         if update:
-            existing_license = self.getLicensesForResource(resource_id)
+            existing_license = self.get_license_for_resource(resource_id)
             if existing_license:
                 request_url += "/" + existing_license[0]["id"]
             else:
                 logger.info(
                     "No existing license for resource -> {} found - adding a new license...".format(
                         resource_id
                     )
@@ -387,27 +486,27 @@
         retries = 0
         while True:
             if update:
                 # Do a REST PUT call for update an existing license:
                 response = requests.put(
                     request_url,
                     json=licensePostBodyJson,
-                    headers=requestHeaders,
+                    headers=REQUEST_HEADERS,
                     cookies=self.cookie(),
                 )
             else:
                 # Do a REST POST call for creation of a new license:
                 response = requests.post(
                     request_url,
                     json=licensePostBodyJson,
-                    headers=requestHeaders,
+                    headers=REQUEST_HEADERS,
                     cookies=self.cookie(),
                 )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -418,43 +517,56 @@
                         response.status_code,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getLicensesForResource(self, resource_id: str):
+    def get_license_for_resource(self, resource_id: str):
         """Get a product license for a resource in OTDS.
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
         Returns:
             Licenses for a resource or None if the REST call fails
+
+        licenses have this format:
+        {
+          '_oTLicenseType': 'NON-PRODUCTION',
+          '_oTLicenseResource': '7382094f-a434-4714-9696-82864b6803da',
+          '_oTLicenseResourceName': 'cs',
+          '_oTLicenseProduct': 'EXTENDED_ECM',
+          'name': 'EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da',
+          'location': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+          'id': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+          'description': 'CS license',
+          'values': [{...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, ...]
+        }
         """
 
         request_url = (
-            self.licenseUrl()
+            self.license_url()
             + "/assignedlicenses?resourceID="
             + resource_id
             + "&validOnly=false"
         )
 
         logger.info(
             "Get license for resource -> {}; calling -> {}".format(
                 resource_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                response_dict = self.parseRequestResponse(response)
+                response_dict = self.parse_request_response(response)
                 if not response_dict:
                     return None
                 return response_dict["licenseObjects"]["_licenses"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -465,36 +577,36 @@
                         resource_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def deleteLicenseFromResource(self, resource_id: str, license_id: str) -> bool:
+    def delete_license_from_resource(self, resource_id: str, license_id: str) -> bool:
         """Delete a product license for a resource in OTDS.
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_id (string): OTDS license ID (this is the ID not the license name!)
         Returns:
             boolean: True if successful or False if the REST call fails
         """
 
-        request_url = "{}/{}".format(self.licenseUrl(), license_id)
+        request_url = "{}/{}".format(self.license_url(), license_id)
 
         logger.info(
             "Deleting product license -> {} from resource -> {}; calling -> {}".format(
                 license_id, resource_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.delete(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -505,15 +617,15 @@
                         license_id, resource_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def assignUserToLicense(
+    def assign_user_to_license(
         self,
         partition: str,
         user_id: str,
         resource_id: str,
         license_feature: str,
         license_name: str,
         license_type: str = "Full",
@@ -527,15 +639,15 @@
             license_feature (string): name of the license feature
             license_name (string): name of the license to assign
             license_type (string, optional): deault is "Full", Extended ECM also has "Occasional"
         Returns:
             boolean: True if successful or False if the REST call fails or the license is not found
         """
 
-        licenses = self.getLicensesForResource(resource_id)
+        licenses = self.get_license_for_resource(resource_id)
 
         for lic in licenses:
             if lic["_oTLicenseProduct"] == license_name:
                 license_location = lic["id"]
 
         try:
             license_location
@@ -543,42 +655,42 @@
             logger.error(
                 "Cannot find license -> {} for resource -> {}".format(
                     license_name, resource_id
                 )
             )
             return False
 
-        user = self.getUser(partition, user_id)
+        user = self.get_user(partition, user_id)
         if user:
-            userLocation = user["location"]
+            user_location = user["location"]
         else:
             logger.error("Cannot find location for user -> {}".format(user_id))
             return False
 
         licensePostBodyJson = {
             "_oTLicenseType": license_type,
             "_oTLicenseProduct": "users",
-            "name": userLocation,
+            "name": user_location,
             "values": [{"name": "counter", "values": [license_feature]}],
         }
 
-        request_url = self.licenseUrl() + "/object/" + license_location
+        request_url = self.license_url() + "/object/" + license_location
 
         logger.info(
             "Assign license feature -> {} of license -> {} associated with resource -> {} to user -> {}; calling -> {}".format(
                 license_feature, license_location, resource_id, user_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=licensePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 logger.info(
                     "Added license feature -> {} for user -> {}".format(
                         license_feature, user_id
                     )
@@ -599,15 +711,15 @@
                         response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
-    def assignPartitionToLicense(
+    def assign_partition_to_license(
         self,
         partition_name: str,
         resource_id: str,
         license_feature: str,
         license_name: str,
         license_type: str = "Full",
     ) -> bool:
@@ -619,15 +731,15 @@
             license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
             license_type (string, optional): deault is "Full", Extended ECM also has "Occasional"
         Returns:
             boolean: True if successful or False if the REST call fails or the license is not found
         """
 
-        licenses = self.getLicensesForResource(resource_id)
+        licenses = self.get_license_for_resource(resource_id)
         if not licenses:
             logger.error(
                 "Resource with ID -> {} does not exist or has no licenses".format(
                     resource_id
                 )
             )
             return False
@@ -661,15 +773,15 @@
         licensePostBodyJson = {
             "_oTLicenseType": license_type,
             "_oTLicenseProduct": "partitions",
             "name": partition_name,
             "values": [{"name": "counter", "values": [license_feature]}],
         }
 
-        request_url = self.licenseUrl() + "/object/" + license_location
+        request_url = self.license_url() + "/object/" + license_location
 
         logger.info(
             "Assign license feature -> {} of license -> {} associated with resource -> {} to partition -> {}; calling -> {}".format(
                 license_feature,
                 license_location,
                 resource_id,
                 partition_name,
@@ -678,15 +790,15 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=licensePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 logger.info(
                     "Added license feature -> {} for partition -> {}".format(
                         license_feature, partition_name
                     )
@@ -707,20 +819,20 @@
                         response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
-    def getLicensedObjects(
+    def get_licensed_objects(
         self,
         resource_id: str,
         license_feature: str,
         license_name: str,
-    ):
+    ) -> dict | None:
         """Return the licensed objects (users, groups, partitions) in OTDS for a license + license feature
            associated with an OTDS resource (like "cs").
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
@@ -736,15 +848,15 @@
                 'listGroupsResults': {'groups': [...], 'actualPageSize': 0, 'nextPageCookie': None, 'requestedPageSize': 250},
                 'listUsersResults': {'users': [...], 'actualPageSize': 53, 'nextPageCookie': None, 'requestedPageSize': 250},
                 'listUserPartitionResult': {'_userPartitions': [...], 'warningMessage': None, 'actualPageSize': 0, 'nextPageCookie': None, 'requestedPageSize': 250},
                 'version': 1
             }
         """
 
-        licenses = self.getLicensesForResource(resource_id)
+        licenses = self.get_license_for_resource(resource_id)
         if not licenses:
             logger.error(
                 "Resource with ID -> {} does not exist or has no licenses".format(
                     resource_id
                 )
             )
             return False
@@ -772,15 +884,15 @@
                 "Cannot find license -> {} for resource -> {}".format(
                     license_name, resource_id
                 )
             )
             return False
 
         request_url = (
-            self.licenseUrl()
+            self.license_url()
             + "/object/"
             + license_location
             + "?counter="
             + license_feature
         )
 
         logger.info(
@@ -792,19 +904,19 @@
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -816,174 +928,170 @@
                         response.status_code,
                     )
                 )
                 return None
 
     # end method definition
 
-    def isUserLicensed(self, user_name: str, resource_id: str, license_feature: str, license_name: str) -> bool:
+    def is_user_licensed(
+        self, user_name: str, resource_id: str, license_feature: str, license_name: str
+    ) -> bool:
         """Check if a user is licensed for a license and license feature associated with a particular OTDS resource.
 
         Args:
             user_name (str): login name of the OTDS user
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
 
         Returns:
             bool: True if the user is licensed and False otherwise
         """
 
-        response = self.getLicensedObjects(
+        response = self.get_licensed_objects(
             resource_id=resource_id,
             license_feature=license_feature,
             license_name=license_name,
         )
 
         if not response or not response["listUsersResults"]:
             return False
 
         users = response["listUsersResults"]["users"]
 
         if not users:
             return False
 
         user = next(
-            (
-                item
-                for item in users
-                if item["name"] == user_name
-            ),
+            (item for item in users if item["name"] == user_name),
             None,
         )
 
         if user:
             return True
-        
+
         return False
 
     # end method definition
 
-    def isGroupLicensed(self, group_name: str, resource_id: str, license_feature: str, license_name: str) -> bool:
+    def is_group_licensed(
+        self, group_name: str, resource_id: str, license_feature: str, license_name: str
+    ) -> bool:
         """Check if a group is licensed for a license and license feature associated with a particular OTDS resource.
 
         Args:
             group_name (str): name of the OTDS user group
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
 
         Returns:
             bool: True if the group is licensed and False otherwise
         """
 
-        response = self.getLicensedObjects(
+        response = self.get_licensed_objects(
             resource_id=resource_id,
             license_feature=license_feature,
             license_name=license_name,
         )
 
         if not response or not response["listGroupsResults"]:
             return False
 
         groups = response["listGroupsResults"]["groups"]
 
         if not groups:
             return False
 
         group = next(
-            (
-                item
-                for item in groups
-                if item["name"] == group_name
-            ),
+            (item for item in groups if item["name"] == group_name),
             None,
         )
 
         if group:
             return True
-        
+
         return False
 
     # end method definition
 
-    def isPartitionLicensed(
-        self, partition_name: str, resource_id: str, license_feature: str, license_name: str
-    ):
+    def is_partition_licensed(
+        self,
+        partition_name: str,
+        resource_id: str,
+        license_feature: str,
+        license_name: str,
+    ) -> bool:
         """Check if a user is licensed for a license and license feature associated with a particular OTDS resource.
 
         Args:
             partition_name (str): name of the OTDS user partition, e.g. "Content Server Members"
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
 
         Returns:
             bool: True if the partition is licensed and False otherwise
         """
 
-        response = self.getLicensedObjects(
+        response = self.get_licensed_objects(
             resource_id=resource_id,
             license_feature=license_feature,
             license_name=license_name,
         )
 
         if not response or not response["listUserPartitionResult"]:
             return False
 
         partitions = response["listUserPartitionResult"]["_userPartitions"]
 
         if not partitions:
             return False
 
         partition = next(
-            (
-                item
-                for item in partitions
-                if item["name"] == partition_name
-            ),
+            (item for item in partitions if item["name"] == partition_name),
             None,
         )
 
         if partition:
             return True
-        
+
         return False
 
     # end method definition
 
-    def addPartition(self, name: str, description: str) -> dict:
+    def add_partition(self, name: str, description: str) -> dict | None:
         """Add a new user partition to OTDS
 
         Args:
             name (string): name of the new partition
         Returns:
             dictionary: Request response or None if the creation fails.
         """
 
         partitionPostBodyJson = {"name": name, "description": description}
 
-        request_url = self.partitionUrl()
+        request_url = self.partition_url()
 
         logger.info(
             "Adding user partition -> {} ({}); calling -> {}".format(
                 name, description, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=partitionPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -991,15 +1099,15 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getPartition(self, name: str, show_error: bool = True) -> dict:
+    def get_partition(self, name: str, show_error: bool = True) -> dict | None:
         """Get an existing user partition from OTDS
 
         Args:
             name (string): name of the partition to retrieve
             show_error (boolean, optional): whether or not we want to log an error if partion is not found
         Returns:
             dictionary: Request response or None if the creation fails.
@@ -1010,18 +1118,18 @@
         logger.info(
             "Getting user partition -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -1030,23 +1138,23 @@
                             name, response.text, response.status_code
                         )
                     )
                 return None
 
     # end method definition
 
-    def addUser(
+    def add_user(
         self,
         partition: str,
         name: str,
         description: str = "",
         first_name: str = "",
         last_name: str = "",
         email: str = "",
-    ) -> dict:
+    ) -> dict | None:
         """Add a new user to a user partition in OTDS
 
         Args:
             partition (string): name of the OTDS user partition (needs to exist)
             name (string): login name of the new user
             description (string, optional): description of the new user
             first_name (string, optional): first name of the new user
@@ -1063,33 +1171,33 @@
                 {"name": "givenName", "values": [first_name]},
                 {"name": "mail", "values": [email]},
             ],
             "name": name,
             "description": description,
         }
 
-        request_url = self.usersUrl()
+        request_url = self.users_url()
 
         logger.info(
             "Adding user -> {} to partition -> {}; calling -> {}".format(
                 name, partition, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userPostBodyJson))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=userPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1097,39 +1205,39 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getUser(self, partition: str, user_id: str) -> dict:
+    def get_user(self, partition: str, user_id: str) -> dict:
         """Get a user by its partition and user ID
 
         Args:
             partition (string): name of the partition
             user_id (string): ID of the user (= login name)
         Returns:
             dictionary: Request response or None if the user was not found.
         """
 
-        request_url = self.usersUrl() + "/" + user_id + "@" + partition
+        request_url = self.users_url() + "/" + user_id + "@" + partition
 
         logger.info(
             "Get user -> {} in partition -> {}; calling -> {}".format(
                 user_id, partition, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1137,15 +1245,15 @@
                         user_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUser(
+    def update_user(
         self, partition: str, user_id: str, attribute_name: str, attribute_value: str
     ) -> dict:
         """Update a user attribute with a new value
 
         Args:
             partition (string): name of the partition
             user_id (string): ID of the user (= login name)
@@ -1156,32 +1264,32 @@
         """
 
         userPatchBodyJson = {
             "userPartitionID": partition,
             "values": [{"name": attribute_name, "values": [attribute_value]}],
         }
 
-        request_url = self.usersUrl() + "/" + user_id
+        request_url = self.users_url() + "/" + user_id
 
         logger.info(
             "Update user -> {} attribute -> {} to value -> {}; calling -> {}".format(
                 user_id, attribute_name, attribute_value, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.patch(
                 request_url,
                 json=userPatchBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1189,36 +1297,36 @@
                         user_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def deleteUser(self, partition: str, user_id: str) -> bool:
+    def delete_user(self, partition: str, user_id: str) -> bool:
         """Delete an existing user
 
         Args:
             partition (string): name of the partition
             user_id (string): Id (= login name) of the user
         Returns:
             Boolean: True = success, False = error
         """
 
-        request_url = self.usersUrl() + "/" + user_id + "@" + partition
+        request_url = self.users_url() + "/" + user_id + "@" + partition
 
         logger.info(
             "Delete user -> {} in partition -> {}; calling -> {}".format(
                 user_id, partition, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.delete(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -1229,40 +1337,40 @@
                         user_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def resetUserPassword(self, user_id: str, password: str) -> bool:
+    def reset_user_password(self, user_id: str, password: str) -> bool:
         """Reset a password of an existing user
 
         Args:
             user_id (string): Id (= login name) of the user
             password (string): new password of the user
         Returns:
             boolean: True = success, False = error.
         """
 
         userPostBodyJson = {"newPassword": password}
 
-        request_url = "{}/{}/password".format(self.usersUrl(), user_id)
+        request_url = "{}/{}/password".format(self.users_url(), user_id)
 
         logger.info(
             "Resetting password for user -> {}; calling -> {}".format(
                 user_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.put(
                 request_url,
                 json=userPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -1274,15 +1382,15 @@
                         user_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroup(self, partition: str, name: str, description: str) -> dict:
+    def add_group(self, partition: str, name: str, description: str) -> dict | None:
         """Add a new user group to a user partition in OTDS
 
         Args:
             partition (string): name of the OTDS user partition (needs to exist)
             name (string): name of the new group
             description (string): description of the new group
         Returns:
@@ -1291,33 +1399,33 @@
 
         groupPostBodyJson = {
             "userPartitionID": partition,
             "name": name,
             "description": description,
         }
 
-        request_url = self.groupsUrl()
+        request_url = self.groups_url()
 
         logger.info(
             "Adding group -> {} to partition -> {}; calling -> {}".format(
                 name, partition, request_url
             )
         )
         logger.info("Group Attributes -> {}".format(groupPostBodyJson))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=groupPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1325,15 +1433,15 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroup(self, group: str) -> dict:
+    def get_group(self, group: str) -> dict | None:
         """Get a OTDS group by its group name
 
         Args:
             group (string): ID of the group (= group name)
         Return:
             dictionary: Request response or None if the group was not found.
             Example values:
@@ -1350,25 +1458,25 @@
                 'customAttributes': None,
                 'originUUID': None,
                 'urlId': 'Sales@Content Server Members',
                 'urlLocation': 'oTGroup=3f921294-b92a-4c9e-bf7c-b50df16bb937,orgunit=groups,partition=Content Server Members,dc=identity,dc=opentext,dc=net'
             }
         """
 
-        request_url = self.groupsUrl() + "/" + group
+        request_url = self.groups_url() + "/" + group
 
         logger.info("Get group -> {}; calling -> {}".format(group, request_url))
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1376,40 +1484,40 @@
                         group, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addUserToGroup(self, user: str, group: str) -> bool:
+    def add_user_to_group(self, user: str, group: str) -> bool:
         """Add an existing user to an existing group in OTDS
 
         Args:
             user (string): name of the OTDS user (needs to exist)
             group (string): name of the OTDS group (needs to exist)
         Returns:
             boolean: Request return code.
         """
 
         userToGroupPostBodyJson = {"stringList": [group]}
 
-        request_url = self.usersUrl() + "/" + user + "/memberof"
+        request_url = self.users_url() + "/" + user + "/memberof"
 
         logger.info(
             "Adding user -> {} to group -> {}; calling -> {}".format(
                 user, group, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=userToGroupPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -1421,40 +1529,40 @@
                         user, group, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroupToParentGroup(self, group: str, parent_group: str) -> bool:
+    def add_group_to_parent_group(self, group: str, parent_group: str) -> bool:
         """Add an existing group to an existing parent group in OTDS
 
         Args:
             group (string): name of the OTDS group (needs to exist)
             parent_group (string): name of the OTDS parent group (needs to exist)
         Returns:
             boolean: Request return code.
         """
 
         groupToParentGroupPostBodyJson = {"stringList": [parent_group]}
 
-        request_url = self.groupsUrl() + "/" + group + "/memberof"
+        request_url = self.groups_url() + "/" + group + "/memberof"
 
         logger.info(
             "Adding group -> {} to parent group -> {}; calling -> {}".format(
                 group, parent_group, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=groupToParentGroupPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
 
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
@@ -1467,21 +1575,21 @@
                         group, parent_group, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addResource(
+    def add_resource(
         self,
         name: str,
         description: str,
         display_name: str,
         additional_payload: dict = {},
-    ) -> dict:
+    ) -> dict | None:
         """Add an OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
             description (string): description of the new OTDS resource
             display_name (string): display name of the OTDS resource
             additional_payload (dictionary, optional): additional values for the json payload
@@ -1509,19 +1617,19 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=resourcePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1529,15 +1637,15 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getResource(self, name: str, show_error: bool = False) -> dict:
+    def get_resource(self, name: str, show_error: bool = False) -> dict | None:
         """Get an existing OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
             show_error (boolean, optional): treat as error if resource is not found
         Returns:
             dictionary: Request response or None if the REST call fails.
@@ -1548,18 +1656,18 @@
         logger.info(
             "Retrieving resource -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 # We don't necessarily want to log an error as this function
@@ -1572,41 +1680,41 @@
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def updateResource(
+    def update_resource(
         self, name: str, resource: object, show_error: bool = True
-    ) -> dict:
+    ) -> dict | None:
         """Update an existing OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
-            resource (object): updated resource object of getResource called before
+            resource (object): updated resource object of get_resource called before
             show_error (boolean, optional): treat as error if resource is not found
         Returns:
             dictionary: Request response (json) or None if the REST call fails.
         """
 
         request_url = "{}/{}".format(self.config()["resourceUrl"], name)
 
         logger.info("Updating resource -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
             response = requests.put(
                 request_url,
                 json=resource,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 # We don't necessarily want to log an error as this function
@@ -1619,15 +1727,15 @@
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def activateResource(self, resource_id: str) -> dict:
+    def activate_resource(self, resource_id: str) -> dict | None:
         """Activate an OTDS resource
 
         Args:
             resource_id (string): ID of the OTDS resource
         Returns:
             dictionary: Request response (json) or None if the REST call fails.
         """
@@ -1641,19 +1749,19 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=resourcePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1661,33 +1769,33 @@
                         resource_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getAccessRoles(self) -> dict:
+    def get_access_roles(self) -> dict | None:
         """Get a list of all OTDS access roles
 
         Args: None
         Returns:
             dictionary: Request response or None if the REST call fails.
         """
 
         request_url = self.config()["accessRoleUrl"]
 
         logger.info("Retrieving access roles; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1695,15 +1803,15 @@
                         response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getAccessRole(self, name: str) -> dict:
+    def get_access_role(self, name: str) -> dict | None:
         """Get an OTDS access role
 
         Args:
             name (string): name of the access role
         Returns:
             dictionary: Request response (json) or None if the REST call fails.
         """
@@ -1713,18 +1821,18 @@
         logger.info(
             "Retrieving access role -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1732,15 +1840,15 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addPartitionToAccessRole(
+    def add_partition_to_access_role(
         self, access_role: str, partition: str, location: str = ""
     ) -> bool:
         """Add an OTDS partition to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             partition (string): name of the partition
@@ -1766,15 +1874,15 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=accessRolePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -1785,15 +1893,15 @@
                         partition, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addUserToAccessRole(
+    def add_user_to_access_role(
         self, access_role: str, user_id: str, location: str = ""
     ) -> bool:
         """Add an OTDS user to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             user_id (string): ID of the user (= login name)
@@ -1801,15 +1909,15 @@
                                          most of the times you will want to keep it to empty string ("")
         Returns:
             boolean: True if user is in access role or has been successfully added.
                      False if user has been not been added (error)
         """
 
         # get existing members to check if user is already a member:
-        accessRolesGetResponse = self.getAccessRole(access_role)
+        accessRolesGetResponse = self.get_access_role(access_role)
 
         if not accessRolesGetResponse:
             return False
 
         # Checking if user already added to access role
         accessRoleUsers = accessRolesGetResponse["accessRoleMembers"]["users"]
         for user in accessRoleUsers:
@@ -1841,15 +1949,15 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=accessRolePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -1860,15 +1968,15 @@
                         user_id, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroupToAccessRole(
+    def add_group_to_access_role(
         self, access_role: str, group: str, location: str = ""
     ) -> bool:
         """Add an OTDS group to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             group (string): name of the group
@@ -1876,15 +1984,15 @@
                                          most of the times you will want to keep it to empty string ("")
         Returns:
             boolean: True if group is in access role or has been successfully added.
                      False if group has been not been added (error)
         """
 
         # get existing members to check if user is already a member:
-        accessRolesGetResponse = self.getAccessRole(access_role)
+        accessRolesGetResponse = self.get_access_role(access_role)
         if not accessRolesGetResponse:
             return False
 
         # Checking if group already added to access role
         accessRoleGroups = accessRolesGetResponse["accessRoleMembers"]["groups"]
         for accessRoleGroup in accessRoleGroups:
             if accessRoleGroup["name"] == group:
@@ -1915,15 +2023,15 @@
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=accessRolePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -1934,15 +2042,17 @@
                         group, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def updateAccessRoleAttributes(self, name: str, attribute_list: list) -> dict:
+    def update_access_role_attributes(
+        self, name: str, attribute_list: list
+    ) -> dict | None:
         """Update some attributes of an existing OTDS Access Role
 
         Args:
             name (string): name of the existing access role
             attribute_list (list): list of attribute name and attribute value pairs
                                    The values need to be a list as well. Example:
                                    [{name: "pushAllGroups", values: ["True"]}]
@@ -1951,15 +2061,15 @@
         """
 
         # Return if list is empty:
         if not attribute_list:
             return None
 
         # create payload for REST call:
-        access_role = self.getAccessRole(name)
+        access_role = self.get_access_role(name)
         if not access_role:
             logger.error("Failed to get access role -> {}".format(name))
             return None
 
         accessRolePutBodyJson = {"attributes": attribute_list}
 
         request_url = "{}/{}/attributes".format(self.config()["accessRoleUrl"], name)
@@ -1971,19 +2081,19 @@
         )
 
         retries = 0
         while True:
             response = requests.put(
                 request_url,
                 json=accessRolePutBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -1991,15 +2101,17 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addSystemAttribute(self, name: str, value: str, description: str = "") -> dict:
+    def add_system_attribute(
+        self, name: str, value: str, description: str = ""
+    ) -> dict | None:
         """Add a new system attribute to OTDS
 
         Args:
             name (string): name of the new system attribute
             value (string): value of the system attribute
             description (string, optional): optional description of the system attribute
         Returns:
@@ -2028,19 +2140,19 @@
             )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=systemAttributePostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2048,15 +2160,15 @@
                         name, value, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getTrustedSites(self) -> dict:
+    def get_trusted_sites(self) -> dict | None:
         """Get all configured OTDS trusted sites
 
         Args:
             None
         Returns:
             dictionary: Request response or None if the REST call fails.
         """
@@ -2064,18 +2176,18 @@
         request_url = "{}/whitelist".format(self.config()["systemConfigUrl"])
 
         logger.info("Retrieving trusted sites; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2083,28 +2195,28 @@
                         response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addTrustedSite(self, trusted_site: str) -> dict:
+    def add_trusted_site(self, trusted_site: str) -> dict | None:
         """Add a new OTDS trusted site
 
         Args:
             trusted_site (string): name of the new trusted site
         Return:
             dictionary: Request response or None if the REST call fails.
         """
 
         trustedSitePostBodyJson = {"stringList": [trusted_site]}
 
         # we need to first retrieve the existing sites and then
         # append the new one:
-        existingTrustedSites = self.getTrustedSites()
+        existingTrustedSites = self.get_trusted_sites()
 
         if existingTrustedSites:
             trustedSitePostBodyJson["stringList"].extend(
                 existingTrustedSites["stringList"]
             )
 
         request_url = "{}/whitelist".format(self.config()["systemConfigUrl"])
@@ -2112,30 +2224,30 @@
         logger.info(
             "Add trusted site -> {}; calling -> {}".format(trusted_site, request_url)
         )
 
         response = requests.put(
             request_url,
             json=trustedSitePostBodyJson,
-            headers=requestHeaders,
+            headers=REQUEST_HEADERS,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
                 "Failed to add trusted site -> {}; error -> {} ({})".format(
                     trusted_site, response.text, response.status_code
                 )
             )
             return None
         return response  # don't parse it!
 
     # end method definition
 
-    def enableAudit(self):
-        """enable Audit
+    def enable_audit(self):
+        """enable OTDS Audit
 
         Args:
             None
         Return:
             Request response (json) or None if the REST call fails.
         """
 
@@ -2197,38 +2309,38 @@
         request_url = "{}/audit".format(self.config()["systemConfigUrl"])
 
         logger.info("Enable audit; calling -> {}".format(request_url))
 
         response = requests.put(
             request_url,
             json=auditPutBodyJson,
-            headers=requestHeaders,
+            headers=REQUEST_HEADERS,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
                 "Failed to enable audit; error -> {} ({})".format(
                     response.text, response.status_code
                 )
             )
         return response
 
     # end method definition
 
-    def addOauthClient(
+    def add_oauth_client(
         self,
         client_id: str,
         description: str,
         redirect_urls: list = [],
         allow_impersonation: bool = True,
         confidential: bool = True,
         auth_scopes: list = [],  # empty list = "Global"
         allowed_scopes: list = [],  # in OTDS UI: Permissible scopes
         default_scopes: list = [],  # in OTDS UI: Default scopes
-    ) -> dict:
+    ) -> dict | None:
         """Add a new OAuth client to OTDS
 
         Args:
             client_id (string): name of the new OAuth client (should not have blanks)
             description (string): description of the OAuth client
             redirect_urls (list): list of redirect URLs (strings)
             allow_impersonation (boolean, optional): allow impresonation
@@ -2252,32 +2364,32 @@
             "useSessionRefreshTokenLifeTime": True,
             "confidential": confidential,
             "authScopes": auth_scopes,
             "allowedScopes": allowed_scopes,
             "defaultScopes": default_scopes,
         }
 
-        request_url = self.oauthClientUrl()
+        request_url = self.oauth_client_url()
 
         logger.info(
             "Adding oauth client -> {} ({}); calling -> {}".format(
                 description, client_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=oauthClientPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2285,37 +2397,37 @@
                         client_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def getOauthClient(self, client_id: str, show_error: bool = True):
+    def get_oauth_client(self, client_id: str, show_error: bool = True) -> dict | None:
         """Get an existing OAuth client from OTDS
 
         Args:
             client_id (string): name (= ID) of the OAuth client to retrieve
             show_error (boolean): whether or not we want to log an error if partion is not found
         Returns:
             Request response (json) or None if the client is not found.
         """
 
-        request_url = "{}/{}".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}".format(self.oauth_client_url(), client_id)
 
         logger.info(
             "Get oauth client -> {}; calling -> {}".format(client_id, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
-                request_url, headers=requestHeaders, cookies=self.cookie()
+                request_url, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
@@ -2324,35 +2436,46 @@
                             client_id, response.text, response.status_code
                         )
                     )
                 return None
 
     # end method definition
 
-    def updateOauthClient(self, client_id, updates: dict):
+    def update_oauth_client(self, client_id: str, updates: dict) -> dict | None:
+        """Updates the OAuth client with new values
+
+        Args:
+            client_id (str): name (= ID) of the OAuth client
+            updates (dict): new values for OAuth client, e.g.
+                            {"description": "this is the new value"}
+
+        Returns:
+            dict: Request response (json) or None if the REST call fails.
+        """
+
         oauthClientPatchBodyJson = updates
 
-        request_url = "{}/{}".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}".format(self.oauth_client_url(), client_id)
 
         logger.info(
             "Update OAuth client -> {} with -> {}; calling -> {}".format(
                 client_id, updates, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.patch(
                 request_url,
                 json=oauthClientPatchBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2360,15 +2483,15 @@
                         client_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addOauthClientsToAccessRole(self, access_role_name: str):
+    def add_oauth_clients_to_access_role(self, access_role_name: str):
         """Add Oauth clients user partion to an OTDS Access Role
 
         Args:
             access_role_name (string): name of the OTDS Access Role
         Returns:
             response of REST call or None in case of an error
         """
@@ -2380,18 +2503,18 @@
                 access_role_name, accessRolesUrl
             )
         )
 
         retries = 0
         while True:
             response = requests.get(
-                accessRolesUrl, headers=requestHeaders, cookies=self.cookie()
+                accessRolesUrl, headers=REQUEST_HEADERS, cookies=self.cookie()
             )
             if response.ok:
-                accessRolesJson = self.parseRequestResponse(response)
+                accessRolesJson = self.parse_request_response(response)
                 break
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
@@ -2416,18 +2539,18 @@
                 )
                 return None
 
         # Getting location info for the OAuthClients partition
         # so it can be added to access roles json
         oauthPartitionsUrl = self.config()["partitionsUrl"] + "/OAuthClients"
         partitionsResponse = requests.get(
-            oauthPartitionsUrl, headers=requestHeaders, cookies=self.cookie()
+            oauthPartitionsUrl, headers=REQUEST_HEADERS, cookies=self.cookie()
         )
         if partitionsResponse.ok:
-            response_dict = self.parseRequestResponse(partitionsResponse)
+            response_dict = self.parse_request_response(partitionsResponse)
             if not response_dict:
                 return None
             oauthClientLocation = response_dict["location"]
         else:
             logger.error(
                 "Failed to get partition info for OAuthClients; url -> {} : error -> {} ({})".format(
                     oauthPartitionsUrl, partitionsResponse.text, response.status_code
@@ -2444,15 +2567,15 @@
         accessRolesJson["accessRoleMembers"]["organizationalUnits"].append(
             oauthClientsOuBlock
         )
 
         response = requests.put(
             accessRolesUrl,
             json=accessRolesJson,
-            headers=requestHeaders,
+            headers=REQUEST_HEADERS,
             cookies=self.cookie(),
         )
 
         if response.ok:
             logger.info(
                 "OauthClients partition successfully added to access role -> {}".format(
                     access_role_name
@@ -2466,49 +2589,62 @@
                     response.text,
                 )
             )
         return response
 
     # end method definition
 
-    def getAccessToken(self, client_id, client_secret):
-        encodedClientSecret = "{}:{}".format(client_id, client_secret).encode("utf-8")
+    def get_access_token(self, client_id: str, client_secret: str) -> str | None:
+        """Get the access token
+
+        Args:
+            client_id (str): OAuth client name (= ID)
+            client_secret (str): OAuth client secret. This is typically returned
+                                 by add_oauth_client() method in ["secret"] field
+
+        Returns:
+            string: access token, or None
+        """
+
+        encoded_client_secret = "{}:{}".format(client_id, client_secret).encode("utf-8")
         accessTokenRequestHeaders = {
             "Authorization": "Basic "
-            + base64.b64encode(encodedClientSecret).decode("utf-8"),
+            + base64.b64encode(encoded_client_secret).decode("utf-8"),
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
-        request_url = self.tokenUrl()
+        request_url = self.token_url()
 
         response = requests.post(
             request_url,
             data={"grant_type": "client_credentials"},
             headers=accessTokenRequestHeaders,
         )
 
         accessToken = None
         if response.ok:
-            accessTokenJson = self.parseRequestResponse(response)
+            accessTokenJson = self.parse_request_response(response)
 
             if "access_token" in accessTokenJson:
                 accessToken = accessTokenJson["access_token"]
+            else:
+                return None
 
         return accessToken
 
     # end method definition
 
-    def addAuthHandlerSAML(
+    def add_auth_handler_saml(
         self,
         name: str,
         description: str,
         provider_name: str,
         saml_url: str,
         otds_url: str,
-    ):
+    ) -> dict | None:
         """Add a new SAML authentication handler
 
         Args:
             name (string): name of the new authentication handler
             description (string): description of the new authentication handler
             provider_name (string): description of the new authentication handler
             saml_url (string): SAML URL
@@ -2590,32 +2726,32 @@
                     "_name": "Auth Response Binding",
                     "_description": "Specifies the SAML binding to use for the response to an AuthnRequest",
                     "_value": "urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST",
                 },
             ],
         }
 
-        request_url = self.authHandlerUrl()
+        request_url = self.auth_handler_url()
 
         logger.info(
             "Adding SAML auth handler -> {} ({}); calling -> {}".format(
                 name, description, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=authHandlerPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -2623,15 +2759,15 @@
                         name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
-    def addAuthHandlerSAP(
+    def add_auth_handler_sap(
         self,
         name: str,
         description: str,
         certificate_file: str,
         certificate_password: str,
     ):
         """Add a new SAP authentication handler
@@ -2696,26 +2832,26 @@
                     "_confidential": True,
                     "_keepOriginal": False,
                 },
             ],
         }
 
         # 2. Create the auth handler in OTDS
-        request_url = self.authHandlerUrl()
+        request_url = self.auth_handler_url()
 
         logger.info(
             "Adding SAP auth handler -> {} ({}); calling -> {}".format(
                 name, description, request_url
             )
         )
 
         response = requests.post(
             request_url,
             json=authHandlerPostBodyJson,
-            headers=requestHeaders,
+            headers=REQUEST_HEADERS,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
                 "Failed to add SAP auth handler -> {}; error -> {} ({})".format(
                     name, response.text, response.status_code
                 )
@@ -2790,15 +2926,15 @@
             "file1": (
                 os.path.basename(certificate_file),
                 open(certificate_file, "rb"),
                 "application/octet-stream",
             )
         }
 
-        request_url = self.authHandlerUrl() + "/" + name + "/files"
+        request_url = self.auth_handler_url() + "/" + name + "/files"
 
         logger.info(
             "Uploading certificate file -> {} for SAP auth handler -> {} ({}); calling -> {}".format(
                 certificate_file, name, description, request_url
             )
         )
 
@@ -2819,15 +2955,15 @@
             )
             return None
 
         return response
 
     # end method definition
 
-    def addAuthHandlerOAuth(
+    def add_auth_handler_oauth(
         self,
         name: str,
         description: str,
         provider_name: str,
         client_id: str,
         client_secret: str,
         active_by_default: bool = False,
@@ -3189,32 +3325,32 @@
                     "_allowedValues": None,
                     "_confidential": False,
                     "_keepOriginal": False,
                 },
             ],
         }
 
-        request_url = self.authHandlerUrl()
+        request_url = self.auth_handler_url()
 
         logger.info(
             "Adding OAuth auth handler -> {} ({}); calling -> {}".format(
                 name, description, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=authHandlerPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return self.parseRequestResponse(response)
+                return self.parse_request_response(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
@@ -3231,49 +3367,47 @@
 
         Args:
             resource_name (string): resource to be consolidated
         Returns:
             boolean: True if the consolidation succeeded or False if it failed.
         """
 
-        resource = self.getResource(resource_name)
+        resource = self.get_resource(resource_name)
         if not resource:
             logger.error(
-                "Resource -> {} not found - cannot consolidate; error -> {} ({})".format(
-                    resource_name, response.text, response.status_code
-                )
+                "Resource -> {} not found - cannot consolidate".format(resource_name)
             )
             return False
 
-        resourceDN = resource["resourceDN"]
-        if not resourceDN:
+        resource_dn = resource["resourceDN"]
+        if not resource_dn:
             logger.error("Resource DN is empty - cannot consolidate")
             return False
 
         consolidationPostBodyJson = {
             "cleanupUsersInResource": False,
             "cleanupGroupsInResource": False,
-            "resourceList": [resourceDN],
-            "objectToConsolidate": resourceDN,
+            "resourceList": [resource_dn],
+            "objectToConsolidate": resource_dn,
         }
 
-        request_url = "{}".format(self.consolidationUrl())
+        request_url = "{}".format(self.consolidation_url())
 
         logger.info(
             "Consolidation of resource -> {}; calling -> {}".format(
-                resourceDN, request_url
+                resource_dn, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=consolidationPostBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -3285,15 +3419,15 @@
                         response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def impersonateResource(
+    def impersonate_resource(
         self,
         resource_name: str,
         allow_impersonation: bool = True,
         impersonation_list: list = [],
     ) -> bool:
         """Configure impersonation for an OTDS resource
 
@@ -3306,28 +3440,28 @@
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
-        request_url = "{}/{}/impersonation".format(self.resourceUrl(), resource_name)
+        request_url = "{}/{}/impersonation".format(self.resource_url(), resource_name)
 
         logger.info(
             "Impersonation settings for resource -> {}; calling -> {}".format(
                 resource_name, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.put(
                 request_url,
                 json=impersonationPutBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
@@ -3339,15 +3473,15 @@
                         resource_name, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def impersonateOauthClient(
+    def impersonate_oauth_client(
         self,
         client_id: str,
         allow_impersonation: bool = True,
         impersonation_list: list = [],
     ) -> bool:
         """Configure impersonation for an OTDS OAuth Client
 
@@ -3360,28 +3494,28 @@
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
-        request_url = "{}/{}/impersonation".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}/impersonation".format(self.oauth_client_url(), client_id)
 
         logger.info(
             "Impersonation settings for OAuth Client -> {}; calling -> {}".format(
                 client_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.put(
                 request_url,
                 json=impersonationPutBodyJson,
-                headers=requestHeaders,
+                headers=REQUEST_HEADERS,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
```

### Comparing `pyxecm-0.2.0/pyxecm/otiv.py` & `pyxecm-0.3.0/pyxecm/otiv.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
-import os
 import logging
 
 logger = logging.getLogger("pyxecm.otiv")
 
 
 class OTIV:
     """Used to manage stettings for OpenText Intelligent Viewing."""
@@ -29,34 +28,41 @@
     def __init__(
         self,
         resource_name: str,
         product_name: str,
         product_description: str,
         license_file: str,
         default_license: str = "FULLTIME_USERS_REGULAR",
+        **kwargs,
     ):
         """Initialize the OTIV class for Intelligent Viewing
 
         Args:
             resource_name (string): OTDS resource name
             product_name (string): OTDS product name for licensing
             license_file (string): path to license file
             default_license (string, optional): Defaults to "FULLTIME_USERS_REGULAR".
+            **kwargs
         """
 
-        # Initialize otcsConfig as an empty dictionary
-        otcsConfig = {}
+        # Initialize otiv_config as an empty dictionary
+        otiv_config = {}
 
-        otcsConfig["resource"] = resource_name
-        otcsConfig["product"] = product_name
-        otcsConfig["description"] = product_description
-        otcsConfig["license_file"] = license_file
-        otcsConfig["license"] = default_license
+        otiv_config["resource"] = resource_name
+        otiv_config["product"] = product_name
+        otiv_config["description"] = product_description
+        otiv_config["license_file"] = license_file
+        otiv_config["license"] = default_license
 
-        self._config = otcsConfig
+        self._config = otiv_config
 
     # end method definition
 
-    def config(self):
+    def config(self) -> dict:
+        """Returns the configuration dictionary
+
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
     # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/otpd.py` & `pyxecm-0.3.0/pyxecm/otpd.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,42 @@
 OTPD Module to implement functions to read / write PowerDocs objects
 
 Class: OTPD
 Methods:
 
 __init__ : class initializer
 config : returns config data set
-importDatabase: imports the PowerDocs database from a zip file
-applySetting: apply a setting to a PowerDocs tenant
+credentials: Get credentials (username and password)
+set_credentials: Set new credentials
+hostname: Get the configured PowerDocs hostname
+set_hostname: Set the hostname of PowerDocs
+base_url : Get PowerDocs base URL
+rest_url : Get PowerDocs REST base URL
+
+parse_request_response: Converts the text property of a request
+                        response object to a Python dict in a safe way
+
+authenticate : Authenticates at PowerDocs and retrieve OTCS Ticket.
+
+import_database: imports the PowerDocs database from a zip file
+apply_setting: apply a setting to a PowerDocs tenant
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import json
+import logging
 import requests
 from requests.auth import HTTPBasicAuth
 from requests_toolbelt.multipart.encoder import MultipartEncoder
-import os
-import logging
 
 logger = logging.getLogger("pyxecm.otpd")
 
 requestHeaders = {
     "accept": "application/json;charset=utf-8",
     "Connection": "keep-alive",
     "Content-Type": "application/json",
@@ -36,106 +47,142 @@
 class OTPD:
     """Used to automate stettings in OpenText Extended ECM PowerDocs."""
 
     _config = None
     _jsessionid = None
 
     def __init__(
-        self, protocol: str, hostname: str, port: int, username: str, password: str
+        self,
+        protocol: str,
+        hostname: str,
+        port: int,
+        username: str,
+        password: str,
+        **kwargs
     ):
         """Initialize the OTPD object
 
         Args:
             protocol (string): Either http or https.
             hostname (string): The hostname of the PowerDocs Server Manager to communicate with.
             port (integer): The port number used to talk to the PowerDocs Server Manager.
             username (string): The admin user name of PowerDocs Server Manager.
             password (string): The admin password of PowerDocs Server Manager.
+            **kwargs
         """
 
-        otpdConfig = {}
+        otpd_config = {}
 
         if hostname:
-            otpdConfig["hostname"] = hostname
+            otpd_config["hostname"] = hostname
         else:
-            otpdConfig["hostname"] = ""
+            otpd_config["hostname"] = ""
 
         if protocol:
-            otpdConfig["protocol"] = protocol
+            otpd_config["protocol"] = protocol
         else:
-            otpdConfig["protocol"] = "http"
+            otpd_config["protocol"] = "http"
 
         if port:
-            otpdConfig["port"] = port
+            otpd_config["port"] = port
         else:
-            otpdConfig["port"] = 80
+            otpd_config["port"] = 80
 
         if username:
-            otpdConfig["username"] = username
+            otpd_config["username"] = username
         else:
-            otpdConfig["username"] = "admin"
+            otpd_config["username"] = "admin"
 
         if password:
-            otpdConfig["password"] = password
+            otpd_config["password"] = password
         else:
-            otpdConfig["password"] = ""
+            otpd_config["password"] = ""
 
-        otpdBaseUrl = protocol + "://" + otpdConfig["hostname"]
+        otpd_base_url = protocol + "://" + otpd_config["hostname"]
         if str(port) not in ["80", "443"]:
-            otpdBaseUrl += ":{}".format(port)
-        otpdBaseUrl += "/ServerManager"
-        otpdConfig["baseUrl"] = otpdBaseUrl
+            otpd_base_url += ":{}".format(port)
+        otpd_base_url += "/ServerManager"
+        otpd_config["baseUrl"] = otpd_base_url
+
+        otpd_rest_url = otpd_base_url + "/api"
+        otpd_config["restUrl"] = otpd_rest_url
 
-        otpdRestUrl = otpdBaseUrl + "/api"
-        otpdConfig["restUrl"] = otpdRestUrl
+        otpd_config["settingsUrl"] = otpd_rest_url + "/v1/settings"
 
-        otpdConfig["settingsUrl"] = otpdRestUrl + "/v1/settings"
+        otpd_config["importDatabaseUrl"] = otpd_base_url + "/servlet/import"
 
-        otpdConfig["importDatabaseUrl"] = otpdBaseUrl + "/servlet/import"
+        self._config = otpd_config
 
-        self._config = otpdConfig
+    def config(self) -> dict:
+        """Returns the configuration dictionary
 
-    def config(self):
+        Returns:
+            dict: Configuration dictionary
+        """
         return self._config
 
-    def credentials(self):
+    def credentials(self) -> dict:
+        """Get credentials (username + password)
+
+        Returns:
+            dict: dictionary with username and password
+        """
         return {
             "username": self.config()["username"],
             "password": self.config()["password"],
         }
 
-    def hostname(self):
+    def set_credentials(self, username: str = "admin", password: str = ""):
+        """Set the credentials for PowerDocs for the based on user name and password.
+
+        Args:
+            username (str, optional): Username. Defaults to "admin".
+            password (str, optional): Password of the user. Defaults to "".
+        """
+        self.config()["username"] = username
+        self.config()["password"] = password
+
+    def hostname(self) -> str:
+        """Returns the hostname of PowerDocs (e.g. "otpd")
+
+        Returns:
+            string: hostname
+        """
         return self.config()["hostname"]
 
-    def setHostname(self, hostname: str):
-        self.config()["hostname"] = hostname
+    def set_hostname(self, hostname: str):
+        """Sets the hostname of PowerDocs
 
-    def setCredentials(self, username: str = "", password: str = ""):
-        if username:
-            self.config()["username"] = username
-        else:
-            self.config()["username"] = "admin"
+        Args:
+            hostname (str): new hostname
+        """
+        self.config()["hostname"] = hostname
 
-        if password:
-            self.config()["password"] = password
-        else:
-            self.config()["password"] = ""
+    def base_url(self):
+        """Returns the base URL of PowerDocs
 
-    def baseUrl(self):
+        Returns:
+            string: base URL
+        """
         return self.config()["baseUrl"]
 
-    def restUrl(self):
+    def rest_url(self):
+        """Returns the REST URL of PowerDocs
+
+        Returns:
+            string: REST URL
+        """
         return self.config()["restUrl"]
 
-    def parseRequestResponse(
+    def parse_request_response(
         self,
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
-    ) -> dict:
+    ) -> dict | None:
         """Converts the request response to a Python dict in a safe way
            that also handles exceptions.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
             additional_error_message (string): print a custom error message
             show_error (boolean): if True log an error, if False log a warning
@@ -161,54 +208,32 @@
                 logger.warning(message)
             return None
         else:
             return dict_object
 
     # end method definition
 
-    def importDatabase(self, filename: str):
-        """Import PowerDocs database backup from a zip file"""
-
-        file = filename.split("/")[-1]
-        file_tup = (file, open(filename, "rb"), "application/zip")
-
-        # fields attribute is set according to the other party's interface description
-        m = MultipartEncoder(fields={"name": file, "zipfile": file_tup})
-
-        requestUrl = self.config()["otpdImportDatabaseUrl"]
-
-        logger.info(
-            "Importing Database backup -> {}, in to ServerManager on-> {}".format(
-                filename, requestUrl
-            )
-        )
-        resourceResponse = requests.post(
-            requestUrl, data=m, headers={"content-type": m.content_type}, timeout=60
-        )
-
-        if resourceResponse.ok:
-            return resourceResponse
-        else:
-            logger.error(
-                "Failed to Import Database backup -> {} in to -> {}; error => {}".format(
-                    filename, requestUrl, resourceResponse.text
-                )
-            )
-            return None
+    # This method is currently not used and not working...
+    def authenticate(self, revalidate: bool = False) -> dict:
+        """Authenticates at PowerDocs and retrieve OTCS Ticket.
 
-    # end method definition
+        Args:
+            revalidate (boolean): determinse if a re-athentication is enforced
+                                  (e.g. if session has timed out with 401 error)
+        Returns:
+            dictionary: Cookie information of None in case of an error.
+                        Also stores cookie information in self._cookie
+        """
 
-    # This method is currently not used and not working...
-    def authenticate(self, revalidate: bool = False):
         # Already authenticated and session still valid?
         if self._jsessionid and not revalidate:
             return self._jsessionid
 
         auth_url = (
-            self.baseUrl()
+            self.base_url()
             + "/j_security_check?j_username="
             + self.config()["username"]
             + "&j_password="
             + self.config()["password"]
         )
         payLoad = {}
         payLoad["settingname"] = "LocalOtdsUrl"
@@ -221,41 +246,76 @@
         # Step2: fetch session id from the response, and hit j_security_check with proper authentication
         # Step3: get session id from the response, add to self. It can be used for other transactions
         session = requests.Session()
         response = session.put(requestUrl, json=payLoad)
         logger.info("Initiating dummy rest call to Tomcat to get initial session id")
         logger.info(response.text)
         if response.ok:
-            logger.info("Url to authenticate Tomcat for Session id -> " + auth_url)
+            logger.info("Url to authenticate Tomcat for Session id -> %s", auth_url)
             sessionResponse = session.post(auth_url)
             if sessionResponse.ok:
-                logger.info("Response for -> {}, {} ".format(auth_url, sessionResponse))
+                logger.info(
+                    "Response for -> %s is -> %s", auth_url, str(sessionResponse)
+                )
                 session_dict = session.cookies.get_dict()
                 logger.info(
-                    "Session id to perform Rest api calls to Tomcat -> "
-                    + session_dict["JSESSIONID"]
+                    "Session id to perform Rest api calls to Tomcat -> %s",
+                    session_dict["JSESSIONID"],
                 )
                 self._jsessionid = session_dict["JSESSIONID"]
                 requestHeaders["Cookie"] = "JSESSIONID=" + self._jsessionid
             else:
                 logger.info(
-                    "Fetching session id from -> {} failed with j_security_check. Response -> {}".format(
-                        auth_url, sessionResponse.text
-                    )
+                    "Fetching session id from -> %s failed with j_security_check. Response -> %s",
+                    auth_url,
+                    sessionResponse.text,
                 )
         else:
             logger.info(
-                "Fetching session id from -> {} failed. Response => {}".format(
-                    requestUrl, response.text
-                )
+                "Fetching session id from -> %s failed. Response -> %s",
+                requestUrl,
+                response.text,
             )
 
     # end method definition
 
-    def applySetting(
+    def import_database(self, filename: str):
+        """Import PowerDocs database backup from a zip file"""
+
+        file = filename.split("/")[-1]
+        file_tup = (file, open(filename, "rb"), "application/zip")
+
+        # fields attribute is set according to the other party's interface description
+        m = MultipartEncoder(fields={"name": file, "zipfile": file_tup})
+
+        request_url = self.config()["otpdImportDatabaseUrl"]
+
+        logger.info(
+            "Importing Database backup -> %s, into PowerDocs ServerManager on -> %s",
+            filename,
+            request_url,
+        )
+        response = requests.post(
+            request_url, data=m, headers={"content-type": m.content_type}, timeout=60
+        )
+
+        if response.ok:
+            return response
+        else:
+            logger.error(
+                "Failed to Import Database backup -> %s into -> %s; error -> %s",
+                filename,
+                request_url,
+                response.text,
+            )
+            return None
+
+    # end method definition
+
+    def apply_setting(
         self, setting_name: str, setting_value: str, tenant_name: str = ""
     ) -> dict:
         """Appy a setting to the PowerDocs Server Manager
 
         Args:
             setting_name (string): name of the setting
             setting_value (string): new value of the setting
@@ -271,39 +331,40 @@
 
         if tenant_name:
             settingsPutBody["tenantName"] = tenant_name
 
         requestUrl = self.config()["settingsUrl"]
 
         logger.info(
-            "Update setting -> {} with value -> {}; calling -> {}".format(
-                setting_name, setting_value, requestUrl
-            )
+            "Update setting -> %s with value -> %s; calling -> %s",
+            setting_name,
+            setting_value,
+            requestUrl,
         )
 
         retries = 0
         while True:
             settingResponse = requests.put(
                 requestUrl,
                 json=settingsPutBody,
                 headers=requestHeaders,
                 auth=HTTPBasicAuth(
                     self.config()["username"], self.config()["password"]
                 ),
                 verify=False,  # for localhost deployments this will fail otherwise
             )
             if settingResponse.ok:
-                return self.parseRequestResponse(settingResponse)
+                return self.parse_request_response(settingResponse)
             # Check if Session has expired - then re-authenticate and try once more
             elif settingResponse.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to update setting -> {}; error -> {}".format(
-                        setting_name, settingResponse.text
-                    )
+                    "Failed to update setting -> %s; error -> %s",
+                    setting_name,
+                    settingResponse.text,
                 )
                 return None
 
     # end method definition
```

### Comparing `pyxecm-0.2.0/pyxecm/payload.py` & `pyxecm-0.3.0/pyxecm/customizer/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,30 @@
 determineGroupID: determine the id of a group - either from payload or from OTCS
 determineUserID: determine the id of a user - either from payload or from OTCS
 determineWorkspaceID: determine the nodeID of a workspace - either from payload or from OTCS
 
 processPayload: process payload (main method)
 processWebHooks: process list of web hooks
 processPartitions: process the OTDS partitions
-processPartitionLicenses: process the licenses that should be assigned to OTDS partitions (this includes existing partitions)
+processPartitionLicenses: process the licenses that should be assigned to OTDS partitions
+                          (this includes existing partitions)
 processOAuthClients: process the OTDS OAuth clients
 processTrustedSites: process the OTDS trusted sites
 processSystemAttributes: process the OTDS system attributes
 processGroups: process Extended ECM user groups
 processGroupsM365: process M365 user groups
 processUsers: process Extended ECM users
 processUsersM365: process M365 users
 processAdminSettings: process Extended ECM administration settings (LLConfig)
 processExternalSystems: process Extended ECM external systems
 processTransportPackages: process Extended ECM transport packages
 processUserPhotos: process Extended ECM user photos (user profile)
 processUserPhotosM365: process user photos in payload and assign them to Microsoft 365 users.
-processWorkspaceTypes: process Extended ECM workspace types (needs to run after processTransportPackages)
+processWorkspaceTypes: process Extended ECM workspace types
+                       (needs to run after processTransportPackages)
 processWorkspaces: process Extended ECM workspace instances
 processWorkspaceRelationships: process Extended ECM workspace relationships
 processWorkspaceMembers: process Extended ECM workspace members (users and groups)
 processWebReports: process Extended ECM Web Reports (starts them with parameters)
 processCSApplications: process Extended ECM CS Applications
 processUserSettings: Process user settings in payload and apply themin OTDS.
 processUserFavoritesAndProfile: Process user favorites in payload and create them in Extended ECM
@@ -104,25 +106,21 @@
 from typing import Callable
 from urllib.parse import urlparse
 
 import yaml
 import hcl2.api
 
 # OpenText specific modules:
-from pyxecm.k8s import K8s
-from pyxecm.m365 import M365
-from pyxecm.otac import OTAC
-from pyxecm.otcs import OTCS
-from pyxecm.otds import OTDS
-from pyxecm.sap import SAP
-from pyxecm.otiv import OTIV
-from pyxecm.otpd import OTPD
-from pyxecm.helper.web import HTTP as web
+from pyxecm import OTAC, OTCS, OTDS, OTIV
+from pyxecm.customizer.k8s import K8s
+from pyxecm.customizer.m365 import M365
+from pyxecm.customizer.sap import SAP
+from pyxecm.helper.web import HTTP
 
-logger = logging.getLogger("customizer.payload")
+logger = logging.getLogger("pyxecm.customizer.payload")
 
 
 class Payload:
     """Used to process Terrarium payload."""
 
     # _debug controls whether or not transport processing is
     # stopped if one transport fails:
@@ -130,15 +128,15 @@
     _otcs: OTCS
     _otcs_backend: OTCS
     _otcs_frontend: OTCS
     _otac: OTAC | None
     _otds: OTDS
     _otiv = OTIV | None
     _k8s = K8s | None
-    _web = web
+    _web = HTTP
     _m365 = M365 | None
     _custom_settings_dir = ""
 
     # _payload_source (string): This is either path + filename of the yaml payload
     # or an path + filename of the Terraform HCL payload
     _payload_source = ""
     # _payload is a dict of the complete payload file.
@@ -239,16 +237,18 @@
             otds_object (OTDS): OTDS object
             otac_object (OTAC): OTAC object
             otcs_backend_object (OTCS): OTCS backend object
             otcs_frontend_object (OTCS): OTCS frontend object
             otcs_restart_callback (callable): function to call if OTCS service needs a restart
             otiv_object (object): OTIV object
             m365_object (object): M365 object to talk to Microsoft Graph API
-            placeholder_values (dict): dictionary of placeholder values to be replaced in admin settings
-            stop_on_error (bool): controls if transport deployment should stop if one transport fails
+            placeholder_values (dict): dictionary of placeholder values
+                                       to be replaced in admin settings
+            stop_on_error (bool): controls if transport deployment should stop
+                                  if one transport fails
         """
 
         self._stop_on_error = stop_on_error
         self._payload_source = payload_source
         self._k8s = k8s_object
         self._otds = otds_object
         self._otac = otac_object
@@ -449,35 +449,35 @@
         """
 
         logger.info(
             "Check if payload section -> %s has been processed successfully before...",
             payload_section_name,
         )
 
-        response = self._otcs.getNodeByVolumeAndPath(
+        response = self._otcs.get_node_by_volume_and_path(
             142
         )  # write to Personal Workspace of Admin
-        target_folder_id = self._otcs.getResultValue(response, "id")
+        target_folder_id = self._otcs.get_result_value(response, "id")
         if not target_folder_id:
             target_folder_id = 2004  # use Personal Workspace of Admin as fallback
 
         # Some sections are actually not payload specific like teamsM365Cleanup
         # we don't want external payload runs to re-apply this processing:
         if payload_specific:
             file_name = os.path.basename(self._payload_source)  # remove directories
             file_name = os.path.splitext(file_name)[0]  # remove file suffix
             file_name = "success_" + file_name + "_" + payload_section_name + ".txt"
         else:
             file_name = "success_" + payload_section_name + ".txt"
 
-        status_document = self._otcs.getNodeByParentAndName(
+        status_document = self._otcs.get_node_by_parent_and_name(
             parent_id=int(target_folder_id), name=file_name, show_error=False
         )
         if status_document and status_document["results"]:
-            name = self._otcs.getResultValue(status_document, "name")
+            name = self._otcs.get_result_value(status_document, "name")
             if name == file_name:
                 logger.info(
                     "Payload section -> %s has been processed successfully before. Skipping...",
                     payload_section_name,
                 )
                 return True
         logger.info(
@@ -506,18 +506,18 @@
                                      each payload file or if success is "global" - like for the deletion
                                      of the existing M365 teams (which we don't want to execute per
                                      payload file)
         Returns:
             bool: True if the status file as been upladed to Extended ECM successfully, False otherwise
         """
 
-        response = self._otcs.getNodeByVolumeAndPath(
+        response = self._otcs.get_node_by_volume_and_path(
             142
         )  # write to Personal Workspace of Admin (with Volume Type ID = 142)
-        target_folder_id = self._otcs.getResultValue(response, "id")
+        target_folder_id = self._otcs.get_result_value(response, "id")
         if not target_folder_id:
             target_folder_id = 2004  # use Personal Workspace of Admin as fallback
 
         # Some sections are actually not payload specific like teamsM365Cleanup
         # we don't want external payload runs to re-apply this processing:
         if payload_specific:
             file_name = os.path.basename(self._payload_source)  # remove directories
@@ -526,15 +526,15 @@
         else:
             file_name = "success_" + payload_section_name + ".txt"
         full_path = "/tmp/" + file_name
 
         with open(full_path, mode="w", encoding="utf-8") as localfile:
             localfile.write(json.dumps(payload_section, indent=2))
 
-        response = self._otcs.uploadFileToParent(
+        response = self._otcs.upload_file_to_parent(
             file_url=full_path,
             file_name=file_name,
             mime_type="text/plain",
             parent_id=int(target_folder_id),
         )
 
         if response:
@@ -566,15 +566,15 @@
             return group["id"]
 
         if not "name" in group:
             logger.error("Group needs a name to lookup the ID.")
             return 0
         group_name = group["name"]
 
-        existing_groups = self._otcs.getGroup(name=group_name)
+        existing_groups = self._otcs.get_group(name=group_name)
         if not existing_groups or not existing_groups["data"]:
             logger.info("Cannot find an existing group with name -> %s", group_name)
             return 0
 
         # Get list of all matching groups:
         existing_groups_list = existing_groups["data"]
         # Find the group with the exact match of the name:
@@ -610,15 +610,15 @@
             return user["id"]
 
         if not "name" in user:
             logger.error("User needs a login name to lookup the ID.")
             return 0
         user_name = user["name"]
 
-        existing_users = self._otcs.getUser(name=user_name)
+        existing_users = self._otcs.get_user(name=user_name)
         if not existing_users or not existing_users["data"]:
             logger.info("Cannot find an existing user with name -> %s", user_name)
             return 0
 
         # Get list of all matching users:
         existing_users_list = existing_users["data"]
         # Find the group with the exact match of the name:
@@ -648,18 +648,18 @@
             the workspace items are modified by adding an "nodeId" dict element that
             includes the node ID of the workspace in Extended ECM
         """
 
         if "nodeId" in workspace:
             return workspace["nodeId"]
 
-        response = self._otcs.getWorkspaceByTypeAndName(
+        response = self._otcs.get_workspace_by_type_and_name(
             workspace["type_name"], workspace["name"]
         )
-        workspace_id = self._otcs.getResultValue(response, "id")
+        workspace_id = self._otcs.get_result_value(response, "id")
         if workspace_id:
             workspace["nodeId"] = workspace_id
             return workspace_id
         else:
             logger.info(
                 "Workspace of type -> %s and name -> %s does not yet exist.",
                 workspace["type_name"],
@@ -1048,15 +1048,15 @@
             headers = webhook.get("headers", {})
 
             if description:
                 logger.info("Calling Web Hook -> %s: %s (%s)", method, url, description)
             else:
                 logger.info("Calling Web Hook -> %s: %s", method, url)
 
-            self._http_object.httpRequest(url, method, payload, headers)
+            self._http_object.http_request(url, method, payload, headers)
 
         #        if success:
         #            self.writeStatusFile(section_name, webhooks)
 
         return success
 
         # end method definition
@@ -1100,35 +1100,35 @@
             partition_description = partition.get("description")
 
             # Check if Partition does already exist
             # (in an attempt to make the code idem-potent)
             logger.info(
                 "Check if OTDS partition -> %s does already exist...", partition_name
             )
-            response = self._otds.getPartition(partition_name, show_error=False)
+            response = self._otds.get_partition(partition_name, show_error=False)
             if response:
                 logger.info(
                     "Partition -> %s does already exist. Skipping...", partition_name
                 )
                 continue
 
             # Only continue if Partition does not exist already
             logger.info("Partition -> %s does not exist. Creating...", partition_name)
 
-            response = self._otds.addPartition(partition_name, partition_description)
+            response = self._otds.add_partition(partition_name, partition_description)
             if response:
                 logger.info("Added OTDS partition -> %s", partition_name)
             else:
                 logger.error("Failed to add OTDS partition -> %s", partition_name)
                 success = False
                 continue
 
             access_role = partition.get("access_role")
             if access_role:
-                response = self._otds.addPartitionToAccessRole(
+                response = self._otds.add_partition_to_access_role(
                     access_role, partition_name
                 )
                 if response:
                     logger.info(
                         "Added OTDS partition -> %s to access role -> %s",
                         partition_name,
                         access_role,
@@ -1144,23 +1144,23 @@
 
             # Partions may have an optional list of licenses in
             # the payload. Assign the partition to all these licenses:
             partition_specific_licenses = partition.get("licenses")
             if partition_specific_licenses:
                 # We assume these licenses are Extended ECM licenses!
                 otcs_resource_name = self._otcs.config()["resource"]
-                otcs_resource = self._otds.getResource(otcs_resource_name)
+                otcs_resource = self._otds.get_resource(otcs_resource_name)
                 if not otcs_resource:
                     logger.error("Cannot find OTCS resource -> %s", otcs_resource_name)
                     success = False
                     continue
                 otcs_resource_id = otcs_resource["resourceID"]
                 license_name = "EXTENDED_ECM"
                 for license_feature in partition_specific_licenses:
-                    assigned_license = self._otds.assignPartitionToLicense(
+                    assigned_license = self._otds.assign_partition_to_license(
                         partition_name,
                         otcs_resource_id,
                         license_feature,
                         license_name,
                     )
 
                     if not assigned_license:
@@ -1219,50 +1219,50 @@
             if "enabled" in partition and not partition["enabled"]:
                 logger.info(
                     "Payload for Partition -> %s is disabled. Skipping...",
                     partition_name,
                 )
                 continue
 
-            response = self._otds.getPartition(partition_name, show_error=True)
+            response = self._otds.get_partition(partition_name, show_error=True)
             if not response:
                 logger.error(
                     "Partition -> %s does not exist. Skipping...", partition_name
                 )
                 success = False
                 continue
 
             # Partions may have an optional list of licenses in
             # the payload. Assign the partition to all these licenses:
             partition_specific_licenses = partition.get("licenses")
             if partition_specific_licenses:
                 # We assume these licenses are Extended ECM licenses!
                 otcs_resource_name = self._otcs.config()["resource"]
-                otcs_resource = self._otds.getResource(otcs_resource_name)
+                otcs_resource = self._otds.get_resource(otcs_resource_name)
                 if not otcs_resource:
                     logger.error("Cannot find OTCS resource -> %s", otcs_resource_name)
                     success = False
                     continue
                 otcs_resource_id = otcs_resource["resourceID"]
                 license_name = "EXTENDED_ECM"
                 for license_feature in partition_specific_licenses:
-                    if self._otds.isPartitionLicensed(
+                    if self._otds.is_partition_licensed(
                         partition_name=partition_name,
                         resource_id=otcs_resource_id,
                         license_feature=license_feature,
                         license_name=license_name,
                     ):
                         logger.info(
                             "Partition -> %s is already licensed for -> %s (%s)",
                             partition_name,
                             license_name,
                             license_feature,
                         )
                         continue
-                    assigned_license = self._otds.assignPartitionToLicense(
+                    assigned_license = self._otds.assign_partition_to_license(
                         partition_name,
                         otcs_resource_id,
                         license_feature,
                         license_name,
                     )
 
                     if not assigned_license:
@@ -1335,26 +1335,26 @@
             client_allow_impersonation = oauth_client.get("allow_impersonation")
 
             # Check if OAuth client does already exist
             # (in an attempt to make the code idem-potent)
             logger.info(
                 "Check if OTDS OAuth Client -> %s does already exist...", client_name
             )
-            response = self._otds.getOauthClient(client_name, show_error=False)
+            response = self._otds.get_oauth_client(client_name, show_error=False)
             if response:
                 logger.info(
                     "OAuth Client -> %s does already exist. Skipping...", client_name
                 )
                 continue
             else:
                 logger.info(
                     "OAuth Client -> %s does not exist. Creating...", client_name
                 )
 
-            response = self._otds.addOauthClient(
+            response = self._otds.add_oauth_client(
                 client_id=client_name,
                 description=client_description,
                 redirect_urls=client_redirect_urls,
                 allow_impersonation=client_allow_impersonation,
                 confidential=client_confidential,
                 auth_scopes=client_partition,
                 allowed_scopes=client_permission_scopes,
@@ -1369,24 +1369,24 @@
 
             client_secret = response.get("secret")
             if not client_secret:
                 logger.error("OAuth client -> %s does not have a secret!", client_name)
                 continue
 
             client_description += " Client Secret Key: " + str(client_secret)
-            response = self._otds.updateOauthClient(
+            response = self._otds.update_oauth_client(
                 client_name, {"description": client_description}
             )
 
         if success:
             self.writeStatusFile(section_name, self._oauth_clients)
 
         return success
 
-    #        self._otds.addOauthClientsToAccessRole()
+    #        self._otds.add_oauth_clients_to_access_role()
 
     # end method definition
 
     def processTrustedSites(self, section_name: str = "trustedSites") -> bool:
         """Process OTDS trusted sites in payload and create them in OTDS.
 
         Args:
@@ -1403,15 +1403,15 @@
         # and skip processing once more
         if self.checkStatusFile(section_name):
             return True
 
         success: bool = True
 
         for trusted_site in self._trusted_sites:
-            response = self._otds.addTrustedSite(trusted_site)
+            response = self._otds.add_trusted_site(trusted_site)
             if response:
                 logger.info("Added OTDS trusted site -> %s", trusted_site)
             else:
                 logger.error("Failed to add trusted site -> %s", trusted_site)
                 success = False
 
         if success:
@@ -1458,15 +1458,15 @@
 
             if not system_attribute.get("value"):
                 logger.error("OTDS System Attribute needs a value. Skipping...")
                 continue
 
             attribute_value = system_attribute["value"]
             attribute_description = system_attribute.get("description")
-            response = self._otds.addSystemAttribute(
+            response = self._otds.add_system_attribute(
                 attribute_name, attribute_value, attribute_description
             )
             if response:
                 logger.info(
                     "Added OTDS system attribute -> %s with value -> %s",
                     attribute_name,
                     attribute_value,
@@ -1619,15 +1619,15 @@
                     group_id,
                 )
                 continue
 
             logger.info("Did not find an existing group - creating a new group...")
 
             # Now we know it is a new group...
-            new_group = self._otcs.addGroup(group_name)
+            new_group = self._otcs.add_group(group_name)
             if new_group is not None:
                 logger.debug("New group -> %s", new_group)
                 group["id"] = new_group["id"]
             else:
                 logger.error("Failed to create group -> %s", new_group)
                 success = False
                 continue
@@ -1652,15 +1652,15 @@
                     ),
                     None,
                 )
                 if parent_group is None:
                     # If this didn't work, try to get the parent group from OTCS. This covers
                     # cases where the parent group is system generated or part
                     # of a former payload processing:
-                    parent_group = self._otcs.getGroup(parent_group_name)
+                    parent_group = self._otcs.get_group(parent_group_name)
                     if not parent_group:
                         logger.error(
                             "Parent Group -> %s not found. Skipping...",
                             parent_group_name,
                         )
                         success = False
                         continue
@@ -1670,16 +1670,16 @@
                         "Parent Group -> %s does not have an ID. Skipping...",
                         parent_group["name"],
                     )
                     success = False
                     continue
 
                 # retrieve all members of the parent group (1 = get only groups)
-                members = self._otcs.getGroupMembers(parent_group["id"], 1)
-                if self._otcs.existResultItem(members, "id", group["id"]):
+                members = self._otcs.get_group_members(parent_group["id"], 1)
+                if self._otcs.exist_result_item(members, "id", group["id"]):
                     #                if existing_member:
                     logger.info(
                         "Group -> %s (%s) is already a member of parent group -> %s (%s) - skipping to next parent group...",
                         group["name"],
                         group["id"],
                         parent_group["name"],
                         parent_group["id"],
@@ -1688,15 +1688,15 @@
                     logger.info(
                         "Add group -> %s (%s) to parent group -> %s (%s)",
                         group["name"],
                         group["id"],
                         parent_group["name"],
                         parent_group["id"],
                     )
-                    self._otcs.addGroupMember(group["id"], parent_group["id"])
+                    self._otcs.add_group_member(group["id"], parent_group["id"])
 
         if success:
             self.writeStatusFile(section_name, self._groups)
 
         return success
 
         # end method definition
@@ -1748,15 +1748,15 @@
                     "Office 365 is not enabled in payload for Group -> %s. Skipping...",
                     group_name,
                 )
                 continue
 
             # Check if the group does already exist (e.g. if job is restarted)
             # as this is a pattern search it could return multiple groups:
-            existing_groups = self._m365.getGroup(group_name)
+            existing_groups = self._m365.get_group(group_name)
 
             if existing_groups and existing_groups["value"]:
                 logger.debug(
                     "Found existing Microsoft 365 groups -> %s",
                     existing_groups["value"],
                 )
                 # Get list of all matching groups:
@@ -1784,15 +1784,15 @@
                 )
             else:
                 logger.info(
                     "Did not find any matching group - creating a new Microsoft 365 group..."
                 )
 
             # Now we know it is a new group...
-            new_group = self._m365.addGroup(group_name)
+            new_group = self._m365.add_group(group_name)
             if new_group is not None:
                 # Store the Microsoft 365 group ID in payload:
                 group["m365_id"] = new_group["id"]
                 logger.info(
                     "New Microsoft 365 group -> %s with ID -> %s has been created",
                     group_name,
                     group["m365_id"],
@@ -1885,15 +1885,15 @@
                     for item in self._groups
                     if item["name"] == user["base_group"] and item.get("id")
                 ),
                 1001,
             )
 
             # Now we know it is a new user...
-            new_user = self._otcs.addUser(
+            new_user = self._otcs.add_user(
                 name=user_name,
                 password=user["password"],
                 # be careful - can be empty
                 first_name=user.get("firstname", ""),
                 # be careful - can be empty
                 last_name=user.get("lastname", ""),
                 email=user.get("email", ""),  # be careful - can be empty
@@ -1915,15 +1915,15 @@
                     group = next(
                         (item for item in self._groups if item["name"] == group_name),
                         None,
                     )
                     if group is None:
                         # if group is not in payload try to find group in OTCS
                         # in case it is a pre-existing group:
-                        group = self._otcs.getGroup(group_name)
+                        group = self._otcs.get_group(group_name)
                         if group is None:
                             logger.error(
                                 "Group -> %s not found. Skipping...", group_name
                             )
                             success = False
                             continue
                         group = group["data"][0]
@@ -1939,20 +1939,22 @@
                     logger.info(
                         "Add user -> %s (%s) to group -> %s (%s)",
                         user["name"],
                         user["id"],
                         group["name"],
                         group["id"],
                     )
-                    response = self._otcs.addGroupMember(user["id"], group["id"])
+                    response = self._otcs.add_group_member(user["id"], group["id"])
                     if not response:
                         success = False
                 # for some unclear reason the user is not added to its base group in OTDS
                 # so we do this explicitly:
-                response = self._otds.addUserToGroup(user["name"], user["base_group"])
+                response = self._otds.add_user_to_group(
+                    user["name"], user["base_group"]
+                )
                 if not response:
                     success = False
 
                 # Extra OTDS attributes for the user can be provided in "extra_attributes"
                 # as part of the user payload.
                 if "extra_attributes" in user:
                     extra_attributes = user["extra_attributes"]
@@ -1971,15 +1973,15 @@
                             attribute_value,
                         )
                         user_partition = self._otcs.config()["partition"]
                         if not user_partition:
                             logger.error("User partition not found!")
                             success = False
                             continue
-                        self._otds.updateUser(
+                        self._otds.update_user(
                             user_partition,
                             user["name"],
                             attribute_name,
                             attribute_value,
                         )
 
         if success:
@@ -2054,30 +2056,30 @@
             user_first_name = user.get("firstname", "")
             user_last_name = user.get("lastname", "")
             user_location = user.get("location", "US")
 
             # Check if the user does already exist (e.g. if job is restarted)
             # As this is a pattern search it could return multiple users:
             user_name = user_name + "@" + self._m365.config()["domain"]
-            existing_user = self._m365.getUser(user_name)
+            existing_user = self._m365.get_user(user_name)
             if existing_user:
                 logger.info(
                     "Found existing Microsoft 365 user -> %s (%s) with ID -> %s",
                     existing_user["displayName"],
                     existing_user["userPrincipalName"],
                     existing_user["id"],
                 )
                 user["m365_id"] = existing_user["id"]
             else:
                 logger.info(
                     "Did not find existing user - creating a new Microsoft 365 user..."
                 )
 
                 # Now we know it is a new user...
-                new_user = self._m365.addUser(
+                new_user = self._m365.add_user(
                     email=user_name,
                     password=user_password,
                     first_name=user_first_name,
                     last_name=user_last_name,
                     location=user_location,
                     department=user_department,
                 )
@@ -2097,22 +2099,24 @@
                     success = False
                     continue
 
             # Now we assign a license to the new M365 user.
             # First we see if there's a M365 SKU list in user
             # payload - if not we wrap the default SKU configured
             # for the m365 object into a single item list:
-            existing_user_licenses = self._m365.getUserLicenses(user["m365_id"])
+            existing_user_licenses = self._m365.get_user_licenses(user["m365_id"])
             sku_list = user.get("m365_skus", [self._m365.config()["skuId"]])
             for sku_id in sku_list:
                 # Check if the M365 user already has this license:
-                if not self._m365.existResultItem(
+                if not self._m365.exist_result_item(
                     existing_user_licenses, "skuId", sku_id
                 ):
-                    response = self._m365.assignLicenseToUser(user["m365_id"], sku_id)
+                    response = self._m365.assign_license_to_user(
+                        user["m365_id"], sku_id
+                    )
                     if not response:
                         logger.error(
                             "Failed to assign license -> %s to Microsoft 365 user -> %s",
                             sku_id,
                             user_name,
                         )
                         success = False
@@ -2134,30 +2138,34 @@
                     )
 
             # Now we assign the Extended ECM Teams App to the new M365 user.
             # First we check if the app is already assigned to the user.
             # If not we install / assign the app. If the user already has
             # the Extended ECM app we try to uprade it:
             app_name = self._m365.config()["teamsAppName"]
-            response = self._m365.getTeamsAppsOfUser(
+            response = self._m365.get_teams_apps_of_user(
                 user["m365_id"],
                 f"contains(teamsAppDefinition/displayName, '{app_name}')",
             )
-            if self._m365.existResultItem(
+            if self._m365.exist_result_item(
                 response, "displayName", app_name, sub_dict_name="teamsAppDefinition"
             ):
                 logger.info(
                     "Upgrade MS Teams app -> %s for user -> %s", app_name, user_name
                 )
-                response = self._m365.upgradeTeamsAppOfUser(user["m365_id"], app_name)
+                response = self._m365.upgrade_teams_app_of_user(
+                    user["m365_id"], app_name
+                )
             else:
                 logger.info(
                     "Install MS Teams app -> %s for user -> %s", app_name, user_name
                 )
-                response = self._m365.assignTeamsAppToUser(user["m365_id"], app_name)
+                response = self._m365.assign_teams_app_to_user(
+                    user["m365_id"], app_name
+                )
 
             # Process Microsoft 365 group memberships of new user:
             if "m365_id" in user:
                 user_id = user["m365_id"]
                 # don't forget the base group (department) !
                 group_names = user["groups"]
                 if user_department:
@@ -2190,15 +2198,15 @@
                         # the payload we don't create a M365 but we do NOT continue
                         # as there may still be parent groups that are M365 enabled
                         # we want to put the user in (see below):
                         logger.info(
                             "Payload Group -> %s is not enabled for M365.", group_name
                         )
                     else:
-                        response = self._m365.getGroup(group_name)
+                        response = self._m365.get_group(group_name)
                         if (
                             response is None
                             or not "value" in response
                             or not response["value"]
                         ):
                             logger.error(
                                 "Microsoft 365 Group -> %s not found. Skipping...",
@@ -2206,15 +2214,17 @@
                             )
                             success = False
                         else:
                             group_id = response["value"][0]["id"]
 
                             # Check if user is already a member. We don't want
                             # to throw an error if the user is not found as a member:
-                            if self._m365.isMember(group_id, user_id, show_error=False):
+                            if self._m365.is_member(
+                                group_id, user_id, show_error=False
+                            ):
                                 logger.info(
                                     "Microsoft 365 user -> %s (%s) is already in Microsoft 365 group -> %s (%s)",
                                     user["name"],
                                     user_id,
                                     group_name,
                                     group_id,
                                 )
@@ -2222,26 +2232,26 @@
                                 logger.info(
                                     "Add Microsoft 365 user -> %s (%s) to Microsoft 365 group -> %s (%s)",
                                     user["name"],
                                     user_id,
                                     group_name,
                                     group_id,
                                 )
-                                self._m365.addGroupMember(group_id, user_id)
+                                self._m365.add_group_member(group_id, user_id)
                                 # As each group should have at least one owner in M365
                                 # we set all users also as owners for now. Later we
                                 # may want to configure this via payload:
                                 logger.info(
                                     "Make Microsoft 365 user -> %s (%s) owner of Microsoft 365 group -> %s (%s)",
                                     user["name"],
                                     user_id,
                                     group_name,
                                     group_id,
                                 )
-                                self._m365.addGroupOwner(group_id, user_id)
+                                self._m365.add_group_owner(group_id, user_id)
 
                     # As M365 groups are flat (not nested) we also add the
                     # user as member to the parent groups of the current group
                     # if the parent group is enabled for M365:
                     parent_group_names = group.get("parent_groups")
                     logger.info(
                         "Group -> %s has the following parent groups -> %s",
@@ -2269,15 +2279,15 @@
                             # the payload we can also skip:
                             logger.info(
                                 "Parent Group -> %s is not enabled for M365. Skipping...",
                                 group_name,
                             )
                             continue
 
-                        response = self._m365.getGroup(parent_group_name)
+                        response = self._m365.get_group(parent_group_name)
                         if (
                             response is None
                             or not "value" in response
                             or not response["value"]
                         ):
                             logger.error(
                                 "Microsoft 365 Group -> %s not found. Skipping...",
@@ -2285,15 +2295,15 @@
                             )
                             success = False
                             continue
                         parent_group_id = response["value"][0]["id"]
 
                         # Check if user is already a member. We don't want
                         # to throw an error if the user is not found as a member:
-                        if self._m365.isMember(
+                        if self._m365.is_member(
                             parent_group_id, user_id, show_error=False
                         ):
                             logger.info(
                                 "Microsoft 365 user -> %s (%s) is already in Microsoft 365 group -> %s (%s)",
                                 user["name"],
                                 user_id,
                                 parent_group_name,
@@ -2304,15 +2314,15 @@
                         logger.info(
                             "Add Microsoft 365 user -> %s (%s) to Microsoft 365 group -> %s (%s)",
                             user["name"],
                             user_id,
                             parent_group_name,
                             parent_group_id,
                         )
-                        self._m365.addGroupMember(parent_group_id, user_id)
+                        self._m365.add_group_member(parent_group_id, user_id)
 
         if success:
             self.writeStatusFile(section_name, self._users)
 
         return success
 
         # end method definition
@@ -2373,22 +2383,22 @@
                 logger.error(
                     "No M365 Group exist for group -> %s (M365 Group creation may have failed). Skipping...",
                     group_name,
                 )
                 success = False
                 continue
 
-            if not self._m365.hasTeam(group_name):
+            if not self._m365.has_team(group_name):
                 logger.info(
                     "Create M365 Team -> %s for existing M365 Group -> %s...",
                     group_name,
                     group_name,
                 )
                 # Now "upgrading" this group to a MS Team:
-                new_team = self._m365.addTeam(group_name)
+                new_team = self._m365.add_team(group_name)
                 if not new_team:
                     success = False
             else:
                 logger.info(
                     "M365 group -> %s already has an MS Team connected. Skipping...",
                     group_name,
                 )
@@ -2422,29 +2432,29 @@
         for workspace_type in workspace_types:
             if not "name" in workspace_type:
                 logger.error(
                     "Workspace type -> %s does not have a name. Skipping...",
                     workspace_type,
                 )
                 continue
-            response = self._otcs.getWorkspaceInstances(workspace_type["name"])
+            response = self._otcs.get_workspace_instances(workspace_type["name"])
             workspace_instances = response["results"]
             if not workspace_instances:
                 logger.info(
                     "Workspace type -> %s does not have any instances!",
                     workspace_type["name"],
                 )
                 continue
             for workspace_instance in workspace_instances:
                 workspace_name = workspace_instance["data"]["properties"]["name"]
                 logger.info(
                     "Check if stale Microsoft 365 Teams with name -> %s exist...",
                     workspace_name,
                 )
-                response = self._m365.deleteTeams(workspace_name)
+                response = self._m365.delete_teams(workspace_name)
 
         # end method definition
 
     def cleanupAllTeamsM365(self, section_name: str = "teamsM365Cleanup") -> bool:
         """Delete Microsoft Teams that are left-overs from former deployments
 
         Args:
@@ -2487,15 +2497,15 @@
         pattern_list = [
             r"\(\d+\)",
             r"\d+\s-\s",
             r"^WS\d{1,4}$",
             r"^.+?\s\(.{1,2}-\d+\)$",
         ]
 
-        result = self._m365.deleteAllTeams(exception_list, pattern_list)
+        result = self._m365.delete_all_teams(exception_list, pattern_list)
 
         # We want this cleanup to only run once even if we have
         # multiple payload files - so we pass payload_specific=False here:
         self.writeStatusFile(
             payload_section_name=section_name,
             payload_section=exception_list + pattern_list,
             payload_specific=False,
@@ -2563,15 +2573,15 @@
                 file_content = self.replacePlaceholders(file_content)
 
                 # Write the updated config file:
                 tmpfile = "/tmp/" + os.path.basename(settings_file)
                 with open(tmpfile, "w", encoding="utf-8") as file:
                     file.write(file_content)
 
-                response = self._otcs.applyConfig(tmpfile)
+                response = self._otcs.apply_config(tmpfile)
                 if response and response["results"]["data"]["restart"]:
                     logger.info("A restart of Extended ECM service is required.")
                     restart_required = True
             else:
                 logger.error("Admin settings file -> %s not found.", settings_file)
                 success = False
 
@@ -2701,15 +2711,15 @@
             # Extract the port:
             external_system_port = (
                 urlparse(as_url).port if urlparse(as_url).port else 80
             )
             # Write this information back into the data structure:
             external_system["external_system_port"] = external_system_port
 
-            if self._http_object.checkHostReachable(
+            if self._http_object.check_host_reachable(
                 external_system_hostname, external_system_port
             ):
                 logger.info(
                     "Mark external system -> %s as reachable for later workspace creation...",
                     system_name,
                 )
                 external_system["reachable"] = True
@@ -2773,28 +2783,28 @@
                     return False
 
             # We do this existance test late in this function to make sure the payload
             # datastructure is properly updated for debugging purposes.
             logger.info(
                 "Test if external system -> %s does already exist...", system_name
             )
-            if self._otcs.getExternalSystemConnection(system_name):
+            if self._otcs.get_external_system_connection(system_name):
                 logger.info(
                     "External System connection -> %s already exists! Skipping to next external system...",
                     system_name,
                 )
                 continue
 
             #
             # 2: Create External System:
             #
             logger.info(
                 "Create external system -> %s; type -> %s", system_name, connection_type
             )
-            response = self._otcs.addExternalSystemConnection(
+            response = self._otcs.add_external_system_connection(
                 system_name,
                 connection_type,
                 as_url,
                 base_url,
                 str(username),
                 str(password),
                 auth_method,
@@ -2833,15 +2843,15 @@
                             system_name,
                             connection_type,
                         )
                         success = False
                         continue
                     otds_sp_endpoint = external_system["otds_sp_endpoint"]
 
-                    response = self._otds.addAuthHandlerSAML(
+                    response = self._otds.add_auth_handler_saml(
                         name=system_name,
                         description=description,
                         provider_name=provider_name,
                         saml_url=saml_url,
                         otds_url=otds_sp_endpoint,
                     )
                     if response:
@@ -2866,15 +2876,15 @@
                             external_system["certificate_file"],
                         )
                         success = False
                         continue
                     certificate_file = external_system["certificate_file"]
                     certificate_password = external_system["certificate_password"]
                     certificate_description = external_system["description"]
-                    response = self._otds.addAuthHandlerSAP(
+                    response = self._otds.add_auth_handler_sap(
                         name=system_name,
                         description=certificate_description,
                         certificate_file=certificate_file,
                         certificate_password=certificate_password,
                     )
                     if response:
                         logger.info("Successfully added SAP authentication handler.")
@@ -2889,25 +2899,25 @@
                         and self._otac
                     ):
                         logger.info(
                             "Put certificate file -> %s for logical archive -> %s into Archive Center",
                             external_system["archive_certificate_file"],
                             external_system["archive_logical_name"],
                         )
-                        response = self._otac.putCert(
+                        response = self._otac.put_cert(
                             external_system["external_system_name"],
                             external_system["archive_logical_name"],
                             external_system["archive_certificate_file"],
                         )
                         logger.info(
                             "Enable certificate file -> %s for logical archive -> %s",
                             external_system["archive_certificate_file"],
                             external_system["archive_logical_name"],
                         )
-                        response = self._otac.enableCert(
+                        response = self._otac.enable_cert(
                             external_system["external_system_name"],
                             external_system["archive_logical_name"],
                             True,
                         )
                 case "Salesforce":
                     # Configure an OAuth-based authentication handler:
                     if not "authorization_endpoint" in external_system:
@@ -2924,15 +2934,15 @@
                             "Salesforce system -> %s (%s) is missing the token endpoint!",
                             system_name,
                             connection_type,
                         )
                         success = False
                         continue
                     token_endpoint = external_system["token_endpoint"]
-                    response = self._otds.addAuthHandlerOAuth(
+                    response = self._otds.add_auth_handler_oauth(
                         name=system_name,
                         description=description,
                         provider_name=provider_name,
                         client_id=oauth_client_id,
                         client_secret=oauth_client_secret,
                         active_by_default=False,
                         authorization_endpoint=authorization_endpoint,
@@ -3010,20 +3020,20 @@
                 replacements = transport_package["replacements"]
                 logger.info(
                     "Deploy transport -> %s with replacements -> %s; URL -> %s",
                     description,
                     url,
                     replacements,
                 )
-                response = self._otcs.deployTransport(
+                response = self._otcs.deploy_transport(
                     url, name, description, replacements
                 )
             else:
                 logger.info("Deploy transport -> %s; URL -> %s", description, url)
-                response = self._otcs.deployTransport(url, name, description)
+                response = self._otcs.deploy_transport(url, name, description)
             if response is None:
                 logger.error("Failed to deploy transport -> %s; URL -> %s", name, url)
                 success = False
                 if self._stop_on_error:
                     break
             else:
                 logger.info("Successfully deployed transport -> %s", name)
@@ -3074,36 +3084,36 @@
                     user_name,
                 )
                 success = False
                 continue
 
             user_id = user["id"]
 
-            response = self._otcs.getNodeFromNickname(user_name)
+            response = self._otcs.get_node_from_nickname(user_name)
             if response is None:
                 logger.warning(
                     "Missing photo for user -> %s - nickname not found. Skipping...",
                     user_name,
                 )
                 continue
-            photo_id = self._otcs.getResultValue(response, "id")
-            response = self._otcs.updateUserPhoto(user_id, photo_id)
+            photo_id = self._otcs.get_result_value(response, "id")
+            response = self._otcs.update_user_photo(user_id, photo_id)
             if not response:
                 logger.error("Failed to add photo for user -> %s", user_name)
                 success = False
             else:
                 logger.info("Successfully added photo for user -> %s", user_name)
 
         # Check if Admin has a photo as well (nickname needs to be "admin"):
-        response = self._otcs.getNodeFromNickname("admin")
+        response = self._otcs.get_node_from_nickname("admin")
         if response is None:
             logger.warning("Missing photo for admin - nickname not found. Skipping...")
         else:
-            photo_id = self._otcs.getResultValue(response, "id")
-            response = self._otcs.updateUserPhoto(1000, photo_id)
+            photo_id = self._otcs.get_result_value(response, "id")
+            response = self._otcs.update_user_photo(1000, photo_id)
             if response is None:
                 logger.warning("Failed to add photo for admin")
             else:
                 logger.info("Successfully added photo for admin")
 
         if success:
             self.writeStatusFile(section_name, self._users)
@@ -3169,54 +3179,54 @@
                     "Office 365 user -> %s has not been created. Skipping...", user_name
                 )
                 success = False
                 continue
 
             user_m365_id = user["m365_id"]
 
-            if self._m365.getUserPhoto(user_m365_id, show_error=False):
+            if self._m365.get_user_photo(user_m365_id, show_error=False):
                 logger.info(
                     "User -> %s (%s) has already a photo in Microsoft 365. Skipping...",
                     user_name,
                     user_m365_id,
                 )
                 continue
             else:
                 logger.info(
                     "User -> %s (%s) has not yet a photo in Microsoft 365. Uploading...",
                     user_name,
                     user_m365_id,
                 )
 
-            response = self._otcs.getNodeFromNickname(user_name)
+            response = self._otcs.get_node_from_nickname(user_name)
             if response is None:
                 logger.warning(
                     "Missing photo for user -> %s - nickname not found. Skipping...",
                     user_name,
                 )
                 continue
-            photo_id = self._otcs.getResultValue(response, "id")
-            photo_name = self._otcs.getResultValue(response, "name")
+            photo_id = self._otcs.get_result_value(response, "id")
+            photo_name = self._otcs.get_result_value(response, "name")
             photo_path = "/tmp/" + str(photo_name)
-            response = self._otcs.downloadDocument(photo_id, photo_path)
+            response = self._otcs.download_document(photo_id, photo_path)
             if response is None:
                 logger.warning(
                     "Failed to download photo for user -> %s from Extended ECM",
                     user_name,
                 )
                 success = False
             else:
                 logger.info(
                     "Successfully downloaded photo for user -> %s from Extended ECM to file -> %s",
                     user_name,
                     photo_path,
                 )
 
             # Upload photo to M365:
-            response = self._m365.updateUserPhoto(user_m365_id, photo_path)
+            response = self._m365.update_user_photo(user_m365_id, photo_path)
             if response is None:
                 logger.error(
                     "Failed to upload photo for user -> %s to Microsoft 365", user_name
                 )
                 success = False
             else:
                 logger.info(
@@ -3247,15 +3257,15 @@
 
         # if this payload section has been processed successfully before we can return True
         # and skip processing once more
         if self.checkStatusFile(section_name):
             return []
 
         # get all workspace types (these have been created by the transports and are not in the payload!):
-        response = self._otcs.getWorkspaceTypes()
+        response = self._otcs.get_workspace_types()
         if response is None:
             logger.error("No workspace types found!")
             self._workspace_types = []
         else:
             self._workspace_types = response["results"]
 
         # now we enrich the workspace_type list elments (which are dicts)
@@ -3285,36 +3295,36 @@
                         "id": workspace_template_id,
                     }
                     workspace_type["templates"].append(template)
 
                     # Workaround for problem with workspace role inheritance
                     # which may be related to Transport or REST API: to work-around this we
                     # push down the workspace roles to the workspace folders explicitly:
-                    response = self._otcs.getWorkspaceRoles(workspace_template_id)
+                    response = self._otcs.get_workspace_roles(workspace_template_id)
 
                     for roles in response["results"]:
                         role_name = roles["data"]["properties"]["name"]
                         role_id = roles["data"]["properties"]["id"]
                         permissions = roles["data"]["properties"]["perms"]
-                        # as getWorkspaceRoles() delivers permissions as a value (bit encoded)
+                        # as get_workspace_roles() delivers permissions as a value (bit encoded)
                         # we need to convert it to a permissions string list:
                         permission_string_list = (
-                            self._otcs.convertPermissionValueToPermissionString(
+                            self._otcs.convert_permission_value_to_permission_string(
                                 permissions
                             )
                         )
 
                         logger.info(
                             "Inherit permissions of workspace template -> %s and role -> %s to workspace folders...",
                             workspace_template_name,
                             role_name,
                         )
 
                         # Inherit permissions to folders of workspace template:
-                        response = self._otcs.assignWorkspacePermissions(
+                        response = self._otcs.assign_workspace_permissions(
                             workspace_template_id,
                             role_id,
                             permission_string_list,
                             1,  # Only sub items - workspace node itself is OK
                         )
 
             else:
@@ -3429,15 +3439,15 @@
                 logger.info(
                     "Parent Workspace with logical ID -> %s has node ID -> %s",
                     parent_id,
                     parent_workspace_node_id,
                 )
             else:
                 # if no parent_id is specified the workspace location is determined by the workspace type definition
-                # and we pass None as parent ID to the getWorkspaceCreateForm and createWorkspace methods below:
+                # and we pass None as parent ID to the get_workspace_create_form and create_workspace methods below:
                 parent_workspace_node_id = None
 
             # Find the workspace type with the name given in the payload:
             workspace_type = next(
                 (item for item in self._workspace_types if item["name"] == type_name),
                 None,
             )
@@ -3572,15 +3582,15 @@
                     "Workspace payload has no category data! Will leave category attributes empty..."
                 )
                 category_create_data = {}
             else:
                 categories = workspace["categories"]
                 category_create_data = {"categories": {}}
 
-                response = self._otcs.getWorkspaceCreateForm(
+                response = self._otcs.get_workspace_create_form(
                     template_id, ext_system_id, bo_type, bo_id, parent_workspace_node_id
                 )
                 if response is None:
                     logger.error(
                         "Failed to retrieve create information for template -> %s",
                         template_id,
                     )
@@ -3891,15 +3901,15 @@
                                 if attr_type == str(11480):
                                     logger.info(
                                         "Attribute -> %s is is of type -> Organizational Unit (%s). Looking up group ID for group name -> %s",
                                         attr_name,
                                         attr_type,
                                         attribute["value"],
                                     )
-                                    response = self._otcs.getGroup(attribute["value"])
+                                    response = self._otcs.get_group(attribute["value"])
                                     # retrieve the list of matching group names - should just be 1
                                     group_list = response["data"]
                                     # Make sure we have an exact match:
                                     group = next(
                                         (
                                             item
                                             for item in group_list
@@ -3931,15 +3941,15 @@
                                 elif attr_type == "otcs_user_picker":
                                     logger.info(
                                         "Attribute -> %s is is of type -> User Picker (%s). Looking up user ID for user login name -> %s",
                                         attr_name,
                                         attr_type,
                                         attribute["value"],
                                     )
-                                    response = self._otcs.getUser(attribute["value"])
+                                    response = self._otcs.get_user(attribute["value"])
                                     # retrieve the list of matching group names - should just be 1
                                     user_list = response["data"]
                                     # Make sure we have an exact match:
                                     user = next(
                                         (
                                             item
                                             for item in user_list
@@ -3969,15 +3979,15 @@
                                     # Put the value from the payload into data structure
                                     data_attributes[attr_data] = attribute["value"]
                     category_create_data["categories"][cat_data] = data_attributes
 
             logger.debug("Category Create Data -> %s", category_create_data)
 
             # Create the workspace with all provided information:
-            response = self._otcs.createWorkspace(
+            response = self._otcs.create_workspace(
                 template_id,
                 name,
                 description,
                 workspace_type_id,
                 category_create_data,
                 ext_system_id,
                 bo_type,
@@ -3986,41 +3996,41 @@
             )
             if response is None:
                 logger.error("Failed to create workspace -> %s", name)
                 continue
 
             # Now we add the node ID of the new workspace to the payload data structure
             # This will be reused when creating the workspace relationships!
-            workspace["nodeId"] = self._otcs.getResultValue(response, "id")
+            workspace["nodeId"] = self._otcs.get_result_value(response, "id")
 
             # We also get the name the workspace was finally created with.
             # This can be different form the name in the payload as additional
             # naming conventions from the Workspace Type definitions may apply.
             # This is important to make the python container idem-potent.
-            response = self._otcs.getWorkspace(workspace["nodeId"])
-            workspace["name"] = self._otcs.getResultValue(response, "name")
+            response = self._otcs.get_workspace(workspace["nodeId"])
+            workspace["name"] = self._otcs.get_result_value(response, "name")
 
             logger.info(
                 "Successfully created workspace with final name -> %s and node ID -> %s",
                 workspace["name"],
                 workspace["nodeId"],
             )
 
             # Check if an RM classification is specified for the workspace:
             # RM Classification is specified as list of path elements (top-down)
             if (
                 "rm_classification_path" in workspace
                 and workspace["rm_classification_path"] != []
             ):
-                rm_class_node = self._otcs.getNodeByVolumeAndPath(
+                rm_class_node = self._otcs.get_node_by_volume_and_path(
                     198, workspace["rm_classification_path"]
                 )
-                rm_class_node_id = self._otcs.getResultValue(rm_class_node, "id")
+                rm_class_node_id = self._otcs.get_result_value(rm_class_node, "id")
                 if rm_class_node_id:
-                    response = self._otcs.assignRMClassification(
+                    response = self._otcs.assign_rm_classification(
                         workspace["nodeId"], rm_class_node_id, False
                     )
                     if response is None:
                         logger.error(
                             "Failed to assign RM classification -> %s (%s) to workspace -> %s",
                             workspace["rm_classification_path"][-1],
                             rm_class_node_id,
@@ -4035,20 +4045,20 @@
             # Check if one or multiple classifications are specified for the workspace
             # Classifications are specified as list of path elements (top-down)
             if (
                 "classification_pathes" in workspace
                 and workspace["classification_pathes"] != []
             ):
                 for classification_path in workspace["classification_pathes"]:
-                    class_node = self._otcs.getNodeByVolumeAndPath(
+                    class_node = self._otcs.get_node_by_volume_and_path(
                         198, classification_path
                     )
-                    class_node_id = self._otcs.getResultValue(class_node, "id")
+                    class_node_id = self._otcs.get_result_value(class_node, "id")
                     if class_node_id:
-                        response = self._otcs.assignClassification(
+                        response = self._otcs.assign_classification(
                             workspace["nodeId"], [class_node_id], False
                         )
                         if response is None:
                             logger.error(
                                 "Failed to assign classification -> %s to workspace -> %s",
                                 class_node_id,
                                 name,
@@ -4182,28 +4192,28 @@
                 logger.info(
                     "Create Workspace Relationship between workspace node ID -> %s and workspace node ID -> %s",
                     workspace_node_id,
                     related_workspace_node_id,
                 )
 
                 # Check if relationship does already exists:
-                response = self._otcs.getWorkspaceRelationships(workspace_node_id)
+                response = self._otcs.get_workspace_relationships(workspace_node_id)
 
-                existing_workspace_relationship = self._otcs.existResultItem(
+                existing_workspace_relationship = self._otcs.exist_result_item(
                     response, "id", related_workspace_node_id
                 )
                 if existing_workspace_relationship:
                     logger.info(
                         "Workspace relationship between workspace ID -> %s and related workspace ID -> %s does already exist. Skipping...",
                         workspace_node_id,
                         related_workspace_node_id,
                     )
                     continue
 
-                response = self._otcs.createWorkspaceRelationship(
+                response = self._otcs.create_workspace_relationship(
                     workspace_node_id, related_workspace_node_id
                 )
                 if not response:
                     logger.error("Failed to create workspace relationship.")
                     success = False
                 else:
                     logger.info("Successfully created workspace relationship.")
@@ -4269,41 +4279,41 @@
             if not workspace_node_id:
                 logger.warning(
                     "Workspace without node ID cannot have a members (workspaces creation may have failed) - skipping to next workspace..."
                 )
                 continue
 
             # now determine the actual node IDs of the workspaces (have been created by processWorkspaces()):
-            workspace_node = self._otcs.getNode(workspace_node_id)
-            workspace_owner_id = self._otcs.getResultValue(
+            workspace_node = self._otcs.get_node(workspace_node_id)
+            workspace_owner_id = self._otcs.get_result_value(
                 workspace_node, "owner_user_id"
             )
-            workspace_owner_name = self._otcs.getResultValue(workspace_node, "owner")
+            workspace_owner_name = self._otcs.get_result_value(workspace_node, "owner")
 
-            workspace_roles = self._otcs.getWorkspaceRoles(workspace_node_id)
+            workspace_roles = self._otcs.get_workspace_roles(workspace_node_id)
             if workspace_roles is None:
                 logger.info(
                     "Workspace with ID -> %s and node Id -> %s has no roles - skipping to next workspace...",
                     workspace_id,
                     workspace_node_id,
                 )
                 continue
 
             # We don't want the workspace creator to be in the leader role
             # of automatically created workspaces - this can happen because the
             # creator gets added to the leader role automatically:
-            leader_role_id = int(
-                self._otcs.lookupResultValue(workspace_roles, "leader", "True", "id")
+            leader_role_id = self._otcs.lookup_result_value(
+                workspace_roles, "leader", "True", "id"
             )
 
             if leader_role_id:
-                leader_role_name = self._otcs.lookupResultValue(
+                leader_role_name = self._otcs.lookup_result_value(
                     workspace_roles, "leader", str(True), "name"
                 )
-                response = self._otcs.removeMemberFromWorkspace(
+                response = self._otcs.remove_member_from_workspace(
                     workspace_node_id, leader_role_id, workspace_owner_id, False
                 )
                 if response:
                     logger.info(
                         "Removed creator user -> %s (%s) from leader role -> {%s (%s) of workspace -> %s",
                         workspace_owner_name,
                         workspace_owner_id,
@@ -4341,15 +4351,15 @@
                     logger.warning(
                         "Role -> %s of workspace -> %s does not have any members (no users nor groups).",
                         member_role_name,
                         workspace_name,
                     )
                     continue
 
-                role_id = self._otcs.lookupResultValue(
+                role_id = self._otcs.lookup_result_value(
                     workspace_roles, "name", member_role_name, "id"
                 )
                 if role_id is None:
                     #    if member_role is None:
                     logger.error(
                         "Workspace -> %s does not have a role with name -> %s",
                         workspace_name,
@@ -4372,30 +4382,30 @@
                         # If this didn't work, try to get the member user from OTCS. This covers
                         # cases where the user is system generated or part
                         # of a former payload processing (thus not in the current payload):
                         logger.info(
                             "Member -> %s not found in current payload - check if it exists in OTCS already...",
                             member_user,
                         )
-                        existing_user = self._otcs.getUser(member_user)
+                        existing_user = self._otcs.get_user(member_user)
                         if (
                             not existing_user or not existing_user["data"]
-                        ):  # we cannot use getResultValue() here - not a V2 call
+                        ):  # we cannot use get_result_value() here - not a V2 call
                             logger.error(
                                 "Cannot find member user with login -> %s. Skipping...",
                                 member_user,
                             )
                             continue
                         user_id = existing_user["data"][0][
                             "id"
-                        ]  # we cannot use getResultValue()here!
+                        ]  # we cannot use get_result_value()here!
 
                     # Add member if it does not yet exists - suppress warning
                     # message if user is already in role:
-                    response = self._otcs.addMemberToWorkspace(
+                    response = self._otcs.add_member_to_workspace(
                         workspace_node_id, int(role_id), user_id, False
                     )
                     if response is None:
                         logger.error(
                             "Failed to add user -> %s (%s) to role -> %s of workspace -> %s",
                             member_user_id["name"],
                             user_id,
@@ -4420,15 +4430,15 @@
                     )
                     if member_group_id is None:
                         logger.error("Cannot find group with name -> %s", member_group)
                         success = False
                         continue
                     group_id = member_group_id["id"]
 
-                    response = self._otcs.addMemberToWorkspace(
+                    response = self._otcs.add_member_to_workspace(
                         workspace_node_id, int(role_id), group_id
                     )
                     if response is None:
                         logger.error(
                             "Failed to add group -> %s (%s) to role -> %s of workspace -> %s",
                             member_group_id["name"],
                             group_id,
@@ -4484,27 +4494,27 @@
                 logger.info(
                     "Payload for Web Report -> %s is disabled. Skipping...", nick_name
                 )
                 continue
 
             description = web_report["description"]
 
-            if not self._otcs.getNodeFromNickname(nick_name):
+            if not self._otcs.get_node_from_nickname(nick_name):
                 logger.error(
                     "Web Report with nickname -> %s does not exist! Skipping...",
                     nick_name,
                 )
                 success = False
                 continue
 
             # be careful to avoid key errors as Web Report parameters are optional:
             actual_params = (
                 web_report["parameters"] if web_report.get("parameters") else {}
             )
-            formal_params = self._otcs.getWebReportParameters(nick_name)
+            formal_params = self._otcs.get_web_report_parameters(nick_name)
             if actual_params:
                 logger.info(
                     "Running Web Report -> %s (%s) with parameters -> %s ...",
                     nick_name,
                     description,
                     actual_params,
                 )
@@ -4551,15 +4561,15 @@
                         )
                         success = False
                         lets_continue = True  # we cannot do a "continue" here directly as we are in an inner loop
                 # Did any of the checks fail?
                 if lets_continue:
                     continue
                 # Actual parameters are validated, we can run the Web Report:
-                response = self._otcs.runWebReport(nick_name, actual_params)
+                response = self._otcs.run_web_report(nick_name, actual_params)
             else:
                 logger.info(
                     "Running Web Report -> %s (%s) without parameters...",
                     nick_name,
                     description,
                 )
                 # Check if there's a formal parameter that is mandatory but
@@ -4583,15 +4593,15 @@
                         success = False
                         continue
                     else:  # we are good to proceed!
                         logger.debug(
                             "Web Report -> %s does not have a mandatory parameter without a default value!",
                             nick_name,
                         )
-                response = self._otcs.runWebReport(nick_name)
+                response = self._otcs.run_web_report(nick_name)
             if response is None:
                 logger.error("Failed to run web report -> %s", nick_name)
                 success = False
 
         if success:
             self.writeStatusFile(section_name, web_reports)
 
@@ -4642,15 +4652,15 @@
             application_description = cs_application["description"]
 
             logger.info(
                 "Install CS Application -> %s (%s)...",
                 application_name,
                 application_description,
             )
-            response = otcs_object.installCSApplication(application_name)
+            response = otcs_object.install_cs_application(application_name)
             if response is None:
                 logger.error(
                     "Failed to install CS Application -> %s!", application_name
                 )
                 success = False
 
         if success:
@@ -4699,15 +4709,15 @@
                 continue
 
             # Set the OTDS display name. Extended ECM does not use this but
             # it makes AppWorks display users correctly (and it doesn't hurt)
             # We only set this if firstname _and_ last name are in the payload:
             if "firstname" in user and "lastname" in user:
                 user_display_name = user["firstname"] + " " + user["lastname"]
-                response = self._otds.updateUser(
+                response = self._otds.update_user(
                     user_partition, user_name, "displayName", user_display_name
                 )
                 if response:
                     logger.info(
                         "Display name for user -> %s has been updated to -> %s",
                         user_name,
                         user_display_name,
@@ -4718,15 +4728,15 @@
                         user_name,
                         user_display_name,
                     )
                     success = False
 
             # Don't enforce the user to reset password at first login (settings in OTDS):
             logger.info("Don't enforce password change for user -> %s...", user_name)
-            response = self._otds.updateUser(
+            response = self._otds.update_user(
                 user_partition, user_name, "UserMustChangePasswordAtNextSignIn", "False"
             )
             if not response:
                 success = False
 
         if success:
             self.writeStatusFile(section_name, self._users)
@@ -4779,27 +4789,27 @@
                     "Payload for User -> %s is disabled. Skipping...", user_name
                 )
                 continue
 
             user_password = user["password"]
 
             # we change the otcs credentials to the user:
-            self._otcs.setCredentials(user_name, user_password)
+            self._otcs.set_credentials(user_name, user_password)
 
             # we re-authenticate as the user:
             logger.info("Authenticate user -> %s...", user_name)
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
             if not cookie:
                 logger.error("Couldn't authenticate user -> %s", user_name)
                 success = False
                 continue
 
             # we update the user profile to activate navigation tree:
-            response = self._otcs.updateUserProfile("conwsNavigationTreeView", True)
+            response = self._otcs.update_user_profile("conwsNavigationTreeView", True)
             if response is None:
                 logger.warning("Profile for user -> %s couldn't be updated!", user_name)
             else:
                 logger.info(
                     "Profile for user -> %s has been updated to enable Workspace Navigation Tree.",
                     user_name,
                 )
@@ -4825,25 +4835,25 @@
                             favorite_item["name"],
                         )
                         continue
 
                     is_workspace = True
                 else:
                     # alternatively try to find the item as a nickname:
-                    favorite_item = self._otcs.getNodeFromNickname(favorite)
-                    favorite_id = self._otcs.getResultValue(favorite_item, "id")
+                    favorite_item = self._otcs.get_node_from_nickname(favorite)
+                    favorite_id = self._otcs.get_result_value(favorite_item, "id")
                     #                    if favorite_item is None:
                     if favorite_id is None:
                         logger.warning(
                             "Favorite -> %s neither found as workspace ID nor as nickname - skipping to next favorite...",
                             favorite,
                         )
                         continue
 
-                response = self._otcs.addFavorite(favorite_id)
+                response = self._otcs.add_favorite(favorite_id)
                 if response is None:
                     logger.warning(
                         "Favorite ID -> %s couldn't be added for user -> %s!",
                         favorite_id,
                         user_name,
                     )
                 else:
@@ -4855,17 +4865,17 @@
                     logger.info(
                         "Simulate user -> %s browsing node ID -> %s.",
                         user_name,
                         favorite_id,
                     )
                     # simulate a browse by the user to populate recently accessed items
                     if is_workspace:
-                        response = self._otcs.getWorkspace(favorite_id)
+                        response = self._otcs.get_workspace(favorite_id)
                     else:
-                        response = self._otcs.getNode(favorite_id)
+                        response = self._otcs.get_node(favorite_id)
 
             # we work through the list of proxies defined for the user
             # (we need to consider that not all users have the proxies element):
             proxies = user["proxies"] if user.get("proxies") else []
 
             for proxy in proxies:
                 proxy_user = next(
@@ -4879,34 +4889,34 @@
                         user_name,
                     )
                     success = False
                     continue
                 proxy_user_id = proxy_user["id"]
 
                 # Check if the proxy is already set:
-                if not self._otcs.isProxy(proxy):
+                if not self._otcs.is_proxy(proxy):
                     logger.info(
                         "Set user -> %s (%s) as proxy for user -> %s.",
                         proxy,
                         proxy_user_id,
                         user_name,
                     )
                     # set the user proxy - currently we don't support time based proxies in payload.
                     # The called method is ready to support this.
-                    response = self._otcs.updateUserProxy(proxy_user_id)
+                    response = self._otcs.update_user_proxy(proxy_user_id)
                 else:
                     logger.info(
                         "User -> %s (%s) is already proxy for user -> %s. Skipping...",
                         proxy,
                         proxy_user_id,
                         user_name,
                     )
         if self._users:
             # Set back admin credentials:
-            self._otcs.setCredentials(
+            self._otcs.set_credentials(
                 admin_credentials["username"], admin_credentials["password"]
             )
 
             # we re-authenticate as the admin user:
             logger.info(
                 "Authenticate as admin user -> %s...", admin_credentials["username"]
             )
@@ -4958,15 +4968,15 @@
                 clearance_description = ""
             if clearance_level and clearance_name:
                 logger.info(
                     "Creating Security Clearance -> %s : %s",
                     clearance_level,
                     clearance_name,
                 )
-                self._otcs.runWebReport(
+                self._otcs.run_web_report(
                     "web_report_security_clearance", security_clearance
                 )
             else:
                 logger.error(
                     "Cannot create Security Clearance - either level or name is missing!"
                 )
                 success = False
@@ -5016,15 +5026,15 @@
             description = supplemental_marking.get("description")
             if not description:
                 description = ""
             if code:
                 logger.info(
                     "Creating Supplemental Marking -> %s : %s", code, description
                 )
-                self._otcs.runWebReport(
+                self._otcs.run_web_report(
                     "web_report_supplemental_marking", supplemental_marking
                 )
             else:
                 logger.error(
                     "Cannot create Supplemental Marking - either code or description is missing!"
                 )
                 success = False
@@ -5067,20 +5077,22 @@
                     "Payload for User -> %s is disabled. Skipping...", user_name
                 )
                 continue
 
             # Read security clearance from user payload (it is optional!)
             user_security_clearance = user.get("security_clearance")
             if user_id and user_security_clearance:
-                self._otcs.assignUserSecurityClearance(user_id, user_security_clearance)
+                self._otcs.assign_user_security_clearance(
+                    user_id, user_security_clearance
+                )
 
             # Read supplemental markings from user payload (it is optional!)
             user_supplemental_markings = user.get("supplemental_markings")
             if user_id and user_supplemental_markings:
-                self._otcs.assignUserSupplementalMarkings(
+                self._otcs.assign_user_supplemental_markings(
                     user_id, user_supplemental_markings
                 )
 
         if success:
             self.writeStatusFile(section_name, self._users)
 
         return success
@@ -5116,88 +5128,88 @@
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings[
                     "records_management_system_settings"
                 ]
             )
-            response = self._otcs.importRecordsManagementSettings(filename)
+            response = self._otcs.import_records_management_settings(filename)
             if not response:
                 success = False
 
         if (
             "records_management_codes" in self._records_management_settings
             and self._records_management_settings["records_management_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["records_management_codes"]
             )
-            response = self._otcs.importRecordsManagementCodes(filename)
+            response = self._otcs.import_records_management_codes(filename)
             if not response:
                 success = False
 
         if (
             "records_management_rsis" in self._records_management_settings
             and self._records_management_settings["records_management_rsis"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["records_management_rsis"]
             )
-            response = self._otcs.importRecordsManagementRSIs(filename)
+            response = self._otcs.import_records_management_rsis(filename)
             if not response:
                 success = False
 
         if (
             "physical_objects_system_settings" in self._records_management_settings
             and self._records_management_settings["physical_objects_system_settings"]
             != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_system_settings"]
             )
-            response = self._otcs.importPhysicalObjectsSettings(filename)
+            response = self._otcs.import_physical_objects_settings(filename)
             if not response:
                 success = False
 
         if (
             "physical_objects_codes" in self._records_management_settings
             and self._records_management_settings["physical_objects_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_codes"]
             )
-            response = self._otcs.importPhysicalObjectsCodes(filename)
+            response = self._otcs.import_physical_objects_codes(filename)
             if not response:
                 success = False
 
         if (
             "physical_objects_locators" in self._records_management_settings
             and self._records_management_settings["physical_objects_locators"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_locators"]
             )
-            response = self._otcs.importPhysicalObjectsLocators(filename)
+            response = self._otcs.import_physical_objects_locators(filename)
             if not response:
                 success = False
 
         if (
             "security_clearance_codes" in self._records_management_settings
             and self._records_management_settings["security_clearance_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["security_clearance_codes"]
             )
-            response = self._otcs.importSecurityClearanceCodes(filename)
+            response = self._otcs.import_security_clearance_codes(filename)
             if not response:
                 success = False
 
         if success:
             self.writeStatusFile(section_name, self._records_management_settings)
 
         return success
@@ -5253,34 +5265,34 @@
             hold_date_suspend = hold.get("date_to_remove")
 
             if hold_group:
                 # Check if the Hold Group (folder) does already exist.
                 # 2122 is the ID of the "Hold Maintenance" top level
                 # folder in Records Management area that (we hope) will remain
                 # stable:
-                response = self._otcs.getNodeByParentAndName(2122, hold_group)
-                parent_id = self._otcs.getResultValue(response, "id")
+                response = self._otcs.get_node_by_parent_and_name(2122, hold_group)
+                parent_id = self._otcs.get_result_value(response, "id")
                 if not parent_id:
-                    response = self._otcs.createItem(2122, "833", hold_group)
-                    parent_id = self._otcs.getResultValue(response, "id")
+                    response = self._otcs.create_item(2122, "833", hold_group)
+                    parent_id = self._otcs.get_result_value(response, "id")
             else:
                 parent_id = 2122
 
             # Holds are special - they ahve folders that cannot be traversed
             # in the normal way - we need to get the whole list of holds and use
-            # specialparameters for the existResultItems() method as the REST
+            # specialparameters for the exist_result_items() method as the REST
             # API calls delivers a results->data->holds structure (not properties)
-            response = self._otcs.getRecordsManagementHolds()
-            if self._otcs.existResultItem(
+            response = self._otcs.get_records_management_holds()
+            if self._otcs.exist_result_item(
                 response, "HoldName", hold_name, property_name="holds"
             ):
                 logger.info("Hold -> %s does already exist. Skipping...", hold_name)
                 continue
 
-            hold = self._otcs.createRecordsManagementHold(
+            hold = self._otcs.create_records_management_hold(
                 hold_type,
                 hold_name,
                 hold_comment,
                 hold_alternate_id,
                 int(parent_id),
                 hold_date_applied,
                 hold_date_suspend,
@@ -5351,28 +5363,30 @@
             if "group_name" in additional_group_member:
                 group_name = additional_group_member["group_name"]
                 logger.info(
                     "Adding group -> %s to parent group -> %s in OTDS.",
                     group_name,
                     parent_group,
                 )
-                response = self._otds.addGroupToParentGroup(group_name, parent_group)
+                response = self._otds.add_group_to_parent_group(
+                    group_name, parent_group
+                )
                 if not response:
                     logger.error(
                         "Failed to add group -> %s to parent group -> %s in OTDS.",
                         group_name,
                         parent_group,
                     )
                     success = False
             elif "user_name" in additional_group_member:
                 user_name = additional_group_member["user_name"]
                 logger.info(
                     "Adding user -> %s to group -> %s in OTDS.", user_name, parent_group
                 )
-                response = self._otds.addUserToGroup(user_name, parent_group)
+                response = self._otds.add_user_to_group(user_name, parent_group)
                 if not response:
                     logger.error(
                         "Failed to add user -> %s to group -> %s in OTDS.",
                         user_name,
                         parent_group,
                     )
                     success = False
@@ -5435,45 +5449,45 @@
             if "group_name" in additional_access_role_member:
                 group_name = additional_access_role_member["group_name"]
                 logger.info(
                     "Adding group -> %s to access role -> %s in OTDS.",
                     group_name,
                     access_role,
                 )
-                response = self._otds.addGroupToAccessRole(access_role, group_name)
+                response = self._otds.add_group_to_access_role(access_role, group_name)
                 if not response:
                     logger.error(
                         "Failed to add group -> %s to access role -> %s in OTDS.",
                         group_name,
                         access_role,
                     )
                     success = False
             elif "user_name" in additional_access_role_member:
                 user_name = additional_access_role_member["user_name"]
                 logger.info(
                     "Adding user -> %s to access role -> %s in OTDS.",
                     user_name,
                     access_role,
                 )
-                response = self._otds.addUserToAccessRole(access_role, user_name)
+                response = self._otds.add_user_to_access_role(access_role, user_name)
                 if not response:
                     logger.error(
                         "Failed to add user -> %s to access role -> %s in OTDS.",
                         user_name,
                         access_role,
                     )
                     success = False
             elif "partition_name" in additional_access_role_member:
                 partition_name = additional_access_role_member["partition_name"]
                 logger.info(
                     "Adding partition -> %s to access role -> %s in OTDS.",
                     partition_name,
                     access_role,
                 )
-                response = self._otds.addPartitionToAccessRole(
+                response = self._otds.add_partition_to_access_role(
                     access_role, partition_name
                 )
                 if not response:
                     logger.error(
                         "Failed to add partition -> %s to access role -> %s in OTDS.",
                         partition_name,
                         access_role,
@@ -5511,26 +5525,26 @@
             if not "nodeid" in renaming:
                 if not "volume" in renaming:
                     logger.error(
                         "Renamings require either a node ID or a volume! Skipping to next renaming..."
                     )
                     continue
                 # Determine object ID of volume:
-                volume = self._otcs.getVolume(renaming["volume"])
-                node_id = self._otcs.getResultValue(volume, "id")
+                volume = self._otcs.get_volume(renaming["volume"])
+                node_id = self._otcs.get_result_value(volume, "id")
             else:
                 node_id = renaming["nodeid"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in renaming and not renaming["enabled"]:
                 logger.info("Payload for Renaming is disabled. Skipping...")
                 continue
 
-            response = self._otcs.renameNode(
+            response = self._otcs.rename_node(
                 int(node_id), renaming["name"], renaming["description"]
             )
             if not response:
                 logger.error(
                     "Failed to rename node ID -> %s to new name -> %s.",
                     node_id,
                     renaming["name"],
@@ -5585,55 +5599,57 @@
             else:
                 item_description = item["description"]
 
             parent_nickname = item.get("parent_nickname")
             parent_path = item.get("parent_path")
 
             if parent_nickname:
-                parent_node = self._otcs.getNodeFromNickname(parent_nickname)
-                parent_id = self._otcs.getResultValue(parent_node, "id")
+                parent_node = self._otcs.get_node_from_nickname(parent_nickname)
+                parent_id = self._otcs.get_result_value(parent_node, "id")
                 # if not parent_node:
                 if not parent_id:
                     logger.error(
                         "Item -> %s has a parent nickname -> %s that does not exist. Skipping...",
                         item_name,
                         parent_nickname,
                     )
                     success = False
                     continue
             else:  # use parent_path and Enterprise Volume
-                parent_node = self._otcs.getNodeByVolumeAndPath(141, parent_path)
-                parent_id = self._otcs.getResultValue(parent_node, "id")
+                parent_node = self._otcs.get_node_by_volume_and_path(141, parent_path)
+                parent_id = self._otcs.get_result_value(parent_node, "id")
                 if not parent_id:
                     # if not parent_node:
                     logger.error(
                         "Item -> %s has a parent path that does not exist. Skipping...",
                         item_name,
                     )
                     success = False
                     continue
 
             original_nickname = item.get("original_nickname")
             original_path = item.get("original_path")
 
             if original_nickname:
-                original_node = self._otcs.getNodeFromNickname(original_nickname)
-                original_id = self._otcs.getResultValue(original_node, "id")
+                original_node = self._otcs.get_node_from_nickname(original_nickname)
+                original_id = self._otcs.get_result_value(original_node, "id")
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> %s has a original nickname -> %s that does not exist. Skipping...",
                         item_name,
                         original_nickname,
                     )
                     success = False
                     continue
             elif original_path:
-                original_node = self._otcs.getNodeByVolumeAndPath(141, original_path)
-                original_id = self._otcs.getResultValue(original_node, "id")
+                original_node = self._otcs.get_node_by_volume_and_path(
+                    141, original_path
+                )
+                original_id = self._otcs.get_result_value(original_node, "id")
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> %s has a original path that does not exist. Skipping...",
                         item_name,
                     )
                     success = False
@@ -5668,25 +5684,25 @@
                         )
                         success = False
                         continue
 
             # Check if an item with the same name does already exist.
             # This can also be the case if the python container runs a 2nd time.
             # For this reason we are also not issuing an error but just an info (False):
-            response = self._otcs.getNodeByParentAndName(
+            response = self._otcs.get_node_by_parent_and_name(
                 int(parent_id), item_name, show_error=False
             )
-            if self._otcs.getResultValue(response, "name") == item_name:
+            if self._otcs.get_result_value(response, "name") == item_name:
                 logger.info(
                     "Item with name -> %s does already exist in parent folder with ID -> %s",
                     item_name,
                     parent_id,
                 )
                 continue
-            response = self._otcs.createItem(
+            response = self._otcs.create_item(
                 int(parent_id),
                 str(item_type),
                 item_name,
                 item_description,
                 item_url,
                 int(original_id),
             )
@@ -5767,16 +5783,16 @@
             # Check if "volume" is in payload and not empty string:
             if "volume" in permission and permission["volume"]:
                 volume_type = permission["volume"]
                 logger.info(
                     "Found volume type -> %s in permission definition. Determine volume ID...",
                     volume_type,
                 )
-                volume = self._otcs.getVolume(volume_type)
-                node_id = self._otcs.getResultValue(volume, "id")
+                volume = self._otcs.get_volume(volume_type)
+                node_id = self._otcs.get_result_value(volume, "id")
                 if not node_id:
                     logger.error(
                         "Illegal volume -> %s in permission specification. Skipping...",
                         volume_type,
                     )
                     success = False
                     continue
@@ -5787,44 +5803,44 @@
             # (path can be combined with volume so we need to take volume into account):
             if "path" in permission and permission["path"]:
                 path = permission["path"]
                 logger.info(
                     "Found path -> %s in permission definition. Determine node ID...",
                     path,
                 )
-                node = self._otcs.getNodeByVolumeAndPath(volume_type, path)
-                node_id = self._otcs.getResultValue(node, "id")
+                node = self._otcs.get_node_by_volume_and_path(volume_type, path)
+                node_id = self._otcs.get_result_value(node, "id")
                 if not node_id:
                     logger.error("Path -> %s does not exist. Skipping...", path)
                     success = False
                     continue
 
             # Check if "nickname" is in payload and not empty string:
             if "nickname" in permission and permission["nickname"]:
                 nickname = permission["nickname"]
                 logger.info(
                     "Found nickname -> %s in permission definition. Determine node ID...",
                     nickname,
                 )
-                node = self._otcs.getNodeFromNickname(nickname)
-                node_id = self._otcs.getResultValue(node, "id")
+                node = self._otcs.get_node_from_nickname(nickname)
+                node_id = self._otcs.get_result_value(node, "id")
                 if not node_id:
                     logger.error("Nickname -> {} does not exist. Skipping...")
                     success = False
                     continue
             else:
                 continue
 
             # Now we should have a value for node_id:
             if not node_id:
                 logger.error("No node ID found! Skipping permission...")
                 success = False
                 continue
 
-            node_name = self._otcs.getResultValue(node, "name")
+            node_name = self._otcs.get_result_value(node, "name")
             logger.info(
                 "Found node -> %s with ID -> %s to apply permission to.",
                 node_name,
                 node_id,
             )
 
             if "apply_to" in permission:
@@ -5836,15 +5852,15 @@
             if "owner_permissions" in permission:
                 permissions = permission["owner_permissions"]
                 logger.info(
                     "Update owner permissions for item -> %s to -> %s",
                     node_id,
                     permissions,
                 )
-                response = self._otcs.assignPermission(
+                response = self._otcs.assign_permission(
                     int(node_id), "owner", 0, permissions, apply_to
                 )
                 if not response:
                     logger.error(
                         "Failed to update owner permissions for item -> %s.", node_id
                     )
                     success = False
@@ -5853,15 +5869,15 @@
             if "owner_group_permissions" in permission:
                 permissions = permission["owner_group_permissions"]
                 logger.info(
                     "Update owner group permissions for item -> %s to -> %s",
                     node_id,
                     permissions,
                 )
-                response = self._otcs.assignPermission(
+                response = self._otcs.assign_permission(
                     int(node_id), "group", 0, permissions, apply_to
                 )
                 if not response:
                     logger.error(
                         "Failed to update group permissions for item -> %s.", node_id
                     )
                     success = False
@@ -5870,15 +5886,15 @@
             if "public_permissions" in permission:
                 permissions = permission["public_permissions"]
                 logger.info(
                     "Update public permissions for item -> %s to -> %s",
                     node_id,
                     permissions,
                 )
-                response = self._otcs.assignPermission(
+                response = self._otcs.assign_permission(
                     int(node_id), "public", 0, permissions, apply_to
                 )
                 if not response:
                     logger.error(
                         "Failed to update public permissions for item -> %s.", node_id
                     )
                     success = False
@@ -5892,30 +5908,30 @@
                         logger.error(
                             "Missing user name or permissions in user permission specificiation. Cannot set user permissions. Skipping..."
                         )
                         success = False
                         continue
                     user_name = user["name"]
                     permissions = user["permissions"]
-                    otcs_user = self._otcs.getUser(user_name, True)
+                    otcs_user = self._otcs.get_user(user_name, True)
                     if not otcs_user or not otcs_user["data"]:
                         logger.error(
                             "Cannot find user with name -> %s; cannot set user permissions. Skipping user...",
                             user_name,
                         )
                         success = False
                         continue
                     user_id = otcs_user["data"][0]["id"]
                     logger.info(
                         "Update user -> %s permissions for item -> %s to -> %s",
                         user_name,
                         node_id,
                         permissions,
                     )
-                    response = self._otcs.assignPermission(
+                    response = self._otcs.assign_permission(
                         int(node_id), "custom", user_id, permissions, apply_to
                     )
                     if not response:
                         logger.error(
                             "Failed to update assigned user permissions for item -> %s.",
                             node_id,
                         )
@@ -5934,24 +5950,24 @@
                     permissions = group["permissions"]
                     logger.info(
                         "Update group -> %s permissions for item -> %s to -> %s",
                         group_name,
                         node_id,
                         permissions,
                     )
-                    otcs_group = self._otcs.getGroup(group_name, True)
+                    otcs_group = self._otcs.get_group(group_name, True)
                     if not otcs_group or not otcs_group["data"]:
                         logger.error(
                             "Cannot find group with name -> %s; cannot set group permissions. Skipping group...",
                             group_name,
                         )
                         success = False
                         continue
                     group_id = otcs_group["data"][0]["id"]
-                    response = self._otcs.assignPermission(
+                    response = self._otcs.assign_permission(
                         int(node_id), "custom", group_id, permissions, apply_to
                     )
                     if not response:
                         logger.error(
                             "Failed to update assigned group permissions for item -> %s.",
                             node_id,
                         )
@@ -6040,16 +6056,16 @@
                         subject,
                         assignment["workspace"],
                     )
                     success = False
                     continue
             # If we don't have a workspace then check if a nickname is specified for the assignment:
             elif "nickname" in assignment:
-                response = self._otcs.getNodeFromNickname(assignment["nickname"])
-                node_id = self._otcs.getResultValue(response, "id")
+                response = self._otcs.get_node_from_nickname(assignment["nickname"])
+                node_id = self._otcs.get_result_value(response, "id")
                 if not node_id:
                     # if response == None:
                     logger.error(
                         "Assignment item with nickname -> %s not found",
                         assignment["nickname"],
                     )
                     success = False
@@ -6125,15 +6141,15 @@
                     "Cannot add assignment -> %s for node ID -> %s because no assignee was found.",
                     subject,
                     node_id,
                 )
                 success = False
                 continue
 
-            response = self._otcs.assignItemToUserGroup(
+            response = self._otcs.assign_item_to_user_group(
                 int(node_id), subject, instruction, assignees
             )
             if not response:
                 logger.error(
                     "Failed to add assignment -> %s for node ID -> %s with assignees -> %s.",
                     subject,
                     node_id,
@@ -6176,15 +6192,15 @@
         # if this payload section has been processed successfully before we can return True
         # and skip processing once more
         if self.checkStatusFile(section_name):
             return True
 
         success: bool = True
 
-        otds_resource = self._otds.getResource(resource_name)
+        otds_resource = self._otds.get_resource(resource_name)
         if not otds_resource:
             logger.error(
                 "OTDS Resource -> {} not found. Cannot assign licenses to users."
             )
             return False
 
         user_partition = self._otcs.config()["partition"]
@@ -6211,28 +6227,28 @@
                     license_feature,
                 )
                 user_license_feature = user[user_specific_payload_field]
             else:  # use the default feature from the actual parameter
                 user_license_feature = [license_feature]
 
             for license_feature in user_license_feature:
-                if self._otds.isUserLicensed(
+                if self._otds.is_user_licensed(
                     user_name=user_name,
                     resource_id=otds_resource["resourceID"],
                     license_feature=license_feature,
                     license_name=license_name,
                 ):
                     logger.info(
                         "User -> %s is already licensed for -> %s (%s)",
                         user_name,
                         license_name,
                         license_feature,
                     )
                     continue
-                assigned_license = self._otds.assignUserToLicense(
+                assigned_license = self._otds.assign_user_to_license(
                     user_partition,
                     user_name,  # we want the plain login name here
                     otds_resource["resourceID"],
                     license_feature,
                     license_name,
                 )
 
@@ -6314,21 +6330,21 @@
                     description,
                 )
 
             if (
                 not "interactive" in exec_pod_command
                 or exec_pod_command["interactive"] is False
             ):
-                result = self._k8s.execPodCommand(pod_name, command)
+                result = self._k8s.exec_pod_command(pod_name, command)
             else:
                 if not "timeout" in exec_pod_command:
-                    result = self._k8s.execPodCommandInteractive(pod_name, command)
+                    result = self._k8s.exec_pod_command_interactive(pod_name, command)
                 else:
                     timeout = exec_pod_command["timeout"]
-                    result = self._k8s.execPodCommandInteractive(
+                    result = self._k8s.exec_pod_command_interactive(
                         pod_name, command, timeout
                     )
 
             if result:
                 logger.info(
                     "Execution of command -> %s in pod -> %s returned result -> %s",
                     command,
@@ -6452,15 +6468,15 @@
                 )
                 # Have we found the user in the payload?
                 if exec_user is not None:
                     logger.info(
                         "Executing document generator with user -> %s", exec_as_user
                     )
                     # we change the otcs credentials to the user:
-                    self._otcs.setCredentials(exec_user["name"], exec_user["password"])
+                    self._otcs.set_credentials(exec_user["name"], exec_user["password"])
 
                     # we re-authenticate as the user:
                     logger.info("Authenticate user -> %s...", exec_as_user)
                     # True = force new login with new user
                     cookie = self._otcs.authenticate(True)
                     if not cookie:
                         logger.error("Couldn't authenticate user -> %s", exec_as_user)
@@ -6475,35 +6491,38 @@
                     admin_context = True
                     success = False
             else:
                 admin_context = True
 
             if admin_context and authenticated_user != "admin":
                 # Set back admin credentials:
-                self._otcs.setCredentials(
+                self._otcs.set_credentials(
                     admin_credentials["username"], admin_credentials["password"]
                 )
 
                 # we re-authenticate as the admin user:
                 logger.info(
                     "Authenticate as admin user -> %s...", admin_credentials["username"]
                 )
                 # True = force new login with new user
                 cookie = self._otcs.authenticate(True)
                 authenticated_user = "admin"
 
-            template = self._otcs.getNodeByVolumeAndPath(20541, template_path)
-            template_id = self._otcs.getResultValue(template, "id")
-            template_name = self._otcs.getResultValue(template, "name")
-            classification = self._otcs.getNodeByVolumeAndPath(198, classification_path)
-            classification_id = self._otcs.getResultValue(classification, "id")
-
-            category_id, attribute_definitions = self._otcs.getNodeCategoryDefinition(
-                template_id, category_name
+            template = self._otcs.get_node_by_volume_and_path(20541, template_path)
+            template_id = self._otcs.get_result_value(template, "id")
+            template_name = self._otcs.get_result_value(template, "name")
+            classification = self._otcs.get_node_by_volume_and_path(
+                198, classification_path
             )
+            classification_id = self._otcs.get_result_value(classification, "id")
+
+            (
+                category_id,
+                attribute_definitions,
+            ) = self._otcs.get_node_category_definition(template_id, category_name)
             logger.info(
                 "Category ID -> %s, Attribute definitions -> %s",
                 category_id,
                 attribute_definitions,
             )
 
             category_data = {str(category_id): {}}
@@ -6513,15 +6532,15 @@
                 attribute_value = attribute["value"]
                 attribute_type = attribute_definitions[attribute_name]["type"]
                 attribute_id = attribute_definitions[attribute_name]["id"]
 
                 # Special treatment for type user: determine the ID for the login name.
                 # the ID is the actual value we have to put in the attribute:
                 if attribute_type == "user":
-                    user = self._otcs.getUser(attribute_value, show_error=True)
+                    user = self._otcs.get_user(attribute_value, show_error=True)
 
                     if not user or not user["data"]:
                         logger.error(
                             "Cannot find user with login name -> %s. Skipping...",
                             attribute_value,
                         )
                         success = False
@@ -6533,24 +6552,24 @@
             logger.info(
                 "Generate documents for workspace type -> %s based on template -> %s with metadata -> %s...",
                 workspace_type,
                 template_name,
                 category_data,
             )
 
-            workspace_instances = self._otcs.getWorkspaceInstances(workspace_type)
+            workspace_instances = self._otcs.get_workspace_instances(workspace_type)
             for workspace_instance in workspace_instances["results"]:
                 workspace_id = workspace_instance["data"]["properties"]["id"]
                 workspace_name = workspace_instance["data"]["properties"]["name"]
                 if workspace_folder_path:
-                    workspace_folder = self._otcs.getNodeByWorkspaceAndPath(
+                    workspace_folder = self._otcs.get_node_by_workspace_and_path(
                         workspace_id, workspace_folder_path
                     )
                     if workspace_folder:
-                        workspace_folder_id = self._otcs.getResultValue(
+                        workspace_folder_id = self._otcs.get_result_value(
                             workspace_folder, "id"
                         )
                     else:
                         # If the workspace template is not matching
                         # the path we may have an error here. Then
                         # we fall back to workspace root level.
                         logger.info(
@@ -6559,25 +6578,25 @@
                         )
                         workspace_folder_id = workspace_id
                 else:
                     workspace_folder_id = workspace_id
 
                 document_name = workspace_name + " - " + template_name
 
-                response = self._otcs.checkNodeName(
+                response = self._otcs.check_node_name(
                     int(workspace_folder_id), document_name
                 )
                 if response["results"]:
                     logger.warning(
                         "Node with name -> %s does already exist in workspace folder with ID -> %s",
                         document_name,
                         workspace_folder_id,
                     )
                     continue
-                response = self._otcs.createDocumentFromTemplate(
+                response = self._otcs.create_document_from_template(
                     int(template_id),
                     int(workspace_folder_id),
                     int(classification_id),
                     category_data,
                     document_name,
                     "This document has been auto-generated by Terrarium",
                 )
@@ -6593,15 +6612,15 @@
                         "Successfully generated document -> %s in workspace -> %s",
                         document_name,
                         workspace_name,
                     )
 
         if authenticated_user != "admin":
             # Set back admin credentials:
-            self._otcs.setCredentials(
+            self._otcs.set_credentials(
                 admin_credentials["username"], admin_credentials["password"]
             )
 
             # we authenticate back as the admin user:
             logger.info(
                 "Authenticate as admin user -> %s...", admin_credentials["username"]
             )
```

### Comparing `pyxecm-0.2.0/pyxecm/sap.py` & `pyxecm-0.3.0/pyxecm/customizer/sap.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 * client (the client or "Mandant" to which to logon, e.g. 100)
 * user (e.g. "nwheeler")
 * passwd (password of the user)
 * lang (logon language as two-character ISO-Code, e.g. EN)
 * trace (on of 0(off), 1(brief), 2(verbose), 3(detailed), 4(full))
 * use_tls (activates SSL/TLS encryption. Set to 0 or 1. By default TLS is turned on (1))
 * tls_client_pse (Specifies the PSE file containing the necessary certificates for TLS communication.
-                  A PSE file is a SAP proprietary certificate store, similar to a p12 file, containing the private key and
-                  the certificate chain to be used in the TLS handshake with the server, beginning with the server's public
-                  certificate and ending with the root CA certifcate. It should also contain the client certificate used for
-                  login at the server, if your client program does not use basic user & password authentication)
+                  A PSE file is a SAP proprietary certificate store, similar to a p12 file,
+                  containing the private key and the certificate chain to be used in the TLS
+                  handshake with the server, beginning with the server's public certificate and
+                  ending with the root CA certifcate. It should also contain the client certificate
+                  used for login at the server, if your client program does not use basic
+                  user & password authentication)
 
 Class: SAP
 Methods:
 
 __init__ : class initializer
 call: Calls and RFC based on its name and passes parameters.
 
@@ -36,25 +38,25 @@
 __email__ = "mdiefenb@opentext.com"
 
 import logging
 
 try:
     import pyrfc
 
-    pyrfc_available = True
+    _has_pyrfc = True
 
 except ModuleNotFoundError as e:
-    logging.error("pyrfc could not be loaded, SAP integration impatcted: %s", e)
-    pyrfc_available = False
+    logging.error("pyrfc not installed, SAP integration impatcted")
+    _has_pyrfc = False
 
 except ImportError as e:
-    logging.error("pyrfc could not be loaded, SAP integration impatcted: %s", e)
-    pyrfc_available = False
+    logging.error("pyrfc could not be loaded, SAP integration impatcted")
+    _has_pyrfc = False
 
-logger = logging.getLogger("customizer.sap")
+logger = logging.getLogger("pyxecm.customizer.sap")
 
 
 class SAP(object):
     """Used to implement Remote Function Calls (RFC) to SAP S/4HANA"""
 
     _connection_parameters = {}
 
@@ -68,14 +70,15 @@
         msport: str = "3601",
         group: str = "PUBLIC",
         destination: str = "",
         client: str = "100",
         system_number: str = "00",
         lang: str = "EN",
         trace: str = "3",
+        **kwargs,
     ):
         """Initialize the SAP object."""
 
         logger.info("Initializing SAP object...")
         logger.info("Using PyRFC version -> %s", pyrfc.__version__)
 
         # Set up connection parameters
```

### Comparing `pyxecm-0.2.0/pyxecm/translate.py` & `pyxecm-0.3.0/pyxecm/customizer/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import logging
 
 import requests
 
-logger = logging.getLogger("customizer.translate")
+logger = logging.getLogger("pyxecm.customizer.translate")
 
 
 class Translator:
     _config = None
     _headers = None
 
     def __init__(self, api_key: str, project_key: str = "", domain: str = ""):
```

### Comparing `pyxecm-0.2.0/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.3.0/pyxecm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: customizer
 License-File: LICENSE
 
 # PYXECM
 
 A python library to interact with Opentext Extended ECM REST API. 
 API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
```

