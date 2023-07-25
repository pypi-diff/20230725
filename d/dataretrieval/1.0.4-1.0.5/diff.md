# Comparing `tmp/dataretrieval-1.0.4.tar.gz` & `tmp/dataretrieval-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataretrieval-1.0.4.tar", last modified: Wed Apr 26 21:39:09 2023, max compression
+gzip compressed data, was "dataretrieval-1.0.5.tar", last modified: Tue Jul 25 18:44:58 2023, max compression
```

## Comparing `dataretrieval-1.0.4.tar` & `dataretrieval-1.0.5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.688598 dataretrieval-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/sphinx-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.688598 dataretrieval-1.0.4/.gitlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitlab/issue_templates/reviewer_checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitlab/merge_request_templates/reviewer_checklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/code.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval/codes/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/nadp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40711 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/nwis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/streamstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/waterwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/wqp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/demos/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9869 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/NWIS_demo_1.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)    13027 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/R Python Vignette equivalents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/demos/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/datasets/peak_discharge_trends.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/demos/hydroshare/
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.704598 dataretrieval-1.0.4/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.704598 dataretrieval-1.0.4/docs/source/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/datasets/peak_discharge_trends.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/nwisdemo01.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/readme_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/rvignettes.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/siteinfo_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/nadp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/nwis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/streamstats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/waterwatch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/wqp.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/userguide/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/dataportals.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/timeconventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.712598 dataretrieval-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.768599 dataretrieval-1.0.4/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22902 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/nwis_sites.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    48992 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/water_use_allegheny.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/water_use_national.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14065 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_measurements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_pmcodes.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)  5998995 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_qwdata.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14869 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_dv.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_gwlevels.txt
--rwxr-xr-x   0 runner    (1001) docker     (123) 22180871 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_iv.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_peaks.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_ratings.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1429 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_site.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   198769 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_stats.txt
--rw-r--r--   0 runner    (1001) docker     (123) 21772141 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_activities.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_activity_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1442378 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_detection_limits.txt
--rw-r--r--   0 runner    (1001) docker     (123)   436730 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_habitat_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_organizations.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1029205 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_project_weights.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_projects.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_results.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)  2276131 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/nadp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/nwis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13455 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/waterservices_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7787 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/wqp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.742724 dataretrieval-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.622716 dataretrieval-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.634717 dataretrieval-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.github/workflows/sphinx-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.622716 dataretrieval-1.0.5/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.634717 dataretrieval-1.0.5/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.gitlab/issue_templates/reviewer_checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.634717 dataretrieval-1.0.5/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/.gitlab/merge_request_templates/reviewer_checklist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-25 18:44:58.742724 dataretrieval-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/code.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.638717 dataretrieval-1.0.5/dataretrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.642717 dataretrieval-1.0.5/dataretrieval/codes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/codes/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/codes/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/nadp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44127 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/streamstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/waterwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/dataretrieval/wqp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.638717 dataretrieval-1.0.5/dataretrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 18:44:58.000000 dataretrieval-1.0.5/dataretrieval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.642717 dataretrieval-1.0.5/demos/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9869 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/NWIS_demo_1.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13027 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/R Python Vignette equivalents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.642717 dataretrieval-1.0.5/demos/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/datasets/peak_discharge_trends.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.646718 dataretrieval-1.0.5/demos/hydroshare/
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.646718 dataretrieval-1.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.650718 dataretrieval-1.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.654718 dataretrieval-1.0.5/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.658718 dataretrieval-1.0.5/docs/source/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/datasets/peak_discharge_trends.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/nwisdemo01.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/readme_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/rvignettes.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/examples/siteinfo_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.658718 dataretrieval-1.0.5/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/meta/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/meta/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.662719 dataretrieval-1.0.5/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/nadp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/nwis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/streamstats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/waterwatch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/reference/wqp.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.662719 dataretrieval-1.0.5/docs/source/userguide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/userguide/dataportals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/docs/source/userguide/timeconventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:44:58.742724 dataretrieval-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.666719 dataretrieval-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:44:58.738724 dataretrieval-1.0.5/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22902 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/nwis_sites.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48992 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/water_use_allegheny.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/water_use_national.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14065 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterdata_measurements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterdata_pmcodes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5998995 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterdata_qwdata.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14869 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_dv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_gwlevels.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123) 22180871 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_iv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_peaks.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_ratings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1429 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_site.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   198769 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/waterservices_stats.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 21772141 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_activities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_activity_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1442378 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_detection_limits.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   436730 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_habitat_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_organizations.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1029205 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_project_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_projects.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_results.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2276131 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/data/wqp_sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/nadp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/nwis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13455 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/waterservices_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7787 2023-07-25 18:44:35.000000 dataretrieval-1.0.5/tests/wqp_test.py
```

### Comparing `dataretrieval-1.0.4/.github/workflows/python-package.yml` & `dataretrieval-1.0.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/.github/workflows/python-publish.yml` & `dataretrieval-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/.github/workflows/sphinx-docs.yml` & `dataretrieval-1.0.5/.github/workflows/sphinx-docs.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/.gitignore` & `dataretrieval-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/.gitlab/issue_templates/reviewer_checklist.md` & `dataretrieval-1.0.5/.gitlab/issue_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/.gitlab/merge_request_templates/reviewer_checklist.md` & `dataretrieval-1.0.5/.gitlab/merge_request_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/CONTRIBUTING.md` & `dataretrieval-1.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/DISCLAIMER.md` & `dataretrieval-1.0.5/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/LICENSE.md` & `dataretrieval-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/PKG-INFO` & `dataretrieval-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `dataretrieval-1.0.4/README.md` & `dataretrieval-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/code.json` & `dataretrieval-1.0.5/code.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/dataretrieval/codes/states.py` & `dataretrieval-1.0.5/dataretrieval/codes/states.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/dataretrieval/codes/timezones.py` & `dataretrieval-1.0.5/dataretrieval/codes/timezones.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/dataretrieval/nadp.py` & `dataretrieval-1.0.5/dataretrieval/nadp.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,76 +29,28 @@
 """
 
 import requests
 import zipfile
 import io
 import os
 import re
-import warnings
-
-try:
-    import gdal
-except:
-    try:
-        from osgeo import gdal
-    except:
-        warnings.warn('GDAL not installed. Some functions will not work.')
-        import unittest.mock as mock
-        gdal = mock.MagicMock()
-
 from os.path import basename
-from uuid import uuid4
+
 
 NADP_URL = 'https://nadp.slh.wisc.edu'
 NADP_MAP_EXT = 'filelib/maps'
 
 NTN_CONC_PARAMS = ['pH', 'So4', 'NO3', 'NH4', 'Ca',
                    'Mg', 'K', 'Na', 'Cl', 'Br']
 NTN_DEP_PARAMS  = ['H', 'So4', 'NO3', 'NH4', 'Ca', 'Mg',
                    'K', 'Na', 'Cl', 'Br', 'N', 'SPlusN']
 
 NTN_MEAS_TYPE = ['conc', 'dep', 'precip']  # concentration or deposition
 
 
-class GDALMemFile():
-    """Creates a GDAL memory-mapped file
-
-    Modeled after ``rasterio`` function of same name
-
-    .. code::
-
-        with GDALMemFile(buf).open() as dataset:
-            # do something
-
-    .. todo::
-
-        could this work on url, file, or buf?
-
-    """
-    def __init__(self, buf):
-        """
-        Parameters
-        ----------
-        buf : buffer
-            Buffer containing gdal formatted data.
-
-        """
-        self.buf = buf
-
-    def open(self):
-        """
-        see https://gist.github.com/jleinonen/5781308
-
-        """
-        mmap_name = '/vsimem/' + uuid4().hex  # vsimem is special GDAL string
-        gdal.FileFromMemBuffer(mmap_name, self.buf)
-
-        return gdal.Open(mmap_name)
-
-
 class NADP_ZipFile(zipfile.ZipFile):
     """Extend zipfile.ZipFile for working on data from NADP
     """
     def tif_name(self):
         """Get the name of the tif file in the zip file."""
         filenames = self.namelist()
         r = re.compile(".*tif$")
@@ -106,78 +58,68 @@
         return tif_list[0]
 
     def tif(self):
         """Read the tif file in the zip file."""
         return self.read(self.tif_name())
 
 
-def get_annual_MDN_map(measurement_type, year, path=None):
+def get_annual_MDN_map(measurement_type, year, path):
     """Download a MDN map from NDAP.
 
     This function looks for a zip file containing gridded information at:
     https://nadp.slh.wisc.edu/maps-data/mdn-gradient-maps/.
     The function will download the zip file and extract it, exposing the tif
-    file if a path is provided. If not, then a
-    :obj:`dataretrieval.nadp.GDALMemFile` object is returned.
+    file if a path is provided.
 
     Parameters
     ----------
     measurement_type: string
         The type of measurement (concentration or deposition) as a string,
         either 'conc' or 'dep' respectively.
 
     year: string
         Year as a string 'YYYY'
 
     path: string
-        Download directory
+        Download directory.
 
     Returns
     -------
     path: string
         Path that zip file was extracted into if path was specified.
 
-    GDALMemFile: :obj:`dataretrieval.nadp.GDALMemFile`
-        GDALMemFile containing in-memory GDAL object.
-
     Examples
     --------
     .. code::
 
         >>> # get map of mercury concentration in 2010 and extract it to a path
         >>> data_path = dataretrieval.nadp.get_annual_MDN_map(
         ...     measurement_type='conc', year='2010', path='somepath')
 
-        >>> # get map of mercury deposition in 2008 as a GDALMemFile object
-        >>> gmem = dataretrieval.nadp.get_annual_MDN_map(
-        ...     measurement_type='dep', year='2008')
-
     """
     url = '{}/{}/MDN/grids/'.format(NADP_URL, NADP_MAP_EXT)
 
     filename = 'Hg_{}_{}.zip'.format(measurement_type, year)
 
     z = get_zip(url, filename)
 
     if path:
         z.extractall(path)
-        return '{}{}{}'.format(path, os.sep, basename(filename))
 
-    # else if no path return a buffer
-    return GDALMemFile(z.tif())
+    return '{}{}{}'.format(path, os.sep, basename(filename))
 
 
-def get_annual_NTN_map(measurement_type, measurement=None, year=None, path=None):
+def get_annual_NTN_map(measurement_type, measurement=None, year=None,
+                       path="."):
     """Download a NTN map from NDAP.
 
     This function looks for a zip file containing gridded information at:
     https://nadp.slh.wisc.edu/maps-data/ntn-gradient-maps/.
     The function will download the zip file and extract it, exposing the tif
-    file if a path is provided. If not, then a
-    :obj:`dataretrieval.nadp.GDALMemFile` object is returned.
+    file at the provided path.
 
     .. note::
 
         Measurement type abbreviations for concentration and deposition are
         all lower-case, but for precipitation data, the first letter must be
         capitalized!
 
@@ -187,32 +129,25 @@
         The measured constituent to return.
     measurement_type : string
         The type of measurement, 'conc', 'dep', or 'Precip', which represent
         concentration, deposition, or precipitation respectively.
     year : string
         Year as a string 'YYYY'
     path : string
-        Download directory
+        Download directory, defaults to current directory if not specified.
 
     Returns
     -------
     path: string
         Path that zip file was extracted into if path was specified.
 
-    GDALMemFile: :obj:`dataretrieval.nadp.GDALMemFile`
-        GDALMemFile containing in-memory GDAL object.
-
     Examples
     --------
     .. code::
 
-        >>> # get a map of nitrate concentration in 1996
-        >>> gmem = dataretrieval.nadp.get_annual_NTN_map(
-        ...     measurement='NO3', measurement_type='conc', year='1996')
-
         >>> # get a map of precipitation in 2015 and extract it to a path
         >>> data_path = dataretrieval.nadp.get_annual_NTN_map(
         ...     measurement_type='Precip', year='2015', path='somepath')
 
     """
     url = '{}/{}/NTN/grids/{}/'.format(NADP_URL, NADP_MAP_EXT, year)
 
@@ -221,18 +156,16 @@
     if measurement:
         filename = '{}_{}'.format(measurement, filename)
 
     z = get_zip(url, filename)
 
     if path:
         z.extractall(path)
-        return '{}{}{}'.format(path, os.sep, basename(filename))
 
-    # else if no path return a buffer
-    return GDALMemFile(z.tif())
+    return '{}{}{}'.format(path, os.sep, basename(filename))
 
 
 def get_zip(url, filename):
     """Gets a ZipFile at url and returns it
 
     Parameters
     ----------
```

