# Comparing `tmp/python-sonarqube-api-2.0.3.tar.gz` & `tmp/python-sonarqube-api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-sonarqube-api-2.0.3.tar", last modified: Fri Jun  2 15:15:26 2023, max compression
+gzip compressed data, was "python-sonarqube-api-2.0.4.tar", last modified: Tue Jul 25 01:36:08 2023, max compression
```

## Comparing `python-sonarqube-api-2.0.3.tar` & `python-sonarqube-api-2.0.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/
--rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     6883 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     4824 2023-06-02 14:25:09.000000 python-sonarqube-api-2.0.3/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6883 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     1144 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2524 2023-06-02 15:15:14.000000 python-sonarqube-api-2.0.3/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-06-02 15:10:53.000000 python-sonarqube-api-2.0.3/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/rest/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6232 2023-05-28 13:08:14.000000 python-sonarqube-api-2.0.3/sonarqube/rest/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:35:59.000000 python-sonarqube-api-2.0.3/sonarqube/rest/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2110 2023-05-28 13:03:06.000000 python-sonarqube-api-2.0.3/sonarqube/rest/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:36:14.000000 python-sonarqube-api-2.0.3/sonarqube/rest/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:36:44.000000 python-sonarqube-api-2.0.3/sonarqube/rest/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:37:00.000000 python-sonarqube-api-2.0.3/sonarqube/rest/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:37:35.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:37:53.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:38:08.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:38:21.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:39:31.000000 python-sonarqube-api-2.0.3/sonarqube/rest/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2389 2023-05-28 13:03:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:41:06.000000 python-sonarqube-api-2.0.3/sonarqube/rest/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8231 2023-05-28 13:06:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2928 2023-05-28 13:06:43.000000 python-sonarqube-api-2.0.3/sonarqube/rest/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:42:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:43:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/views.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2370 2023-05-28 13:08:01.000000 python-sonarqube-api-2.0.3/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:36:08.569800 python-sonarqube-api-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-25 01:36:08.569800 python-sonarqube-api-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:36:08.561800 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-25 01:36:08.000000 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 01:36:08.000000 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:36:08.000000 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 01:36:08.000000 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 01:36:08.000000 python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:36:08.569800 python-sonarqube-api-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:36:08.561800 python-sonarqube-api-2.0.4/sonarqube/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:36:08.565800 python-sonarqube-api-2.0.4/sonarqube/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/editions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/favorites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/qualitygates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/qualityprofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/user_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/rest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:36:08.565800 python-sonarqube-api-2.0.4/sonarqube/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-25 01:35:56.000000 python-sonarqube-api-2.0.4/sonarqube/utils/rest_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-sonarqube-api-2.0.3/LICENSE` & `python-sonarqube-api-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/PKG-INFO` & `python-sonarqube-api-2.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPLv3
-Description: 
-        .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
-            :target: https://pypi.python.org/pypi/python-sonarqube-api
-        .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
-            :target: https://pypi.python.org/pypi/python-sonarqube-api
-        .. image:: https://pepy.tech/badge/python-sonarqube-api
-            :target: https://pepy.tech/project/python-sonarqube-api
-        .. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
-            :target: https://pepy.tech/project/python-sonarqube-api
-        .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
-            :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
-        .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
-            :target: LICENSE
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        
-        ==========================================================================================================================================
-        Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
-        ==========================================================================================================================================
-        
-        python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
-        
-        Editions
-        ========
-        
-        There are two editions of python-sonarqube-api:
-        
-         * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
-         * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-           that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
-           please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
-        
-        +---------------------+---------------------+-----------------------+
-        | Differences         | Community Edition   | Professional Edition  |
-        +=====================+=====================+=======================+
-        | License             | GNU AGPLv3 License  | MIT License           |
-        +---------------------+---------------------+-----------------------+
-        | Commercial Use      | No                  | Yes                   |
-        +---------------------+---------------------+-----------------------+
-        | Supported APIs      | 40                  | more than 280         |
-        | (SonarQube Web APIs)|                     |                       |
-        +---------------------+---------------------+-----------------------+
-        | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
-        | (SonarQube Versions)|                     |                       |
-        +---------------------+---------------------+-----------------------+
-        
-        **Payment only needs to be made once, and library updates will be provided for free.**
-        
-        Installation
-        ============
-        
-        Community Edition
-        -----------------
-        
-        The easiest way to install the latest version is by using pip to pull it from PyPI::
-        
-            pip install  --upgrade python-sonarqube-api
-        
-        Professional Edition
-        --------------------
-        Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
-        
-            pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
-        
-        
-        Documentation
-        =============
-        
-        The full documentation for API is available on `readthedocs
-        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
-        
-        
-        Compatibility
-        =============
-        
-        * This package is compatible Python versions 2.7, 3.3+.
-        * Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
-        
-        Donate
-        ======
-        
-        donations are not mandatory but very welcomed
-        If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-        
-        Usage
-        =====
-        
-        The Client is easy to use, you just need to initialize it with the
-        connection parameters (default sonarqube url is http://localhost:9000).
-        
-        Example::
-        
-            from sonarqube import SonarQubeClient
-        
-            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
-        
-        
-        Sonar authentication tokens can also be used in place of username and password::
-        
-            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
-        
-        
-        API example
-        -----------
-        
-        The example documentation for SonarQubeClient APIs is available on `API examples
-        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
-        
-        
-        Licensing
-        -----------
-        See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
-        
 Keywords: api sonarqube sonar client wrapper sonarcloud
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
@@ -134,7 +19,138 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
+    :target: https://pypi.python.org/pypi/python-sonarqube-api
+.. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
+    :target: https://pypi.python.org/pypi/python-sonarqube-api
+.. image:: https://pepy.tech/badge/python-sonarqube-api
+    :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+    :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
+    :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
+.. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
+    :target: LICENSE
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+
+==========================================================================================================================================
+Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
+==========================================================================================================================================
+
+python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
+
+Editions
+========
+
+There are two editions of python-sonarqube-api:
+
+ * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
+ * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
+   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
+   please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
+
+Notice: Professional Edition's extra features have been remarked by using **Only available on the professional edition** in API Document.
+
++---------------------+---------------------+-----------------------+
+| Differences         | Community Edition   | Professional Edition  |
++=====================+=====================+=======================+
+| License             | GNU AGPLv3 License  | MIT License           |
++---------------------+---------------------+-----------------------+
+| Commercial Use      | No                  | Yes                   |
++---------------------+---------------------+-----------------------+
+| Supported APIs      | 40                  | more than 280         |
+| (SonarQube Web APIs)|                     |                       |
++---------------------+---------------------+-----------------------+
+| Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
+| (SonarQube Versions)|                     |                       |
++---------------------+---------------------+-----------------------+
+
+**Payment only needs to be made once, and library updates will be provided for free.**
+
+
+Change Log
+==========
+
+Community Edition
+-----------------
+
+See the `CHANGELOG-CE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-CE.md>`_ file for Community Edition.
+
+Professional Edition
+--------------------
+
+See the `CHANGELOG-PE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-PE.md>`_ file for Professional Edition.
+
+
+Installation
+============
+
+Community Edition
+-----------------
+
+The easiest way to install the latest version is by using pip to pull it from PyPI::
+
+    pip install  --upgrade python-sonarqube-api
+
+Professional Edition
+--------------------
+Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
+
+    pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
+
+
+Documentation
+=============
+
+The full documentation for API is available on `readthedocs
+<https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
+
+
+Compatibility
+=============
+
+* This package is compatible Python versions 2.7, 3.3+.
+* Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
+
+Donate
+======
+
+donations are not mandatory but very welcomed
+If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+
+Usage
+=====
+
+The Client is easy to use, you just need to initialize it with the
+connection parameters (default sonarqube url is http://localhost:9000).
+
+Example::
+
+    from sonarqube import SonarQubeClient
+
+    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
+
+
+Sonar authentication tokens can also be used in place of username and password::
+
+    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
+
+
+API example
+-----------
+
+The example documentation for SonarQubeClient APIs is available on `API examples
+<https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
+
+
+Licensing
+-----------
+See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.3/README.rst` & `python-sonarqube-api-2.0.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://pepy.tech/badge/python-sonarqube-api
     :target: https://pepy.tech/project/python-sonarqube-api
 .. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
