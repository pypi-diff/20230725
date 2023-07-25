# Comparing `tmp/discovery-capability-0.4.7.tar.gz` & `tmp/discovery-capability-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.4.7.tar", last modified: Mon Jul 24 23:04:29 2023, max compression
+gzip compressed data, was "discovery-capability-0.4.8.tar", last modified: Tue Jul 25 13:19:27 2023, max compression
```

## Comparing `discovery-capability-0.4.7.tar` & `discovery-capability-0.4.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.714758 discovery-capability-0.4.7/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.7/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.7/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 23:04:29.714969 discovery-capability-0.4.7/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.7/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.523233 discovery-capability-0.4.7/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 23:04:29.000000 discovery-capability-0.4.7/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-24 23:04:29.000000 discovery-capability-0.4.7/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-24 23:04:29.000000 discovery-capability-0.4.7/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-24 23:04:29.000000 discovery-capability-0.4.7/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-24 23:04:29.000000 discovery-capability-0.4.7/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.523637 discovery-capability-0.4.7/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-24 23:02:22.000000 discovery-capability-0.4.7/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.526218 discovery-capability-0.4.7/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.7/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13503 2023-07-24 23:04:05.000000 discovery-capability-0.4.7/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3135 2023-07-24 22:34:35.000000 discovery-capability-0.4.7/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5246 2023-07-24 22:53:50.000000 discovery-capability-0.4.7/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.7/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.526927 discovery-capability-0.4.7/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.7/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.531104 discovery-capability-0.4.7/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.7/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.7/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.7/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.7/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    65928 2023-07-23 23:20:52.000000 discovery-capability-0.4.7/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.7/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.534013 discovery-capability-0.4.7/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.7/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.7/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.7/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.7/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.706140 discovery-capability-0.4.7/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.7/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.7/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-24 23:04:29.715585 discovery-capability-0.4.7/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.7/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.709036 discovery-capability-0.4.7/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.7/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.710734 discovery-capability-0.4.7/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.7/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.7/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.7/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.711579 discovery-capability-0.4.7/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.7/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 23:04:29.714207 discovery-capability-0.4.7/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.7/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.7/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.7/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2983 2023-07-21 16:56:46.000000 discovery-capability-0.4.7/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.7/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.751383 discovery-capability-0.4.8/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-25 13:19:27.751701 discovery-capability-0.4.8/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.601534 discovery-capability-0.4.8/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.602381 discovery-capability-0.4.8/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-24 23:05:27.000000 discovery-capability-0.4.8/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.606983 discovery-capability-0.4.8/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.8/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13503 2023-07-24 23:04:05.000000 discovery-capability-0.4.8/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3135 2023-07-24 22:34:35.000000 discovery-capability-0.4.8/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5246 2023-07-24 22:53:50.000000 discovery-capability-0.4.8/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.8/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.608039 discovery-capability-0.4.8/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.8/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.613149 discovery-capability-0.4.8/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.8/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.8/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.8/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    66414 2023-07-25 13:15:36.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.618163 discovery-capability-0.4.8/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.8/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.8/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.8/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.8/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.740487 discovery-capability-0.4.8/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.8/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-25 13:19:27.752799 discovery-capability-0.4.8/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.8/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.744904 discovery-capability-0.4.8/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.8/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.746289 discovery-capability-0.4.8/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.8/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.8/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.8/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.747314 discovery-capability-0.4.8/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.8/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.750591 discovery-capability-0.4.8/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.8/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.8/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.8/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-25 13:17:32.000000 discovery-capability-0.4.8/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.8/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.4.7/LICENSE.txt` & `discovery-capability-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/PKG-INFO` & `discovery-capability-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.7
+Version: 0.4.8
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.7/README.rst` & `discovery-capability-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.4.8/discovery_capability.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.7
+Version: 0.4.8
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.7/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.4.8/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.4.8/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/components/commons.py` & `discovery-capability-0.4.8/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/components/discovery.py` & `discovery-capability-0.4.8/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/components/feature_build.py` & `discovery-capability-0.4.8/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.4.8/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/intent/common_intent.py` & `discovery-capability-0.4.8/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.4.8/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.4.8/ds_capability/intent/feature_build_intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -913,35 +913,42 @@
         _ = self.get_sample(sample_name='us_street_names', size=size, seed=seed, column_name='string',  save_intent=False)
         canonical = Commons.table_append(canonical, _)
         # binary
         _ = self.get_string_pattern(pattern='cccccccc', as_binary=True, size=size, seed=seed, column_name='binary', save_intent=False)
         canonical = Commons.table_append(canonical, _)
 
         if isinstance(inc_nulls, bool) and inc_nulls:
+            gen = np.random.default_rng()
             # cat_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_category(selection=['M', 'F', 'U'], relative_freq=[9,8,4], quantity=1 - prob_nulls,
                                   column_name='cat_null', size=size, seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # num_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_number(start=-1.0, stop=1.0, relative_freq=[1, 1, 2, 3, 5, 8, 13, 21], size=size,
                                 quantity=1 - prob_nulls, column_name='num_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # int_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_number(start=-1000, stop=1000, size=size, quantity=1 - prob_nulls, column_name='int_null',
                                 seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # bool_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_boolean(size=size, probability=0.4, seed=seed, quantity=1 - prob_nulls,
                                  column_name='bool_null', save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # date_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_datetime(start='2022-12-01', until='2023-03-31', ordered=True, size=size, quantity=1 - prob_nulls,
                                   column_name='date_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # string_null
+            prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_sample(sample_name='us_cities', size=size, quantity=1 - prob_nulls,
                                 column_name='string_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # nulls_int
             _ = pa.table([pa.array(pa.nulls(size), pa.int64())], names=['nulls_int'])
             canonical = Commons.table_append(canonical, _)
             # nulls_date
```

### Comparing `discovery-capability-0.4.7/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.4.8/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.4.8/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.4.8/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.4.8/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.4.8/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.4.8/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.4.8/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.4.8/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.4.8/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/ds_capability/sample/sample_data.py` & `discovery-capability-0.4.8/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/setup.py` & `discovery-capability-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/test/component/discovery_test.py` & `discovery-capability-0.4.8/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/test/component/synthetic_test.py` & `discovery-capability-0.4.8/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.4.8/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.4.8/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.7/test/intent/fb_intent_test.py` & `discovery-capability-0.4.8/test/intent/fb_intent_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     def test_for_smoke(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
         tbl = tools.get_synthetic_data_types(100)
         self.assertEqual((100, 7), tbl.shape)
         tbl = tools.get_synthetic_data_types(100, inc_nulls=True, prob_nulls=0.03)
         self.assertEqual((100, 17), tbl.shape)
-        self.assertEqual(3, tbl.column('int_null').null_count)
 
     def test_run_component_pipeline(self):
         fb = FeatureBuild.from_env('test', has_contract=False)
         tools: FeatureBuildIntentModel = fb.tools
         # reload the properties
         fb = FeatureBuild.from_env('test')
         _ = tools.get_synthetic_data_types(10, inc_nulls=True, column_name='d_types')
```

### Comparing `discovery-capability-0.4.7/test/intent/fb_model_intent_test.py` & `discovery-capability-0.4.8/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