### Comparing `dataretrieval-1.0.4/dataretrieval/nwis.py` & `dataretrieval-1.0.5/dataretrieval/nwis.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 PARAMCODES_URL = 'https://help.waterdata.usgs.gov/code/parameter_cd_nm_query?'
 ALLPARAMCODES_URL = 'https://help.waterdata.usgs.gov/code/parameter_cd_query?'
 
 WATERSERVICES_SERVICES = ['dv', 'iv', 'site', 'stat', 'gwlevels']
 WATERDATA_SERVICES = ['qwdata', 'measurements', 'peaks', 'pmcodes', 'water_use', 'ratings']
 
 
-def format_response(df, service=None, **kwargs):
+def format_response(df: pd.DataFrame, service=None, **kwargs) -> pd.DataFrame:
     """Setup index for response from query.
 
     This function formats the response from the NWIS web services, in
     particular it sets the index of the data frame. This function tries to
     convert the NWIS response into pandas datetime values localized to UTC,
     and if possible, uses these timestamps to define the data frame index.
 
@@ -75,15 +75,15 @@
         df.set_index(['datetime'], inplace=True)
         if hasattr(df.index, 'tzinfo') and df.index.tzinfo is None:
             df = df.tz_localize('UTC')
 
     return df.sort_index()
 
 
-def preformat_peaks_response(df):
+def preformat_peaks_response(df: pd.DataFrame):
     """Datetime formatting for the 'peaks' service response.
 
     Function to format the datetime column of the 'peaks' service response.
 
     Parameters
     ----------
     df: ``pandas.DataFrame``
