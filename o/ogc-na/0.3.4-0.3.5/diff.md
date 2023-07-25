# Comparing `tmp/ogc_na-0.3.4.tar.gz` & `tmp/ogc_na-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.3.4.tar", last modified: Mon Jul 24 11:05:22 2023, max compression
+gzip compressed data, was "ogc_na-0.3.5.tar", last modified: Tue Jul 25 09:00:54 2023, max compression
```

## Comparing `ogc_na-0.3.4.tar` & `ogc_na-0.3.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.359281 ogc_na-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.351281 ogc_na-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.355280 ogc_na-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 11:05:09.000000 ogc_na-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-24 11:05:09.000000 ogc_na-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 11:05:09.000000 ogc_na-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-24 11:05:22.359281 ogc_na-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-24 11:05:09.000000 ogc_na-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.355280 ogc_na-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-24 11:05:09.000000 ogc_na-0.3.4/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 11:05:09.000000 ogc_na-0.3.4/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 11:05:09.000000 ogc_na-0.3.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-24 11:05:09.000000 ogc_na-0.3.4/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 11:05:09.000000 ogc_na-0.3.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.351281 ogc_na-0.3.4/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.355280 ogc_na-0.3.4/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc/na/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.355280 ogc_na-0.3.4/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-24 11:05:09.000000 ogc_na-0.3.4/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.359281 ogc_na-0.3.4/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 11:05:22.000000 ogc_na-0.3.4/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-24 11:05:09.000000 ogc_na-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.359281 ogc_na-0.3.4/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 11:05:09.000000 ogc_na-0.3.4/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-24 11:05:09.000000 ogc_na-0.3.4/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 11:05:09.000000 ogc_na-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:05:22.359281 ogc_na-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 11:05:09.000000 ogc_na-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.359281 ogc_na-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:22.359281 ogc_na-0.3.4/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/schema-vocab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-24 11:05:09.000000 ogc_na-0.3.4/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.430309 ogc_na-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 09:00:41.000000 ogc_na-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-25 09:00:41.000000 ogc_na-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 09:00:41.000000 ogc_na-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 09:00:54.438309 ogc_na-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 09:00:41.000000 ogc_na-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-25 09:00:41.000000 ogc_na-0.3.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.430309 ogc_na-0.3.5/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc/na/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-25 09:00:41.000000 ogc_na-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-25 09:00:41.000000 ogc_na-0.3.5/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-25 09:00:41.000000 ogc_na-0.3.5/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 09:00:41.000000 ogc_na-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:00:54.438309 ogc_na-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 09:00:41.000000 ogc_na-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/schema-vocab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_profile.py
```

### Comparing `ogc_na-0.3.4/.github/workflows/python-publish.yml` & `ogc_na-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/.gitignore` & `ogc_na-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/PKG-INFO` & `ogc_na-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.3.4
+Version: 0.3.5
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.4/README.md` & `ogc_na-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/docs/examples.md` & `ogc_na-0.3.5/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/docs/gen_ref_pages.py` & `ogc_na-0.3.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/docs/index.md` & `ogc_na-0.3.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/docs/tutorials.md` & `ogc_na-0.3.5/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/mkdocs.yml` & `ogc_na-0.3.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/annotate_schema.py` & `ogc_na-0.3.5/ogc/na/annotate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,27 +654,24 @@
 
             if property_chain is None:
                 property_chain = []
 
             if not isinstance(subschema, dict):
                 return None
 
+            sub_context = read_properties(subschema, from_schema, property_chain) or {}
+
             if '$ref' in subschema:
                 ref = subschema['$ref']
                 if self._ref_mapper:
                     ref = self._ref_mapper(ref)
                 referenced_schema = self._resolver.resolve_schema(ref, from_schema)
                 if referenced_schema:
-                    subschema = referenced_schema.subschema
-                    from_schema = referenced_schema
-
-            if not subschema:
-                return None
-
-            sub_context = read_properties(subschema, from_schema, property_chain) or {}
+                    merge_contexts(sub_context,
+                                   process_subschema(referenced_schema.subschema, referenced_schema))
 
             for i in ('allOf', 'anyOf', 'oneOf'):
                 l = subschema.get(i)
                 if isinstance(l, list):
                     for idx, sub_subschema in enumerate(l):
                         sub_context = merge_contexts(sub_context,
                                                      process_subschema(sub_subschema,
```

### Comparing `ogc_na-0.3.4/ogc/na/domain_config.py` & `ogc_na-0.3.5/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/download.py` & `ogc_na-0.3.5/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/gsp.py` & `ogc_na-0.3.5/ogc/na/gsp.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/ingest_json.py` & `ogc_na-0.3.5/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/input_filters/__init__.py` & `ogc_na-0.3.5/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/input_filters/csv.py` & `ogc_na-0.3.5/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/profile.py` & `ogc_na-0.3.5/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/provenance.py` & `ogc_na-0.3.5/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/update_vocabs.py` & `ogc_na-0.3.5/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/util.py` & `ogc_na-0.3.5/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc/na/validation.py` & `ogc_na-0.3.5/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.3.5/ogc_na.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.3.4
+Version: 0.3.5
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.4/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.3.5/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/pyproject.toml` & `ogc_na-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/rdf/domaincfg.vocab.ttl` & `ogc_na-0.3.5/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/data/headers.csv` & `ogc_na-0.3.5/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/data/uplift_context_valid.yml` & `ogc_na-0.3.5/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/test_annotate_schema.py` & `ogc_na-0.3.5/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/test_ingest_json.py` & `ogc_na-0.3.5/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/test_input_filters_csv.py` & `ogc_na-0.3.5/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.4/test/test_profile.py` & `ogc_na-0.3.5/test/test_profile.py`

 * *Files identical despite different names*

