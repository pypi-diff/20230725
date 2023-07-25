# Comparing `tmp/pip_services4_config-0.0.1.tar.gz` & `tmp/pip_services4_config-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_config-0.0.1.tar", last modified: Mon Jul 24 11:29:19 2023, max compression
+gzip compressed data, was "pip_services4_config-0.0.2.tar", last modified: Tue Jul 25 19:30:15 2023, max compression
```

## Comparing `pip_services4_config-0.0.1.tar` & `pip_services4_config-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.279080 pip_services4_config-0.0.1/
--rw-rw-rw-   0        0        0      290 2023-07-24 11:04:05.000000 pip_services4_config-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_config-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_config-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4327 2023-07-24 11:29:19.279080 pip_services4_config-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3366 2023-07-24 10:46:59.000000 pip_services4_config-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.235083 pip_services4_config-0.0.1/pip_services4_config/
--rw-rw-rw-   0        0        0      301 2023-07-24 09:51:54.000000 pip_services4_config-0.0.1/pip_services4_config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.247079 pip_services4_config-0.0.1/pip_services4_config/auth/
--rw-rw-rw-   0        0        0     8264 2023-07-24 10:07:28.000000 pip_services4_config-0.0.1/pip_services4_config/auth/CredentialParams.py
--rw-rw-rw-   0        0        0     6081 2023-07-24 10:51:20.000000 pip_services4_config-0.0.1/pip_services4_config/auth/CredentialResolver.py
--rw-rw-rw-   0        0        0     1322 2023-07-24 11:14:28.000000 pip_services4_config-0.0.1/pip_services4_config/auth/DefaultCredentialStoreFactory.py
--rw-rw-rw-   0        0        0     1540 2023-07-24 10:52:02.000000 pip_services4_config-0.0.1/pip_services4_config/auth/ICredentialStore.py
--rw-rw-rw-   0        0        0     3540 2023-07-24 10:52:38.000000 pip_services4_config-0.0.1/pip_services4_config/auth/MemoryCredentialStore.py
--rw-rw-rw-   0        0        0     1268 2023-07-24 09:57:54.000000 pip_services4_config-0.0.1/pip_services4_config/auth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.249078 pip_services4_config-0.0.1/pip_services4_config/build/
--rw-rw-rw-   0        0        0     1863 2023-07-24 11:15:53.000000 pip_services4_config-0.0.1/pip_services4_config/build/DefaultConfigFactory.py
--rw-rw-rw-   0        0        0      486 2023-07-24 11:13:55.000000 pip_services4_config-0.0.1/pip_services4_config/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.256082 pip_services4_config-0.0.1/pip_services4_config/config/
--rw-rw-rw-   0        0        0     2953 2023-07-24 10:53:04.000000 pip_services4_config-0.0.1/pip_services4_config/config/ConfigReader.py
--rw-rw-rw-   0        0        0     1878 2023-07-24 11:13:55.000000 pip_services4_config-0.0.1/pip_services4_config/config/DefaultConfigReaderFactory.py
--rw-rw-rw-   0        0        0     1811 2023-07-24 10:33:01.000000 pip_services4_config-0.0.1/pip_services4_config/config/FileConfigReader.py
--rw-rw-rw-   0        0        0     2019 2023-07-24 10:53:16.000000 pip_services4_config-0.0.1/pip_services4_config/config/IConfigReader.py
--rw-rw-rw-   0        0        0     4702 2023-07-24 10:54:22.000000 pip_services4_config-0.0.1/pip_services4_config/config/JsonConfigReader.py
--rw-rw-rw-   0        0        0     2979 2023-07-24 10:54:55.000000 pip_services4_config-0.0.1/pip_services4_config/config/MemoryConfigReader.py
--rw-rw-rw-   0        0        0     4696 2023-07-24 10:56:14.000000 pip_services4_config-0.0.1/pip_services4_config/config/YamlConfigReader.py
--rw-rw-rw-   0        0        0     1163 2023-07-24 09:57:54.000000 pip_services4_config-0.0.1/pip_services4_config/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.265080 pip_services4_config-0.0.1/pip_services4_config/connect/
--rw-rw-rw-   0        0        0     9998 2023-07-24 10:57:37.000000 pip_services4_config-0.0.1/pip_services4_config/connect/CompositeConnectionResolver.py
--rw-rw-rw-   0        0        0     8050 2023-07-24 10:34:30.000000 pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionParams.py
--rw-rw-rw-   0        0        0     9744 2023-07-24 11:01:32.000000 pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionResolver.py
--rw-rw-rw-   0        0        0     8972 2023-07-24 10:34:59.000000 pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionUtils.py
--rw-rw-rw-   0        0        0     1229 2023-07-24 11:13:55.000000 pip_services4_config-0.0.1/pip_services4_config/connect/DefaultDiscoveryFactory.py
--rw-rw-rw-   0        0        0     2068 2023-07-24 11:02:33.000000 pip_services4_config-0.0.1/pip_services4_config/connect/IDiscovery.py
--rw-rw-rw-   0        0        0     4566 2023-07-24 11:02:11.000000 pip_services4_config-0.0.1/pip_services4_config/connect/MemoryDiscovery.py
--rw-rw-rw-   0        0        0     2880 2023-07-24 09:57:54.000000 pip_services4_config-0.0.1/pip_services4_config/connect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.241077 pip_services4_config-0.0.1/pip_services4_config.egg-info/
--rw-rw-rw-   0        0        0     4327 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1949 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 11:29:19.000000 pip_services4_config-0.0.1/pip_services4_config.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-24 11:29:19.280079 pip_services4_config-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1760 2023-07-24 11:04:51.000000 pip_services4_config-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.227072 pip_services4_config-0.0.1/test/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.268079 pip_services4_config-0.0.1/test/auth/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.1/test/auth/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-24 10:35:54.000000 pip_services4_config-0.0.1/test/auth/test_CredentialParams.py
--rw-rw-rw-   0        0        0     2351 2023-07-24 11:03:09.000000 pip_services4_config-0.0.1/test/auth/test_CredentialResolver.py
--rw-rw-rw-   0        0        0     1231 2023-07-24 10:36:24.000000 pip_services4_config-0.0.1/test/auth/test_MemoryCredentialStore.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.273080 pip_services4_config-0.0.1/test/config/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.1/test/config/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-24 10:36:56.000000 pip_services4_config-0.0.1/test/config/test_ConfigReader.py
--rw-rw-rw-   0        0        0     1311 2023-07-24 10:36:56.000000 pip_services4_config-0.0.1/test/config/test_JsonConfigReader.py
--rw-rw-rw-   0        0        0     1237 2023-07-24 10:36:56.000000 pip_services4_config-0.0.1/test/config/test_YamlConfigReader.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:29:19.278090 pip_services4_config-0.0.1/test/connect/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.1/test/connect/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-07-24 10:43:51.000000 pip_services4_config-0.0.1/test/connect/test_ConnectionParams.py
--rw-rw-rw-   0        0        0     2974 2023-07-24 11:03:42.000000 pip_services4_config-0.0.1/test/connect/test_ConnectionResolver.py
--rw-rw-rw-   0        0        0     5720 2023-07-24 10:44:20.000000 pip_services4_config-0.0.1/test/connect/test_ConnectionUtils.py
--rw-rw-rw-   0        0        0     1078 2023-07-24 10:44:32.000000 pip_services4_config-0.0.1/test/connect/test_MemoryDiscovery.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.952757 pip_services4_config-0.0.2/
+-rw-rw-rw-   0        0        0      290 2023-07-25 19:30:11.000000 pip_services4_config-0.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_config-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_config-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4327 2023-07-25 19:30:15.952757 pip_services4_config-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3366 2023-07-24 10:46:59.000000 pip_services4_config-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.883934 pip_services4_config-0.0.2/pip_services4_config/
+-rw-rw-rw-   0        0        0      301 2023-07-24 09:51:54.000000 pip_services4_config-0.0.2/pip_services4_config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.900941 pip_services4_config-0.0.2/pip_services4_config/auth/
+-rw-rw-rw-   0        0        0     8264 2023-07-24 10:07:28.000000 pip_services4_config-0.0.2/pip_services4_config/auth/CredentialParams.py
+-rw-rw-rw-   0        0        0     6081 2023-07-24 10:51:20.000000 pip_services4_config-0.0.2/pip_services4_config/auth/CredentialResolver.py
+-rw-rw-rw-   0        0        0     1322 2023-07-24 11:14:28.000000 pip_services4_config-0.0.2/pip_services4_config/auth/DefaultCredentialStoreFactory.py
+-rw-rw-rw-   0        0        0     1540 2023-07-24 10:52:02.000000 pip_services4_config-0.0.2/pip_services4_config/auth/ICredentialStore.py
+-rw-rw-rw-   0        0        0     3540 2023-07-24 10:52:38.000000 pip_services4_config-0.0.2/pip_services4_config/auth/MemoryCredentialStore.py
+-rw-rw-rw-   0        0        0     1268 2023-07-24 09:57:54.000000 pip_services4_config-0.0.2/pip_services4_config/auth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.903940 pip_services4_config-0.0.2/pip_services4_config/build/
+-rw-rw-rw-   0        0        0     1863 2023-07-24 11:15:53.000000 pip_services4_config-0.0.2/pip_services4_config/build/DefaultConfigFactory.py
+-rw-rw-rw-   0        0        0      486 2023-07-24 11:13:55.000000 pip_services4_config-0.0.2/pip_services4_config/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.919221 pip_services4_config-0.0.2/pip_services4_config/config/
+-rw-rw-rw-   0        0        0     2953 2023-07-24 10:53:04.000000 pip_services4_config-0.0.2/pip_services4_config/config/ConfigReader.py
+-rw-rw-rw-   0        0        0     1878 2023-07-24 11:13:55.000000 pip_services4_config-0.0.2/pip_services4_config/config/DefaultConfigReaderFactory.py
+-rw-rw-rw-   0        0        0     1811 2023-07-24 10:33:01.000000 pip_services4_config-0.0.2/pip_services4_config/config/FileConfigReader.py
+-rw-rw-rw-   0        0        0     2019 2023-07-24 10:53:16.000000 pip_services4_config-0.0.2/pip_services4_config/config/IConfigReader.py
+-rw-rw-rw-   0        0        0     4702 2023-07-24 10:54:22.000000 pip_services4_config-0.0.2/pip_services4_config/config/JsonConfigReader.py
+-rw-rw-rw-   0        0        0     2979 2023-07-24 10:54:55.000000 pip_services4_config-0.0.2/pip_services4_config/config/MemoryConfigReader.py
+-rw-rw-rw-   0        0        0     4696 2023-07-24 10:56:14.000000 pip_services4_config-0.0.2/pip_services4_config/config/YamlConfigReader.py
+-rw-rw-rw-   0        0        0     1163 2023-07-24 09:57:54.000000 pip_services4_config-0.0.2/pip_services4_config/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.933227 pip_services4_config-0.0.2/pip_services4_config/connect/
+-rw-rw-rw-   0        0        0     9998 2023-07-24 10:57:37.000000 pip_services4_config-0.0.2/pip_services4_config/connect/CompositeConnectionResolver.py
+-rw-rw-rw-   0        0        0     8050 2023-07-24 10:34:30.000000 pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionParams.py
+-rw-rw-rw-   0        0        0     9744 2023-07-24 11:01:32.000000 pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionResolver.py
+-rw-rw-rw-   0        0        0     8972 2023-07-24 10:34:59.000000 pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionUtils.py
+-rw-rw-rw-   0        0        0     1229 2023-07-24 11:13:55.000000 pip_services4_config-0.0.2/pip_services4_config/connect/DefaultDiscoveryFactory.py
+-rw-rw-rw-   0        0        0     2068 2023-07-24 11:02:33.000000 pip_services4_config-0.0.2/pip_services4_config/connect/IDiscovery.py
+-rw-rw-rw-   0        0        0     4566 2023-07-24 11:02:11.000000 pip_services4_config-0.0.2/pip_services4_config/connect/MemoryDiscovery.py
+-rw-rw-rw-   0        0        0     2880 2023-07-24 09:57:54.000000 pip_services4_config-0.0.2/pip_services4_config/connect/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.892940 pip_services4_config-0.0.2/pip_services4_config.egg-info/
+-rw-rw-rw-   0        0        0     4327 2023-07-25 19:30:15.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1949 2023-07-25 19:30:15.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:30:15.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-07-25 19:30:15.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-25 19:30:15.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 11:29:19.000000 pip_services4_config-0.0.2/pip_services4_config.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 19:30:15.954864 pip_services4_config-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2023-07-25 19:30:11.000000 pip_services4_config-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.875725 pip_services4_config-0.0.2/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.939605 pip_services4_config-0.0.2/test/auth/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.2/test/auth/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-24 10:35:54.000000 pip_services4_config-0.0.2/test/auth/test_CredentialParams.py
+-rw-rw-rw-   0        0        0     2351 2023-07-24 11:03:09.000000 pip_services4_config-0.0.2/test/auth/test_CredentialResolver.py
+-rw-rw-rw-   0        0        0     1231 2023-07-24 10:36:24.000000 pip_services4_config-0.0.2/test/auth/test_MemoryCredentialStore.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.945609 pip_services4_config-0.0.2/test/config/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.2/test/config/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-24 10:36:56.000000 pip_services4_config-0.0.2/test/config/test_ConfigReader.py
+-rw-rw-rw-   0        0        0     1311 2023-07-24 10:36:56.000000 pip_services4_config-0.0.2/test/config/test_JsonConfigReader.py
+-rw-rw-rw-   0        0        0     1237 2023-07-24 10:36:56.000000 pip_services4_config-0.0.2/test/config/test_YamlConfigReader.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:30:15.951759 pip_services4_config-0.0.2/test/connect/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_config-0.0.2/test/connect/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-07-24 10:43:51.000000 pip_services4_config-0.0.2/test/connect/test_ConnectionParams.py
+-rw-rw-rw-   0        0        0     2974 2023-07-24 11:03:42.000000 pip_services4_config-0.0.2/test/connect/test_ConnectionResolver.py
+-rw-rw-rw-   0        0        0     5720 2023-07-24 10:44:20.000000 pip_services4_config-0.0.2/test/connect/test_ConnectionUtils.py
+-rw-rw-rw-   0        0        0     1078 2023-07-24 10:44:32.000000 pip_services4_config-0.0.2/test/connect/test_MemoryDiscovery.py
```

### Comparing `pip_services4_config-0.0.1/LICENSE` & `pip_services4_config-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/PKG-INFO` & `pip_services4_config-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_config
-Version: 0.0.1
+Version: 0.0.2
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-config-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_config-0.0.1/README.md` & `pip_services4_config-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/CredentialParams.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/CredentialParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/CredentialResolver.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/CredentialResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/DefaultCredentialStoreFactory.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/DefaultCredentialStoreFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/ICredentialStore.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/ICredentialStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/MemoryCredentialStore.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/MemoryCredentialStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/auth/__init__.py` & `pip_services4_config-0.0.2/pip_services4_config/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/build/DefaultConfigFactory.py` & `pip_services4_config-0.0.2/pip_services4_config/build/DefaultConfigFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/ConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/ConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/DefaultConfigReaderFactory.py` & `pip_services4_config-0.0.2/pip_services4_config/config/DefaultConfigReaderFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/FileConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/FileConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/IConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/IConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/JsonConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/JsonConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/MemoryConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/MemoryConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/YamlConfigReader.py` & `pip_services4_config-0.0.2/pip_services4_config/config/YamlConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/config/__init__.py` & `pip_services4_config-0.0.2/pip_services4_config/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/CompositeConnectionResolver.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/CompositeConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionParams.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionResolver.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/ConnectionUtils.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/ConnectionUtils.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/DefaultDiscoveryFactory.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/DefaultDiscoveryFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/IDiscovery.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/IDiscovery.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/MemoryDiscovery.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/MemoryDiscovery.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config/connect/__init__.py` & `pip_services4_config-0.0.2/pip_services4_config/connect/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/pip_services4_config.egg-info/PKG-INFO` & `pip_services4_config-0.0.2/pip_services4_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-config
-Version: 0.0.1
+Version: 0.0.2
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-config-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_config-0.0.1/pip_services4_config.egg-info/SOURCES.txt` & `pip_services4_config-0.0.2/pip_services4_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/setup.py` & `pip_services4_config-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_config',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-config-python',
     license='MIT',
     description='Component definitions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['config', 'data', 'test']),
     include_package_data=True,
     zip_safe=True,
     platforms='any',
     install_requires=[
         'PyYAML >= 6.0, < 7.0',
-        'pip_services4_commons >= 0.0.1, < 4.0',
-        'pip_services4_components >= 0.0.2, < 4.0',
-        'pip_services4_expressions >= 0.0.1, < 4.0',
+        'pip_services4_commons >= 0.0.2, < 1.0',
+        'pip_services4_components >= 0.0.2, < 1.0',
+        'pip_services4_expressions >= 0.0.2, < 1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `pip_services4_config-0.0.1/test/auth/test_CredentialParams.py` & `pip_services4_config-0.0.2/test/auth/test_CredentialParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/auth/test_CredentialResolver.py` & `pip_services4_config-0.0.2/test/auth/test_CredentialResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/auth/test_MemoryCredentialStore.py` & `pip_services4_config-0.0.2/test/auth/test_MemoryCredentialStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/config/test_ConfigReader.py` & `pip_services4_config-0.0.2/test/config/test_ConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/config/test_JsonConfigReader.py` & `pip_services4_config-0.0.2/test/config/test_JsonConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/config/test_YamlConfigReader.py` & `pip_services4_config-0.0.2/test/config/test_YamlConfigReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/connect/test_ConnectionParams.py` & `pip_services4_config-0.0.2/test/connect/test_ConnectionParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/connect/test_ConnectionResolver.py` & `pip_services4_config-0.0.2/test/connect/test_ConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/connect/test_ConnectionUtils.py` & `pip_services4_config-0.0.2/test/connect/test_ConnectionUtils.py`

 * *Files identical despite different names*

### Comparing `pip_services4_config-0.0.1/test/connect/test_MemoryDiscovery.py` & `pip_services4_config-0.0.2/test/connect/test_MemoryDiscovery.py`

 * *Files identical despite different names*

