# Comparing `tmp/nasa-wildfires-1.1.1.tar.gz` & `tmp/nasa-wildfires-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasa-wildfires-1.1.1.tar", last modified: Mon Jul 24 19:51:32 2023, max compression
+gzip compressed data, was "nasa-wildfires-1.2.0.tar", last modified: Tue Jul 25 19:28:31 2023, max compression
```

## Comparing `nasa-wildfires-1.1.1.tar` & `nasa-wildfires-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.909660 nasa-wildfires-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.913660 nasa-wildfires-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    54927 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.913660 nasa-wildfires-1.1.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/modis.json
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/viirs-noaa.json
--rw-r--r--   0 runner    (1001) docker     (123) 43384153 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/data/viirs-suomi.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.909660 nasa-wildfires-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.961664 nasa-wildfires-1.1.1/nasa_wildfires/
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/nasa_wildfires/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 19:51:32.000000 nasa-wildfires-1.1.1/nasa_wildfires.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 19:51:32.965664 nasa-wildfires-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 19:51:16.000000 nasa-wildfires-1.1.1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.397324 nasa-wildfires-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.401324 nasa-wildfires-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    46896 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.401324 nasa-wildfires-1.2.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/data/modis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/data/viirs-noaa.json
+-rw-r--r--   0 runner    (1001) docker     (123) 43384153 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/data/viirs-suomi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.449324 nasa-wildfires-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.397324 nasa-wildfires-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.449324 nasa-wildfires-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/nasa_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/nasa_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/nasa_wildfires/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/nasa_wildfires/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 19:28:31.000000 nasa-wildfires-1.2.0/nasa_wildfires.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-25 19:28:31.453324 nasa-wildfires-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-25 19:28:13.000000 nasa-wildfires-1.2.0/test.py
```

### Comparing `nasa-wildfires-1.1.1/.github/workflows/continuous-deployment.yml` & `nasa-wildfires-1.2.0/.github/workflows/continuous-deployment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
       - id: install-pipenv
         name: Install pipenv
         run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
         shell: bash
 
       - id: pipenv-install
         name: Install Python dependencies
-        run: pipenv install --skip-lock --python `which python`
+        run: pipenv install --skip-lock --dev --python `which python`
         shell: bash
 
       - id: run
         name: Run
         run: pipenv run python test.py
         shell: bash
```

### Comparing `nasa-wildfires-1.1.1/.github/workflows/docs.yml` & `nasa-wildfires-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/.github/workflows/scrape.yml` & `nasa-wildfires-1.2.0/.github/workflows/scrape.yml`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/.gitignore` & `nasa-wildfires-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/.pre-commit-config.yaml` & `nasa-wildfires-1.2.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -42,7 +42,8 @@
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
     -   id: mypy
         additional_dependencies:
           - types-requests
+          - types-retry
```

### Comparing `nasa-wildfires-1.1.1/CODE_OF_CONDUCT.md` & `nasa-wildfires-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/LICENSE` & `nasa-wildfires-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/PKG-INFO` & `nasa-wildfires-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-wildfires
-Version: 1.1.1
+Version: 1.2.0
 Summary: Download wildfire hotspots detected by NASA satellites and the Fire Information for Resource Management System (FIRMS)
 Home-page: https://palewi.re/docs/nasa-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nasa-wildfires
```

### Comparing `nasa-wildfires-1.1.1/Pipfile.lock` & `nasa-wildfires-1.2.0/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9182291666666665%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'683ad3695b21015a0c838c2a0dc20ccd102cdf6d1ac155aa7d608728f2d67bb9'}}",*

 * * "'default'": '{\'urllib3\': {\'markers\': "python_version >= \'3.7\'"}, \'decorator\': '*

 * *              "OrderedDict([('hashes', "*

 * *              "['sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330', "*

 * *              "'sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186']), "*

 * *              '(\'markers\', "python_version >= \'3.5\'"), (\'version\', \' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "bccbc7eabc4a929b5563f4449b4afb86f460b30561e6ed0397c59eff69c00e31"
+            "sha256": "683ad3695b21015a0c838c2a0dc20ccd102cdf6d1ac155aa7d608728f2d67bb9"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -109,14 +109,22 @@
             "hashes": [
                 "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
                 "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "index": "pypi",
             "version": "==8.1.6"
         },
