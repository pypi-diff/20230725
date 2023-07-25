# Comparing `tmp/iomete_sdk-1.1.0.tar.gz` & `tmp/iomete_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iomete_sdk-1.1.0.tar", last modified: Wed Jul 19 23:25:35 2023, max compression
+gzip compressed data, was "iomete_sdk-1.2.0.tar", last modified: Tue Jul 25 03:47:10 2023, max compression
```

## Comparing `iomete_sdk-1.1.0.tar` & `iomete_sdk-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.952982 iomete_sdk-1.1.0/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-19 23:25:35.953036 iomete_sdk-1.1.0/PKG-INFO
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2038 2023-07-19 22:03:57.000000 iomete_sdk-1.1.0/README.md
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       38 2023-07-19 23:25:35.953189 iomete_sdk-1.1.0/setup.cfg
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     1407 2023-07-19 22:03:57.000000 iomete_sdk-1.1.0/setup.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.949592 iomete_sdk-1.1.0/src/
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.950171 iomete_sdk-1.1.0/src/iomete_sdk/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     1298 2023-07-19 11:02:26.000000 iomete_sdk-1.1.0/src/iomete_sdk/api_utils.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.951664 iomete_sdk-1.1.0/src/iomete_sdk/security/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       68 2023-07-17 22:30:18.000000 iomete_sdk-1.1.0/src/iomete_sdk/security/__init__.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     7340 2023-07-19 22:02:18.000000 iomete_sdk-1.1.0/src/iomete_sdk/security/data_security.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2281 2023-07-19 11:57:58.000000 iomete_sdk-1.1.0/src/iomete_sdk/security/policy_models.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.952088 iomete_sdk-1.1.0/src/iomete_sdk/spark/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       57 2023-07-17 22:30:18.000000 iomete_sdk-1.1.0/src/iomete_sdk/spark/__init__.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2658 2023-07-18 22:38:50.000000 iomete_sdk-1.1.0/src/iomete_sdk/spark/spark_job.py
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.950935 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-19 23:25:35.000000 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/PKG-INFO
--rw-r--r--   0 fuadmusayev   (501) staff       (20)      504 2023-07-19 23:25:35.000000 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)        1 2023-07-19 23:25:35.000000 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       56 2023-07-19 23:25:35.000000 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/requires.txt
--rw-r--r--   0 fuadmusayev   (501) staff       (20)       11 2023-07-19 23:25:35.000000 iomete_sdk-1.1.0/src/iomete_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-19 23:25:35.952690 iomete_sdk-1.1.0/tests/
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     5670 2023-07-19 11:57:22.000000 iomete_sdk-1.1.0/tests/test_data_security_api_client.py
--rw-r--r--   0 fuadmusayev   (501) staff       (20)     4529 2023-07-18 20:56:50.000000 iomete_sdk-1.1.0/tests/test_spark_job_api_client.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.820174 iomete_sdk-1.2.0/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-25 03:47:10.820223 iomete_sdk-1.2.0/PKG-INFO
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2038 2023-07-19 22:03:57.000000 iomete_sdk-1.2.0/README.md
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       38 2023-07-25 03:47:10.820372 iomete_sdk-1.2.0/setup.cfg
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     1407 2023-07-25 03:44:56.000000 iomete_sdk-1.2.0/setup.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.818189 iomete_sdk-1.2.0/src/
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.818773 iomete_sdk-1.2.0/src/iomete_sdk/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     1298 2023-07-25 03:41:17.000000 iomete_sdk-1.2.0/src/iomete_sdk/api_utils.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.819644 iomete_sdk-1.2.0/src/iomete_sdk/security/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       68 2023-07-17 22:30:18.000000 iomete_sdk-1.2.0/src/iomete_sdk/security/__init__.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     7484 2023-07-25 03:42:46.000000 iomete_sdk-1.2.0/src/iomete_sdk/security/data_security.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     3607 2023-07-25 03:24:00.000000 iomete_sdk-1.2.0/src/iomete_sdk/security/policy_models.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.819867 iomete_sdk-1.2.0/src/iomete_sdk/spark/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       57 2023-07-17 22:30:18.000000 iomete_sdk-1.2.0/src/iomete_sdk/spark/__init__.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2658 2023-07-18 22:38:50.000000 iomete_sdk-1.2.0/src/iomete_sdk/spark/spark_job.py
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.819338 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     2854 2023-07-25 03:47:10.000000 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)      504 2023-07-25 03:47:10.000000 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)        1 2023-07-25 03:47:10.000000 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       56 2023-07-25 03:47:10.000000 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/requires.txt
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)       11 2023-07-25 03:47:10.000000 iomete_sdk-1.2.0/src/iomete_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 fuadmusayev   (501) staff       (20)        0 2023-07-25 03:47:10.820074 iomete_sdk-1.2.0/tests/
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)    11694 2023-07-25 03:41:33.000000 iomete_sdk-1.2.0/tests/test_data_security_api_client.py
+-rw-r--r--   0 fuadmusayev   (501) staff       (20)     4529 2023-07-18 20:56:50.000000 iomete_sdk-1.2.0/tests/test_spark_job_api_client.py
```

### Comparing `iomete_sdk-1.1.0/PKG-INFO` & `iomete_sdk-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iomete_sdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: IOMETE SDK for Python.
 Home-page: https://github.com/iomete/iomete-sdk
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,sdk,spark-job,data-security-api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iomete_sdk-1.1.0/README.md` & `iomete_sdk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.1.0/setup.py` & `iomete_sdk-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from distutils.core import setup
 
 package_name = "iomete_sdk"