@@ -27,14 +26,16 @@
 There are two editions of python-sonarqube-api:
 
  * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
  * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
    that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
    please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
 
+Notice: Professional Edition's extra features have been remarked by using **Only available on the professional edition** in API Document.
+
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
@@ -43,14 +44,29 @@
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
 **Payment only needs to be made once, and library updates will be provided for free.**
 
+
+Change Log
+==========
+
+Community Edition
+-----------------
+
+See the `CHANGELOG-CE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-CE.md>`_ file for Community Edition.
+
+Professional Edition
+--------------------
+
+See the `CHANGELOG-PE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-PE.md>`_ file for Professional Edition.
+
+
 Installation
 ============
 
 Community Edition
 -----------------
 
 The easiest way to install the latest version is by using pip to pull it from PyPI::
```

### Comparing `python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/PKG-INFO` & `python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: AGPLv3
-Description: 
-        .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
-            :target: https://pypi.python.org/pypi/python-sonarqube-api
-        .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
-            :target: https://pypi.python.org/pypi/python-sonarqube-api
-        .. image:: https://pepy.tech/badge/python-sonarqube-api
-            :target: https://pepy.tech/project/python-sonarqube-api
-        .. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
-            :target: https://pepy.tech/project/python-sonarqube-api
-        .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
-            :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
-        .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
-            :target: LICENSE
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        
-        ==========================================================================================================================================
-        Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
-        ==========================================================================================================================================
-        
-        python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
-        
-        Editions
-        ========
-        
-        There are two editions of python-sonarqube-api:
-        
-         * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
-         * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-           that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
-           please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
-        
-        +---------------------+---------------------+-----------------------+
-        | Differences         | Community Edition   | Professional Edition  |
-        +=====================+=====================+=======================+
-        | License             | GNU AGPLv3 License  | MIT License           |
-        +---------------------+---------------------+-----------------------+
-        | Commercial Use      | No                  | Yes                   |
-        +---------------------+---------------------+-----------------------+
-        | Supported APIs      | 40                  | more than 280         |
-        | (SonarQube Web APIs)|                     |                       |
-        +---------------------+---------------------+-----------------------+
-        | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
-        | (SonarQube Versions)|                     |                       |
-        +---------------------+---------------------+-----------------------+
-        
-        **Payment only needs to be made once, and library updates will be provided for free.**
-        
-        Installation
-        ============
-        
-        Community Edition
-        -----------------
-        
-        The easiest way to install the latest version is by using pip to pull it from PyPI::
-        
-            pip install  --upgrade python-sonarqube-api
-        
-        Professional Edition
-        --------------------
-        Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
-        
-            pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
-        
-        
-        Documentation
-        =============
-        
-        The full documentation for API is available on `readthedocs
-        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
-        
-        
-        Compatibility
-        =============
-        
-        * This package is compatible Python versions 2.7, 3.3+.
-        * Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
-        
-        Donate
-        ======
-        
-        donations are not mandatory but very welcomed
-        If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-        
-        Usage
-        =====
-        
-        The Client is easy to use, you just need to initialize it with the
-        connection parameters (default sonarqube url is http://localhost:9000).
-        
-        Example::
-        
-            from sonarqube import SonarQubeClient
-        
-            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
-        
-        
-        Sonar authentication tokens can also be used in place of username and password::
-        
-            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
-        
-        
-        API example
-        -----------
-        
-        The example documentation for SonarQubeClient APIs is available on `API examples
-        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
-        
-        
-        Licensing
-        -----------
-        See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
-        
 Keywords: api sonarqube sonar client wrapper sonarcloud
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
@@ -134,7 +19,138 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
+    :target: https://pypi.python.org/pypi/python-sonarqube-api
+.. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
+    :target: https://pypi.python.org/pypi/python-sonarqube-api
+.. image:: https://pepy.tech/badge/python-sonarqube-api
+    :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+    :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
+    :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
+.. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
+    :target: LICENSE
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+
+==========================================================================================================================================
+Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
+==========================================================================================================================================
+
+python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
+
+Editions
+========
+
+There are two editions of python-sonarqube-api:
+
+ * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
+ * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
+   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
+   please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
+
+Notice: Professional Edition's extra features have been remarked by using **Only available on the professional edition** in API Document.
+
++---------------------+---------------------+-----------------------+
+| Differences         | Community Edition   | Professional Edition  |
++=====================+=====================+=======================+
+| License             | GNU AGPLv3 License  | MIT License           |
++---------------------+---------------------+-----------------------+
+| Commercial Use      | No                  | Yes                   |
++---------------------+---------------------+-----------------------+
+| Supported APIs      | 40                  | more than 280         |
+| (SonarQube Web APIs)|                     |                       |
++---------------------+---------------------+-----------------------+
+| Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
+| (SonarQube Versions)|                     |                       |
++---------------------+---------------------+-----------------------+
+
+**Payment only needs to be made once, and library updates will be provided for free.**
+
+
+Change Log
+==========
+
+Community Edition
+-----------------
+
+See the `CHANGELOG-CE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-CE.md>`_ file for Community Edition.
+
+Professional Edition
+--------------------
+
+See the `CHANGELOG-PE.md <https://github.com/shijl0925/python-sonarqube-api/blob/master/CHANGELOG-PE.md>`_ file for Professional Edition.
+
+
+Installation
+============
+
+Community Edition
+-----------------
+
+The easiest way to install the latest version is by using pip to pull it from PyPI::
+
+    pip install  --upgrade python-sonarqube-api
+
+Professional Edition
+--------------------
+Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
+
+    pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
+
+
+Documentation
+=============
+
+The full documentation for API is available on `readthedocs
+<https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
+
+
+Compatibility
+=============
+
+* This package is compatible Python versions 2.7, 3.3+.
+* Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
+
+Donate
+======
+
+donations are not mandatory but very welcomed
+If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+
+Usage
+=====
+
+The Client is easy to use, you just need to initialize it with the
+connection parameters (default sonarqube url is http://localhost:9000).
+
+Example::
+
+    from sonarqube import SonarQubeClient
+
+    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
+
+
+Sonar authentication tokens can also be used in place of username and password::
+
+    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
+
+
+API example
+-----------
+
+The example documentation for SonarQubeClient APIs is available on `API examples
+<https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
+
+
+Licensing
+-----------
+See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/SOURCES.txt` & `python-sonarqube-api-2.0.4/python_sonarqube_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 sonarqube/rest/languages.py
 sonarqube/rest/measures.py
 sonarqube/rest/metrics.py
 sonarqube/rest/project_analyses.py
 sonarqube/rest/project_badges.py
 sonarqube/rest/project_branches.py
 sonarqube/rest/project_dump.py
