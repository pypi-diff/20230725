# Comparing `tmp/floatcsep-0.1.3.tar.gz` & `tmp/floatcsep-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatcsep-0.1.3.tar", last modified: Thu Jul 20 11:05:04 2023, max compression
+gzip compressed data, was "floatcsep-0.1.4.tar", last modified: Tue Jul 25 13:33:52 2023, max compression
```

## Comparing `floatcsep-0.1.3.tar` & `floatcsep-0.1.4.tar`

### file list

```diff
@@ -1,136 +1,125 @@
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/
--rw-r--r--   0 pciturri (19030) rs        (1400)     5219 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 pciturri (19030) rs        (1400)     8212 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 pciturri (19030) rs        (1400)      439 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CREDITS.md
--rw-r--r--   0 pciturri (19030) rs        (1400)     1518 2023-05-23 12:15:34.000000 floatcsep-0.1.3/LICENSE
--rw-r--r--   0 pciturri (19030) rs        (1400)      455 2023-05-31 12:03:11.000000 floatcsep-0.1.3/MANIFEST.in
--rw-r--r--   0 pciturri (19030) rs        (1400)     4688 2023-07-20 11:05:04.920320 floatcsep-0.1.3/PKG-INFO
--rw-r--r--   0 pciturri (19030) rs        (1400)     4023 2023-07-20 10:59:33.000000 floatcsep-0.1.3/README.md
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/
--rw-r--r--   0 pciturri (19030) rs        (1400)      773 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/Makefile
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/_static/
--rw-r--r--   0 pciturri (19030) rs        (1400)    82639 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/CSEP2_Logo_CMYK.png
--rw-r--r--   0 pciturri (19030) rs        (1400)    33945 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/floatCSEP_Logo_CMYK.png
--rw-r--r--   0 pciturri (19030) rs        (1400)    65939 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/floatcsep_logo.svg
--rw-r--r--   0 pciturri (19030) rs        (1400)     1947 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/conf.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/deployment/
--rw-r--r--   0 pciturri (19030) rs        (1400)       42 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/deployment/intro.rst
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/examples/
--rw-r--r--   0 pciturri (19030) rs        (1400)     6130 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_a.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     2941 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_b.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     2619 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_c.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     3710 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_d.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     3148 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_e.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     5439 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_f.rst
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/guide/
--rw-r--r--   0 pciturri (19030) rs        (1400)       62 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/config.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)       46 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/model_config.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)       40 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/region_config.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)       50 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/tests_config.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)       44 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/time_config.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     1086 2023-05-31 13:57:12.000000 floatcsep-0.1.3/docs/index.rst
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/intro/
--rw-r--r--   0 pciturri (19030) rs        (1400)     1924 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/intro/concepts.rst
--rw-r--r--   0 pciturri (19030) rs        (1400)     1486 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/intro/installation.rst
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/reference/
--rw-r--r--   0 pciturri (19030) rs        (1400)     3152 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/reference/api_reference.rst
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/
--rw-r--r--   0 pciturri (19030) rs        (1400)      268 2023-07-20 10:59:33.000000 floatcsep-0.1.3/floatcsep/__init__.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    11610 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/accessors.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/artifacts/
--rw-r--r--   0 pciturri (19030) rs        (1400)   178905 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/artifacts/new_zealand_csep_testing.csv
--rw-r--r--   0 pciturri (19030) rs        (1400)      810 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/artifacts/patterns.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/cmd/
--rw-r--r--   0 pciturri (19030) rs        (1400)     2544 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/cmd/main.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    14225 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/evaluation.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    39254 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/experiment.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    33199 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/extras.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     1223 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/logger.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    19583 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/model.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    12132 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/readers.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     9988 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/registry.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     3175 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/report.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    54973 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/utils.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep.egg-info/
--rw-r--r--   0 pciturri (19030) rs        (1400)     4688 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/PKG-INFO
--rw-r--r--   0 pciturri (19030) rs        (1400)     3090 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/SOURCES.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)        1 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/dependency_links.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)       59 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/entry_points.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)        1 2023-05-23 12:47:51.000000 floatcsep-0.1.3/floatcsep.egg-info/not-zip-safe
--rw-r--r--   0 pciturri (19030) rs        (1400)      388 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/requires.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)       10 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/top_level.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)      179 2023-05-23 12:15:35.000000 floatcsep-0.1.3/pyproject.toml
--rw-r--r--   0 pciturri (19030) rs        (1400)      110 2023-07-19 14:28:35.000000 floatcsep-0.1.3/requirements.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)      204 2023-07-19 14:28:35.000000 floatcsep-0.1.3/requirements_dev.txt
--rw-r--r--   0 pciturri (19030) rs        (1400)     1336 2023-07-20 11:05:04.920320 floatcsep-0.1.3/setup.cfg
--rw-r--r--   0 pciturri (19030) rs        (1400)       69 2023-05-23 12:15:35.000000 floatcsep-0.1.3/setup.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/
--rw-r--r--   0 pciturri (19030) rs        (1400)    53248 2023-07-19 13:22:13.000000 floatcsep-0.1.3/tests/.coverage
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-31 12:15:02.000000 floatcsep-0.1.3/tests/.floatcsep.log
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/
--rw-r--r--   0 pciturri (19030) rs        (1400)     1064 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/catalog.json
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/evaluations/
--rw-r--r--   0 pciturri (19030) rs        (1400)      377 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/evaluations/tests_cfg.yml
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/gcmt/
--rw-r--r--   0 pciturri (19030) rs        (1400)     1722 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/gcmt/vcr_search.yaml
--rw-r--r--   0 pciturri (19030) rs        (1400)     1347 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/gcmt/vcr_summary.yaml
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/models/
--rw-r--r--   0 pciturri (19030) rs        (1400)      182 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model.csv
--rw-r--r--   0 pciturri (19030) rs        (1400)      184 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model_cfg.yml
--rw-r--r--   0 pciturri (19030) rs        (1400)     4640 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model_h5.hdf5
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/qtree/
--rw-r--r--   0 pciturri (19030) rs        (1400)  5734026 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N10L11.csv
--rw-r--r--   0 pciturri (19030) rs        (1400)  2468253 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N25L11.csv
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/artifacts/models/td_model/
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/td_model/input/
--rw-r--r--   0 pciturri (19030) rs        (1400)       32 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/artifacts/models/td_model/input/args.txt
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/template/
--rw-r--r--   0 pciturri (19030) rs        (1400)     2010 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/Dockerfile
--rw-r--r--   0 pciturri (19030) rs        (1400)     3522 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/README.md
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/docs/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/docs/userguide
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/artifacts/models/template/examples/
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/case3_run
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/data/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/data/case3_catalog
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/forecasts/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/forecasts/template_2023-01-01
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/input/
--rw-r--r--   0 pciturri (19030) rs        (1400)      169 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/input/catalog
--rw-r--r--   0 pciturri (19030) rs        (1400)      715 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/parameters
--rw-r--r--   0 pciturri (19030) rs        (1400)       35 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/requirements
--rw-r--r--   0 pciturri (19030) rs        (1400)      768 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/run
--rw-r--r--   0 pciturri (19030) rs        (1400)      138 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/run_tests
--rw-r--r--   0 pciturri (19030) rs        (1400)      148 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/setup
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/source/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/lib_a
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/lib_b
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/main
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/tests/
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_liba
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_libb
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_main
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/
--rw-r--r--   0 pciturri (19030) rs        (1400)      341 2023-05-23 14:47:58.000000 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/datapackage.json
--rw-r--r--   0 pciturri (19030) rs        (1400)     6144 2023-05-23 14:48:00.000000 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/table.xls
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/regions/
--rw-r--r--   0 pciturri (19030) rs        (1400)   106101 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/regions/italy_midpoints
--rw-r--r--   0 pciturri (19030) rs        (1400)       23 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/regions/mock_region
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/integration/
--rw-r--r--   0 pciturri (19030) rs        (1400)     1178 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/integration/experiment typologies
--rw-r--r--   0 pciturri (19030) rs        (1400)     2423 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/integration/test_data.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     3349 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/integration/test_model_interface.py
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/unit/
--rw-r--r--   0 pciturri (19030) rs        (1400)    53248 2023-07-19 14:25:04.000000 floatcsep-0.1.3/tests/unit/.coverage
--rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-31 12:31:59.000000 floatcsep-0.1.3/tests/unit/.floatcsep.log
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/unit/results/
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/
-drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/catalog/
--rw-r--r--   0 pciturri (19030) rs        (1400)     1317 2023-07-19 14:25:04.000000 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/catalog/catalog.json
--rw-r--r--   0 pciturri (19030) rs        (1400)     3884 2023-05-31 12:35:27.000000 floatcsep-0.1.3/tests/unit/test_accessors.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     3068 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/unit/test_evaluation.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     6871 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_experiment.py
--rw-r--r--   0 pciturri (19030) rs        (1400)    10846 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_model.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     7282 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/unit/test_readers.py
--rw-r--r--   0 pciturri (19030) rs        (1400)     6854 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.642913 floatcsep-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-25 13:32:44.000000 floatcsep-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-25 13:32:44.000000 floatcsep-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 13:32:44.000000 floatcsep-0.1.4/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-25 13:32:44.000000 floatcsep-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 13:32:44.000000 floatcsep-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-25 13:33:52.642913 floatcsep-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-25 13:32:44.000000 floatcsep-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.610913 floatcsep-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.610913 floatcsep-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    82639 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/_static/CSEP2_Logo_CMYK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/_static/floatCSEP_Logo_CMYK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65939 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/_static/floatcsep_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.610913 floatcsep-0.1.4/docs/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/deployment/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.614913 floatcsep-0.1.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_a.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_b.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_c.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_d.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_e.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/examples/case_f.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.614913 floatcsep-0.1.4/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/guide/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/guide/model_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/guide/region_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/guide/tests_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/guide/time_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.614913 floatcsep-0.1.4/docs/intro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/intro/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/intro/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.614913 floatcsep-0.1.4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-25 13:32:44.000000 floatcsep-0.1.4/docs/reference/api_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.614913 floatcsep-0.1.4/floatcsep/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/accessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/floatcsep/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)   178905 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/artifacts/new_zealand_csep_testing.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/artifacts/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/floatcsep/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/cmd/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39254 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-07-25 13:32:44.000000 floatcsep-0.1.4/floatcsep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/floatcsep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 13:33:52.000000 floatcsep-0.1.4/floatcsep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 13:32:44.000000 floatcsep-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 13:32:44.000000 floatcsep-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-25 13:32:44.000000 floatcsep-0.1.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-25 13:33:52.642913 floatcsep-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 13:32:44.000000 floatcsep-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.606913 floatcsep-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/tests/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/catalog.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/tests/artifacts/evaluations/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/evaluations/tests_cfg.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/tests/artifacts/gcmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/gcmt/vcr_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/gcmt/vcr_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.618913 floatcsep-0.1.4/tests/artifacts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/model_cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/model_h5.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.630913 floatcsep-0.1.4/tests/artifacts/models/qtree/
+-rw-r--r--   0 runner    (1001) docker     (123)  5734026 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/qtree/TEAM=N10L11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2468253 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/qtree/TEAM=N25L11.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.606913 floatcsep-0.1.4/tests/artifacts/models/td_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.634913 floatcsep-0.1.4/tests/artifacts/models/td_model/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/td_model/input/args.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.634913 floatcsep-0.1.4/tests/artifacts/models/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.634913 floatcsep-0.1.4/tests/artifacts/models/template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/docs/userguide
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.606913 floatcsep-0.1.4/tests/artifacts/models/template/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.634913 floatcsep-0.1.4/tests/artifacts/models/template/examples/case_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/examples/case_3/case3_run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.634913 floatcsep-0.1.4/tests/artifacts/models/template/examples/case_3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/examples/case_3/data/case3_catalog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/artifacts/models/template/forecasts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/forecasts/template_2023-01-01
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/artifacts/models/template/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/input/catalog
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/parameters
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/requirements
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/run
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/run_tests
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/setup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/artifacts/models/template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/source/lib_a
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/source/lib_b
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/source/main
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/artifacts/models/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/tests/test_liba
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/tests/test_libb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/models/template/tests/test_main
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/artifacts/regions/
+-rw-r--r--   0 runner    (1001) docker     (123)   106101 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/regions/italy_midpoints
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/artifacts/regions/mock_region
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.638913 floatcsep-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/integration/experiment typologies
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/integration/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/integration/test_model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:33:52.642913 floatcsep-0.1.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-25 13:32:44.000000 floatcsep-0.1.4/tests/unit/test_utils.py
```

### Comparing `floatcsep-0.1.3/CODE_OF_CONDUCT.md` & `floatcsep-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/CONTRIBUTING.md` & `floatcsep-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/LICENSE` & `floatcsep-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/PKG-INFO` & `floatcsep-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatcsep
-Version: 0.1.3
+Version: 0.1.4
 Summary: CSEP Floating Experiment application
 Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta
 Author-email: pciturri@gfz-potsdam.de
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: floatcsep Version: 0.1.3 Summary: CSEP Floating
+Metadata-Version: 2.1 Name: floatcsep Version: 0.1.4 Summary: CSEP Floating
 Experiment application Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta Author-email: pciturri@gfz-potsdam.de License: BSD 3-
 Clause License Platform: unix Platform: linux Platform: osx Platform: win32
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `floatcsep-0.1.3/README.md` & `floatcsep-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/Makefile` & `floatcsep-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/_static/CSEP2_Logo_CMYK.png` & `floatcsep-0.1.4/docs/_static/CSEP2_Logo_CMYK.png`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/_static/floatCSEP_Logo_CMYK.png` & `floatcsep-0.1.4/docs/_static/floatCSEP_Logo_CMYK.png`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/_static/floatcsep_logo.svg` & `floatcsep-0.1.4/docs/_static/floatcsep_logo.svg`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/conf.py` & `floatcsep-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_a.rst` & `floatcsep-0.1.4/docs/examples/case_a.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_b.rst` & `floatcsep-0.1.4/docs/examples/case_b.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_c.rst` & `floatcsep-0.1.4/docs/examples/case_c.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_d.rst` & `floatcsep-0.1.4/docs/examples/case_d.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_e.rst` & `floatcsep-0.1.4/docs/examples/case_e.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/examples/case_f.rst` & `floatcsep-0.1.4/docs/examples/case_f.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/index.rst` & `floatcsep-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/intro/concepts.rst` & `floatcsep-0.1.4/docs/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/intro/installation.rst` & `floatcsep-0.1.4/docs/intro/installation.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/docs/reference/api_reference.rst` & `floatcsep-0.1.4/docs/reference/api_reference.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/accessors.py` & `floatcsep-0.1.4/floatcsep/accessors.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/artifacts/new_zealand_csep_testing.csv` & `floatcsep-0.1.4/floatcsep/artifacts/new_zealand_csep_testing.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/artifacts/patterns.py` & `floatcsep-0.1.4/floatcsep/artifacts/patterns.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/cmd/main.py` & `floatcsep-0.1.4/floatcsep/cmd/main.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/evaluation.py` & `floatcsep-0.1.4/floatcsep/evaluation.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/experiment.py` & `floatcsep-0.1.4/floatcsep/experiment.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/extras.py` & `floatcsep-0.1.4/floatcsep/extras.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy
 import scipy.stats