@@ -98,15 +98,15 @@
     df['datetime'] = pd.to_datetime(df.pop('peak_dt'), errors='coerce')
     df.dropna(subset=['datetime'], inplace=True)
     return df
 
 
 def get_qwdata(sites=None, start=None, end=None,
                multi_index=True, wide_format=True, datetime_index=True,
-               **kwargs):
+               ssl_check=True, **kwargs):
     """
     Get water sample data from qwdata service.
 
     .. warning::
 
         The NWIS qw data service is being deprecated. See this note from the
         R package for more information:
@@ -128,14 +128,17 @@
     multi_index: boolean
         If False, a dataframe with a single-level index (datetime) is returned
     wide_format : boolean
         If True, return data in wide format with multiple samples per row and
         one row per time
     datetime_index : boolean
         If True, create a datetime index
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
@@ -154,18 +157,18 @@
     if wide_format:
         kwargs['qw_sample_wide'] = 'qw_sample_wide'
     start = kwargs.pop('begin_date', start)
     end = kwargs.pop('end_date', end)
     sites = kwargs.pop('site_no', sites)
     return _qwdata(site_no=sites, begin_date=start, end_date=end,
                    datetime_index=datetime_index,
-                   multi_index=multi_index, **kwargs)
+                   multi_index=multi_index, ssl_check=ssl_check, **kwargs)
 
 
-def _qwdata(datetime_index=True, **kwargs):
+def _qwdata(datetime_index=True, ssl_check=True, **kwargs):
     # check number of sites, may need to create multiindex
 
     payload = {'agency_cd': 'USGS',
                'format': 'rdb',
                'pm_cd_compare': 'Greater than',
                'inventory_output': '0',
                'rdb_inventory_output': 'file',
@@ -196,40 +199,44 @@
     kwargs.update(payload)
 
     warnings.warn(
         "NWIS qw web services are being retired. " +
         "See this note from the R package for more: " +
         "https://doi-usgs.github.io/dataRetrieval/articles/qwdata_changes.html",
         category=DeprecationWarning)
-    response = query_waterdata('qwdata', **kwargs)
+    response = query_waterdata('qwdata', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
     if datetime_index == True:
         df = format_datetime(df, 'sample_dt', 'sample_tm',
                              'sample_start_time_datum_cd')
 
     return format_response(df, **kwargs), _set_metadata(response, **kwargs)
 
 
-def get_discharge_measurements(sites=None, start=None, end=None, **kwargs):
+def get_discharge_measurements(sites=None, start=None, end=None,
+                               ssl_check=True, **kwargs):
     """
     Get discharge measurements from the waterdata service.
 
     Parameters
     ----------
     sites: array of strings
         If the qwdata parameter site_no is supplied, it will overwrite the
         sites parameter
     start: string
         If the qwdata parameter begin_date is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
     end: string
         If the qwdata parameter end_date is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
@@ -249,24 +256,26 @@
         ...     start='2012-01-09', end='2012-01-10', stateCd='AK')
 
     """
     start = kwargs.pop('begin_date', start)
     end = kwargs.pop('end_date', end)
     sites = kwargs.pop('site_no', sites)
     return _discharge_measurements(
-        site_no=sites, begin_date=start, end_date=end, **kwargs)
+        site_no=sites, begin_date=start, end_date=end,
+        ssl_check=ssl_check, **kwargs)
 
 
-def _discharge_measurements(**kwargs):
-    response = query_waterdata('measurements', format='rdb', **kwargs)
+def _discharge_measurements(ssl_check=True, **kwargs):
+    response = query_waterdata('measurements', format='rdb',
+                               ssl_check=ssl_check, **kwargs)
     return _read_rdb(response.text), _set_metadata(response, **kwargs)
 
 
 def get_discharge_peaks(sites=None, start=None, end=None,
-                        multi_index=True, **kwargs):
+                        multi_index=True, ssl_check=True, **kwargs):
     """
     Get discharge peaks from the waterdata service.
 
     Parameters
     ----------
     sites: array of strings
         If the waterdata parameter site_no is supplied, it will overwrite the