+sonarqube/rest/project_links.py
 sonarqube/rest/project_tags.py
 sonarqube/rest/projects.py
 sonarqube/rest/qualitygates.py
 sonarqube/rest/qualityprofiles.py
 sonarqube/rest/rules.py
 sonarqube/rest/server.py
 sonarqube/rest/user_groups.py
```

### Comparing `python-sonarqube-api-2.0.3/setup.py` & `python-sonarqube-api-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/__init__.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from sonarqube.rest.qualityprofiles import SonarQubeQualityProfiles
 from sonarqube.rest.duplications import SonarQubeDuplications
 from sonarqube.rest.metrics import SonarQubeMetrics
 from sonarqube.rest.auth import SonarQubeAuth
 from sonarqube.rest.favorites import SonarQubeFavorites
 from sonarqube.rest.languages import SonarQubeLanguages
 from sonarqube.rest.project_badges import SonarQubeProjectBadges
+from sonarqube.rest.project_links import SonarQubeProjectLinks
 from sonarqube.rest.project_tags import SonarQubeProjectTags
 from sonarqube.rest.project_analyses import SonarQubeProjectAnalyses
 from sonarqube.rest.server import SonarQubeServer
 from sonarqube.rest.user_tokens import SonarQubeUserTokens
 from sonarqube.rest.project_dump import SonarQubeProjectDump
 from sonarqube.rest.editions import SonarQubeEditions
 from sonarqube.rest.views import SonarQubeViews