+from matplotlib import pyplot
 from csep.models import EvaluationResult
 from csep.core.poisson_evaluations import _simulate_catalog, paired_t_test, \
     w_test, _poisson_likelihood_test
 from csep.core.exceptions import CSEPCatalogException
 from typing import Sequence
 from csep.core.forecasts import GriddedForecast
 from csep.core.catalogs import CSEPCatalog
@@ -335,21 +336,21 @@
         test_distribution=[0],
         sim_name=forecast.name
     )
     return result
 
 
 def _nbd_number_test_ndarray(fore_cnt, obs_cnt, variance, epsilon=1e-6):
-    """ 
+    """
     Computes delta1 and delta2 values from the Negative Binomial (NBD) number test.
 
     Args:
         fore_cnt (float): parameter of negative binomial distribution coming from expected value of the forecast
         obs_cnt (float): count of earthquakes observed during the testing period.
-        variance (float): variance parameter of negative binomial distribution coming from historical catalog. 
+        variance (float): variance parameter of negative binomial distribution coming from historical catalog.
         A variance value of approximately 23541 has been calculated using M5.95+ earthquakes observed worldwide from 1982 to 2013.
         epsilon (float): tolerance level to satisfy the requirements of two-sided p-value
 
     Returns
         result (tuple): (delta1, delta2)
     """
     var = variance
@@ -366,27 +367,27 @@
 
 def negative_binomial_number_test(gridded_forecast, observed_catalog,
                                   variance):
     """
     Computes "negative binomial N-Test" on a gridded forecast.
 
     Computes Number (N) test for Observed and Forecasts. Both data sets are expected to be in terms of event counts.