@@ -275,14 +284,17 @@
         If the waterdata parameter begin_date is supplied, it will overwrite
         the start parameter (YYYY-MM-DD)
     end: string
         If the waterdata parameter end_date is supplied, it will overwrite
         the end parameter (YYYY-MM-DD)
     multi_index: boolean
         If False, a dataframe with a single-level index (datetime) is returned
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
@@ -302,28 +314,31 @@
         ...     start='1980-01-01', end='1980-01-02', stateCd='HI')
 
     """
     start = kwargs.pop('begin_date', start)
     end = kwargs.pop('end_date', end)
     sites = kwargs.pop('site_no', sites)
     return _discharge_peaks(site_no=sites, begin_date=start, end_date=end,
-                            multi_index=multi_index, **kwargs)
+                            multi_index=multi_index, ssl_check=ssl_check,
+                            **kwargs)
 
 
-def _discharge_peaks(**kwargs):
-    response = query_waterdata('peaks', format='rdb', **kwargs)
+def _discharge_peaks(ssl_check=True, **kwargs):
+    response = query_waterdata('peaks', format='rdb',
+                               ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
     return format_response(df, service='peaks', **kwargs), _set_metadata(
         response, **kwargs)
 
 
 def get_gwlevels(sites=None, start='1851-01-01', end=None,
-                 multi_index=True, datetime_index=True, **kwargs):
+                 multi_index=True, datetime_index=True,
+                 ssl_check=True, **kwargs):
     """
     Queries the groundwater level service from waterservices
 
     Parameters
     ----------
     start: string
         If the waterdata parameter begin_date is supplied, it will overwrite
@@ -331,14 +346,17 @@
     end: string
         If the waterdata parameter end_date is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
     multi_index: boolean
         If False, a dataframe with a single-level index (datetime) is returned
     datetime_index : boolean
         If True, create a datetime index
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
@@ -354,40 +372,43 @@
 
     """
     start = kwargs.pop('startDT', start)
     end = kwargs.pop('endDT', end)
     sites = kwargs.pop('sites', sites)
     return _gwlevels(startDT=start, endDT=end,
                      datetime_index=datetime_index, sites=sites,
-                     multi_index=multi_index, **kwargs)
+                     multi_index=multi_index, ssl_check=ssl_check, **kwargs)
 
 
-def _gwlevels(datetime_index=True, **kwargs):
+def _gwlevels(datetime_index=True, ssl_check=True, **kwargs):
 
-    response = query_waterservices('gwlevels', **kwargs)
+    response = query_waterservices('gwlevels', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
     if datetime_index == True:
         df = format_datetime(df, 'lev_dt', 'lev_tm', 'lev_tz_cd')
 
     return format_response(df, **kwargs), _set_metadata(response, **kwargs)
 
 
-def get_stats(sites, **kwargs):
+def get_stats(sites, ssl_check=True, **kwargs):
     """
     Queries water services statistics information.
 
     For more information about the water services statistics service, visit
     https://waterservices.usgs.gov/rest/Statistics-Service.html
 
     Parameters
     ----------
     sites: string or list
         USGS site number (or list of site numbers)
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
 
     Additional Parameters
     ---------------------
     statReportType: string
         daily (default), monthly, or annual
     statTypeCd: string
         all, mean, max, min, median
@@ -415,20 +436,21 @@
         ...     sites='01646500', statReportType='annual', statYearType='water')
 
         >>> # Get monthly statistics for a site
         >>> df, md = dataretrieval.nwis.get_stats(
         ...     sites='01646500', statReportType='monthly')
 
     """
-    response = query_waterservices('stat', sites=sites, **kwargs)
+    response = query_waterservices('stat', sites=sites,
+                                   ssl_check=ssl_check, **kwargs)
 
     return _read_rdb(response.text), _set_metadata(response, **kwargs)
 
 
-def query_waterdata(service, **kwargs):
+def query_waterdata(service, ssl_check=True, **kwargs):
     """
     Queries waterdata.
     """
     major_params = ['site_no', 'state_cd']
     bbox_params = ['nw_longitude_va', 'nw_latitude_va',
                    'se_longitude_va', 'se_latitude_va']
 
@@ -440,42 +462,48 @@
         raise TypeError('One or more lat/long coordinates missing or invalid.')
 
     if service not in WATERDATA_SERVICES:
         raise TypeError('Service not recognized')
 
     url = WATERDATA_URL + service
 
-    return query(url, payload=kwargs)
+    return query(url, payload=kwargs, ssl_check=ssl_check)
 
 
-def query_waterservices(service, **kwargs):
+def query_waterservices(service, ssl_check=True, **kwargs):
     """
     Queries waterservices.usgs.gov
 
     For more documentation see https://waterservices.usgs.gov/rest/
 
     .. note::
 
         User must specify one major filter: sites, stateCd, or bBox
 
     Parameters
     ----------
     service: string
         String specifying the service to query: 'site', 'stats', etc.
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     bBox: string
         7-digit Hydrologic Unit Code (HUC)
     startDT: string
         Start date (e.g., '2017-12-31')
     endDT: string
         End date (e.g., '2018-01-01')
     modifiedSince: string
         Used to return only sites where attributes or period of record data
         have changed during the request period. String expected to be formatted
         in ISO-8601 duration format (e.g., 'P1D' for one day,
         'P1Y' for one year)
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
 
     Other Parameters
     ----------------
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
@@ -491,18 +519,19 @@
         raise TypeError('Service not recognized')
 
     if 'format' not in kwargs:
         kwargs['format'] = 'rdb'
 
     url = WATERSERVICE_URL + service
 
