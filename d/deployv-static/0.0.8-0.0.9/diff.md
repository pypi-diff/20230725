# Comparing `tmp/deployv_static-0.0.8.tar.gz` & `tmp/deployv_static-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deployv_static-0.0.8.tar", last modified: Tue Dec  3 04:25:51 2019, max compression
+gzip compressed data, was "dist/deployv_static-0.0.9.tar", last modified: Tue Dec  3 10:56:22 2019, max compression
```

## Comparing `deployv_static-0.0.8.tar` & `deployv_static-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1467 2019-12-03 03:23:47.000000 deployv_static-0.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       83 2019-12-03 03:23:47.000000 deployv_static-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      998 2019-12-03 04:25:51.000000 deployv_static-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      506 2019-12-03 03:23:47.000000 deployv_static-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/docs/
--rwxrwxrwx   0 root         (0) root         (0)     8454 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)     6475 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       33 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     6794 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       89 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      515 2019-12-03 03:23:47.000000 deployv_static-0.0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      147 2019-12-03 03:23:47.000000 deployv_static-0.0.8/AUTHORS.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/tests/
--rwxrwxrwx   0 root         (0) root         (0)      597 2019-12-03 03:23:47.000000 deployv_static-0.0.8/tests/test_deployv-static.py
--rwxrwxrwx   0 root         (0) root         (0)       24 2019-12-03 03:23:47.000000 deployv_static-0.0.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2019-12-03 04:25:51.000000 deployv_static-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3234 2019-12-03 03:23:47.000000 deployv_static-0.0.8/CONTRIBUTING.rst
--rwxrwxrwx   0 root         (0) root         (0)     1492 2019-12-03 03:26:24.000000 deployv_static-0.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2019-12-03 03:23:47.000000 deployv_static-0.0.8/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      319 2019-12-03 03:23:47.000000 deployv_static-0.0.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static/
--rwxrwxrwx   0 root         (0) root         (0)      282 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/deployv_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3419 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/base_dockerfile.jinja
--rw-rw-rw-   0 root         (0) root         (0)     1606 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/orchestv_default_config.json
--rw-rw-rw-   0 root         (0) root         (0)      249 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/config_lc_collate.jinja
--rw-rw-rw-   0 root         (0) root         (0)      414 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/supervisord_service.conf
--rw-rw-rw-   0 root         (0) root         (0)      710 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/deployv.conf
--rw-rw-rw-   0 root         (0) root         (0)     6817 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/deactivation.jinja
--rw-rw-rw-   0 root         (0) root         (0)     1504 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/default_config.json
--rw-rw-rw-   0 root         (0) root         (0)     3918 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/l10n_mx_edi.certificate.csv
--rw-rw-rw-   0 root         (0) root         (0)     1608 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/nginx_sites.jinja
--rw-rw-rw-   0 root         (0) root         (0)     5161 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/install_deps.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/entrypoint_image.jinja
--rw-rw-rw-   0 root         (0) root         (0)      389 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/postgres_service.jinja
--rw-rw-rw-   0 root         (0) root         (0)      264 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/get_release_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/openerp_serverrc
--rw-rw-rw-   0 root         (0) root         (0)      392 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/odoo_service.jinja
--rwxrwxrwx   0 root         (0) root         (0)     7722 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/getaddons.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/dev_instances.jinja
--rw-rw-rw-   0 root         (0) root         (0)     2175 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/dev_dockerfile.jinja
--rw-rw-rw-   0 root         (0) root         (0)     5945 2019-12-03 03:23:47.000000 deployv_static-0.0.8/deployv_static/templates/transitions.json
--rwxrwxrwx   0 root         (0) root         (0)      159 2019-12-03 03:26:24.000000 deployv_static-0.0.8/deployv_static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2019-12-03 03:23:47.000000 deployv_static-0.0.8/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)       14 2019-12-03 03:23:47.000000 deployv_static-0.0.8/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/
--rw-r--r--   0 root         (0) root         (0)      998 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1499 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       14 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-03 04:25:51.000000 deployv_static-0.0.8/deployv_static.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:22.000000 deployv_static-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2019-12-03 08:57:18.000000 deployv_static-0.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2019-12-03 08:57:18.000000 deployv_static-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      998 2019-12-03 10:56:22.000000 deployv_static-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      506 2019-12-03 08:57:18.000000 deployv_static-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:22.000000 deployv_static-0.0.9/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     8454 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6475 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       33 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6794 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       89 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      515 2019-12-03 08:57:18.000000 deployv_static-0.0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      147 2019-12-03 08:57:18.000000 deployv_static-0.0.9/AUTHORS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:22.000000 deployv_static-0.0.9/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      597 2019-12-03 08:57:18.000000 deployv_static-0.0.9/tests/test_deployv-static.py
+-rwxrwxrwx   0 root         (0) root         (0)       24 2019-12-03 08:57:18.000000 deployv_static-0.0.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2019-12-03 10:56:22.000000 deployv_static-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2019-12-03 08:57:18.000000 deployv_static-0.0.9/CONTRIBUTING.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2019-12-03 10:52:10.000000 deployv_static-0.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2019-12-03 08:57:18.000000 deployv_static-0.0.9/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      319 2019-12-03 08:57:18.000000 deployv_static-0.0.9/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static/
+-rwxrwxrwx   0 root         (0) root         (0)      282 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/deployv_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:22.000000 deployv_static-0.0.9/deployv_static/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/base_dockerfile.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/orchestv_default_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      249 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/config_lc_collate.jinja
+-rw-rw-rw-   0 root         (0) root         (0)      414 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/supervisord_service.conf
+-rw-rw-rw-   0 root         (0) root         (0)      725 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/deployv.conf
+-rw-rw-rw-   0 root         (0) root         (0)     6817 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/deactivation.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/default_config.json
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/l10n_mx_edi.certificate.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/nginx_sites.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     5161 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/install_deps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/entrypoint_image.jinja
+-rw-rw-rw-   0 root         (0) root         (0)      389 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/postgres_service.jinja
+-rw-rw-rw-   0 root         (0) root         (0)      264 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/get_release_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/openerp_serverrc
+-rw-rw-rw-   0 root         (0) root         (0)      392 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/odoo_service.jinja
+-rwxrwxrwx   0 root         (0) root         (0)     7722 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/getaddons.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/dev_instances.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/dev_dockerfile.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     5945 2019-12-03 08:57:18.000000 deployv_static-0.0.9/deployv_static/templates/transitions.json
+-rwxrwxrwx   0 root         (0) root         (0)      159 2019-12-03 10:52:10.000000 deployv_static-0.0.9/deployv_static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2019-12-03 08:57:18.000000 deployv_static-0.0.9/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)       14 2019-12-03 08:57:18.000000 deployv_static-0.0.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      998 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1499 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-12-03 10:56:21.000000 deployv_static-0.0.9/deployv_static.egg-info/dependency_links.txt
```

### Comparing `deployv_static-0.0.8/LICENSE` & `deployv_static-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/PKG-INFO` & `deployv_static-0.0.9/deployv_static.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: deployv_static
-Version: 0.0.8
+Name: deployv-static
+Version: 0.0.9
 Summary: DeployV static files: Dockerfiles, json, configs, templates
 Home-page: https://github.com/Vauxoo/deployv-static
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Description: # DeployV static files
```

### Comparing `deployv_static-0.0.8/docs/conf.py` & `deployv_static-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/docs/make.bat` & `deployv_static-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/docs/Makefile` & `deployv_static-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/docs/index.rst` & `deployv_static-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/tests/test_deployv-static.py` & `deployv_static-0.0.9/tests/test_deployv-static.py`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/CONTRIBUTING.rst` & `deployv_static-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/setup.py` & `deployv_static-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     history = history_file.read().replace('.. :changelog:', '')
 
 requirements = open('requirements.txt').readlines()
 test_requirements = open('test-requirements.txt').readlines()
 
 setup(
     name='deployv_static',
-    version='0.0.8',
+    version='0.0.9',
     description="DeployV static files: Dockerfiles, json, configs, templates",
     long_description=readme + '\n\n' + history,
     author="Vauxoo",
     author_email='info@vauxoo.com',
     url='https://github.com/Vauxoo/deployv-static',
     packages=[
         'deployv_static',
```

