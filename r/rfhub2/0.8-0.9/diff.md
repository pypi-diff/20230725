# Comparing `tmp/rfhub2-0.8.tar.gz` & `tmp/rfhub2-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rfhub2-0.8.tar", last modified: Wed Oct  9 17:19:03 2019, max compression
+gzip compressed data, was "dist/rfhub2-0.9.tar", last modified: Sun Oct 27 23:25:27 2019, max compression
```

## Comparing `rfhub2-0.8.tar` & `rfhub2-0.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-10-09 17:16:32.000000 rfhub2-0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2019-10-09 17:19:03.000000 rfhub2-0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2902 2019-10-09 17:16:32.000000 rfhub2-0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2060 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-10-09 17:19:03.000000 rfhub2-0.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/static/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/static/static/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/css/main.2733a44a.chunk.css.map
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/css/main.2733a44a.chunk.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/static/static/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8289 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/runtime~main.e6c9c1d2.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)    16930 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/main.6e17c374.chunk.js
--rw-rw-r--   0 travis    (2000) travis    (2000)  1505210 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/2.5121adea.chunk.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/runtime~main.e6c9c1d2.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    44453 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/main.6e17c374.chunk.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)   358473 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/static/js/2.5121adea.chunk.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     1197 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/service-worker.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      833 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/asset-manifest.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/robots.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/favicon.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/manifest.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/static/precache-manifest.95603e8d1f2f1671dd56de6f64a31767.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2218 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/templates/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/__main__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/model/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/router.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/api/endpoints/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3057 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/endpoints/keywords.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2281 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/endpoints/collections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/endpoints/healthcheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/endpoints/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/endpoints/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/api/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/utils/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      639 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/utils/db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/utils/auth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/api/middleware/
--rw-rw-r--   0 travis    (2000) travis    (2000)      431 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/middleware/db_session_middleware.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/api/middleware/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/utils/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      979 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/ui/search_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      375 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/ui/ui_router.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/ui/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9761 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/cli/rfhub_importer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2286 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/cli/api_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1930 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/cli/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/cli/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/cli/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/db/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/db/repository/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/repository/keyword_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1220 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/repository/collection_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/repository/query_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/repository/base_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/repository/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/init_db.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-09 17:19:03.000000 rfhub2-0.8/rfhub2/db/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      267 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/model/base_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/model/collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/model/doc_mixin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      931 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/model/keyword.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      762 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/sample_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/db/session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2019-10-09 17:16:32.000000 rfhub2-0.8/rfhub2/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1990 2019-10-09 17:16:32.000000 rfhub2-0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-10-27 23:25:05.000000 rfhub2-0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4967 2019-10-27 23:25:27.000000 rfhub2-0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3326 2019-10-27 23:25:05.000000 rfhub2-0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4967 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2060 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2019-10-27 23:25:26.000000 rfhub2-0.9/rfhub2.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-10-27 23:25:27.000000 rfhub2-0.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/static/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/static/static/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      702 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/css/main.2733a44a.chunk.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/css/main.2733a44a.chunk.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/static/static/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8289 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/runtime~main.e6c9c1d2.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16930 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/main.6e17c374.chunk.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1505210 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/2.5121adea.chunk.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/runtime~main.e6c9c1d2.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44453 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/main.6e17c374.chunk.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)   358473 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/static/js/2.5121adea.chunk.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1197 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/service-worker.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      833 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/asset-manifest.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/robots.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/favicon.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/manifest.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/static/precache-manifest.95603e8d1f2f1671dd56de6f64a31767.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2218 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/templates/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      422 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/model/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/router.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/api/endpoints/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3057 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/endpoints/keywords.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2281 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/endpoints/collections.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/endpoints/healthcheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/endpoints/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/endpoints/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/api/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/utils/http.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      639 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/utils/db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/utils/auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/api/middleware/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      431 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/middleware/db_session_middleware.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/api/middleware/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/utils/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      979 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/ui/search_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      375 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/ui/ui_router.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/ui/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/cli/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17904 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/cli/rfhub_importer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/cli/api_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/cli/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/cli/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/cli/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/db/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/db/repository/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/repository/keyword_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1220 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/repository/collection_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/repository/query_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/repository/base_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/repository/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/init_db.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:27.000000 rfhub2-0.9/rfhub2/db/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      267 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/model/base_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/model/collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/model/doc_mixin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      931 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/model/keyword.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      762 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/sample_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/db/session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      153 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      771 2019-10-27 23:25:05.000000 rfhub2-0.9/rfhub2/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1990 2019-10-27 23:25:05.000000 rfhub2-0.9/setup.py
```

### Comparing `rfhub2-0.8/PKG-INFO` & `rfhub2-0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfhub2
-Version: 0.8
+Version: 0.9
 Summary: Webserver for robot framework and python assets documentation
 Home-page: https://github.com/pbylicki/rfhub2/
 Author: Pawel Bylicki, Maciej Wiczk
 Author-email: pawelkbylicki@gmail.com, maciejwiczk@gmail.com
 License: Apache License 2.0
 Description: # rfhub2
         
