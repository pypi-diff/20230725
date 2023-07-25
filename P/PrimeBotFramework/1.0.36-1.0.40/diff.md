# Comparing `tmp/PrimeBotFramework-1.0.36.tar.gz` & `tmp/PrimeBotFramework-1.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-mlxcdra4/PrimeBotFramework-1.0.36.tar", last modified: Thu Jun  8 14:34:16 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-bq2ef79p/PrimeBotFramework-1.0.40.tar", last modified: Tue Jul 25 14:04:21 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.36.tar` & `PrimeBotFramework-1.0.40.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10192 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10192 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     5465 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.950693 PrimeBotFramework-1.0.40/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-25 14:04:21.000000 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-25 14:04:21.000000 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-25 14:04:21.000000 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-25 14:04:21.000000 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-25 14:04:21.000000 PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-25 14:04:21.954693 PrimeBotFramework-1.0.40/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-25 14:04:13.000000 PrimeBotFramework-1.0.40/setup.py
```

### Comparing `PrimeBotFramework-1.0.36/PKG-INFO` & `PrimeBotFramework-1.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.36
+Version: 1.0.40
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/Cnab750/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/Cnab750/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.40/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/FeriadosBancarios/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.40/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.36
+Version: 1.0.40
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.40/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.36/setup.py` & `PrimeBotFramework-1.0.40/setup.py`

 * *Files identical despite different names*