-    We find the Total number of events in Observed Catalog and Forecasted Catalogs. Which are then employed to compute the 
+    We find the Total number of events in Observed Catalog and Forecasted Catalogs. Which are then employed to compute the
     probablities of
     (i) At least no. of events (delta 1)
     (ii) At most no. of events (delta 2) assuming the negative binomial distribution.
 
     Args:
         gridded_forecast:   Forecast of a Model (Gridded) (Numpy Array)
                     A forecast has to be in terms of Average Number of Events in Each Bin
                     It can be anything greater than zero
         observed_catalog:   Observed (Gridded) seismicity (Numpy Array):
                     An Observation has to be Number of Events in Each Bin
                     It has to be a either zero or positive integer only (No Floating Point)
-        variance:   Variance parameter of negative binomial distribution obtained from historical catalog.            
+        variance:   Variance parameter of negative binomial distribution obtained from historical catalog.
 
     Returns:
         out (tuple): (delta_1, delta_2)
     """
     result = EvaluationResult()
 
     # observed count
@@ -413,15 +414,15 @@
 
     return result
 
 
 def binomial_joint_log_likelihood_ndarray(forecast, catalog):
     """
     Computes Bernoulli log-likelihood scores, assuming that earthquakes follow a binomial distribution.
-    
+
     Args:
         forecast:   Forecast of a Model (Gridded) (Numpy Array)
                     A forecast has to be in terms of Average Number of Events in Each Bin
                     It can be anything greater than zero
         catalog:    Observed (Gridded) seismicity (Numpy Array):
                     An Observation has to be Number of Events in Each Bin
                     It has to be a either zero or positive integer only (No Floating Point)