-    return query(url, payload=kwargs)
+    return query(url, payload=kwargs, ssl_check=ssl_check)
 
 
-def get_dv(sites=None, start=None, end=None, multi_index=True, **kwargs):
+def get_dv(sites=None, start=None, end=None, multi_index=True,
+           ssl_check=True, **kwargs):
     """
     Get daily values data from NWIS and return it as a ``pandas.DataFrame``.
 
     .. note:
 
         If no start or end date are provided, only the most recent record
         is returned.
@@ -511,14 +540,20 @@
     ----------
     start: string
         If the waterdata parameter startDT is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
     end: string
         If the waterdata parameter endDT is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
+    multi_index: bool
+        If True, return a multi-index dataframe, if False, return a
+        single-index dataframe, default is True
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
@@ -538,25 +573,26 @@
         >>> df, md = dataretrieval.nwis.get_dv(sites='01646500')
 
     """
     start = kwargs.pop('startDT', start)
     end = kwargs.pop('endDT', end)
     sites = kwargs.pop('sites', sites)
     return _dv(startDT=start, endDT=end, sites=sites,
-               multi_index=multi_index, **kwargs)
+               multi_index=multi_index, ssl_check=ssl_check, **kwargs)
 
 
-def _dv(**kwargs):
-    response = query_waterservices('dv', format='json', **kwargs)
+def _dv(ssl_check=True, **kwargs):
+    response = query_waterservices('dv', format='json',
+                                   ssl_check=ssl_check, **kwargs)
     df = _read_json(response.json())
 
     return format_response(df, **kwargs), _set_metadata(response, **kwargs)
 
 
-def get_info(**kwargs):
+def get_info(ssl_check=True, **kwargs):
     """
     Get site description information from NWIS.
 
     **Note:** *Must specify one major parameter.*
 
     For additional parameter options see
     https://waterservices.usgs.gov/rest/Site-Service.html#stateCd
@@ -580,14 +616,17 @@
         product of the range of latitude range and longitude cannot exceed 25
         degrees. Whole or decimal degrees must be specified, up to six digits
         of precision. Minutes and seconds are not allowed.
     countyCd: string or list
         A list of county numbers, in a 5 digit numeric format. The first two
         digits of a county's code are the FIPS State Code.
         (url: https://help.waterdata.usgs.gov/code/county_query?fmt=html)
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Other Parameters
     ----------------
     startDt: string
         Selects sites based on whether data was collected at a point in time
@@ -646,20 +685,21 @@
     if seriesCatalogOutput in ['True', 'TRUE', 'true', True]:
         # convert bool to string if necessary
         kwargs['seriesCatalogOutput'] = 'True'
     else:
         # cannot have both seriesCatalogOutput and the expanded format
         kwargs['siteOutput'] = 'Expanded'
 
-    response = query_waterservices('site', **kwargs)
+    response = query_waterservices('site', ssl_check=ssl_check, **kwargs)
 
     return _read_rdb(response.text), _set_metadata(response, **kwargs)
 
 
-def get_iv(sites=None, start=None, end=None, multi_index=True, **kwargs):
+def get_iv(sites=None, start=None, end=None, multi_index=True,
+           ssl_check=True, **kwargs):
     """Get instantaneous values data from NWIS and return it as a DataFrame.
 
     .. note::
 
         If no start or end date are provided, only the most recent record
         is returned.
 
@@ -667,14 +707,17 @@
     ----------
     start: string
         If the waterdata parameter startDT is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
     end: string
         If the waterdata parameter endDT is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
@@ -689,34 +732,38 @@
         ...     parameterCd='00060')
 
     """
     start = kwargs.pop('startDT', start)
     end = kwargs.pop('endDT', end)
     sites = kwargs.pop('sites', sites)
     return _iv(startDT=start, endDT=end, sites=sites,
-               multi_index=multi_index, **kwargs)
+               multi_index=multi_index, ssl_check=ssl_check, **kwargs)
 
 
-def _iv(**kwargs):
-    response = query_waterservices('iv', format='json', **kwargs)
+def _iv(ssl_check=True, **kwargs):
+    response = query_waterservices('iv', format='json',
+                                   ssl_check=ssl_check, **kwargs)
     df = _read_json(response.json())
     return format_response(df, **kwargs), _set_metadata(response, **kwargs)
 
 
-def get_pmcodes(parameterCd='All', partial=True):
+def get_pmcodes(parameterCd='All', partial=True, ssl_check=True):
     """
     Return a ``pandas.DataFrame`` containing all NWIS parameter codes.
 
     Parameters
     ----------
     parameterCd: string or list
         Accepts parameter codes or names
     partial: boolean
         Default is True (partial querying). If False, the function will query
         only exact matches
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Data retrieved from the NWIS web service.
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
@@ -740,15 +787,15 @@
     payload = {'fmt': 'rdb'}
     url = PARAMCODES_URL
 
     if isinstance(parameterCd, str):  # when a single code or name is given
         if parameterCd.lower() == "all":
             payload.update({'group_cd': '%'})
             url = ALLPARAMCODES_URL
-            response = query(url, payload)
+            response = query(url, payload, ssl_check=ssl_check)
             return _read_rdb(response.text), _set_metadata(response)
 
         else:
             parameterCd = [parameterCd]
 
     if not isinstance(parameterCd, list):
         raise TypeError('Parameter information (code or name) must be type string or list')
@@ -756,39 +803,43 @@
     # Querying with a list of parameters names, codes, or mixed
     l = []
     for param in parameterCd:
         if isinstance(param, str):
             if partial:
                 param ='%{0}%'.format(param)
             payload.update({'parm_nm_cd': param})