@@ -210,14 +211,23 @@
         SonarQube project badges Operations
 
         :return:
         """
         return SonarQubeProjectBadges(api=self)
 
     @property
+    def project_links(self):
+        """
+        SonarQube project links Operations
+
+        :return:
+        """
+        return SonarQubeProjectLinks(api=self)
+
+    @property
     def project_tags(self):
         """
         SonarQube project tags Operations
 
         :return:
         """
         return SonarQubeProjectTags(api=self)
@@ -277,7 +287,8 @@
 
 class SonarEnterpriseClient(SonarQubeClient):
     pass
 
 
 class SonarCloudClient(SonarQubeClient):
     pass
+
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/audit_logs.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/audit_logs.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/auth.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/ce.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/ce.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         status=None,
         type=None,
     ):
         """
         SINCE 5.2
         Search for tasks.
 
-        :param component: Key of the component (project) to filter on
+        :param component: Key of the component (project) to filter on (since 8.0)
         :param componentId: Id of the component (project) to filter on
         :param maxExecutedAt: Maximum date of end of task processing (inclusive)
         :param minSubmittedAt: Minimum date of task submission (inclusive)
         :param onlyCurrents: Filter on the last tasks (only the most recent finished task by project).
           default value is false.
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 1000
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/duplications.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/editions.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/editions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/favorites.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/favorites.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/issues.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/issues.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeIssues, self).__init__(**kwargs)
 