@@ -450,15 +451,15 @@
     Computes binary conditional-likelihood test from CSEP using an efficient simulation based approach.
     Args:
         forecast_data (numpy.ndarray): nd array where [:, -1] are the magnitude bins.
         observed_data (numpy.ndarray): same format as observation.
         num_simulations: default number of simulations to use for likelihood based simulations
         seed: used for reproducibility of the prng
         random_numbers (numpy.ndarray): can supply an explicit list of random numbers, primarily used for software testing
-        use_observed_counts (bool): if true, will simulate catalogs using the observed events, if false will draw from poisson 
+        use_observed_counts (bool): if true, will simulate catalogs using the observed events, if false will draw from poisson
         distribution
     """
 
     # Array-masking that avoids log singularities:
     forecast_data = numpy.ma.masked_where(forecast_data <= 0.0, forecast_data)
 
     # set seed for the likelihood test
@@ -577,23 +578,23 @@
     result.min_mw = numpy.min(gridded_forecast.magnitudes)
 
     return result
 
 
 def _binary_t_test_ndarray(target_event_rates1, target_event_rates2, n_obs,
                            n_f1, n_f2, catalog, alpha=0.05):
-    """ 
+    """
     Computes binary T test statistic by comparing two target event rate distributions.
 
-    We compare Forecast from Model 1 and with Forecast of Model 2. Information Gain per Active Bin (IGPA) is computed, which is then 
-    employed to compute T statistic. Confidence interval of Information Gain can be computed using T_critical. For a complete 
-    explanation see Rhoades, D. A., et al., (2011). Efficient testing of earthquake forecasting models. Acta Geophysica, 59(4), 
-    728-747. doi:10.2478/s11600-011-0013-5, and Bayona J.A. et al., (2022). Prospective evaluation of multiplicative hybrid earthquake 
+    We compare Forecast from Model 1 and with Forecast of Model 2. Information Gain per Active Bin (IGPA) is computed, which is then
+    employed to compute T statistic. Confidence interval of Information Gain can be computed using T_critical. For a complete
+    explanation see Rhoades, D. A., et al., (2011). Efficient testing of earthquake forecasting models. Acta Geophysica, 59(4),
+    728-747. doi:10.2478/s11600-011-0013-5, and Bayona J.A. et al., (2022). Prospective evaluation of multiplicative hybrid earthquake
     forecasting models in California. doi: 10.1093/gji/ggac018.
-    
+
     Args:
         target_event_rates1 (numpy.ndarray): nd-array storing target event rates
         target_event_rates2 (numpy.ndarray): nd-array storing target event rates
         n_obs (float, int, numpy.ndarray): number of observed earthquakes, should be whole number and >= zero.
         n_f1 (float): Total number of forecasted earthquakes by Model 1
         n_f2 (float): Total number of forecasted earthquakes by Model 2
         catalog: csep.core.catalogs.Catalog
@@ -661,16 +662,16 @@
 
 
 def _standard_deviation(gridded_forecast1, gridded_forecast2,
                         gridded_observation1, gridded_observation2, cell_area1,
                         cell_area2):
     """
     Calculate Variance using forecast 1 and forecast 2.