-package_version = "1.1.0"
+package_version = "1.2.0"
 
 description = """IOMETE SDK for Python."""
 
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), "r", encoding="utf8") as f:
     long_description = f.read()
```

### Comparing `iomete_sdk-1.1.0/src/iomete_sdk/api_utils.py` & `iomete_sdk-1.2.0/src/iomete_sdk/api_utils.py`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.1.0/src/iomete_sdk/security/data_security.py` & `iomete_sdk-1.2.0/src/iomete_sdk/security/data_security.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,130 +33,130 @@
         return result["controller_endpoint"]
 
     def create_access_policy(self, policy: AccessPolicyView) -> AccessPolicyView:
         data = self.api_utils.call(method="POST",
                                    url=f"{self.data_security_endpoint}/access/policy",
                                    payload=policy.to_dict())
 
-        return AccessPolicyView(**data)
+        return AccessPolicyView.from_dict(data)
 
     def get_access_policies(self) -> List[AccessPolicyView]:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/access/policy")
 
-        return [AccessPolicyView(**policy) for policy in data]
+        return [AccessPolicyView.from_dict(policy) for policy in data]
 
     def get_access_policy_by_name(self, policy_name: str) -> AccessPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/access/policy/name/{policy_name}")
 
-        return AccessPolicyView(**data)
+        return AccessPolicyView.from_dict(data)
 
-    def get_access_policy_by_id(self, policy_id: str) -> AccessPolicyView:
+    def get_access_policy_by_id(self, policy_id: int) -> AccessPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/access/policy/{policy_id}")
 
-        return AccessPolicyView(**data)
+        return AccessPolicyView.from_dict(data)
 
     def update_access_policy_by_name(self, policy_name: str, policy: AccessPolicyView) -> AccessPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/access/policy/name/{policy_name}",
                                    payload=policy.to_dict())
 
-        return AccessPolicyView(**data)
+        return AccessPolicyView.from_dict(data)
 
-    def update_access_policy_by_id(self, policy_id: str, policy: AccessPolicyView) -> AccessPolicyView:
+    def update_access_policy_by_id(self, policy_id: int, policy: AccessPolicyView) -> AccessPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/access/policy/{policy_id}",
                                    payload=policy.to_dict())
 
-        return AccessPolicyView(**data)
+        return AccessPolicyView.from_dict(data)
 
-    def delete_access_policy_by_id(self, policy_id: str):
+    def delete_access_policy_by_id(self, policy_id: int):
         self.api_utils.call(method="DELETE",
                             url=f"{self.data_security_endpoint}/access/policy/{policy_id}")
 
     def create_filter_policy(self, policy: RowFilterPolicyView) -> RowFilterPolicyView:
         data = self.api_utils.call(method="POST",
                                    url=f"{self.data_security_endpoint}/filter/policy",
                                    payload=policy.to_dict())
 
-        return RowFilterPolicyView(**data)
+        return RowFilterPolicyView.from_dict(data)
 
     def get_filter_policies(self) -> List[RowFilterPolicyView]:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/filter/policy")
 
-        return [RowFilterPolicyView(**policy) for policy in data]
+        return [RowFilterPolicyView.from_dict(policy) for policy in data]
 
     def get_filter_policy_by_name(self, policy_name: str) -> RowFilterPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/filter/policy/name/{policy_name}")
 
-        return RowFilterPolicyView(**data)
+        return RowFilterPolicyView.from_dict(data)
 
-    def get_filter_policy_by_id(self, policy_id: str) -> RowFilterPolicyView:
+    def get_filter_policy_by_id(self, policy_id: int) -> RowFilterPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/filter/policy/{policy_id}")
 
-        return RowFilterPolicyView(**data)
+        return RowFilterPolicyView.from_dict(data)
 
     def update_filter_policy_by_name(self, policy_name: str, policy: RowFilterPolicyView) -> RowFilterPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/filter/policy/name/{policy_name}",
                                    payload=policy.to_dict())
 
-        return RowFilterPolicyView(**data)
+        return RowFilterPolicyView.from_dict(data)
 
-    def update_filter_policy_by_id(self, policy_id: str, policy: RowFilterPolicyView) -> RowFilterPolicyView:
+    def update_filter_policy_by_id(self, policy_id: int, policy: RowFilterPolicyView) -> RowFilterPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/filter/policy/{policy_id}",
                                    payload=policy.to_dict())
 
-        return RowFilterPolicyView(**data)
+        return RowFilterPolicyView.from_dict(data)
 
-    def delete_filter_policy_by_id(self, policy_id: str):
+    def delete_filter_policy_by_id(self, policy_id: int):
         self.api_utils.call(method="DELETE",
                             url=f"{self.data_security_endpoint}/filter/policy/{policy_id}")
 
     def create_masking_policy(self, policy: DataMaskPolicyView) -> DataMaskPolicyView:
         data = self.api_utils.call(method="POST",
                                    url=f"{self.data_security_endpoint}/mask/policy",
                                    payload=policy.to_dict())
 
-        return DataMaskPolicyView(**data)
+        return DataMaskPolicyView.from_dict(data)
 
     def get_masking_policies(self) -> List[DataMaskPolicyView]:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/mask/policy")
 
-        return [DataMaskPolicyView(**policy) for policy in data]
+        return [DataMaskPolicyView.from_dict(policy) for policy in data]
 
     def get_masking_policy_by_name(self, policy_name: str) -> DataMaskPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/mask/policy/name/{policy_name}")
 
-        return DataMaskPolicyView(**data)
+        return DataMaskPolicyView.from_dict(data)
 
-    def get_masking_policy_by_id(self, policy_id: str) -> DataMaskPolicyView:
+    def get_masking_policy_by_id(self, policy_id: int) -> DataMaskPolicyView:
         data = self.api_utils.call(method="GET",
                                    url=f"{self.data_security_endpoint}/mask/policy/{policy_id}")
 
-        return DataMaskPolicyView(**data)
+        return DataMaskPolicyView.from_dict(data)
 
     def update_masking_policy_by_name(self, policy_name: str, policy: DataMaskPolicyView) -> DataMaskPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/mask/policy/name/{policy_name}",
                                    payload=policy.to_dict())
 
-        return DataMaskPolicyView(**data)
+        return DataMaskPolicyView.from_dict(data)
 
-    def update_masking_policy_by_id(self, policy_id: str, policy: DataMaskPolicyView) -> DataMaskPolicyView:
+    def update_masking_policy_by_id(self, policy_id: int, policy: DataMaskPolicyView) -> DataMaskPolicyView:
         data = self.api_utils.call(method="PUT",
                                    url=f"{self.data_security_endpoint}/mask/policy/{policy_id}",
                                    payload=policy.to_dict())
 
-        return DataMaskPolicyView(**data)
+        return DataMaskPolicyView.from_dict(data)
 
-    def delete_masking_policy_by_id(self, policy_id: str):
+    def delete_masking_policy_by_id(self, policy_id: int):
         self.api_utils.call(method="DELETE",
                             url=f"{self.data_security_endpoint}/mask/policy/{policy_id}")
```

### Comparing `iomete_sdk-1.1.0/src/iomete_sdk/spark/spark_job.py` & `iomete_sdk-1.2.0/src/iomete_sdk/spark/spark_job.py`

 * *Files identical despite different names*

### Comparing `iomete_sdk-1.1.0/src/iomete_sdk.egg-info/PKG-INFO` & `iomete_sdk-1.2.0/src/iomete_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iomete-sdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: IOMETE SDK for Python.
 Home-page: https://github.com/iomete/iomete-sdk
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,sdk,spark-job,data-security-api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iomete_sdk-1.1.0/tests/test_spark_job_api_client.py` & `iomete_sdk-1.2.0/tests/test_spark_job_api_client.py`

 * *Files identical despite different names*