### Comparing `deployv_static-0.0.8/deployv_static/templates/base_dockerfile.jinja` & `deployv_static-0.0.9/deployv_static/templates/base_dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/orchestv_default_config.json` & `deployv_static-0.0.9/deployv_static/templates/orchestv_default_config.json`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/deployv.conf` & `deployv_static-0.0.9/deployv_static/templates/deployv.conf`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 node_id=w01
 workers=1
 max_instances=5
 use_nginx=False
 nginx_folder=~/nginx
 docker_url=unix://var/run/docker.sock
 jobs=0
-commit_history_folder=
+commit_history_folder=/commit_history
 
 [postgres]
 db_host=127.0.0.1
 db_port=5432
 db_user=dockeradmin
 db_password=test
```

### Comparing `deployv_static-0.0.8/deployv_static/templates/deactivation.jinja` & `deployv_static-0.0.9/deployv_static/templates/deactivation.jinja`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/default_config.json` & `deployv_static-0.0.9/deployv_static/templates/default_config.json`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/l10n_mx_edi.certificate.csv` & `deployv_static-0.0.9/deployv_static/templates/l10n_mx_edi.certificate.csv`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/nginx_sites.jinja` & `deployv_static-0.0.9/deployv_static/templates/nginx_sites.jinja`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/install_deps.py` & `deployv_static-0.0.9/deployv_static/templates/install_deps.py`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/entrypoint_image.jinja` & `deployv_static-0.0.9/deployv_static/templates/entrypoint_image.jinja`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/openerp_serverrc` & `deployv_static-0.0.9/deployv_static/templates/openerp_serverrc`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/getaddons.py` & `deployv_static-0.0.9/deployv_static/templates/getaddons.py`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/dev_dockerfile.jinja` & `deployv_static-0.0.9/deployv_static/templates/dev_dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static/templates/transitions.json` & `deployv_static-0.0.9/deployv_static/templates/transitions.json`

 * *Files identical despite different names*

### Comparing `deployv_static-0.0.8/deployv_static.egg-info/PKG-INFO` & `deployv_static-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: deployv-static
-Version: 0.0.8
+Name: deployv_static
+Version: 0.0.9
 Summary: DeployV static files: Dockerfiles, json, configs, templates
 Home-page: https://github.com/Vauxoo/deployv-static
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Description: # DeployV static files
```

### Comparing `deployv_static-0.0.8/deployv_static.egg-info/SOURCES.txt` & `deployv_static-0.0.9/deployv_static.egg-info/SOURCES.txt`

 * *Files identical despite different names*