-    But It is calculated using the forecast values corresponding to the non-zero observations. 
-    The same process is repeated as repeated during calculation of Point Process LL. 
+    But It is calculated using the forecast values corresponding to the non-zero observations.
+    The same process is repeated as repeated during calculation of Point Process LL.
     After we get forecast rates for non-zeros observations, then Pooled Variance is calculated.
 
 
     Parameters
     ----------
         gridded_forecast1 : forecast
         gridded_forecast2 : benchmark_forecast
@@ -802,7 +803,163 @@
     result.observed_statistic = out['information_gain']
     result.quantile = (out['t_statistic'], out['t_critical'])
     result.sim_name = (forecast.name, benchmark_forecast.name)
     result.obs_name = observed_catalog.name
     result.status = 'normal'
     result.min_mw = numpy.min(forecast.magnitudes)
     return result
+
+
+def plot_negbinom_consistency_test(eval_results, normalize=False, axes=None,
+                          one_sided_lower=False, variance=None, plot_args=None,
+                          show=False):
+    """ Plots results from CSEP1 tests following the CSEP1 convention.
+
+    Note: All of the evaluations should be from the same type of evaluation, otherwise the results will not be
+          comparable on the same figure.
+
+    Args:
+        eval_results (list): Contains the tests results :class:`csep.core.evaluations.EvaluationResult` (see note above)
+        normalize (bool): select this if the forecast likelihood should be normalized by the observed likelihood. useful
+                          for plotting simulation based simulation tests.
+        one_sided_lower (bool): select this if the plot should be for a one sided test
+        plot_args(dict): optional argument containing a dictionary of plotting arguments, with keys as strings and items as described below
+
+    Optional plotting arguments:
+        * figsize: (:class:`list`/:class:`tuple`) - default: [6.4, 4.8]
+        * title: (:class:`str`) - default: name of the first evaluation result type
+        * title_fontsize: (:class:`float`) Fontsize of the plot title - default: 10
+        * xlabel: (:class:`str`) - default: 'X'
+        * xlabel_fontsize: (:class:`float`) - default: 10
+        * xticks_fontsize: (:class:`float`) - default: 10
+        * ylabel_fontsize: (:class:`float`) - default: 10
+        * color: (:class:`float`/:class:`None`) If None, sets it to red/green according to :func:`_get_marker_style` - default: 'black'
+        * linewidth: (:class:`float`) - default: 1.5
+        * capsize: (:class:`float`) - default: 4
+        * hbars:  (:class:`bool`)  Flag to draw horizontal bars for each model - default: True
+        * tight_layout: (:class:`bool`) Set matplotlib.figure.tight_layout to remove excess blank space in the plot - default: True
+
+    Returns:
+        ax (:class:`matplotlib.pyplot.axes` object)
+    """
+
+    try:
+        results = list(eval_results)
+    except TypeError:
+        results = [eval_results]
+    results.reverse()
+    # Parse plot arguments. More can be added here
+    if plot_args is None:
+        plot_args = {}
+    figsize = plot_args.get('figsize', None)
+    title = plot_args.get('title', results[0].name)
+    title_fontsize = plot_args.get('title_fontsize', None)
+    xlabel = plot_args.get('xlabel', '')
+    xlabel_fontsize = plot_args.get('xlabel_fontsize', None)
+    xticks_fontsize = plot_args.get('xticks_fontsize', None)
+    ylabel_fontsize = plot_args.get('ylabel_fontsize', None)
+    color = plot_args.get('color', 'black')
+    linewidth = plot_args.get('linewidth', None)
+    capsize = plot_args.get('capsize', 4)
+    hbars = plot_args.get('hbars', True)
+    tight_layout = plot_args.get('tight_layout', True)
+    percentile = plot_args.get('percentile', 95)
+    plot_mean = plot_args.get('mean', False)
+
+    if axes is None:
+        fig, ax = pyplot.subplots(figsize=figsize)
+    else:
+        ax = axes
+        fig = ax.get_figure()
+
+    xlims = []
+
+    for index, res in enumerate(results):
+        var = variance
+        observed_statistic = res.observed_statistic
+        mean = res.test_distribution[1]
+        upsilon = 1.0 - ((var - mean) / var)
+        tau = (mean ** 2 / (var - mean))
+        plow = scipy.stats.nbinom.ppf((1 - percentile / 100.) / 2., tau,
+                                       upsilon)
+        phigh = scipy.stats.nbinom.ppf(1 - (1 - percentile / 100.) / 2.,
+                                      tau, upsilon)
+
+        if not numpy.isinf(
+                observed_statistic):  # Check if test result does not diverges
+            percentile_lims = numpy.array([[mean - plow, phigh - mean]]).T
+            ax.plot(observed_statistic, index,
+                    _get_marker_style(observed_statistic, (plow, phigh),
+                                      one_sided_lower))
+            ax.errorbar(mean, index, xerr=percentile_lims,
+                        fmt='ko' * plot_mean, capsize=capsize,
+                        linewidth=linewidth, ecolor=color)
+            # determine the limits to use
+            xlims.append((plow, phigh, observed_statistic))
+            # we want to only extent the distribution where it falls outside of it in the acceptable tail
+            if one_sided_lower:
+                if observed_statistic >= plow and phigh < observed_statistic:
+                    # draw dashed line to infinity
+                    xt = numpy.linspace(phigh, 99999, 100)
+                    yt = numpy.ones(100) * index
+                    ax.plot(xt, yt, linestyle='--', linewidth=linewidth,
+                            color=color)
+
+        else:
+            print('Observed statistic diverges for forecast %s, index %i.'
+                  ' Check for zero-valued bins within the forecast' % (
+                      res.sim_name, index))
+            ax.barh(index, 99999, left=-10000, height=1, color=['red'],
+                    alpha=0.5)
+
+    try:
+        ax.set_xlim(*_get_axis_limits(xlims))
+    except ValueError:
+        raise ValueError(
+            'All EvaluationResults have infinite observed_statistics')
+    ax.set_yticks(numpy.arange(len(results)))
+    ax.set_yticklabels([res.sim_name for res in results],
+                       fontsize=ylabel_fontsize)
+    ax.set_ylim([-0.5, len(results) - 0.5])
+    if hbars:
+        yTickPos = ax.get_yticks()
+        if len(yTickPos) >= 2:
+            ax.barh(yTickPos, numpy.array([99999] * len(yTickPos)),
+                    left=-10000,
+                    height=(yTickPos[1] - yTickPos[0]), color=['w', 'gray'],
+                    alpha=0.2, zorder=0)
+    ax.set_title(title, fontsize=title_fontsize)
+    ax.set_xlabel(xlabel, fontsize=xlabel_fontsize)
+    ax.tick_params(axis='x', labelsize=xticks_fontsize)
+    if tight_layout:
+        ax.figure.tight_layout()
+        fig.tight_layout()
+
+    if show:
+        pyplot.show()
+
+    return ax
+
+
+def _get_marker_style(obs_stat, p, one_sided_lower):
+    """Returns matplotlib marker style as fmt string"""
+    if obs_stat < p[0] or obs_stat > p[1]:
+        # red circle
+        fmt = 'ro'
+    else:
+        # green square
+        fmt = 'gs'
+    if one_sided_lower:
+        if obs_stat < p[0]:
+            fmt = 'ro'
+        else:
+            fmt = 'gs'
+    return fmt
+
+
+def _get_axis_limits(pnts, border=0.05):
+    """Returns a tuple of x_min and x_max given points on plot."""
+    x_min = numpy.min(pnts)
+    x_max = numpy.max(pnts)
+    xd = (x_max - x_min) * border
+    return (x_min - xd, x_max + xd)
+
```

### Comparing `floatcsep-0.1.3/floatcsep/logger.py` & `floatcsep-0.1.4/floatcsep/logger.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/model.py` & `floatcsep-0.1.4/floatcsep/model.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/readers.py` & `floatcsep-0.1.4/floatcsep/readers.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/registry.py` & `floatcsep-0.1.4/floatcsep/registry.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/report.py` & `floatcsep-0.1.4/floatcsep/report.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep/utils.py` & `floatcsep-0.1.4/floatcsep/utils.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/floatcsep.egg-info/PKG-INFO` & `floatcsep-0.1.4/floatcsep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatcsep
-Version: 0.1.3
+Version: 0.1.4
 Summary: CSEP Floating Experiment application
 Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta
 Author-email: pciturri@gfz-potsdam.de
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: floatcsep Version: 0.1.3 Summary: CSEP Floating
+Metadata-Version: 2.1 Name: floatcsep Version: 0.1.4 Summary: CSEP Floating
 Experiment application Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta Author-email: pciturri@gfz-potsdam.de License: BSD 3-
 Clause License Platform: unix Platform: linux Platform: osx Platform: win32
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `floatcsep-0.1.3/floatcsep.egg-info/SOURCES.txt` & `floatcsep-0.1.4/floatcsep.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 floatcsep.egg-info/entry_points.txt
 floatcsep.egg-info/not-zip-safe
 floatcsep.egg-info/requires.txt
 floatcsep.egg-info/top_level.txt
 floatcsep/artifacts/new_zealand_csep_testing.csv
 floatcsep/artifacts/patterns.py
 floatcsep/cmd/main.py
-tests/.coverage
-tests/.floatcsep.log
 tests/artifacts/catalog.json
 tests/artifacts/evaluations/tests_cfg.yml
 tests/artifacts/gcmt/vcr_search.yaml
 tests/artifacts/gcmt/vcr_summary.yaml
 tests/artifacts/models/model.csv
 tests/artifacts/models/model_cfg.yml
 tests/artifacts/models/model_h5.hdf5
@@ -77,23 +75,18 @@
 tests/artifacts/models/template/input/catalog
 tests/artifacts/models/template/source/lib_a
 tests/artifacts/models/template/source/lib_b
 tests/artifacts/models/template/source/main
 tests/artifacts/models/template/tests/test_liba
 tests/artifacts/models/template/tests/test_libb
 tests/artifacts/models/template/tests/test_main
-tests/artifacts/models/zenodo_test/datapackage.json
-tests/artifacts/models/zenodo_test/table.xls
 tests/artifacts/regions/italy_midpoints
 tests/artifacts/regions/mock_region
 tests/integration/experiment typologies
 tests/integration/test_data.py
 tests/integration/test_model_interface.py
-tests/unit/.coverage
-tests/unit/.floatcsep.log
 tests/unit/test_accessors.py
 tests/unit/test_evaluation.py
 tests/unit/test_experiment.py
 tests/unit/test_model.py
 tests/unit/test_readers.py
-tests/unit/test_utils.py
-tests/unit/results/2021-01-01_2022-01-01/catalog/catalog.json
+tests/unit/test_utils.py
```