-            response = query(url, payload)
+            response = query(url, payload, ssl_check=ssl_check)
             if len(response.text.splitlines()) < 10:  # empty query
                 raise TypeError('One of the parameter codes or names entered does not return any information,'\
                                 ' please try a different value')
             l.append(_read_rdb(response.text))
         else:
             raise TypeError('Parameter information (code or name) must be type string')
     return pd.concat(l), _set_metadata(response)
 
 
-def get_water_use(years="ALL", state=None, counties="ALL", categories="ALL"):
+def get_water_use(years="ALL", state=None, counties="ALL", categories="ALL",
+                  ssl_check=True):
     """
     Water use data retrieval from USGS (NWIS).
 
     Parameters
     ----------
     years: list-like
         List or comma delimited string of years.  Must be years ending in 0 or
         5, or "ALL", which retrieves all available years
     state: string
         full name, abbreviation or id
     county: string
         County IDs from county lookup or "ALL"
     categories: list-like
         List or comma delimited string of Two-letter category abbreviations
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Data from NWIS
@@ -818,19 +869,19 @@
                'wu_year': years,
                'wu_category': categories,
                'wu_county': counties}
     url = WATERDATA_URL + 'water_use'
     if state is not None:
         url = WATERDATA_BASE_URL + state + "/nwis/water_use"
         payload.update({"wu_area": "county"})
-    response = query(url, payload)
+    response = query(url, payload, ssl_check=ssl_check)
     return _read_rdb(response.text), _set_metadata(response)
 
 
-def get_ratings(site=None, file_type="base", **kwargs):
+def get_ratings(site=None, file_type="base", ssl_check=True, **kwargs):
     """
     Rating table for an active USGS streamgage retrieval.
 
     Reads current rating table for an active USGS streamgage from NWISweb.
     Data is retrieved from https://waterdata.usgs.gov/nwis.
 
     Parameters
@@ -841,14 +892,17 @@
         parameter
     base: string
         can be "base", "corr", or "exsa"
     county: string
         County IDs from county lookup or "ALL"
     categories: list-like
         List or comma delimited string of Two-letter category abbreviations
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Return
     ------
     df: ``pandas.DataFrame``
         Formatted requested data
@@ -860,36 +914,40 @@
     .. doctest::
 
         >>> # Get the rating table for USGS streamgage 01594440
         >>> df, md = dataretrieval.nwis.get_ratings(site='01594440')
 
     """
     site = kwargs.pop('site_no', site)
-    return _ratings(site=site, file_type=file_type, **kwargs)
+    return _ratings(site=site, file_type=file_type, ssl_check=ssl_check,
+                    **kwargs)
 
 
-def _ratings(site, file_type):
+def _ratings(site, file_type, ssl_check=True):
     payload = {}
     url = WATERDATA_BASE_URL + 'nwisweb/get_ratings/'
     if site is not None:
         payload.update({"site_no": site})
     if file_type is not None:
         if file_type not in ["base", "corr", "exsa"]:
             raise ValueError('Unrecognized file_type: {}, must be "base", "corr" or "exsa"'.format(file_type))
         payload.update({"file_type" : file_type})
-    response = query(url, payload)
+    response = query(url, payload, ssl_check=ssl_check)
     return _read_rdb(response.text), _set_metadata(response, site_no=site)
 
 
-def what_sites(**kwargs):
+def what_sites(ssl_check=True, **kwargs):
     """
     Search NWIS for sites within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.nwis.get_info`
 
     Examples
     --------
     .. doctest::
 
@@ -898,24 +956,25 @@
 
         >>> # get information about sites with phosphorus in Ohio
         >>> df, md = dataretrieval.nwis.what_sites(
         ...     stateCd='OH', parameterCd='00665')
 
     """
 
-    response = query_waterservices(service='site', **kwargs)
+    response = query_waterservices(service='site', ssl_check=ssl_check,
+                                   **kwargs)
 
     df = _read_rdb(response.text)
 
     return df, _set_metadata(response, **kwargs)
 
 
 def get_record(sites=None, start=None, end=None,
                multi_index=True, wide_format=True, datetime_index=True,
-               state=None, service='iv', **kwargs):
+               state=None, service='iv', ssl_check=True, **kwargs):
     """
     Get data from NWIS and return it as a ``pandas.DataFrame``.
 
     .. note::
 
         If no start or end date are provided, only the most recent record is
         returned.
@@ -936,14 +995,17 @@
         - 'measurements' : discharge measurements
         - 'peaks': discharge peaks
         - 'gwlevels': groundwater levels
         - 'pmcodes': get parameter codes
         - 'water_use': get water use data
         - 'ratings': get rating table
         - 'stat': get statistics
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
         ``pandas.DataFrame`` containing requested data
 
@@ -996,63 +1058,67 @@
 
     """
     if service not in WATERSERVICES_SERVICES + WATERDATA_SERVICES:
         raise TypeError('Unrecognized service: {}'.format(service))
 
     if service == 'iv':
         df, _ = get_iv(sites=sites, startDT=start, endDT=end,
-                       multi_index=multi_index, **kwargs)
+                       multi_index=multi_index, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'dv':
         df, _ = get_dv(sites=sites, startDT=start, endDT=end,
-                       multi_index=multi_index, **kwargs)
+                       multi_index=multi_index, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'qwdata':
         df, _ = get_qwdata(site_no=sites, begin_date=start, end_date=end,
                            multi_index=multi_index,
-                           wide_format=wide_format, **kwargs)
+                           wide_format=wide_format, ssl_check=ssl_check,
+                           **kwargs)
         return df
 
     elif service == 'site':
-        df, _ = get_info(sites=sites, **kwargs)
+        df, _ = get_info(sites=sites, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'measurements':
         df, _ = get_discharge_measurements(site_no=sites, begin_date=start,
-                                           end_date=end, **kwargs)
+                                           end_date=end, ssl_check=ssl_check,
+                                           **kwargs)
         return df
 
     elif service == 'peaks':
         df, _ = get_discharge_peaks(site_no=sites, begin_date=start,
                                     end_date=end,
-                                    multi_index=multi_index, **kwargs)
+                                    multi_index=multi_index,
+                                    ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'gwlevels':
         df, _ = get_gwlevels(sites=sites, startDT=start, endDT=end,
                              multi_index=multi_index,
-                             datetime_index=datetime_index, **kwargs)
+                             datetime_index=datetime_index,
+                             ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'pmcodes':
-        df, _ = get_pmcodes(**kwargs)
+        df, _ = get_pmcodes(ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'water_use':
-        df, _ = get_water_use(state=state, **kwargs)
+        df, _ = get_water_use(state=state, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'ratings':
-        df, _ = get_ratings(site=sites, **kwargs)
+        df, _ = get_ratings(site=sites, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'stat':
-        df, _ = get_stats(sites=sites, **kwargs)
+        df, _ = get_stats(sites=sites, ssl_check=ssl_check, **kwargs)
         return df
 
     else:
         raise TypeError('{} service not yet implemented'.format(service))
 
 
 def _read_json(json):
@@ -1203,15 +1269,16 @@
     elif 'bBox' in parameters:
         md.site_info = lambda: what_sites(bBox=parameters['bBox'])
     else:
         pass  # don't set metadata site_info attribute
 
     # define variable_info metadata based on parameterCd if available
     if 'parameterCd' in parameters:
-        md.variable_info = lambda: get_pmcodes(parameterCd=parameters['parameterCd'])
+        md.variable_info = lambda: get_pmcodes(
+            parameterCd=parameters['parameterCd'])
 
     comments = ""
     for line in response.text.splitlines():
         if line.startswith("#"):
             comments += line.lstrip("#") + "\n"
     if comments != "":
         md.comment = comments
```