-    def get(self, key):
+    def get_issue(self, key):
         result = self.search_issues(issues=key)
         issues = result.get("issues", [])
 
         for issue in issues:
             if issue["key"] == key:
                 return issue
 
@@ -222,8 +222,8 @@
         SINCE 3.6
         Assign/Unassign an issue
 
         :param issue: Issue key
         :param assignee: Login of the assignee. When not set, it will unassign the issue. Use '_me' to
           assign to current user
         :return: request response
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/languages.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/languages.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/measures.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/measures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
         :param component: Component key
         :param branch: Branch key.
         :param pullRequest: Pull request id.
         :param additionalFields: Comma-separated list of additional fields that can be returned in the response.
           Possible values are for: metrics,periods
         :param metricKeys: Comma-separated list of metric keys. Possible values are for: ncloc,complexity,violations
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/metrics.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/project_analyses.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/project_analyses.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/project_badges.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/project_badges.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/project_branches.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/project_branches.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/project_dump.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/project_dump.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/project_tags.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/project_tags.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/projects.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/projects.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeProjects, self).__init__(**kwargs)
 
-    def get(self, key):
-        result = self.search_projects(projects=key)
+    def get_project(self, key, organization=None):
+        result = self.search_projects(organization=organization, projects=key)
         projects = result.get("components", [])
 
         for project in projects:
             if project["key"] == key:
                 return project
 
     @GET(API_PROJECTS_SEARCH_ENDPOINT)
@@ -62,8 +62,8 @@
           qualifiers. Possible values are for:
             * TRK
             * VW
             * APP
           default value is TRK.
 
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/qualitygates.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/qualitygates.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
         :param kwargs:
         """
         super(SonarQubeQualityGates, self).__init__(**kwargs)
 
     @GET(API_QUALITYGATES_SEARCH_ENDPOINT)
     def get_qualitygate_projects(
-        self, gateId, selected="selected", query=None, organization=None, page=None, pageSize=None
+        self, gateName, selected="selected", query=None, organization=None, page=None, pageSize=None
     ):
         """
         SINCE 4.3
         Search for projects associated (or not) to a quality gate.
 
-        :param gateId: Quality Gate ID
+        :param gateName: Quality Gate name. since 8.4
         :param selected: Depending on the value, show only selected items (selected=selected),
           deselected items (selected=deselected), or all items with their selection status (selected=all).
           Possible values are for:
             * all
             * deselected
             * selected
           default value is selected
@@ -61,8 +61,8 @@
         SINCE 4.3
         Associate a project to a quality gate.
 
         :param projectKey: Project key
         :param gateName: Quality gate name (since version 8.4). Refer https://sonarqube.inria.fr/sonarqube/web_api/api/qualitygates
         :param organization: Organization key. If no organization is provided, the default organization is used.
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/qualityprofiles.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/qualityprofiles.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,8 +83,8 @@
         Delete a quality profile and all its descendants.
         The default quality profile cannot be deleted.
 
         :param language: Quality profile language.
         :param qualityProfile: Quality profile name.
         :param organization: Organization key.
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/rules.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,14 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeRules, self).__init__(**kwargs)
 
