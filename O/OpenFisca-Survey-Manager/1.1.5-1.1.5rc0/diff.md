# Comparing `tmp/OpenFisca-Survey-Manager-1.1.5.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.1.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.1.5.tar", last modified: Mon Jul 24 16:53:51 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.1.5rc0.tar", last modified: Tue Jul 25 09:23:35 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.1.5.tar` & `OpenFisca-Survey-Manager-1.1.5rc0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.572287 OpenFisca-Survey-Manager-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)    18922 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.564287 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2583 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-24 16:53:51.000000 OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-24 16:53:51.572287 OpenFisca-Survey-Manager-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.568287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.568287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.568287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/config_files_templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/config_files_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    13337 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.568287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10027 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.572287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:51.572287 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/data_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13736 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-24 16:53:51.572287 OpenFisca-Survey-Manager-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-24 16:53:27.000000 OpenFisca-Survey-Manager-1.1.5/setup.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.718342 OpenFisca-Survey-Manager-1.1.5rc0/
+-rw-r--r--   0 sch        (501) staff       (20)    18922 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/CHANGELOG.md
+-rw-r--r--   0 sch        (501) staff       (20)    34499 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/LICENSE.AGPL.txt
+-rw-r--r--   0 sch        (501) staff       (20)      192 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/MANIFEST.in
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.694063 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 sch        (501) staff       (20)    14349 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 sch        (501) staff       (20)     2583 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 sch        (501) staff       (20)        1 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 sch        (501) staff       (20)       92 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 sch        (501) staff       (20)        1 2022-03-14 13:49:44.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 sch        (501) staff       (20)      759 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 sch        (501) staff       (20)       25 2023-07-25 09:23:35.000000 OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 sch        (501) staff       (20)    14349 2023-07-25 09:23:35.718495 OpenFisca-Survey-Manager-1.1.5rc0/PKG-INFO
+-rw-r--r--   0 sch        (501) staff       (20)    13432 2023-07-20 14:57:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/README.md
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.705047 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/
+-rw-r--r--   0 sch        (501) staff       (20)     2109 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 sch        (501) staff       (20)    17292 2023-07-06 12:30:07.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.708529 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/
+-rw-r--r--   0 sch        (501) staff       (20)     3551 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 sch        (501) staff       (20)      451 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 sch        (501) staff       (20)     1571 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 sch        (501) staff       (20)    12096 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 sch        (501) staff       (20)     6262 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 sch        (501) staff       (20)    10517 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 sch        (501) staff       (20)     9929 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 sch        (501) staff       (20)     3167 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 sch        (501) staff       (20)      741 2023-07-06 12:30:07.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/config.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.709201 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/config_files_templates/
+-rw-r--r--   0 sch        (501) staff       (20)        0 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/config_files_templates/__init__.py
+-rw-r--r--   0 sch        (501) staff       (20)      836 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 sch        (501) staff       (20)    13337 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 sch        (501) staff       (20)     4606 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/matching.py
+-rw-r--r--   0 sch        (501) staff       (20)     1386 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 sch        (501) staff       (20)      653 2023-07-06 12:30:07.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 sch        (501) staff       (20)      493 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 sch        (501) staff       (20)    79765 2023-07-20 14:57:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.710011 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scripts/
+-rw-r--r--   0 sch        (501) staff       (20)        0 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 sch        (501) staff       (20)    10027 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 sch        (501) staff       (20)    11312 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 sch        (501) staff       (20)     5365 2023-07-20 14:57:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 sch        (501) staff       (20)    10119 2022-02-15 09:57:11.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 sch        (501) staff       (20)     9552 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tables.py
+-rw-r--r--   0 sch        (501) staff       (20)     3302 2023-07-06 12:30:07.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.717468 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/
+-rw-r--r--   0 sch        (501) staff       (20)        0 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 sch        (501) staff       (20)        0 2023-07-25 09:23:35.718105 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 sch        (501) staff       (20)        0 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/data_files/__init__.py
+-rw-r--r--   0 sch        (501) staff       (20)      381 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 sch        (501) staff       (20)     3539 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 sch        (501) staff       (20)     2457 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 sch        (501) staff       (20)     1694 2023-07-06 12:30:07.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 sch        (501) staff       (20)     5223 2023-07-20 14:57:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 sch        (501) staff       (20)      989 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 sch        (501) staff       (20)     3556 2023-07-04 09:02:15.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 sch        (501) staff       (20)     4373 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 sch        (501) staff       (20)      792 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 sch        (501) staff       (20)    13736 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 sch        (501) staff       (20)      716 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 sch        (501) staff       (20)     1601 2023-07-25 08:43:49.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 sch        (501) staff       (20)     1671 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 sch        (501) staff       (20)      386 2021-04-26 14:42:27.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 sch        (501) staff       (20)    10433 2023-07-20 14:57:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/utils.py
+-rw-r--r--   0 sch        (501) staff       (20)     2850 2021-12-02 14:02:41.000000 OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/variables.py
+-rw-r--r--   0 sch        (501) staff       (20)     1084 2023-07-25 09:23:35.719856 OpenFisca-Survey-Manager-1.1.5rc0/setup.cfg
+-rw-r--r--   0 sch        (501) staff       (20)     3408 2023-07-25 09:23:20.000000 OpenFisca-Survey-Manager-1.1.5rc0/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.1.5/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.1.5rc0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.1.5rc0/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.5
+Version: 1.1.5rc0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.1.5rc0/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.5
+Version: 1.1.5rc0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.1.5/README.md` & `OpenFisca-Survey-Manager-1.1.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.1.5rc0/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/setup.cfg` & `OpenFisca-Survey-Manager-1.1.5rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.5/setup.py` & `OpenFisca-Survey-Manager-1.1.5rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.1.5',
+    version = '1.1.5-rc.0',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

