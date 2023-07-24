# Comparing `tmp/discovery-capability-0.4.3.tar.gz` & `tmp/discovery-capability-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.4.3.tar", last modified: Mon Jul 24 22:48:02 2023, max compression
+gzip compressed data, was "discovery-capability-0.4.4.tar", last modified: Mon Jul 24 22:50:38 2023, max compression
```

## Comparing `discovery-capability-0.4.3.tar` & `discovery-capability-0.4.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.061051 discovery-capability-0.4.3/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.3/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.3/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:48:02.061400 discovery-capability-0.4.3/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.3/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.899675 discovery-capability-0.4.3/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:48:01.000000 discovery-capability-0.4.3/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-24 22:48:01.000000 discovery-capability-0.4.3/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-24 22:48:01.000000 discovery-capability-0.4.3/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-24 22:48:01.000000 discovery-capability-0.4.3/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-24 22:48:01.000000 discovery-capability-0.4.3/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.900123 discovery-capability-0.4.3/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-24 22:41:17.000000 discovery-capability-0.4.3/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.903198 discovery-capability-0.4.3/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.3/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13439 2023-07-24 22:32:02.000000 discovery-capability-0.4.3/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3135 2023-07-24 22:34:35.000000 discovery-capability-0.4.3/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5367 2023-07-24 22:47:33.000000 discovery-capability-0.4.3/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.3/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.903879 discovery-capability-0.4.3/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.3/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.907789 discovery-capability-0.4.3/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.3/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.3/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.3/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.3/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    65928 2023-07-23 23:20:52.000000 discovery-capability-0.4.3/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.3/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:01.910039 discovery-capability-0.4.3/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.3/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.3/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.3/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.3/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.050034 discovery-capability-0.4.3/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.3/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.3/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-24 22:48:02.062216 discovery-capability-0.4.3/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.3/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.054720 discovery-capability-0.4.3/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.3/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.055968 discovery-capability-0.4.3/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.3/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.3/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.3/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.056618 discovery-capability-0.4.3/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.3/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:48:02.060074 discovery-capability-0.4.3/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.3/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.3/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.3/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2983 2023-07-21 16:56:46.000000 discovery-capability-0.4.3/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.3/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.689153 discovery-capability-0.4.4/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.4/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.4/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:50:38.689373 discovery-capability-0.4.4/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.4/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.541796 discovery-capability-0.4.4/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-24 22:50:38.000000 discovery-capability-0.4.4/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-24 22:50:38.000000 discovery-capability-0.4.4/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-24 22:50:38.000000 discovery-capability-0.4.4/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-24 22:50:38.000000 discovery-capability-0.4.4/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-24 22:50:38.000000 discovery-capability-0.4.4/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.542218 discovery-capability-0.4.4/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-24 22:48:57.000000 discovery-capability-0.4.4/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.545840 discovery-capability-0.4.4/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.4/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13439 2023-07-24 22:32:02.000000 discovery-capability-0.4.4/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3135 2023-07-24 22:34:35.000000 discovery-capability-0.4.4/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5258 2023-07-24 22:50:09.000000 discovery-capability-0.4.4/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.4/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.546664 discovery-capability-0.4.4/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.4/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.551965 discovery-capability-0.4.4/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.4/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.4/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.4/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.4/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    65928 2023-07-23 23:20:52.000000 discovery-capability-0.4.4/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.4/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.554922 discovery-capability-0.4.4/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.4/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.4/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.4/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.4/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.682245 discovery-capability-0.4.4/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.4/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.4/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-24 22:50:38.689973 discovery-capability-0.4.4/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.4/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.684477 discovery-capability-0.4.4/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.4/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.685662 discovery-capability-0.4.4/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.4/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.4/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.4/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.686259 discovery-capability-0.4.4/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.4/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-24 22:50:38.688567 discovery-capability-0.4.4/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.4/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.4/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.4/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2983 2023-07-21 16:56:46.000000 discovery-capability-0.4.4/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.4/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.4.3/LICENSE.txt` & `discovery-capability-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/PKG-INFO` & `discovery-capability-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.3
+Version: 0.4.4
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.3/README.rst` & `discovery-capability-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.4.4/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.3
+Version: 0.4.4
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.3/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.4.4/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.4.4/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/components/commons.py` & `discovery-capability-0.4.4/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/components/discovery.py` & `discovery-capability-0.4.4/ds_capability/components/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,15 @@
             _ = df_style.applymap(DataDiscovery._highlight_null_dom, subset=['Nulls', 'Dominate'])
             _ = df_style.applymap(lambda x: 'color: white' if x > 0.98 else 'color: black', subset=['Nulls', 'Dominate'])
             _ = df_style.applymap(DataDiscovery._dtype_color, subset=['DataType'])
             _ = df_style.applymap(DataDiscovery._color_unique, subset=['Unique'])
             _ = df_style.applymap(lambda x: 'color: white' if x < 2 else 'color: black', subset=['Unique'])
             _ = df_style.format({'Nulls': "{:.1%}", 'Dominate': '{:.1%}'})
             _ = df_style.set_caption(f"dataset has {canonical.num_columns} columns")
-            _ = df_style.set_properties(subset=[f'Attributes ({len(df.columns)})'],  **{'font-weight': 'bold',
-                                                                                        'font-size': "120%"})
+            _ = df_style.set_properties(subset=['Attributes'],  **{'font-weight': 'bold', 'font-size': "120%"})
             return df_style
         return pa.Table.from_pandas(df)
 
     @staticmethod
     def _dtype_color(dtype: str):
         """Apply color to types"""
         if str(dtype).startswith('cat'):
```

### Comparing `discovery-capability-0.4.3/ds_capability/components/feature_build.py` & `discovery-capability-0.4.4/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.4.4/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/intent/common_intent.py` & `discovery-capability-0.4.4/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.4.4/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.4.4/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.4.4/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.4.4/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.4.4/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.4.4/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.4.4/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.4.4/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.4.4/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.4.4/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.4.4/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.4.4/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/ds_capability/sample/sample_data.py` & `discovery-capability-0.4.4/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/setup.py` & `discovery-capability-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/component/discovery_test.py` & `discovery-capability-0.4.4/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/component/synthetic_test.py` & `discovery-capability-0.4.4/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.4.4/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.4.4/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/intent/fb_intent_test.py` & `discovery-capability-0.4.4/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.3/test/intent/fb_model_intent_test.py` & `discovery-capability-0.4.4/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

