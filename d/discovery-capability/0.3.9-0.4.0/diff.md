# Comparing `tmp/discovery-capability-0.3.9.tar.gz` & `tmp/discovery-capability-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.3.9.tar", last modified: Mon Jul 10 15:37:16 2023, max compression
+gzip compressed data, was "discovery-capability-0.4.0.tar", last modified: Mon Jul 24 22:25:03 2023, max compression
```

## Comparing `discovery-capability-0.3.9.tar` & `discovery-capability-0.4.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.669992 discovery-capability-0.3.9/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-10 15:37:16.670201 discovery-capability-0.3.9/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.3.9/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.507549 discovery-capability-0.3.9/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2277 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-10 15:37:16.000000 discovery-capability-0.3.9/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.507878 discovery-capability-0.3.9/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-09 20:27:05.000000 discovery-capability-0.3.9/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.512700 discovery-capability-0.3.9/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.3.9/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13813 2023-07-01 22:58:06.000000 discovery-capability-0.3.9/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1336 2023-06-29 23:02:32.000000 discovery-capability-0.3.9/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6359 2023-07-01 22:36:22.000000 discovery-capability-0.3.9/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.3.9/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.514252 discovery-capability-0.3.9/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.3.9/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.519410 discovery-capability-0.3.9/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.3.9/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11272 2023-07-09 15:15:11.000000 discovery-capability-0.3.9/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.3.9/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    64528 2023-07-09 21:53:32.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13425 2023-07-08 16:42:07.000000 discovery-capability-0.3.9/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.524035 discovery-capability-0.3.9/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.3.9/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.3.9/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.3.9/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.3.9/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.664138 discovery-capability-0.3.9/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.3.9/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.3.9/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-10 15:37:16.671000 discovery-capability-0.3.9/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.3.9/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.665083 discovery-capability-0.3.9/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.3.9/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.666698 discovery-capability-0.3.9/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.3.9/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2072 2023-07-01 22:50:31.000000 discovery-capability-0.3.9/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.3.9/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.667409 discovery-capability-0.3.9/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.3.9/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-10 15:37:16.669327 discovery-capability-0.3.9/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.3.9/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2715 2023-07-09 23:06:27.000000 discovery-capability-0.3.9/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.3.9/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2946 2023-07-09 20:40:49.000000 discovery-capability-0.3.9/test/intent/fb_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.374630 discovery-capability-0.4.0/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.0/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.0/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:25:03.374947 discovery-capability-0.4.0/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.0/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.222906 discovery-capability-0.4.0/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:25:03.000000 discovery-capability-0.4.0/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-24 22:25:03.000000 discovery-capability-0.4.0/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-24 22:25:03.000000 discovery-capability-0.4.0/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-24 22:25:03.000000 discovery-capability-0.4.0/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-24 22:25:03.000000 discovery-capability-0.4.0/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.223234 discovery-capability-0.4.0/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-21 22:52:19.000000 discovery-capability-0.4.0/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.226328 discovery-capability-0.4.0/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.0/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13813 2023-07-01 22:58:06.000000 discovery-capability-0.4.0/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1336 2023-06-29 23:02:32.000000 discovery-capability-0.4.0/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5394 2023-07-24 22:04:51.000000 discovery-capability-0.4.0/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.0/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.227297 discovery-capability-0.4.0/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.0/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.232112 discovery-capability-0.4.0/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.0/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.0/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.0/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.0/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    65928 2023-07-23 23:20:52.000000 discovery-capability-0.4.0/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.0/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.236081 discovery-capability-0.4.0/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.0/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.0/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.0/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.0/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.364553 discovery-capability-0.4.0/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.0/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.0/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-24 22:25:03.375669 discovery-capability-0.4.0/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.0/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.368026 discovery-capability-0.4.0/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.0/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.369431 discovery-capability-0.4.0/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.0/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.0/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.0/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.370689 discovery-capability-0.4.0/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.0/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:25:03.373986 discovery-capability-0.4.0/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.0/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.0/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.0/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2983 2023-07-21 16:56:46.000000 discovery-capability-0.4.0/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.0/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.3.9/LICENSE.txt` & `discovery-capability-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/PKG-INFO` & `discovery-capability-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.3.9
+Version: 0.4.0
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.3.9/README.rst` & `discovery-capability-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.4.0/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.3.9
+Version: 0.4.0
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.3.9/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.4.0/discovery_capability.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 test/component/__init__.py
 test/component/discovery_test.py
 test/component/synthetic_test.py
 test/handlers/__init__.py
 test/intent/__init__.py
 test/intent/fb_analysis_intent_test.py
 test/intent/fb_diff_intent_test.py
