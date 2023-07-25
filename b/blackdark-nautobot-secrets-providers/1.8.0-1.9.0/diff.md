# Comparing `tmp/blackdark_nautobot_secrets_providers-1.8.0.tar.gz` & `tmp/blackdark_nautobot_secrets_providers-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackdark_nautobot_secrets_providers-1.8.0.tar", max compression
+gzip compressed data, was "blackdark_nautobot_secrets_providers-1.9.0.tar", max compression
```

## Comparing `blackdark_nautobot_secrets_providers-1.8.0.tar` & `blackdark_nautobot_secrets_providers-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      591 2023-03-20 19:57:10.731665 blackdark_nautobot_secrets_providers-1.8.0/LICENSE
--rw-r--r--   0        0        0    28239 2023-03-20 20:07:42.742973 blackdark_nautobot_secrets_providers-1.8.0/README.md
--rw-r--r--   0        0        0     1081 2023-03-20 21:50:48.352131 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 19:57:10.738525 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/migrations/__init__.py
--rw-r--r--   0        0        0      710 2023-03-20 20:07:42.743807 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/__init__.py
--rw-r--r--   0        0        0     4656 2023-03-20 19:57:10.739004 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/aws.py
--rw-r--r--   0        0        0     3133 2023-03-20 20:07:42.744149 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/aws_ssm.py
--rw-r--r--   0        0        0      509 2023-03-20 19:57:10.739182 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/choices.py
--rw-r--r--   0        0        0     9522 2023-03-20 21:53:08.439404 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/delinea.py
--rw-r--r--   0        0        0     7687 2023-03-20 21:53:09.489138 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/hashicorp.py
--rw-r--r--   0        0        0      768 2023-03-20 21:51:34.418870 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/secrets.py
--rw-r--r--   0        0        0     1597 2023-03-20 22:37:02.804601 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/template_content.py
--rw-r--r--   0        0        0     3307 2023-03-20 20:07:42.744613 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/home.html
--rw-r--r--   0        0        0      416 2023-03-20 22:27:29.877085 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/tab_secret_detail_check.html
--rw-r--r--   0        0        0       66 2023-03-20 21:51:44.857854 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/__init__.py
--rw-r--r--   0        0        0     2096 2023-03-20 21:53:11.069342 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/nautobot_config.py
--rw-r--r--   0        0        0      631 2023-03-20 21:51:46.623534 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/test_basic.py
--rw-r--r--   0        0        0    23211 2023-03-20 21:53:11.911831 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/test_providers.py
--rw-r--r--   0        0        0      601 2023-03-20 22:27:51.546699 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/urls.py
--rw-r--r--   0        0        0     2575 2023-03-20 22:37:00.965732 blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/views.py
--rw-r--r--   0        0        0     3124 2023-03-20 22:37:15.092528 blackdark_nautobot_secrets_providers-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    29503 1970-01-01 00:00:00.000000 blackdark_nautobot_secrets_providers-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-03-20 19:57:10.731665 blackdark_nautobot_secrets_providers-1.9.0/LICENSE
+-rw-r--r--   0        0        0    28239 2023-03-20 20:07:42.742973 blackdark_nautobot_secrets_providers-1.9.0/README.md
+-rw-r--r--   0        0        0     1081 2023-03-20 21:50:48.352131 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-20 19:57:10.738525 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/migrations/__init__.py
+-rw-r--r--   0        0        0      710 2023-03-20 20:07:42.743807 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/__init__.py
+-rw-r--r--   0        0        0     4656 2023-03-20 19:57:10.739004 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/aws.py
+-rw-r--r--   0        0        0     3133 2023-03-20 20:07:42.744149 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/aws_ssm.py
+-rw-r--r--   0        0        0      509 2023-03-20 19:57:10.739182 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/choices.py
+-rw-r--r--   0        0        0     9522 2023-03-20 21:53:08.439404 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/delinea.py
+-rw-r--r--   0        0        0     7687 2023-03-20 21:53:09.489138 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/hashicorp.py
+-rw-r--r--   0        0        0      768 2023-03-20 21:51:34.418870 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/secrets.py
+-rw-r--r--   0        0        0     1597 2023-03-20 22:37:02.804601 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/template_content.py
+-rw-r--r--   0        0        0     3307 2023-03-20 20:07:42.744613 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/home.html
+-rw-r--r--   0        0        0      448 2023-03-20 23:01:45.587696 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/tab_secret_detail_check.html
+-rw-r--r--   0        0        0       66 2023-03-20 21:51:44.857854 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/__init__.py
+-rw-r--r--   0        0        0     2096 2023-03-20 21:53:11.069342 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/nautobot_config.py
+-rw-r--r--   0        0        0      631 2023-03-20 21:51:46.623534 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/test_basic.py
+-rw-r--r--   0        0        0    23211 2023-03-20 21:53:11.911831 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/test_providers.py
+-rw-r--r--   0        0        0      601 2023-03-20 22:27:51.546699 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/urls.py
+-rw-r--r--   0        0        0     2575 2023-03-20 22:37:00.965732 blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/views.py
+-rw-r--r--   0        0        0     3124 2023-03-20 23:01:50.104217 blackdark_nautobot_secrets_providers-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    29503 1970-01-01 00:00:00.000000 blackdark_nautobot_secrets_providers-1.9.0/PKG-INFO
```

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/LICENSE` & `blackdark_nautobot_secrets_providers-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/README.md` & `blackdark_nautobot_secrets_providers-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/__init__.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/__init__.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/aws.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/aws.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/aws_ssm.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/aws_ssm.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/delinea.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/delinea.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/providers/hashicorp.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/providers/hashicorp.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/secrets.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/secrets.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/template_content.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/template_content.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/home.html` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/templates/blackdark_nautobot_secrets_providers/home.html`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/nautobot_config.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/nautobot_config.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/test_basic.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/tests/test_providers.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/urls.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/urls.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/blackdark_nautobot_secrets_providers/views.py` & `blackdark_nautobot_secrets_providers-1.9.0/blackdark_nautobot_secrets_providers/views.py`

 * *Files identical despite different names*

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/pyproject.toml` & `blackdark_nautobot_secrets_providers-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BlackDark-nautobot-secrets-providers"
-version = "1.8.0"
+version = "1.9.0"
 description = "Nautobot Secrets Providers Plugin."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 repository = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `blackdark_nautobot_secrets_providers-1.8.0/PKG-INFO` & `blackdark_nautobot_secrets_providers-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackdark-nautobot-secrets-providers
-Version: 1.8.0
+Version: 1.9.0
 Summary: Nautobot Secrets Providers Plugin.
 Home-page: https://github.com/nautobot/nautobot-plugin-secrets-providers
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
```