@@ -71,18 +71,23 @@
         ```
         rfhub2-cli -a http://your_host:8000 -u user -p password ../your_repo ../your_other_repo
         ```
         To populate app but to skip loading RFWK installed libraries:
         ```
         rfhub2-cli --no-installed-keywords ../your_repo ../your_other_repo
         ```
-        To preserve previously loaded collections and add new ones:
-        ```
-        rfhub2-cli --no-db-flush ../your_repo ../your_other_repo
-        ```
+        #### Rfhub2-cli can be run in three modes:
+        
+        - `insert`, default mode, that will clean up existing collections app and load all collections found in provided paths  
+        ``` rfhub2-cli mode=insert ../your_repo ../your_other_repo```
+        - `append`, which will only add collections form provided paths  
+        ``` rfhub2-cli mode=append ../your_repo ../your_other_repo```
+        - `update`, which will compare existing collections with newly found ones, and update existing, remove obsolete and add new ones  
+        ``` rfhub2-cli mode=update ../your_repo ../your_other_repo```
+        
         ## License
         RfHub2 is an open source software provided under the [Apache License 2.0](http://apache.org/licenses/LICENSE-2.0)
         
 Keywords: robotframework
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rfhub2-0.8/README.md` & `rfhub2-0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -63,13 +63,18 @@
 ```
 rfhub2-cli -a http://your_host:8000 -u user -p password ../your_repo ../your_other_repo
 ```
 To populate app but to skip loading RFWK installed libraries:
 ```
 rfhub2-cli --no-installed-keywords ../your_repo ../your_other_repo
 ```
-To preserve previously loaded collections and add new ones:
-```
-rfhub2-cli --no-db-flush ../your_repo ../your_other_repo
-```
+#### Rfhub2-cli can be run in three modes:
+
+- `insert`, default mode, that will clean up existing collections app and load all collections found in provided paths  
+``` rfhub2-cli mode=insert ../your_repo ../your_other_repo```
+- `append`, which will only add collections form provided paths  
+``` rfhub2-cli mode=append ../your_repo ../your_other_repo```
+- `update`, which will compare existing collections with newly found ones, and update existing, remove obsolete and add new ones  
+``` rfhub2-cli mode=update ../your_repo ../your_other_repo```
+
 ## License
 RfHub2 is an open source software provided under the [Apache License 2.0](http://apache.org/licenses/LICENSE-2.0)
```

### Comparing `rfhub2-0.8/rfhub2.egg-info/PKG-INFO` & `rfhub2-0.9/rfhub2.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfhub2
-Version: 0.8
+Version: 0.9
 Summary: Webserver for robot framework and python assets documentation
 Home-page: https://github.com/pbylicki/rfhub2/
 Author: Pawel Bylicki, Maciej Wiczk
 Author-email: pawelkbylicki@gmail.com, maciejwiczk@gmail.com
 License: Apache License 2.0
 Description: # rfhub2
         
@@ -71,18 +71,23 @@
         ```
         rfhub2-cli -a http://your_host:8000 -u user -p password ../your_repo ../your_other_repo
         ```
         To populate app but to skip loading RFWK installed libraries:
         ```
         rfhub2-cli --no-installed-keywords ../your_repo ../your_other_repo
         ```
-        To preserve previously loaded collections and add new ones:
-        ```
-        rfhub2-cli --no-db-flush ../your_repo ../your_other_repo
-        ```
+        #### Rfhub2-cli can be run in three modes:
+        
+        - `insert`, default mode, that will clean up existing collections app and load all collections found in provided paths  
+        ``` rfhub2-cli mode=insert ../your_repo ../your_other_repo```
+        - `append`, which will only add collections form provided paths  
+        ``` rfhub2-cli mode=append ../your_repo ../your_other_repo```
+        - `update`, which will compare existing collections with newly found ones, and update existing, remove obsolete and add new ones  
+        ``` rfhub2-cli mode=update ../your_repo ../your_other_repo```
+        
         ## License
         RfHub2 is an open source software provided under the [Apache License 2.0](http://apache.org/licenses/LICENSE-2.0)
         
 Keywords: robotframework
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rfhub2-0.8/rfhub2.egg-info/SOURCES.txt` & `rfhub2-0.9/rfhub2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/css/main.2733a44a.chunk.css.map` & `rfhub2-0.9/rfhub2/static/static/css/main.2733a44a.chunk.css.map`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/runtime~main.e6c9c1d2.js.map` & `rfhub2-0.9/rfhub2/static/static/js/runtime~main.e6c9c1d2.js.map`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/main.6e17c374.chunk.js` & `rfhub2-0.9/rfhub2/static/static/js/main.6e17c374.chunk.js`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/2.5121adea.chunk.js.map` & `rfhub2-0.9/rfhub2/static/static/js/2.5121adea.chunk.js.map`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/runtime~main.e6c9c1d2.js` & `rfhub2-0.9/rfhub2/static/static/js/runtime~main.e6c9c1d2.js`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/main.6e17c374.chunk.js.map` & `rfhub2-0.9/rfhub2/static/static/js/main.6e17c374.chunk.js.map`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/static/js/2.5121adea.chunk.js` & `rfhub2-0.9/rfhub2/static/static/js/2.5121adea.chunk.js`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/service-worker.js` & `rfhub2-0.9/rfhub2/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/asset-manifest.json` & `rfhub2-0.9/rfhub2/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/static/precache-manifest.95603e8d1f2f1671dd56de6f64a31767.js` & `rfhub2-0.9/rfhub2/static/precache-manifest.95603e8d1f2f1671dd56de6f64a31767.js`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/templates/index.html` & `rfhub2-0.9/rfhub2/templates/index.html`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/model/__init__.py` & `rfhub2-0.9/rfhub2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/api/endpoints/keywords.py` & `rfhub2-0.9/rfhub2/api/endpoints/keywords.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/api/endpoints/collections.py` & `rfhub2-0.9/rfhub2/api/endpoints/collections.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/api/utils/db.py` & `rfhub2-0.9/rfhub2/api/utils/db.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/api/utils/auth.py` & `rfhub2-0.9/rfhub2/api/utils/auth.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/ui/search_params.py` & `rfhub2-0.9/rfhub2/ui/search_params.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/cli/api_client.py` & `rfhub2-0.9/rfhub2/cli/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from requests import session, post, get, delete, Response
+from requests import session, Response
 from typing import Dict, Tuple
 
 
 API_V1 = "api/v1"
 TEST_COLLECTION = {
     "name": "healtcheck_collection",
     "type": "a",
@@ -26,19 +26,21 @@
         self.api_url = f"{self.app_url}/{API_V1}"
         self.session.auth = (user, password)
         self.session.headers = {
             "Content-Type": "application/json",
             "accept": "application/json",
         }
 
-    def get_collections(self) -> Response:
+    def get_collections(self, skip: int = 0, limit: int = 100) -> Response:
         """
         Gets list of collections object using request get method.
         """
-        return self._get_request(endpoint="collections")
+        return self._get_request(
+            endpoint="collections", params={"skip": skip, "limit": limit}
+        )
 
     def add_collection(self, data: Dict) -> Dict:
         """
         Adds collection using request post method.
         """
         return self._post_request(endpoint="collections", data=data)
 
@@ -50,19 +52,19 @@
 
     def add_keyword(self, data: Dict) -> Dict:
         """
         Adds keyword using request post method.
         """
         return self._post_request(endpoint="keywords", data=data)
 
-    def _get_request(self, endpoint: str) -> Dict:
+    def _get_request(self, endpoint: str, params: Dict) -> Dict:
         """
         Sends get request from given endpoint.
         """
-        request = self.session.get(url=f"{self.api_url}/{endpoint}/")
+        request = self.session.get(url=f"{self.api_url}/{endpoint}/", params=params)
         return request.json()
 
     def _post_request(self, endpoint: str, data: Dict) -> Tuple[int, Dict]:
         """
         Sends post request to collections or keywords endpoint.
         """
         request = self.session.post(url=f"{self.api_url}/{endpoint}/", json=data)
```

### Comparing `rfhub2-0.8/rfhub2/cli/cli.py` & `rfhub2-0.9/rfhub2/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,32 +33,33 @@
     type=click.BOOL,
     default=False,
     is_flag=True,
     help="Flag specifying if package should skip loading commonly installed libraries, "
     "such as such as BuiltIn, Collections, DateTime etc.",
 )
 @click.option(
-    "--no-db-flush",
-    type=click.BOOL,
-    default=False,
-    is_flag=True,
-    help="Flag specifying if package should delete from rfhub2 all existing libraries.",
+    "--mode",
+    "-m",
+    type=click.Choice(["insert", "append", "update"], case_sensitive=False),
+    default="insert",
+    help="""Choice parameter specifying in what mode package should run:\n
+             - `insert` - default value, removes all existing collections from app and add ones found in paths\n
+             - `append` - adds collections found in paths without removal of existing ones\n
+             - `update` - removes collections not found in paths, adds new ones and updates existing ones.""",
 )
 @click.argument("paths", nargs=-1, type=click.Path(exists=True))
 def main(
     app_url: str,
     user: str,
     password: str,
     paths: Tuple[Path, ...],
-    no_db_flush: bool,
+    mode: str,
     no_installed_keywords: bool,
 ) -> None:
     """Package to populate rfhub2 with robot framework keywords
        from libraries and resource files."""
     client = Client(app_url, user, password)
-    rfhub_importer = RfhubImporter(client, paths, no_installed_keywords)
-    if not no_db_flush:
-        rfhub_importer.delete_all_collections()
+    rfhub_importer = RfhubImporter(client, paths, no_installed_keywords, mode)
     loaded_collections, loaded_keywords = rfhub_importer.import_libraries()
     print(
         f"\nSuccessfully loaded {loaded_collections} collections with {loaded_keywords} keywords."
     )
```

### Comparing `rfhub2-0.8/rfhub2/db/repository/keyword_repository.py` & `rfhub2-0.9/rfhub2/db/repository/keyword_repository.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/repository/collection_repository.py` & `rfhub2-0.9/rfhub2/db/repository/collection_repository.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/repository/query_utils.py` & `rfhub2-0.9/rfhub2/db/repository/query_utils.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/repository/base_repository.py` & `rfhub2-0.9/rfhub2/db/repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/model/collection.py` & `rfhub2-0.9/rfhub2/db/model/collection.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/model/keyword.py` & `rfhub2-0.9/rfhub2/db/model/keyword.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/sample_data.py` & `rfhub2-0.9/rfhub2/db/sample_data.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/db/session.py` & `rfhub2-0.9/rfhub2/db/session.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/rfhub2/app.py` & `rfhub2-0.9/rfhub2/app.py`

 * *Files identical despite different names*

### Comparing `rfhub2-0.8/setup.py` & `rfhub2-0.9/setup.py`

 * *Files identical despite different names*