-test/intent/fb_intent_test.py
+test/intent/fb_intent_test.py
+test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.3.9/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.4.0/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/components/commons.py` & `discovery-capability-0.4.0/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/components/feature_build.py` & `discovery-capability-0.4.0/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.4.0/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,16 @@
         :param params: the parameters passed to the method. use `locals()` in the caller method
         :param exclude: (optional) convenience parameter identifying param keys to exclude.
         :return: dict of the intent
         """
         exclude = []
         if 'canonical' in params.keys() and not isinstance(params.get('canonical'), (str, dict, list)):
             exclude.append('canonical')
+        if 'other' in params.keys() and not isinstance(params.get('other'), (str, dict, list)):
+            exclude.append('other')
         return super()._intent_builder(method=method, params=params, exclude=exclude)
 
     def _set_intend_signature(self, intent_params: dict, column_name: [int, str] = None, intent_order: int = None,
                               replace_intent: bool = None, remove_duplicates: bool = None, save_intent: bool = None):
         """ sets the intent section in the configuration file. Note: by default any identical intent, e.g.
         intent with the same intent (name) and the same parameter values, are removed from any level.
```

### Comparing `discovery-capability-0.3.9/ds_capability/intent/common_intent.py` & `discovery-capability-0.4.0/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.4.0/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.4.0/ds_capability/intent/feature_build_intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         environment variable name
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         start = self._extract_value(start)
         stop = self._extract_value(stop)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if not isinstance(start, (int, float)) and not isinstance(stop, (int, float)):
             raise ValueError(f"either a 'from_value' or a 'from_value' and 'to_value' must be provided")
         if not isinstance(start, (float, int)):
@@ -124,23 +126,23 @@
             try:
                 rtn_arr = pa.array(rtn_arr, pa.int64())
             except pa.lib.ArrowInvalid:
                 pass
         column_name = column_name if isinstance(column_name, str) else next(self.label_gen)
         return pa.table([rtn_arr], names=[column_name])
 