-    def get(self, key):
-        result = self.search_rules(rule_key=key)
-        rules = result.get("rules", [])
-
-        for rule in rules:
-            if rule["key"] == key:
-                return rule
-
     @GET(API_RULES_SEARCH_ENDPOINT)
     def search_rules(
         self,
         organization=None,
         activation=None,
         qprofile=None,
         languages=None,
@@ -258,8 +250,8 @@
             * CODE_SMELL
             * BUG
             * VULNERABILITY
             * SECURITY_HOTSPOT
         :param params: Parameters as semi-colon list of =, for example 'params=key1=v1;key2=v2' (Only for custom rule)
 
         :return: request response
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/server.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/user_groups.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/user_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeUserGroups, self).__init__(**kwargs)
 
-    def get(self, name):
-        result = self.search_user_groups(q=name)
+    def get_user_group(self, name, organization=None):
+        result = self.search_user_groups(organization=organization, q=name)
         groups = result.get("groups", [])
 
         for group in groups:
             if group["name"] == name:
                 return group
 
     @GET(API_USER_GROUPS_SEARCH_ENDPOINT)
@@ -71,8 +71,8 @@
         :param currentName: Name of the group to be updated. (since 8.5)
         :param name: New optional name for the group. A group name cannot be larger than 255 characters and must
           be unique. Value 'anyone' (whatever the case) is reserved and cannot be used. If value is empty or not
           defined, then name is not changed.
         :param description: New optional description for the group. A group description cannot be larger than
           200 characters. If value is not defined, then description is not changed.
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/user_tokens.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/user_tokens.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/users.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeUsers, self).__init__(**kwargs)
 
-    def get(self, login):
+    def get_user(self, login):
         result = self.search_users(q=login)
         users = result.get("users", [])
 
         for user in users:
             if user["login"] == login:
                 return user
 
@@ -36,8 +36,8 @@
         SINCE 3.6
         Get a list of active users.
 
         :param q: Filter on login, name and email
         :param p: page number.
         :param ps: Page size. Must be greater than 0 and less or equal than 500
         :return:
-        """
+        """
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/rest/views.py` & `python-sonarqube-api-2.0.4/sonarqube/rest/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, **kwargs):
         """
 
         :param kwargs:
         """
         super(SonarQubeViews, self).__init__(**kwargs)
 
-    def get(self, key):
+    def get_view(self, key):
         result = self.list()
         for view in result["views"]:
             if view["key"] == key:
                 return view
     @GET(API_VIEWS_LIST)
     def list(self):
         """
@@ -58,7 +58,8 @@
         Requires 'Administrator' permission on the portfolio
 
         :param key: Key of the portfolio to update
         :param name: New name for the portfolio
         :param description: New description for the application
         :return:
         """
+
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/utils/common.py` & `python-sonarqube-api-2.0.4/sonarqube/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.3/sonarqube/utils/config.py` & `python-sonarqube-api-2.0.4/sonarqube/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 API_AUTH_VALIDATE_ENDPOINT = "/api/authentication/validate"
 
 API_FAVORITES_SEARCH_ENDPOINT = "/api/favorites/search"
 
 API_LANGUAGES_LIST_ENDPOINT = "/api/languages/list"
 
 API_PROJECT_BADGES_MEASURE_ENDPOINT = "/api/project_badges/measure"
+API_PROJECT_LINKS_SEARCH_ENDPOINT = "/api/project_links/search"
 
 API_PROJECT_TAGS_SEARCH_ENDPOINT = "/api/project_tags/search"
 API_PROJECT_ANALYSES_DELETE_ENDPOINT = "/api/project_analyses/delete"
 API_PROJECT_ANALYSES_SEARCH_ENDPOINT = "/api/project_analyses/search"
 
 API_SERVER_VERSION_ENDPOINT = "/api/server/version"
 
@@ -51,8 +52,8 @@
 API_PROJECT_DUMP_IMPORT_ENDPOINT = "/api/project_dump/import"
 
 
 API_EDITIONS_SET_LICENSE = "/api/editions/set_license"
 
 API_VIEWS_UPDATE = "/api/views/update"
 API_VIEWS_SHOW = "/api/views/show"
-API_VIEWS_LIST = "/api/views/list"
+API_VIEWS_LIST = "/api/views/list"
```

### Comparing `python-sonarqube-api-2.0.3/sonarqube/utils/rest_client.py` & `python-sonarqube-api-2.0.4/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

