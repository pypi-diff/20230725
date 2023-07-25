# Comparing `tmp/botree-0.3.6.tar.gz` & `tmp/botree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botree-0.3.6.tar", max compression
+gzip compressed data, was "botree-0.4.0.tar", last modified: Tue Jul 25 15:31:31 2023, max compression
```

## Comparing `botree-0.3.6.tar` & `botree-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0     1068 2022-10-31 12:06:26.907860 botree-0.3.6/LICENSE
--rw-r--r--   0        0        0     1929 2022-10-31 12:06:26.907860 botree-0.3.6/README.md
--rw-r--r--   0        0        0      360 2022-10-31 18:06:12.626310 botree-0.3.6/botree/__init__.py
--rw-r--r--   0        0        0     1414 2022-10-31 15:12:09.402283 botree-0.3.6/botree/core.py
--rw-r--r--   0        0        0      822 2022-10-31 14:55:14.036723 botree-0.3.6/botree/decorators.py
--rw-r--r--   0        0        0      391 2022-10-31 12:06:26.907860 botree-0.3.6/botree/models.py
--rw-r--r--   0        0        0        0 2022-10-31 17:52:53.791006 botree-0.3.6/botree/py.typed
--rw-r--r--   0        0        0     5868 2022-10-31 17:46:41.991600 botree-0.3.6/botree/s3.py
--rw-r--r--   0        0        0     7205 2022-10-31 12:06:26.907860 botree-0.3.6/botree/secrets_manager.py
--rw-r--r--   0        0        0     1774 2022-10-31 18:06:17.154349 botree-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 botree-0.3.6/setup.py
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 botree-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 14:00:58.549354 botree-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1507 2023-07-25 15:27:01.222710 botree-0.4.0/README.md
+-rw-r--r--   0        0        0      361 2023-07-25 14:00:58.549354 botree-0.4.0/botree/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-25 14:33:58.247805 botree-0.4.0/botree/core.py
+-rw-r--r--   0        0        0     2103 2023-07-25 14:00:58.549354 botree-0.4.0/botree/cost_explorer.py
+-rw-r--r--   0        0        0     1926 2023-07-25 14:00:58.549354 botree-0.4.0/botree/logs.py
+-rw-r--r--   0        0        0     5656 2023-07-25 15:27:01.222710 botree-0.4.0/botree/s3.py
+-rw-r--r--   0        0        0     6276 2023-07-25 15:27:01.222710 botree-0.4.0/botree/secrets_manager.py
+-rw-r--r--   0        0        0     1511 2023-07-25 15:31:31.020294 botree-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 14:05:32.946672 botree-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-25 14:33:58.247805 botree-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1719 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_cost_explorer.py
+-rw-r--r--   0        0        0      812 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_logs.py
+-rw-r--r--   0        0        0     2030 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_s3.py
+-rw-r--r--   0        0        0     2156 2023-07-25 14:33:58.247805 botree-0.4.0/tests/test_secrets_manager.py
+-rw-r--r--   0        0        0     1787 1970-01-01 00:00:00.000000 botree-0.4.0/PKG-INFO
```

### Comparing `botree-0.3.6/LICENSE` & `botree-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botree-0.3.6/botree/core.py` & `botree-0.4.0/botree/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Botree core functions."""
 from typing import Optional
 
 from boto3.session import Session as boto_session
+
+from botree.cost_explorer import CostExplorer
+from botree.logs import Logs
 from botree.s3 import S3
 from botree.secrets_manager import SecretsManager
 
 
 class Session:
     """Botree, a friendly Boto3 wrapper."""
 
@@ -41,7 +44,17 @@
         """Get a S3 instance."""
         return S3(self.session)
 
     @property
     def secrets_manager(self) -> SecretsManager:
         """Get a SecretsManager instance."""
         return SecretsManager(self.session)
+
+    @property
+    def cost_explorer(self) -> CostExplorer:
+        """Get a CostExplorer instance."""
+        return CostExplorer(self.session)
+
+    @property
+    def logs(self) -> Logs:
+        """Get a Logs instance."""
+        return Logs(self.session)
```

### Comparing `botree-0.3.6/botree/s3.py` & `botree-0.4.0/botree/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def copy(
         self,
         source: Path,
         target: Path,
         source_bucket: Optional[str] = None,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """
         Copy an object stored in the bucket or from another bucket.
 
         If source_bucket is not specified, the object is copied from the current bucket.
 
         if target_key has no suffix, it assumes target_key is a folder and source_key
@@ -174,24 +174,15 @@
         self.client.delete_object(Bucket=self.name, Key=str(target), **kwargs)
 
 
 class S3:
     """AWS S3 operations."""
 
     def __init__(self, session: Session, **kwargs):