-    def get_category(self, selection: list, size: int, relative_freq: list=None, quantity: float=None, seed: int=None,
-                     save_intent: bool=None, column_name: [int, str]=None, intent_order: int=None,
-                     replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
-        """ returns a category from a list. Of particular not is the at_least parameter that allows you to
-        control the number of times a selection can be chosen.
+    def get_category(self, selection: list, size: int, relative_freq: list=None, encode: bool=None,
+                     quantity: float=None, seed: int=None, save_intent: bool=None, column_name: [int, str]=None,
+                     intent_order: int=None, replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
+        """ returns a categorical as a string.
 
         :param selection: a list of items to select from
         :param size: size of the return
         :param relative_freq: a weighting pattern that does not have to add to 1
+        :param encode: if the categorical should be returned encoded as a dictionary type or string type (default)
         :param quantity: a number between 0 and 1 representing the percentage quantity of the data
         :param seed: a seed value for the random function: default to None
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
         :param intent_order: (optional) the order in which each intent should run.
                     - If None: default's to -1
                     - if -1: added to a level above any current instance of the intent section, level 0 if not found
@@ -154,28 +156,33 @@
         :return: an item or list of items chosen from the list
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         if len(selection) < 1:
             return [None] * size
+        encode = encode if isinstance(encode, bool) else False
         seed = self._seed() if seed is None else seed
         relative_freq = relative_freq if isinstance(relative_freq, list) else [1]*len(selection)
         select_index = self._freq_dist_size(relative_freq=relative_freq, size=size, dist_length=len(selection),
                                                   dist_on='right', seed=seed)
         rtn_list = []
         for idx in range(len(select_index)):
             rtn_list += [selection[idx]]*select_index[idx]
         gen = np.random.default_rng(seed)
         gen.shuffle(rtn_list)
         rtn_list = self._set_quantity(rtn_list, quantity=self._quantity(quantity), seed=seed)
         column_name = column_name if isinstance(column_name, str) else next(self.label_gen)
-        return pa.table([pa.DictionaryArray.from_pandas(rtn_list).dictionary_encode()], names=[column_name])
+        if encode:
+            return pa.table([pa.DictionaryArray.from_pandas(rtn_list).dictionary_encode()], names=[column_name])
+        return pa.table([pa.DictionaryArray.from_pandas(rtn_list)], names=[column_name])
 
     def get_boolean(self, size: int, probability: float=None, quantity: float=None, seed: int=None,
                     save_intent: bool=None, column_name: [int, str]=None, intent_order: int=None,
                     replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
         """A boolean discrete random distribution
 
         :param size: the size of the sample
@@ -197,14 +204,16 @@
         :return: a random number
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         prob = probability if isinstance(probability, int) and 0 < probability < 1 else 0.5
         seed = self._seed(seed=seed)
         rtn_list = list(stats.bernoulli.rvs(p=probability, size=size, random_state=seed))
         rtn_list = list(map(bool, rtn_list))
         rtn_list = self._set_quantity(rtn_list, quantity=self._quantity(quantity), seed=seed)
         column_name = column_name if isinstance(column_name, str) else next(self.label_gen)
         return pa.table([pa.NumericArray.from_pandas(rtn_list)], names=[column_name])
@@ -250,31 +259,27 @@
         :param replace_intent: (optional) if the intent method exists at the level, or default level
                     - True - replaces the current intent method with the new
                     - False - leaves it untouched, disregarding the new intent
 
         :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
         :return: a date or size of dates in the format given.
          """
-        # pre check
-        if start is None or until is None:
-            raise ValueError("The start or until parameters cannot be of NoneType")
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if start is None or until is None:
             raise ValueError("The start or until parameters cannot be of NoneType")
         # Code block for intent
         as_num = as_num if isinstance(as_num, bool) else False
         ignore_seconds = ignore_seconds if isinstance(ignore_seconds, bool) else False
         ignore_time = ignore_time if isinstance(ignore_time, bool) else False
-        size = 1 if size is None else size
         seed = self._seed() if seed is None else seed
         # start = start.to_pydatetime() if isinstance(start, pd.Timestamp) else start
         # until = until.to_pydatetime() if isinstance(until, pd.Timestamp) else until
         if isinstance(start, int):
             start = (pd.Timestamp.now() + pd.Timedelta(days=start))
         start = pd.to_datetime(start, errors='coerce', dayfirst=day_first,
                                yearfirst=year_first)
@@ -646,18 +651,19 @@
         :return: a string based on the pattern
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         choice_only = False if choice_only is None or not isinstance(choice_only, bool) else choice_only
         as_binary = as_binary if isinstance(as_binary, bool) else False
         quantity = self._quantity(quantity)
-        size = size if isinstance(size, int) and size > 0 else 1
         seed = self._seed(seed=seed)
         if choices is None or not isinstance(choices, dict):
             choices = {'c': list(string.ascii_letters),
                        'd': list(string.digits),
                        'l': list(string.ascii_lowercase),
                        'U': list(string.ascii_uppercase),
                        'p': list(string.punctuation),
@@ -719,27 +725,29 @@
         :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
         :return: a sample list
         """
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
-        size = 1 if size is None else size
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         sample_size = sample_name if isinstance(sample_size, int) else size
         quantity = self._quantity(quantity)
         seed = self._seed(seed=seed)
         shuffle = shuffle if isinstance(shuffle, bool) else True
         selection = eval(f"Sample.{sample_name}(size={size}, shuffle={shuffle}, seed={seed})")
         rtn_list = self._set_quantity(selection, quantity=quantity, seed=seed)
         column_name = column_name if isinstance(column_name, str) else next(self.label_gen)
         return pa.table([pa.Array.from_pandas(rtn_list)], names=[column_name])
 
     def get_analysis(self, size: int, other: [str, pa.Table], category_limit: int=None, date_jitter: int=None,
-                     date_units: str=None, date_ordered: bool=None, seed: int=None, save_intent: bool=None, column_name: [int, str]=None,
-                     intent_order: int=None, replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
+                     date_units: str=None, date_ordered: bool=None, seed: int=None, save_intent: bool=None,
+                     column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
+                     remove_duplicates: bool=None) -> pa.Table:
         """ builds a set of columns based on another (see analyse_association)
         if a reference DataFrame is passed then as the analysis is run if the column already exists the row
         value will be taken as the reference to the sub category and not the random value. This allows already
         constructed association to be used as reference for a sub category.
 
         :param size: The number of rows
         :param other: a direct or generated pd.DataFrame. see context notes below
@@ -766,24 +774,26 @@
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         other = self._get_canonical(other)
         if other is None or other.num_rows == 0:
             return None
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         date_jitter = date_jitter if isinstance(date_jitter, int) else 2
         units_allowed = ['W', 'D', 'h', 'm', 's', 'milli', 'micro']
         date_units = date_units if isinstance(date_units, str) and date_units in units_allowed else 'D'
         date_ordered = date_ordered if isinstance(date_ordered, bool) else False
         seed = self._seed(seed=seed)
         rtn_tbl = None
         gen = np.random.default_rng(seed)
         for c in other.column_names:
             column = other.column(c)
-            if column.drop_null().length() == 0:
+            if (pa.types.is_boolean(column.type) and pc.all(column).as_py() == False) or len(column.drop_null()) == 0:
                 result = pa.table([pa.nulls(size)], names=[c])
                 rtn_tbl = Commons.table_append(rtn_tbl, result)
                 continue
             nulls = round(column.null_count / other.num_rows, 5)
             column = column.combine_chunks().drop_null()
             if pa.types.is_dictionary(column.type):
                 selection = column.dictionary.to_pylist()
@@ -800,14 +810,16 @@
                     result = pd.concat([result, _], axis=0)
                 result = result.sample(frac=1).iloc[:size].astype(column.type.to_pandas_dtype()).reset_index(drop=True)
                 result = self._set_quantity(result, quantity=self._quantity(1-nulls), seed=seed)
                 result = pa.table([pa.Array.from_pandas(result)], names=[c])
             elif pa.types.is_boolean(column.type):
                 frequency = dict(zip(column.value_counts().field(0).to_pylist(),
                                      column.value_counts().field(1).to_pylist())).get(True)
+                if frequency is None:
+                    frequency = 0
                 prob = frequency/size
                 prob = prob if 0 < prob < 1 else 0.5
                 _ = gen.choice([True, False,], size=size, p=[prob, 1 - prob])
                 result = self._set_quantity(_, quantity=self._quantity(1 - nulls), seed=seed)
                 result = pa.table([pa.BinaryArray.from_pandas(result)], names=[c])
             elif pa.types.is_string(column.type):
                 # for the moment do nothing with strings
@@ -839,23 +851,25 @@
                 result = pa.table([pa.TimestampArray.from_pandas(result)], names=[c])
             else:
                 # return nulls for other types
                 result = pa.table([pa.nulls(size)], names=[c])
             rtn_tbl = Commons.table_append(rtn_tbl, result)
         return rtn_tbl
 
-    def get_synthetic_data_types(self, size: int, inc_nulls: bool=None, p_nulls: float=None, seed: int=None,
-                                 save_intent: bool=None, column_name: [int, str]=None, intent_order: int=None,
-                                 replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
+    def get_synthetic_data_types(self, size: int, inc_nulls: bool=None, prob_nulls: float=None, seed: int=None,
+                                 category_encode: bool=None, save_intent: bool=None, column_name: [int, str]=None,
+                                 intent_order: int=None, replace_intent: bool=None,
+                                 remove_duplicates: bool=None) -> pa.Table:
         """ A dataset with example data types
 
-        :param size:
+        :param size: The size of the sample
         :param inc_nulls: include values with nulls
-        :param p_nulls: a value between 0 an 1 of the percentage of nulls in the *_nulls column. Default is 0.02
-        :param seed: a seed value for the random function: default to None
+        :param prob_nulls: (optional) a value between 0 an 1 of the percentage of nulls. Default 0.02
+        :param category_encode: (optional) if the categorical should be encoded to DictionaryArray
+        :param seed: (optional) a seed value for the random function: default to None
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
         :param intent_order: (optional) the order in which each intent should run.
                     - If None: default's to -1
                     - if -1: added to a level above any current instance of the intent section, level 0 if not found
                     - if int: added to the level specified, overwriting any that already exist
 
@@ -867,19 +881,23 @@
         :return: pandas DataSet
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed(seed=seed)
-        p_nulls = p_nulls if isinstance(p_nulls, float) and 0 < p_nulls < 1 else 0.02
+        prob_nulls = prob_nulls if isinstance(prob_nulls, float) and 0 < prob_nulls < 1 else 0.02
+        category_encode = category_encode if isinstance(category_encode, bool) else True
         # cat
-        _ = self.get_category(selection=['SUSPENDED', 'ACTIVE', 'PENDING', 'INACTIVE'], size=size, seed=seed,
-                              relative_freq=[1, 99, 10, 40], column_name='cat',  save_intent=False)
+        _ = self.get_category(selection=['SUSPENDED', 'ACTIVE', 'PENDING', 'INACTIVE', 'ARCHIVE'], size=size, seed=seed,
+                              relative_freq=[1, 70, 20, 30, 10], encode=category_encode, column_name='cat',
+                              save_intent=False)
         canonical = _
         # num
         _ = self.get_dist_normal(mean=0, std=1, size=size, seed=seed, column_name='num', save_intent=False)
         canonical = Commons.table_append(canonical, _)
         # int
         _ = self.get_number(start=size, stop=size * 10, at_most=1, size=size, seed=seed, column_name='int',
                             save_intent=False)
@@ -896,35 +914,35 @@
         canonical = Commons.table_append(canonical, _)
         # binary
         _ = self.get_string_pattern(pattern='cccccccc', as_binary=True, size=size, seed=seed, column_name='binary', save_intent=False)
         canonical = Commons.table_append(canonical, _)
 
         if isinstance(inc_nulls, bool) and inc_nulls:
             # cat_null
-            _ = self.get_category(selection=['M', 'F', 'U'], relative_freq=[9,8,4], quantity=1 - p_nulls,
+            _ = self.get_category(selection=['M', 'F', 'U'], relative_freq=[9,8,4], quantity=1 - prob_nulls,
                                   column_name='cat_null', size=size, seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # num_null
             _ = self.get_number(start=-1.0, stop=1.0, relative_freq=[1, 1, 2, 3, 5, 8, 13, 21], size=size,
-                                quantity=1 - p_nulls, column_name='num_null', seed=seed, save_intent=False)
+                                quantity=1 - prob_nulls, column_name='num_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # int_null
-            _ = self.get_number(start=-1000, stop=1000, size=size, quantity=1 - p_nulls, column_name='int_null',
+            _ = self.get_number(start=-1000, stop=1000, size=size, quantity=1 - prob_nulls, column_name='int_null',
                                 seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # bool_null
-            _ = self.get_boolean(size=size, probability=0.4, seed=seed, quantity=1 - p_nulls,
+            _ = self.get_boolean(size=size, probability=0.4, seed=seed, quantity=1 - prob_nulls,
                                  column_name='bool_null', save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # date_null
-            _ = self.get_datetime(start='2022-12-01', until='2023-03-31', ordered=True, size=size, quantity=1 - p_nulls,
+            _ = self.get_datetime(start='2022-12-01', until='2023-03-31', ordered=True, size=size, quantity=1 - prob_nulls,
                                   column_name='date_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # string_null
-            _ = self.get_sample(sample_name='us_cities', size=size, quantity=1 - p_nulls,
+            _ = self.get_sample(sample_name='us_cities', size=size, quantity=1 - prob_nulls,
                                 column_name='string_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # nulls_int
             _ = pa.table([pa.array(pa.nulls(size), pa.int64())], names=['nulls_int'])
             canonical = Commons.table_append(canonical, _)
             # nulls_date
             _ = pa.table([pa.array(pa.nulls(size), pa.timestamp('ns'))], names=['nulls_date'])
@@ -963,14 +981,16 @@
         :return: a DataFrame
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
+        if not isinstance(size, int):
+            raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed(seed=seed)
         num_columns = num_columns if isinstance(num_columns, int) else 1
         name_prefix = name_prefix if isinstance(name_prefix, str) else ''
         label_gen = Commons.label_gen()
         rtn_tbl = None
         generator = np.random.default_rng(seed=seed)
         for _ in range(num_columns):
```

### Comparing `discovery-capability-0.3.9/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.4.0/ds_capability/intent/feature_build_model_intent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import inspect
-from typing import Any
-import numpy as np
 import pandas as pd
 import pyarrow as pa
-import pyarrow.compute as pc
 from ds_capability.intent.abstract_feature_build_intent import AbstractFeatureBuildIntentModel
 from ds_capability.intent.common_intent import CommonsIntentModel
 from ds_capability.components.commons import Commons
 from ds_capability.managers.feature_build_property_manager import FeatureBuildPropertyManager
 
 
+# noinspection PyArgumentList
 class FeatureBuildModelIntent(AbstractFeatureBuildIntentModel, CommonsIntentModel):
 
     def __init__(self, property_manager: FeatureBuildPropertyManager, default_save_intent: bool=None,
                  default_intent_level: [str, int, float]=None, order_next_available: bool=None,
                  default_replace_intent: bool=None):
         """initialisation of the Intent class.
 
@@ -28,14 +26,71 @@
         default_intent_level = default_intent_level if isinstance(default_intent_level, (str, int, float)) else 'A'
         default_intent_order = -1 if isinstance(order_next_available, bool) and order_next_available else 0
         super().__init__(property_manager=property_manager, default_save_intent=default_save_intent,
                          default_intent_level=default_intent_level, default_intent_order=default_intent_order,
                          default_replace_intent=default_replace_intent)
         self.label_gen = Commons.label_gen()
 
+    def model_sample_link(self, canonical: pa.Table, other: [str, pa.Table], headers: list, replace: bool=None,
+                          rename_map: [dict, list]=None, multi_map: dict=None, relative_freq: list=None, seed: int=None,
+                          save_intent: bool=None, column_name: [int, str]=None, intent_order: int=None,
+                          replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
+        """ Takes a target dataset and samples from that target to the size of the canonical
+
+        :param canonical: a pa.Table as the reference table
+        :param other: a direct pa.Table or reference to a connector.
+        :param headers: the headers to be selected from the other table
+        :param rename_map: (optional) a direct (list) or named (dict) mapping to the headers names.
+        :param multi_map: (optional) multiple columns from a single e.g. {new_name: name} where name is copied new_name
+        :param replace: (optional) assuming other is bigger than canonical, selects without replacement when True
+        :param relative_freq: (optional) a weighting pattern of the selected data
+        :param seed: (optional) a seed value for the random function: default to None
+        :param save_intent: (optional) if the intent contract should be saved to the property manager
+        :param column_name: (optional) the column name that groups intent to create a column
+        :param intent_order: (optional) the order in which each intent should run.
+                    - If None: default's to -1
+                    - if -1: added to a level above any current instance of the intent section, level 0 if not found
+                    - if int: added to the level specified, overwriting any that already exist
+
+        :param replace_intent: (optional) if the intent method exists at the level, or default level
+                    - True - replaces the current intent method with the new
+                    - False - leaves it untouched, disregarding the new intent
+
+        :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
+        :return: a pa.Table
+        """
+        # intent persist options
+        self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
+                                   column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
+                                   remove_duplicates=remove_duplicates, save_intent=save_intent)
+        # intent action
+        canonical = self._get_canonical(canonical)
+        other = self._get_canonical(other)
+        headers = Commons.list_formatter(headers)
+        replace = replace if isinstance(replace, bool) else True
+        seed = self._seed() if seed is None else seed
+        # build the distribution sizes
+        if isinstance(relative_freq, list) and len(relative_freq) > 1:
+            relative_freq = self._freq_dist_size(relative_freq=relative_freq, size=other.shape[0], seed=seed)
+        else:
+            relative_freq = None
+        other = Commons.filter_columns(other, headers=headers).to_pandas()
+        other = other.sample(n=canonical.shape[0], weights=relative_freq, random_state=seed, ignore_index=True,
+                             replace=replace)
+        if isinstance(rename_map, list) and len(rename_map) == len(headers):
+            other.columns = rename_map
+        elif isinstance(rename_map, dict):
+            other.rename(mapper=rename_map, axis='columns', inplace=True)
+        if isinstance(multi_map, dict):
+            for k, v in multi_map.items():
+                if v in other.columns:
+                    other[k] = other[v]
+        other = pa.Table.from_pandas(other)
+        return Commons.table_append(canonical, other)
+
     def model_difference(self, canonical: pa.Table, other: [str, pa.Table], on_key: [str, list], drop_zero_sum: bool=None,
                          summary_connector: bool=None, flagged_connector: str=None, detail_connector: str=None,
                          unmatched_connector: str=None, seed: int=None, save_intent: bool=None,
                          column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
                          remove_duplicates: bool=None, **kwargs) -> pa.Table:
         """returns the difference between two canonicals, joined on a common and unique key.
         The ``on_key`` parameter can be a direct reference to the canonical column header or to an environment
@@ -49,16 +104,16 @@
 
         If the ``detail connector`` parameter is used, a detail report of the difference where the left and right
         values that differ are shown.
 
         If the ``unmatched connector`` parameter is used, the on_key's that don't match between left and right are
         reported
 
-        :param canonical: a direct or generated pd.DataFrame. see context notes below
-        :param other: a direct or generated pd.DataFrame. to concatenate
+        :param canonical: a pa.Table as the reference table
+        :param other: a direct pa.Table or reference to a connector.
         :param on_key: The name of the key that uniquely joins the canonical to others
         :param drop_zero_sum: (optional) drops rows and columns which has a total sum of zero differences
         :param summary_connector: (optional) a connector name where the summary report is sent
         :param flagged_connector: (optional) a connector name where the differences are flagged
         :param detail_connector: (optional) a connector name where the differences are shown
         :param unmatched_connector: (optional) a connector name where the unmatched keys are shown
         :param seed: (optional) this is a placeholder, here for compatibility across methods
@@ -71,39 +126,20 @@
 
         :param replace_intent: (optional) if the intent method exists at the level, or default level
                     - True - replaces the current intent method with the new
                     - False - leaves it untouched, disregarding the new intent
 
         :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
         :return: a pd.DataFrame
-
-        The other is a pd.DataFrame, a pd.Series or list, a connector contract str reference or a set of
-        parameter instructions on how to generate a pd.Dataframe. the description of each is:
-
-        - pd.Dataframe -> a deep copy of the pd.DataFrame
-        - pd.Series or list -> creates a pd.DataFrameof one column with the 'header' name or 'default' if not given
-        - str -> instantiates a connector handler with the connector_name and loads the DataFrame from the connection
-        - dict -> use canonical2dict(...) to help construct a dict with a 'method' to build a pd.DataFrame
-            methods:
-                - model_*(...) -> one of the SyntheticBuilder model methods and parameters
-                - @empty -> generates an empty pd.DataFrame where size and headers can be passed
-                    :size sets the index size of the dataframe
-                    :headers any initial headers for the dataframe
-                - @generate -> generate a synthetic file from a remote Domain Contract
-                    :task_name the name of the SyntheticBuilder task to run
-                    :repo_uri the location of the Domain Product
-                    :size (optional) a size to generate
-                    :seed (optional) if a seed should be applied
-                    :run_book (optional) if specific intent should be run only
-
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
+        # intent action
         canonical = self._get_canonical(canonical)
         other = self._get_canonical(other)
         seed = seed if isinstance(seed, int) else self._seed()
         drop_zero_sum = drop_zero_sum if isinstance(drop_zero_sum, bool) else False
         flagged_connector = self._extract_value(flagged_connector)
         summary_connector = self._extract_value(summary_connector)
         detail_connector = self._extract_value(detail_connector)
```

### Comparing `discovery-capability-0.3.9/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.4.0/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.4.0/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.4.0/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.4.0/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.4.0/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.4.0/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.4.0/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.4.0/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.4.0/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/ds_capability/sample/sample_data.py` & `discovery-capability-0.4.0/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/setup.py` & `discovery-capability-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/test/component/discovery_test.py` & `discovery-capability-0.4.0/test/component/discovery_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Pandas setup
 pd.set_option('max_colwidth', 320)
 pd.set_option('display.max_rows', 100)
 pd.set_option('display.max_columns', 99)
 pd.set_option('expand_frame_repr', True)
 
 
-class SyntheticTest(unittest.TestCase):
+class DiscoveryTest(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         pass
 
     @classmethod
     def tearDownClass(cls):
@@ -56,15 +56,15 @@
         except OSError:
             pass
 
     def test_for_smoke(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
         tbl = tools.get_synthetic_data_types(1_000)
-        result = DataDiscovery.data_dictionary(tbl)
+        result = DataDiscovery.data_dictionary(tbl, stylise=True)
         pprint(result)
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-capability-0.3.9/test/component/synthetic_test.py` & `discovery-capability-0.4.0/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.3.9/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.4.0/test/intent/fb_intent_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import unittest
 import os
 from pathlib import Path
 import shutil
 import pandas as pd
 import pyarrow as pa
+import pyarrow.compute as pc
 from ds_capability import FeatureBuild
 from ds_capability.intent.feature_build_intent import FeatureBuildIntentModel
 from aistac.properties.property_manager import PropertyManager
 
 # Pandas setup
 pd.set_option('max_colwidth', 320)
 pd.set_option('display.max_rows', 100)
 pd.set_option('display.max_columns', 99)
 pd.set_option('expand_frame_repr', True)
 
 
-class SyntheticTest(unittest.TestCase):
+class FeatureBuilderTest(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         pass
 
     @classmethod
     def tearDownClass(cls):
@@ -40,44 +41,48 @@
             os.makedirs(os.environ['HADRON_PM_PATH'])
         except OSError:
             pass
         try:
             os.makedirs(os.environ['HADRON_DEFAULT_PATH'])
         except OSError:
             pass
-        try:
-            shutil.copytree('../_test_data', os.path.join(os.environ['PWD'], 'working/source'))
-        except OSError:
-            pass
         PropertyManager._remove_all()
 
     def tearDown(self):
         try:
             shutil.rmtree('working')
         except OSError:
             pass
 
     def test_for_smoke(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
-        tbl = tools.get_synthetic_data_types(100, inc_nulls=True)
-        fb.add_connector_uri('sample', './working/source/data_type.parquet')
-        fb.save_canonical('sample', tbl)
+        tbl = tools.get_synthetic_data_types(100)
+        self.assertEqual((100, 7), tbl.shape)
+        tbl = tools.get_synthetic_data_types(100, inc_nulls=True, prob_nulls=0.03)
         self.assertEqual((100, 17), tbl.shape)
-        result = tools.get_analysis(1000, 'sample')
-        self.assertEqual((1000, 17), result.shape)
+        self.assertEqual(3, tbl.column('int_null').null_count)
+
+    def test_run_component_pipeline(self):
+        fb = FeatureBuild.from_env('test', has_contract=False)
+        tools: FeatureBuildIntentModel = fb.tools
+        # reload the properties
+        fb = FeatureBuild.from_env('test')
+        _ = tools.get_synthetic_data_types(10, inc_nulls=True, column_name='d_types')
+        result = fb.tools.run_intent_pipeline(size=20)
+        self.assertEqual((20, 17), result.shape)
 
-    def test_flattened_sample(self):
+    def test_model_noise(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
-        fb.add_connector_uri('sample', './working/source/complex_flatten_records.parquet')
-        tbl = fb.load_canonical('sample')
-        self.assertEqual((4, 20), tbl.shape)
-        result = tools.get_analysis(6, 'sample')
-        self.assertEqual((6, 20), result.shape)
+        tbl = tools.get_noise(10, num_columns=3)
+        self.assertEqual((10, 3), tbl.shape)
+        self.assertEqual(['A', 'B', 'C'], tbl.column_names)
+        tbl = tools.get_noise(10, num_columns=3, name_prefix='P_')
+        self.assertEqual(['P_A', 'P_B', 'P_C'], tbl.column_names)
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-capability-0.3.9/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.4.0/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