+        "decorator": {
+            "hashes": [
+                "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330",
+                "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==5.1.1"
+        },
         "geojson": {
             "hashes": [
                 "sha256:e49df982b204ed481e4c1236c57f587adf71537301cf8faf7120ab27d73c7568",
                 "sha256:ff3d75acab60b1e66504a11f7ea12c104bad32ff3c410a807788663b966dee4a"
             ],
             "index": "pypi",
             "version": "==3.0.1"
@@ -125,28 +133,44 @@
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
+        "py": {
+            "hashes": [
+                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
+                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==1.11.0"
+        },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "version": "==2.31.0"
         },
+        "retry": {
+            "hashes": [
+                "sha256:ccddf89761fa2c726ab29391837d4327f819ea14d244c232a1d24c67a2f98606",
+                "sha256:f8bfa8b99b69c4506d6f5bd3b0aabf77f98cdb17f3c9fc3f5ca820033336fba4"
+            ],
+            "index": "pypi",
+            "version": "==0.9.2"
+        },
         "urllib3": {
             "hashes": [
                 "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
                 "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.0.4"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
@@ -156,102 +180,33 @@
             "version": "==0.7.13"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.12.1"
         },
         "bleach": {
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
                 "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
                 "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2023.7.22"
         },
-        "cffi": {
-            "hashes": [
-                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
-                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
-                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
-                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
-                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
-                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
-                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
-                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
-                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
-                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
-                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
-                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
-                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
-                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
-                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
-                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
-                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
-                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
-                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
-                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
-                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
-                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
-                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
-                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
-                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
-                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
-                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
-                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
-                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
-                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
-                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
-                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
-                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
-                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
-                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
-                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
-                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
-                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
-                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
-                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
-                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
-                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
-                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
-                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
-                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
-                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
-                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
-                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
-                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
-                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
-                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
-                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
-                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
-                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
-                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
-                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
-                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
-                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
-                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
-                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
-                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
-                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
-                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
-                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
-            ],
-            "version": "==1.15.1"
-        },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
@@ -333,64 +288,35 @@
                 "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
                 "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
                 "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.2.0"
         },
-        "cryptography": {
-            "hashes": [
-                "sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711",
-                "sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7",
-                "sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd",
-                "sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e",
-                "sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58",
-                "sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0",
-                "sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d",
-                "sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83",
-                "sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831",
-                "sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766",
-                "sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b",
-                "sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c",
-                "sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182",
-                "sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f",
-                "sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa",
-                "sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4",
-                "sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a",
-                "sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2",
-                "sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76",
-                "sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5",
-                "sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee",
-                "sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f",
-                "sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14"
-            ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==41.0.2"
-        },
         "distlib": {
             "hashes": [
                 "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
                 "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
             "version": "==0.3.7"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
                 "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
@@ -433,28 +359,20 @@
             "hashes": [
                 "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
                 "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.3.0"
         },
-        "jeepney": {
-            "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
-        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
                 "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
                 "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
@@ -518,15 +436,15 @@
                 "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
                 "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
                 "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
                 "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
                 "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
                 "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
@@ -534,15 +452,15 @@
             "version": "==0.7.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
                 "sha256:928d514ffd22b5b0a8fce326d57f423a55d2ff783b093bab217eda71e732330f",
                 "sha256:cd65437d7c4b615ab81c0640c0480bc29a550ea032891977681efd28344d51e1"
             ],
@@ -598,15 +516,15 @@
             "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
@@ -614,15 +532,15 @@
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
                 "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
                 "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==3.9.1"
         },
         "pre-commit": {
             "hashes": [
                 "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
                 "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
@@ -633,36 +551,28 @@
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.10.0"
         },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.21"
-        },
         "pyflakes": {
             "hashes": [
                 "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
                 "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
                 "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
                 "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
@@ -732,39 +642,31 @@
             "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "index": "pypi",
             "version": "==13.4.2"
         },
-        "secretstorage": {
-            "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
-        },
         "setuptools": {
             "hashes": [
                 "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
                 "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==68.0.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
                 "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
@@ -784,19 +686,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
-                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
+                "sha256:8f336d0221c3beb23006b3164ed1d46db9cebcce9cb41cdb9c5ecd4bcc509be0",
+                "sha256:9bdfb5a2b28351d4fdf40a63cd006dbad727f793b243e669fc950d7116c634af"
             ],
             "index": "pypi",
-            "version": "==7.0.1"
+            "version": "==7.1.0"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -862,43 +764,51 @@
             "hashes": [
                 "sha256:56d181c85b5925cbc59f4489a57e72a8b2166f18273fd8ba7b6fe0c0b986f12a",
                 "sha256:6aa3f7faf0ea52d728bb18c0a0d1522d9bfd8c72d26ff6f61bfc3d06a411cf40"
             ],
             "index": "pypi",
             "version": "==2.31.0.2"
         },
+        "types-retry": {
+            "hashes": [
+                "sha256:e4731dc684b56b875d9746459ad665d3bc281a56b530acdf1c97730167799941",
+                "sha256:f29760a9fe8b1fefe253e5fe6be7e4c0eba243932c600e0eccffb42a21d17765"
+            ],
+            "index": "pypi",
+            "version": "==0.9.9.4"
+        },
         "types-urllib3": {
             "hashes": [
                 "sha256:229b7f577c951b8c1b92c1bc2b2fdb0b49847bd2af6d1cc2a2e3dd340f3bda8f",
                 "sha256:9683bbb7fb72e32bfe9d2be6e04875fbe1b3eeec3cbb4ea231435aa7fd6b4f0e"
             ],
             "version": "==1.26.25.14"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
                 "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
                 "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.0.4"
         },
         "virtualenv": {
             "hashes": [
                 "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
                 "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==20.24.2"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
```

### Comparing `nasa-wildfires-1.1.1/data/viirs-suomi.json` & `nasa-wildfires-1.2.0/data/viirs-suomi.json`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/docs/Makefile` & `nasa-wildfires-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/docs/_static/css/custom.css` & `nasa-wildfires-1.2.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/docs/_templates/nav.html` & `nasa-wildfires-1.2.0/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/docs/conf.py` & `nasa-wildfires-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/docs/index.md` & `nasa-wildfires-1.2.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,111 +121,108 @@
 00000780: 0a60 6060 0a0a 446f 776e 6c6f 6164 2061  .```..Download a
 00000790: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
 000007a0: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
 000007b0: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
 000007c0: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
 000007d0: 2032 342d 686f 7572 2070 6572 696f 642e   24-hour period.
 000007e0: 2052 6574 7572 6e73 2047 656f 4a53 4f4e   Returns GeoJSON
-000007f0: 2e0a 0a60 6060 7079 7468 6f6e 0a64 6174  ...```python.dat
-00000800: 6120 3d20 6e61 7361 5f77 696c 6466 6972  a = nasa_wildfir
-00000810: 6573 2e67 6574 5f6d 6f64 6973 2829 0a60  es.get_modis().`
-00000820: 6060 0a0a 446f 776e 6c6f 6164 2061 2072  ``..Download a r
-00000830: 6567 696f 6e61 6c20 4765 6f4a 534f 4e20  egional GeoJSON 
-00000840: 6f66 2068 6f74 7370 6f74 7320 6465 7465  of hotspots dete
-00000850: 6374 6564 2062 7920 7468 6520 4d4f 4449  cted by the MODI
-00000860: 5320 7361 7465 6c6c 6974 6520 696e 2061  S satellite in a
-00000870: 2072 6563 656e 7420 3234 2d68 6f75 7220   recent 24-hour 
-00000880: 7065 7269 6f64 2e0a 0a60 6060 7079 7468  period...```pyth
-00000890: 6f6e 0a64 6174 6120 3d20 6e61 7361 5f77  on.data = nasa_w
-000008a0: 696c 6466 6972 6573 2e67 6574 5f6d 6f64  ildfires.get_mod
-000008b0: 6973 2872 6567 696f 6e3d 2275 7361 2d68  is(region="usa-h
-000008c0: 6177 6169 6922 290a 6060 600a 0a44 6f77  awaii").```..Dow
-000008d0: 6e6c 6f61 6420 6120 7265 6769 6f6e 616c  nload a regional
-000008e0: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
-000008f0: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
-00000900: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
-00000910: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
-00000920: 2037 2d64 6179 2070 6572 696f 642e 0a0a   7-day period...
-00000930: 6060 6070 7974 686f 6e0a 6461 7461 203d  ```python.data =
-00000940: 206e 6173 615f 7769 6c64 6669 7265 732e   nasa_wildfires.
-00000950: 6765 745f 6d6f 6469 7328 7265 6769 6f6e  get_modis(region
-00000960: 3d22 7573 612d 6861 7761 6969 222c 2074  ="usa-hawaii", t
-00000970: 696d 655f 7261 6e67 653d 2237 6422 290a  ime_range="7d").
-00000980: 6060 600a 0a44 6f77 6e6c 6f61 6420 6120  ```..Download a 
-00000990: 4765 6f4a 534f 4e20 6f66 2068 6f74 7370  GeoJSON of hotsp
-000009a0: 6f74 7320 6465 7465 6374 6564 2062 7920  ots detected by 
-000009b0: 7468 6520 5649 4952 5320 532d 4e50 5020  the VIIRS S-NPP 
-000009c0: 7361 7465 6c6c 6974 6520 696e 2061 2072  satellite in a r
-000009d0: 6563 656e 7420 3234 2d68 6f75 7220 7065  ecent 24-hour pe
-000009e0: 7269 6f64 2e20 5265 7475 726e 7320 4765  riod. Returns Ge
-000009f0: 6f4a 534f 4e2e 0a0a 6060 6070 7974 686f  oJSON...```pytho
-00000a00: 6e0a 6461 7461 203d 206e 6173 615f 7769  n.data = nasa_wi
-00000a10: 6c64 6669 7265 732e 6765 745f 7669 6972  ldfires.get_viir
-00000a20: 735f 7375 6f6d 6928 290a 6060 600a 0a44  s_suomi().```..D
-00000a30: 6f77 6e6c 6f61 6420 6120 4765 6f4a 534f  ownload a GeoJSO
-00000a40: 4e20 6f66 2068 6f74 7370 6f74 7320 6465  N of hotspots de
-00000a50: 7465 6374 6564 2062 7920 7468 6520 5649  tected by the VI
-00000a60: 4952 5320 4e4f 4141 2d32 3020 7361 7465  IRS NOAA-20 sate
-00000a70: 6c6c 6974 6520 696e 2061 2072 6563 656e  llite in a recen
-00000a80: 7420 3234 2d68 6f75 7220 7065 7269 6f64  t 24-hour period
-00000a90: 2e20 5265 7475 726e 7320 4765 6f4a 534f  . Returns GeoJSO
-00000aa0: 4e2e 0a0a 6060 6070 7974 686f 6e0a 6461  N...```python.da
-00000ab0: 7461 203d 206e 6173 615f 7769 6c64 6669  ta = nasa_wildfi
-00000ac0: 7265 732e 6765 745f 7669 6972 735f 6e6f  res.get_viirs_no
-00000ad0: 6161 2829 0a60 6060 0a0a 2323 2043 6f6e  aa().```..## Con
-00000ae0: 7472 6962 7574 696e 670a 0a49 6e73 7461  tributing..Insta
-00000af0: 6c6c 2064 6570 656e 6465 6e63 6965 7320  ll dependencies 
-00000b00: 666f 7220 6465 7665 6c6f 706d 656e 742e  for development.
-00000b10: 0a0a 6060 6062 6173 680a 7069 7065 6e76  ..```bash.pipenv
-00000b20: 2069 6e73 7461 6c6c 202d 2d64 6576 0a60   install --dev.`
-00000b30: 6060 0a0a 5275 6e20 7465 7374 732e 0a0a  ``..Run tests...
-00000b40: 6060 6062 6173 680a 7069 7065 6e76 2072  ```bash.pipenv r
-00000b50: 756e 2070 7974 686f 6e20 7465 7374 2e70  un python test.p
-00000b60: 790a 6060 600a 0a23 2320 4465 7665 6c6f  y.```..## Develo
-00000b70: 7069 6e67 2074 6865 2043 4c49 0a0a 5468  ping the CLI..Th
-00000b80: 6520 636f 6d6d 616e 642d 6c69 6e65 2069  e command-line i
-00000b90: 6e74 6572 6661 6365 2069 7320 696d 706c  nterface is impl
-00000ba0: 656d 656e 7465 6420 7573 696e 6720 436c  emented using Cl
-00000bb0: 6963 6b20 616e 6420 7365 7475 7074 6f6f  ick and setuptoo
-00000bc0: 6c73 2e20 546f 2069 6e73 7461 6c6c 2069  ls. To install i
-00000bd0: 7420 6c6f 6361 6c6c 7920 666f 7220 6465  t locally for de
-00000be0: 7665 6c6f 706d 656e 7420 696e 7369 6465  velopment inside
-00000bf0: 2079 6f75 7220 7669 7274 7561 6c20 656e   your virtual en
-00000c00: 7669 726f 6e6d 656e 742c 2072 756e 2074  vironment, run t
-00000c10: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e73  he following ins
-00000c20: 7461 6c6c 6174 696f 6e20 636f 6d6d 616e  tallation comman
-00000c30: 642c 2061 7320 5b70 7265 7363 7269 6265  d, as [prescribe
-00000c40: 6420 6279 2074 6865 2043 6c69 636b 2064  d by the Click d
-00000c50: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00000c60: 7470 733a 2f2f 636c 6963 6b2e 7061 6c6c  tps://click.pall
-00000c70: 6574 7370 726f 6a65 6374 732e 636f 6d2f  etsprojects.com/
-00000c80: 656e 2f37 2e78 2f73 6574 7570 746f 6f6c  en/7.x/setuptool
-00000c90: 732f 2373 6574 7570 746f 6f6c 732d 696e  s/#setuptools-in
-00000ca0: 7465 6772 6174 696f 6e29 2e0a 0a60 6060  tegration)...```
-00000cb0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00000cc0: 202d 2d65 6469 7461 626c 6520 2e0a 6060   --editable ..``
-00000cd0: 600a 0a23 2320 4c69 6e6b 730a 0a2a 2044  `..## Links..* D
-00000ce0: 6f63 733a 205b 7061 6c65 7769 2e72 652f  ocs: [palewi.re/
-00000cf0: 646f 6373 2f6e 6173 612d 7769 6c64 6669  docs/nasa-wildfi
-00000d00: 7265 732f 5d28 6874 7470 733a 2f2f 7061  res/](https://pa
-00000d10: 6c65 7769 2e72 652f 646f 6373 2f6e 6173  lewi.re/docs/nas
-00000d20: 612d 7769 6c64 6669 7265 732f 290a 2a20  a-wildfires/).* 
-00000d30: 4973 7375 6573 3a20 5b67 6974 6875 622e  Issues: [github.
-00000d40: 636f 6d2f 6461 7461 6465 736b 2f6e 6173  com/datadesk/nas
-00000d50: 612d 7769 6c64 6669 7265 732f 6973 7375  a-wildfires/issu
-00000d60: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00000d70: 7562 2e63 6f6d 2f64 6174 6164 6573 6b2f  ub.com/datadesk/
-00000d80: 6e61 7361 2d77 696c 6466 6972 6573 2f69  nasa-wildfires/i
-00000d90: 7373 7565 7329 0a2a 2050 6163 6b61 6769  ssues).* Packagi
-00000da0: 6e67 3a20 5b70 7970 692e 7079 7468 6f6e  ng: [pypi.python
-00000db0: 2e6f 7267 2f70 7970 692f 6e61 7361 2d77  .org/pypi/nasa-w
-00000dc0: 696c 6466 6972 6573 5d28 6874 7470 733a  ildfires](https:
-00000dd0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000de0: 672f 7079 7069 2f6e 6173 612d 7769 6c64  g/pypi/nasa-wild
-00000df0: 6669 7265 7329 0a2a 2054 6573 7469 6e67  fires).* Testing
-00000e00: 3a20 5b67 6974 6875 622e 636f 6d2f 6461  : [github.com/da
-00000e10: 7461 6465 736b 2f6e 6173 612d 7769 6c64  tadesk/nasa-wild
-00000e20: 6669 7265 732f 6163 7469 6f6e 735d 2868  fires/actions](h
-00000e30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e40: 6d2f 6461 7461 6465 736b 2f6e 6173 612d  m/datadesk/nasa-
-00000e50: 7769 6c64 6669 7265 732f 6163 7469 6f6e  wildfires/action
-00000e60: 7329 0a                                  s).
+000007f0: 2e0a 0a60 6060 7079 7468 6f6e 0a6e 6173  ...```python.nas
+00000800: 615f 7769 6c64 6669 7265 732e 6765 745f  a_wildfires.get_
+00000810: 6d6f 6469 7328 290a 6060 600a 0a44 6f77  modis().```..Dow
+00000820: 6e6c 6f61 6420 6120 7265 6769 6f6e 616c  nload a regional
+00000830: 2047 656f 4a53 4f4e 206f 6620 686f 7473   GeoJSON of hots
+00000840: 706f 7473 2064 6574 6563 7465 6420 6279  pots detected by
+00000850: 2074 6865 204d 4f44 4953 2073 6174 656c   the MODIS satel
+00000860: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
+00000870: 2032 342d 686f 7572 2070 6572 696f 642e   24-hour period.
+00000880: 0a0a 6060 6070 7974 686f 6e0a 6e61 7361  ..```python.nasa
+00000890: 5f77 696c 6466 6972 6573 2e67 6574 5f6d  _wildfires.get_m
+000008a0: 6f64 6973 2872 6567 696f 6e3d 2275 7361  odis(region="usa
+000008b0: 2d68 6177 6169 6922 290a 6060 600a 0a44  -hawaii").```..D
+000008c0: 6f77 6e6c 6f61 6420 6120 7265 6769 6f6e  ownload a region
+000008d0: 616c 2047 656f 4a53 4f4e 206f 6620 686f  al GeoJSON of ho
+000008e0: 7473 706f 7473 2064 6574 6563 7465 6420  tspots detected 
+000008f0: 6279 2074 6865 204d 4f44 4953 2073 6174  by the MODIS sat
+00000900: 656c 6c69 7465 2069 6e20 6120 7265 6365  ellite in a rece
+00000910: 6e74 2037 2d64 6179 2070 6572 696f 642e  nt 7-day period.
+00000920: 0a0a 6060 6070 7974 686f 6e0a 6e61 7361  ..```python.nasa
+00000930: 5f77 696c 6466 6972 6573 2e67 6574 5f6d  _wildfires.get_m
+00000940: 6f64 6973 2872 6567 696f 6e3d 2275 7361  odis(region="usa
+00000950: 2d68 6177 6169 6922 2c20 7469 6d65 5f72  -hawaii", time_r
+00000960: 616e 6765 3d22 3764 2229 0a60 6060 0a0a  ange="7d").```..
+00000970: 446f 776e 6c6f 6164 2061 2047 656f 4a53  Download a GeoJS
+00000980: 4f4e 206f 6620 686f 7473 706f 7473 2064  ON of hotspots d
+00000990: 6574 6563 7465 6420 6279 2074 6865 2056  etected by the V
+000009a0: 4949 5253 2053 2d4e 5050 2073 6174 656c  IIRS S-NPP satel
+000009b0: 6c69 7465 2069 6e20 6120 7265 6365 6e74  lite in a recent
+000009c0: 2032 342d 686f 7572 2070 6572 696f 642e   24-hour period.
+000009d0: 2052 6574 7572 6e73 2047 656f 4a53 4f4e   Returns GeoJSON
+000009e0: 2e0a 0a60 6060 7079 7468 6f6e 0a6e 6173  ...```python.nas
+000009f0: 615f 7769 6c64 6669 7265 732e 6765 745f  a_wildfires.get_
+00000a00: 7669 6972 735f 7375 6f6d 6928 290a 6060  viirs_suomi().``
+00000a10: 600a 0a44 6f77 6e6c 6f61 6420 6120 4765  `..Download a Ge
+00000a20: 6f4a 534f 4e20 6f66 2068 6f74 7370 6f74  oJSON of hotspot
+00000a30: 7320 6465 7465 6374 6564 2062 7920 7468  s detected by th
+00000a40: 6520 5649 4952 5320 4e4f 4141 2d32 3020  e VIIRS NOAA-20 
+00000a50: 7361 7465 6c6c 6974 6520 696e 2061 2072  satellite in a r
+00000a60: 6563 656e 7420 3234 2d68 6f75 7220 7065  ecent 24-hour pe
+00000a70: 7269 6f64 2e20 5265 7475 726e 7320 4765  riod. Returns Ge
+00000a80: 6f4a 534f 4e2e 0a0a 6060 6070 7974 686f  oJSON...```pytho
+00000a90: 6e0a 6e61 7361 5f77 696c 6466 6972 6573  n.nasa_wildfires
+00000aa0: 2e67 6574 5f76 6969 7273 5f6e 6f61 6128  .get_viirs_noaa(
+00000ab0: 290a 6060 600a 0a23 2320 436f 6e74 7269  ).```..## Contri
+00000ac0: 6275 7469 6e67 0a0a 496e 7374 616c 6c20  buting..Install 
+00000ad0: 6465 7065 6e64 656e 6369 6573 2066 6f72  dependencies for
+00000ae0: 2064 6576 656c 6f70 6d65 6e74 2e0a 0a60   development...`
+00000af0: 6060 6261 7368 0a70 6970 656e 7620 696e  ``bash.pipenv in
+00000b00: 7374 616c 6c20 2d2d 6465 760a 6060 600a  stall --dev.```.
+00000b10: 0a52 756e 2074 6573 7473 2e0a 0a60 6060  .Run tests...```
+00000b20: 6261 7368 0a70 6970 656e 7620 7275 6e20  bash.pipenv run 
+00000b30: 7079 7468 6f6e 2074 6573 742e 7079 0a60  python test.py.`
+00000b40: 6060 0a0a 2323 2044 6576 656c 6f70 696e  ``..## Developin
+00000b50: 6720 7468 6520 434c 490a 0a54 6865 2063  g the CLI..The c
+00000b60: 6f6d 6d61 6e64 2d6c 696e 6520 696e 7465  ommand-line inte
+00000b70: 7266 6163 6520 6973 2069 6d70 6c65 6d65  rface is impleme
+00000b80: 6e74 6564 2075 7369 6e67 2043 6c69 636b  nted using Click
+00000b90: 2061 6e64 2073 6574 7570 746f 6f6c 732e   and setuptools.
+00000ba0: 2054 6f20 696e 7374 616c 6c20 6974 206c   To install it l
+00000bb0: 6f63 616c 6c79 2066 6f72 2064 6576 656c  ocally for devel
+00000bc0: 6f70 6d65 6e74 2069 6e73 6964 6520 796f  opment inside yo
+00000bd0: 7572 2076 6972 7475 616c 2065 6e76 6972  ur virtual envir
+00000be0: 6f6e 6d65 6e74 2c20 7275 6e20 7468 6520  onment, run the 
+00000bf0: 666f 6c6c 6f77 696e 6720 696e 7374 616c  following instal
+00000c00: 6c61 7469 6f6e 2063 6f6d 6d61 6e64 2c20  lation command, 
+00000c10: 6173 205b 7072 6573 6372 6962 6564 2062  as [prescribed b
+00000c20: 7920 7468 6520 436c 6963 6b20 646f 6375  y the Click docu
+00000c30: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00000c40: 3a2f 2f63 6c69 636b 2e70 616c 6c65 7473  ://click.pallets
+00000c50: 7072 6f6a 6563 7473 2e63 6f6d 2f65 6e2f  projects.com/en/
+00000c60: 372e 782f 7365 7475 7074 6f6f 6c73 2f23  7.x/setuptools/#
+00000c70: 7365 7475 7074 6f6f 6c73 2d69 6e74 6567  setuptools-integ
+00000c80: 7261 7469 6f6e 292e 0a0a 6060 6062 6173  ration)...```bas
+00000c90: 680a 7069 7020 696e 7374 616c 6c20 2d2d  h.pip install --
+00000ca0: 6564 6974 6162 6c65 202e 0a60 6060 0a0a  editable ..```..
+00000cb0: 2323 204c 696e 6b73 0a0a 2a20 446f 6373  ## Links..* Docs
+00000cc0: 3a20 5b70 616c 6577 692e 7265 2f64 6f63  : [palewi.re/doc
+00000cd0: 732f 6e61 7361 2d77 696c 6466 6972 6573  s/nasa-wildfires
+00000ce0: 2f5d 2868 7474 7073 3a2f 2f70 616c 6577  /](https://palew
+00000cf0: 692e 7265 2f64 6f63 732f 6e61 7361 2d77  i.re/docs/nasa-w
+00000d00: 696c 6466 6972 6573 2f29 0a2a 2049 7373  ildfires/).* Iss
+00000d10: 7565 733a 205b 6769 7468 7562 2e63 6f6d  ues: [github.com
+00000d20: 2f64 6174 6164 6573 6b2f 6e61 7361 2d77  /datadesk/nasa-w
+00000d30: 696c 6466 6972 6573 2f69 7373 7565 735d  ildfires/issues]
+00000d40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000d50: 636f 6d2f 6461 7461 6465 736b 2f6e 6173  com/datadesk/nas
+00000d60: 612d 7769 6c64 6669 7265 732f 6973 7375  a-wildfires/issu
+00000d70: 6573 290a 2a20 5061 636b 6167 696e 673a  es).* Packaging:
+00000d80: 205b 7079 7069 2e70 7974 686f 6e2e 6f72   [pypi.python.or
+00000d90: 672f 7079 7069 2f6e 6173 612d 7769 6c64  g/pypi/nasa-wild
+00000da0: 6669 7265 735d 2868 7474 7073 3a2f 2f70  fires](https://p
+00000db0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000dc0: 7970 692f 6e61 7361 2d77 696c 6466 6972  ypi/nasa-wildfir
+00000dd0: 6573 290a 2a20 5465 7374 696e 673a 205b  es).* Testing: [
+00000de0: 6769 7468 7562 2e63 6f6d 2f64 6174 6164  github.com/datad
+00000df0: 6573 6b2f 6e61 7361 2d77 696c 6466 6972  esk/nasa-wildfir
+00000e00: 6573 2f61 6374 696f 6e73 5d28 6874 7470  es/actions](http
+00000e10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000e20: 6174 6164 6573 6b2f 6e61 7361 2d77 696c  atadesk/nasa-wil
+00000e30: 6466 6972 6573 2f61 6374 696f 6e73 290a  dfires/actions).
```

### Comparing `nasa-wildfires-1.1.1/docs/make.bat` & `nasa-wildfires-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/nasa_wildfires/cli.py` & `nasa-wildfires-1.2.0/nasa_wildfires/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
     help="Time range",
 )
 @click.option("--indent", default=0, help="Indentation of output")
 @click.option(
     "--sort-keys/--no-sort-keys", default=True, help="Sort the properties keys"
 )
-def modis(region, time_range, indent, sort_keys):
-    data = get_modis(region, time_range)
+@click.option("--verbose", is_flag=True, help="Print verbose output")
+def modis(region, time_range, indent, sort_keys, verbose):
+    data = get_modis(region, time_range, verbose)
     output = geojson.dumps(data, indent=indent, sort_keys=sort_keys)
     click.echo(output)
 
 
 @cmd.command(
     help="Hotspots detected by the VIIRS satellite (S-NPP) in a recent 24-hour period"
 )
@@ -56,16 +57,17 @@
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
     help="Time range",
 )
 @click.option("--indent", default=0, help="Indentation of output")
 @click.option(
     "--sort-keys/--no-sort-keys", default=True, help="Sort the properties keys"
 )
-def viirs_suomi(region, time_range, indent, sort_keys):
-    data = get_viirs_suomi(region, time_range)
+@click.option("--verbose", is_flag=True, help="Print verbose output")
+def viirs_suomi(region, time_range, indent, sort_keys, verbose):
+    data = get_viirs_suomi(region, time_range, verbose)
     output = geojson.dumps(data, indent=indent, sort_keys=sort_keys)
     click.echo(output)
 
 
 @cmd.command(
     help="Hotspots detected by the VIIRS satellite (NOAA-20) in a recent 24-hour period"
 )
@@ -83,15 +85,16 @@
     type=click.Choice(options.TIME_RANGE_LIST, case_sensitive=False),
     help="Time range",
 )
 @click.option("--indent", default=0, help="Indentation of output")
 @click.option(
     "--sort-keys/--no-sort-keys", default=True, help="Sort the properties keys"
 )
-def viirs_noaa(region, time_range, indent, sort_keys):
-    data = get_viirs_noaa(region, time_range)
+@click.option("--verbose", is_flag=True, help="Print verbose output")
+def viirs_noaa(region, time_range, indent, sort_keys, verbose):
+    data = get_viirs_noaa(region, time_range, verbose)
     output = geojson.dumps(data, indent=indent, sort_keys=sort_keys)
     click.echo(output)
 
 
 if __name__ == "__main__":
     cmd()
```

### Comparing `nasa-wildfires-1.1.1/nasa_wildfires/options.py` & `nasa-wildfires-1.2.0/nasa_wildfires/options.py`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/nasa_wildfires.egg-info/PKG-INFO` & `nasa-wildfires-1.2.0/nasa_wildfires.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-wildfires
-Version: 1.1.1
+Version: 1.2.0
 Summary: Download wildfire hotspots detected by NASA satellites and the Fire Information for Resource Management System (FIRMS)
 Home-page: https://palewi.re/docs/nasa-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nasa-wildfires
```

### Comparing `nasa-wildfires-1.1.1/nasa_wildfires.egg-info/SOURCES.txt` & `nasa-wildfires-1.2.0/nasa_wildfires.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nasa-wildfires-1.1.1/setup.py` & `nasa-wildfires-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     url="https://palewi.re/docs/nasa-wildfires/",
     license="MIT",
     packages=("nasa_wildfires",),
     install_requires=[
         "requests",
         "geojson",
         "click",
+        "retry",
     ],
     entry_points="""
         [console_scripts]
         nasawildfires=nasa_wildfires.cli:cmd
     """,
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     classifiers=[
```