### Comparing `dataretrieval-1.0.4/dataretrieval/streamstats.py` & `dataretrieval-1.0.5/dataretrieval/streamstats.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/dataretrieval/utils.py` & `dataretrieval-1.0.5/dataretrieval/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """
     # create a datetime index from the columns in qwdata response
     df[tz_field] = df[tz_field].map(tz)
 
     df['datetime'] = pd.to_datetime(df[date_field] + ' ' +
                                     df[time_field] + ' ' +
                                     df[tz_field],
-                                    format='%Y-%m-%d %H:%M',
+                                    format='ISO8601',
                                     utc=True)
 
     # if there are any incomplete dates, warn the user
     if any(pd.isna(df['datetime'])):
         count = sum(pd.isna(df['datetime']) == True)
         warnings.warn(
             f'Warning: {count} incomplete dates found, ' +
@@ -158,28 +158,31 @@
     md = Metadata()
     md.url = response.url
     md.query_time = response.elapsed
     md.header = response.headers
     return md
 
 
-def query(url, payload, delimiter=','):
+def query(url, payload, delimiter=',', ssl_check=True):
     """Send a query.
 
     Wrapper for requests.get that handles errors, converts listed
     query parameters to comma separated strings, and returns response.
 
     Parameters
     ----------
     url: string
         URL to query
     payload: dict
         query parameters passed to ``requests.get``
     delimiter: string
         delimiter to use with lists
+    ssl_check: bool
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
 
     Returns
     -------
     string: query response
         The response from the API query ``requests.get`` function call.
     """
 
@@ -189,15 +192,16 @@
     #    key, value = payload[index]
     #    payload[index] = (key, to_str(value))
 
     # define the user agent for the query
     user_agent = {
         'user-agent': f"python-dataretrieval/{dataretrieval.__version__}"}
 
-    response = requests.get(url, params=payload, headers=user_agent)
+    response = requests.get(url, params=payload,
+                            headers=user_agent, verify=ssl_check)
 
     if response.status_code == 400:
         raise ValueError("Bad Request, check that your parameters are correct. URL: {}".format(response.url))
     elif response.status_code == 404:
         raise ValueError(
             "Page Not Found Error. May be the result of an empty query. " +
             f"URL: {response.url}")
```

### Comparing `dataretrieval-1.0.4/dataretrieval/waterwatch.py` & `dataretrieval-1.0.5/dataretrieval/waterwatch.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/dataretrieval/wqp.py` & `dataretrieval-1.0.5/dataretrieval/wqp.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 """
 import pandas as pd
 from io import StringIO
 from .utils import query, set_metadata as set_md
 import warnings
 
 
-def get_results(**kwargs):
+def get_results(ssl_check=True, **kwargs):
     """Query the WQP for results.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     siteid: string
         Concatenate an agency code, a hyphen ("-"), and a site-identification
         number.
     statecode: string
         Concatenate 'US', a colon (":"), and a FIPS numeric code
         (Example: Illinois is US:17)
     countycode: string
@@ -74,25 +77,29 @@
 
         >>> # Get results within a bounding box
         >>> df, md = dataretrieval.wqp.get_results(
         ...     bBox='-92.8,44.2,-88.9,46.0')
 
     """
     kwargs = _alter_kwargs(kwargs)
-    response = query(wqp_url('Result'), kwargs, delimiter=';')
+    response = query(wqp_url('Result'), kwargs, delimiter=';',
+                     ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
     return df, set_metadata(response)
 
 
-def what_sites(**kwargs):
+def what_sites(ssl_check=True, **kwargs):
     """Search WQP for sites within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -107,26 +114,29 @@
         >>> df, md = dataretrieval.wqp.what_sites(
         ...     lat='44.2', long='-88.9', within='2.5')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Station')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_organizations(**kwargs):
+def what_organizations(ssl_check=True, **kwargs):
     """Search WQP for organizations within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -140,26 +150,29 @@
         >>> # Get all organizations in the WQP
         >>> df, md = dataretrieval.wqp.what_organizations()
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Organization')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_projects(**kwargs):
+def what_projects(ssl_check=True, **kwargs):
     """Search WQP for projects within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -173,26 +186,29 @@
         >>> # Get projects within a HUC region
         >>> df, md = dataretrieval.wqp.what_projects(huc='19')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Project')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_activities(**kwargs):
+def what_activities(ssl_check=True, **kwargs):
     """Search WQP for activities within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -209,27 +225,30 @@
         ...     statecode='US:11', startDateLo='12-30-2019',
         ...     startDateHi='01-01-2020')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Activity')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_detection_limits(**kwargs):
+def what_detection_limits(ssl_check=True, **kwargs):
     """Search WQP for result detection limits within a region with specific
     data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -246,26 +265,29 @@
         ...     statecode='US:44', characteristicName='Nitrite',
         ...     startDateLo='01-01-2021', startDateHi='02-20-2021')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ResultDetectionQuantitationLimit')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_habitat_metrics(**kwargs):