### Comparing `floatcsep-0.1.3/setup.cfg` & `floatcsep-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = floatcsep
 description = CSEP Floating Experiment application
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Pablo Iturrieta
 author_email = pciturri@gfz-potsdam.de
 license = BSD 3-Clause License
-version = 0.1.3
+version = 0.1.4
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
```

### Comparing `floatcsep-0.1.3/tests/artifacts/catalog.json` & `floatcsep-0.1.4/tests/artifacts/catalog.json`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/gcmt/vcr_search.yaml` & `floatcsep-0.1.4/tests/artifacts/gcmt/vcr_search.yaml`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/gcmt/vcr_summary.yaml` & `floatcsep-0.1.4/tests/artifacts/gcmt/vcr_summary.yaml`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/model_h5.hdf5` & `floatcsep-0.1.4/tests/artifacts/models/model_h5.hdf5`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N10L11.csv` & `floatcsep-0.1.4/tests/artifacts/models/qtree/TEAM=N10L11.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N25L11.csv` & `floatcsep-0.1.4/tests/artifacts/models/qtree/TEAM=N25L11.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/template/Dockerfile` & `floatcsep-0.1.4/tests/artifacts/models/template/Dockerfile`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/template/README.md` & `floatcsep-0.1.4/tests/artifacts/models/template/README.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/template/parameters` & `floatcsep-0.1.4/tests/artifacts/models/template/parameters`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/models/template/run` & `floatcsep-0.1.4/tests/artifacts/models/template/run`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/artifacts/regions/italy_midpoints` & `floatcsep-0.1.4/tests/artifacts/regions/italy_midpoints`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/integration/experiment typologies` & `floatcsep-0.1.4/tests/integration/experiment typologies`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/integration/test_data.py` & `floatcsep-0.1.4/tests/integration/test_data.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/integration/test_model_interface.py` & `floatcsep-0.1.4/tests/integration/test_model_interface.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_accessors.py` & `floatcsep-0.1.4/tests/unit/test_accessors.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_evaluation.py` & `floatcsep-0.1.4/tests/unit/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_experiment.py` & `floatcsep-0.1.4/tests/unit/test_experiment.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_model.py` & `floatcsep-0.1.4/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_readers.py` & `floatcsep-0.1.4/tests/unit/test_readers.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.3/tests/unit/test_utils.py` & `floatcsep-0.1.4/tests/unit/test_utils.py`

 * *Files identical despite different names*