-        """
-        S3 class init.
-
-        Parameters
-        ----------
-        region : str, optional
-            região AWS do bucket
-        profile : Optional[str], optional
-            profile da AWS CLI, by default None.
-        """
+        """S3 class init."""
         self.session = session
         self.client = self.session.client(service_name="s3", **kwargs)
 
     def create_bucket(self, name: str, *args, **kwargs):
         """Create a bucket."""
         self.client.create_bucket(Bucket=name, *args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `botree-0.3.6/botree/secrets_manager.py` & `botree-0.4.0/botree/secrets_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,17 @@
 import json
 import uuid
 
 from datetime import datetime
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Mapping
-from typing import Optional
 from typing import Union
 
 from boto3.session import Session
-from botree import decorators
-from botree import models
 
 
 class SecretsManager:
     """AWS Secrets Manager wrapper."""
 
     def __init__(
         self,
@@ -25,55 +21,45 @@
         client_kwargs: dict = dict(),
     ):
         self.session = session
         self.client = self.session.client(
             service_name="secretsmanager", **client_kwargs
         )
 
-    @decorators.shorten_response("SecretList")
-    def list_secrets(self, shorten: Optional[bool] = True, *args, **kwargs) -> dict:
+    def list_secrets(self, *args, **kwargs) -> dict:
         """
         Returns a list of all stored secrets.
 
-        Acctually, this returns a list of all secrets within the Boto3 limit of 100.
-
-        Parameters
-        ----------
-        shorten : bool, optional
-            Exclude the response metadata. By default True.
+        Actually, this returns a list of all secrets within the Boto3 limit of 100.
 
         Returns
         -------
         dict
             List of secrets and, optionally, metadata.
         """
         secrets = self.client.list_secrets(*args, **kwargs)
 
         return secrets
 
-    @decorators.shorten_response("RandomPassword")
     def generate_password(
         self,
-        shorten: Optional[bool] = True,
         length: int = 32,
         exclude_characters: str = "",
         exclude_numbers: bool = False,
         exclude_punctuation: bool = False,
         exclude_uppercase: bool = False,
         exclude_lowercase: bool = False,
         exclude_space: bool = True,
         include_each_type: bool = True,
-    ) -> Mapping[Dict[str, str], Dict[str, models.ResponseMetadata]]:
+    ) -> dict:
         r"""
         Generates a strong random password.
 
         Parameters
         ----------
-        shorten : bool, optional.
-            Exclude the response metadata. By default True.
         length : int, optional
             The length of the password. If you don't include this parameter,
             by default 32
         exclude_characters : str, optional
             A string of the characters that you don't want in the password,
             by default ""
         exclude_numbers : bool, optional
@@ -113,15 +99,15 @@
             RequireEachIncludedType=include_each_type,
         )
 
         return random_password
 
     def delete_secret(
         self, name: str, recovery_window: int = 30, force_delete: bool = False
-    ) -> Dict[str, Union[str, datetime, models.ResponseMetadata]]:
+    ) -> dict:
         """
         Delete an existing secret.
 
         Parameters
         ----------
         name : str
             Secret name.
@@ -145,30 +131,24 @@
         else:
             kwargs.update({"RecoveryWindowInDays": recovery_window})
 
         response = self.client.delete_secret(SecretId=name, **kwargs)
 
         return response
 
-    @decorators.shorten_response("SecretString")
     def get_secret(
-        self, name: str, shorten: Optional[bool] = True, *args, **kwargs
+        self, name: str, *args, **kwargs
     ) -> Dict[str, Union[str, Dict[str, str], List[str], int, datetime]]:
         """
         Get a secret from AWS Secrets Manager by name.
 
-        Optionally, output can be shortened by selecting only the secret itself.
-
         Parameters
         ----------
         name : str
             Secret name as in AWS Secrets Manager.
-        shorten : bool, optional
-            Automatically filters the JSON and removes the response details,
-            by default True
 
         Returns
         -------
         Dict[str, Union[str, Dict[str, str], List[str], int, datetime]]
             Chosen secret.
         """
         secret = self.client.get_secret_value(SecretId=name, *args, **kwargs)
@@ -198,11 +178,11 @@
         request_token = str(uuid.uuid4())
         self.client.create_secret(
             Name=name,
             ClientRequestToken=request_token,
             Description=description,
             SecretString=json.dumps(secret),
             *args,
-            **kwargs
+            **kwargs,
         )
 
-        return self.get_secret(name, shorten=True)
+        return self.get_secret(name)
```