+def what_habitat_metrics(ssl_check=True, **kwargs):
     """Search WQP for habitat metrics within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -280,26 +302,29 @@
         >>> df, md = dataretrieval.wqp.what_habitat_metrics(
         ...     statecode='US:44')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('BiologicalMetric')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_project_weights(**kwargs):
+def what_project_weights(ssl_check=True, **kwargs):
     """Search WQP for project weights within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -316,26 +341,29 @@
         ...     statecode='US:38', startDateLo='01-01-2006',
         ...     startDateHi='01-01-2009')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ProjectMonitoringLocationWeighting')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
-def what_activity_metrics(**kwargs):
+def what_activity_metrics(ssl_check=True, **kwargs):
     """Search WQP for activity metrics within a region with specific data.
 
     Parameters
     ----------
+    ssl_check: bool
+        If True, check the SSL certificate. Default is True. If False, SSL
+        certificate is not checked.
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.wqp.get_results`
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Formatted data returned from the API query.
@@ -352,15 +380,15 @@
         ...     statecode='US:38', startDateLo='07-01-2006',
         ...     startDateHi='12-01-2006')
 
     """
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ActivityMetric')
-    response = query(url, payload=kwargs, delimiter=';')
+    response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, set_metadata(response)
 
 
 def wqp_url(service):
```

### Comparing `dataretrieval-1.0.4/dataretrieval.egg-info/PKG-INFO` & `dataretrieval-1.0.5/dataretrieval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `dataretrieval-1.0.4/dataretrieval.egg-info/SOURCES.txt` & `dataretrieval-1.0.5/dataretrieval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/NWIS_demo_1.ipynb` & `dataretrieval-1.0.5/demos/NWIS_demo_1.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/R Python Vignette equivalents.ipynb` & `dataretrieval-1.0.5/demos/R Python Vignette equivalents.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.5/demos/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb` & `dataretrieval-1.0.5/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/Makefile` & `dataretrieval-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/conf.py` & `dataretrieval-1.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/examples/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.5/docs/source/examples/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/examples/index.rst` & `dataretrieval-1.0.5/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/examples/readme_examples.rst` & `dataretrieval-1.0.5/docs/source/examples/readme_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/examples/siteinfo_examples.rst` & `dataretrieval-1.0.5/docs/source/examples/siteinfo_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/index.rst` & `dataretrieval-1.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/meta/contributing.rst` & `dataretrieval-1.0.5/docs/source/meta/contributing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/meta/installing.rst` & `dataretrieval-1.0.5/docs/source/meta/installing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/meta/license.rst` & `dataretrieval-1.0.5/docs/source/meta/license.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/userguide/dataportals.rst` & `dataretrieval-1.0.5/docs/source/userguide/dataportals.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/docs/source/userguide/timeconventions.rst` & `dataretrieval-1.0.5/docs/source/userguide/timeconventions.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/pyproject.toml` & `dataretrieval-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/nwis_sites.txt` & `dataretrieval-1.0.5/tests/data/nwis_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/water_use_allegheny.txt` & `dataretrieval-1.0.5/tests/data/water_use_allegheny.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/water_use_national.txt` & `dataretrieval-1.0.5/tests/data/water_use_national.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterdata_measurements.txt` & `dataretrieval-1.0.5/tests/data/waterdata_measurements.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterdata_qwdata.txt` & `dataretrieval-1.0.5/tests/data/waterdata_qwdata.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_dv.txt` & `dataretrieval-1.0.5/tests/data/waterservices_dv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_gwlevels.txt` & `dataretrieval-1.0.5/tests/data/waterservices_gwlevels.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_iv.txt` & `dataretrieval-1.0.5/tests/data/waterservices_iv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_peaks.txt` & `dataretrieval-1.0.5/tests/data/waterservices_peaks.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_ratings.txt` & `dataretrieval-1.0.5/tests/data/waterservices_ratings.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_site.txt` & `dataretrieval-1.0.5/tests/data/waterservices_site.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/waterservices_stats.txt` & `dataretrieval-1.0.5/tests/data/waterservices_stats.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_activities.txt` & `dataretrieval-1.0.5/tests/data/wqp_activities.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_activity_metrics.txt` & `dataretrieval-1.0.5/tests/data/wqp_activity_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_detection_limits.txt` & `dataretrieval-1.0.5/tests/data/wqp_detection_limits.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_habitat_metrics.txt` & `dataretrieval-1.0.5/tests/data/wqp_habitat_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_organizations.txt` & `dataretrieval-1.0.5/tests/data/wqp_organizations.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_project_weights.txt` & `dataretrieval-1.0.5/tests/data/wqp_project_weights.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_projects.txt` & `dataretrieval-1.0.5/tests/data/wqp_projects.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_results.txt` & `dataretrieval-1.0.5/tests/data/wqp_results.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/data/wqp_sites.txt` & `dataretrieval-1.0.5/tests/data/wqp_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/nwis_test.py` & `dataretrieval-1.0.5/tests/nwis_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/utils_test.py` & `dataretrieval-1.0.5/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/waterservices_test.py` & `dataretrieval-1.0.5/tests/waterservices_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.4/tests/wqp_test.py` & `dataretrieval-1.0.5/tests/wqp_test.py`

 * *Files identical despite different names*

