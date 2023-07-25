# Comparing `tmp/gempyp-1.0.70b4.tar.gz` & `tmp/gempyp-1.0.70b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.70b4.tar", max compression
+gzip compressed data, was "gempyp-1.0.70b6.tar", last modified: Tue Jul 25 11:57:41 2023, max compression
```

## Comparing `gempyp-1.0.70b4.tar` & `gempyp-1.0.70b6.tar`

### file list

```diff
@@ -1,95 +1,109 @@
--rw-r--r--   0        0        0       25 2023-07-25 10:58:40.592853 gempyp-1.0.70b4/gempyp/__init__.py
--rw-r--r--   0        0        0      108 2023-07-25 10:58:40.593918 gempyp-1.0.70b4/gempyp/cli.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.597746 gempyp-1.0.70b4/gempyp/config/__init__.py
--rw-r--r--   0        0        0     7468 2023-07-25 10:59:19.986416 gempyp-1.0.70b4/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0      198 2023-07-25 10:58:40.599911 gempyp-1.0.70b4/gempyp/config/customParser.py
--rw-r--r--   0        0        0     1812 2023-07-25 10:59:19.984833 gempyp-1.0.70b4/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2023-07-25 10:58:40.601333 gempyp-1.0.70b4/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2023-07-25 10:58:40.595914 gempyp-1.0.70b4/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2023-07-25 10:58:40.596983 gempyp-1.0.70b4/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2023-07-25 10:58:40.601333 gempyp-1.0.70b4/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2023-07-25 10:58:40.602332 gempyp-1.0.70b4/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     4003 2023-07-25 10:59:19.987417 gempyp-1.0.70b4/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.603482 gempyp-1.0.70b4/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.604484 gempyp-1.0.70b4/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2023-07-25 10:58:40.606478 gempyp-1.0.70b4/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2023-07-25 10:58:40.607474 gempyp-1.0.70b4/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2023-07-25 10:58:40.607474 gempyp-1.0.70b4/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.609574 gempyp-1.0.70b4/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2023-07-25 10:58:40.610573 gempyp-1.0.70b4/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2023-07-25 10:58:40.611569 gempyp-1.0.70b4/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.612401 gempyp-1.0.70b4/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2023-07-25 10:58:40.614232 gempyp-1.0.70b4/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.612401 gempyp-1.0.70b4/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2023-07-25 10:58:40.615238 gempyp-1.0.70b4/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.616237 gempyp-1.0.70b4/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2023-07-25 10:58:40.617234 gempyp-1.0.70b4/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2023-07-25 10:58:40.618231 gempyp-1.0.70b4/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2023-07-25 10:58:40.618731 gempyp-1.0.70b4/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2023-07-25 10:58:40.619818 gempyp-1.0.70b4/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2023-07-25 10:58:40.621257 gempyp-1.0.70b4/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2023-07-25 10:58:40.622203 gempyp-1.0.70b4/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.622203 gempyp-1.0.70b4/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2023-07-25 10:58:40.623202 gempyp-1.0.70b4/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.624916 gempyp-1.0.70b4/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.624916 gempyp-1.0.70b4/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0     6758 2023-07-25 10:58:40.626573 gempyp-1.0.70b4/gempyp/data_uploader.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.627572 gempyp-1.0.70b4/gempyp/dv/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-25 10:58:40.628569 gempyp-1.0.70b4/gempyp/dv/dfOperations.py
--rw-r--r--   0        0        0    10230 2023-07-25 10:58:40.629709 gempyp-1.0.70b4/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2023-07-25 10:58:40.630679 gempyp-1.0.70b4/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0    10762 2023-07-25 10:59:19.989413 gempyp-1.0.70b4/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2023-07-25 10:58:40.632675 gempyp-1.0.70b4/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2023-07-25 10:58:40.633672 gempyp-1.0.70b4/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    23252 2023-07-25 11:29:16.881871 gempyp-1.0.70b4/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.635861 gempyp-1.0.70b4/gempyp/engine/__init__.py
--rw-r--r--   0        0        0     5092 2023-07-25 10:58:40.636857 gempyp-1.0.70b4/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     8428 2023-07-25 10:59:19.991321 gempyp-1.0.70b4/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    41280 2023-07-25 10:59:19.992397 gempyp-1.0.70b4/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.640707 gempyp-1.0.70b4/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2023-07-25 10:58:40.641430 gempyp-1.0.70b4/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2023-07-25 10:58:40.642428 gempyp-1.0.70b4/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5483 2023-07-25 10:58:40.643425 gempyp-1.0.70b4/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5537 2023-07-25 10:58:40.643425 gempyp-1.0.70b4/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    12428 2023-07-25 10:58:40.645078 gempyp-1.0.70b4/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2023-07-25 10:58:40.646077 gempyp-1.0.70b4/gempyp/final_report.html
--rw-r--r--   0        0        0     4566 2023-07-25 10:58:40.648069 gempyp-1.0.70b4/gempyp/gemPyp.py
--rw-r--r--   0        0        0    14521 2023-07-25 11:29:16.883866 gempyp-1.0.70b4/gempyp/gempyp_plugin.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.650063 gempyp-1.0.70b4/gempyp/jira/__init__.py
--rw-r--r--   0        0        0     2312 2023-07-25 10:59:19.994388 gempyp-1.0.70b4/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2023-07-25 10:58:40.651253 gempyp-1.0.70b4/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.652250 gempyp-1.0.70b4/gempyp/libs/__init__.py
--rw-r--r--   0        0        0     9011 2023-07-25 10:59:19.995992 gempyp-1.0.70b4/gempyp/libs/common.py
--rw-r--r--   0        0        0      131 2023-07-25 10:58:40.655240 gempyp-1.0.70b4/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2023-07-25 10:58:40.656245 gempyp-1.0.70b4/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2023-07-25 10:58:40.657236 gempyp-1.0.70b4/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2023-07-25 10:58:40.659227 gempyp-1.0.70b4/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2023-07-25 10:58:40.661294 gempyp-1.0.70b4/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1465 2023-07-25 10:58:40.662289 gempyp-1.0.70b4/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.662289 gempyp-1.0.70b4/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0    11776 2023-07-25 11:29:16.884864 gempyp-1.0.70b4/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2023-07-25 10:58:40.664909 gempyp-1.0.70b4/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    13694 2023-07-25 10:58:40.666929 gempyp-1.0.70b4/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13567 2023-07-25 10:58:40.667925 gempyp-1.0.70b4/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2023-07-25 10:58:40.670162 gempyp-1.0.70b4/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2023-07-25 10:58:40.671163 gempyp-1.0.70b4/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10792 2023-07-25 10:58:40.672158 gempyp-1.0.70b4/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     4235 2023-07-25 10:59:19.999342 gempyp-1.0.70b4/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2023-07-25 10:58:40.676144 gempyp-1.0.70b4/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     3889 2023-07-25 10:59:20.001329 gempyp-1.0.70b4/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    36757 2023-07-25 10:59:20.002343 gempyp-1.0.70b4/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4333 2023-07-25 10:58:40.678140 gempyp-1.0.70b4/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2023-07-25 10:58:40.680131 gempyp-1.0.70b4/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2023-07-25 10:58:40.680333 gempyp-1.0.70b4/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2023-07-25 10:58:40.681806 gempyp-1.0.70b4/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     5463 2023-07-25 10:58:40.682815 gempyp-1.0.70b4/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2023-07-25 10:58:40.683892 gempyp-1.0.70b4/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0     8517 2023-07-25 10:59:20.004325 gempyp-1.0.70b4/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    13508 2023-07-25 11:29:16.887851 gempyp-1.0.70b4/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     1340 2023-07-25 11:29:16.886855 gempyp-1.0.70b4/gempyp/sdk/Gempytest.py
--rw-r--r--   0        0        0     3126 2023-07-25 11:29:16.888847 gempyp-1.0.70b4/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2023-07-25 10:58:40.688795 gempyp-1.0.70b4/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2023-07-25 10:58:40.583404 gempyp-1.0.70b4/LICENSE
--rw-r--r--   0        0        0     1431 2023-07-25 11:33:30.333678 gempyp-1.0.70b4/pyproject.toml
--rw-r--r--   0        0        0     3161 2023-07-25 10:58:40.583404 gempyp-1.0.70b4/README.md
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 gempyp-1.0.70b4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.279479 gempyp-1.0.70b6/
+-rw-rw-rw-   0        0        0        2 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/LICENSE
+-rw-rw-rw-   0        0        0       79 2023-07-25 11:57:41.277474 gempyp-1.0.70b6/PKG-INFO
+-rw-rw-rw-   0        0        0     3161 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.892225 gempyp-1.0.70b6/gempyp/
+-rw-rw-rw-   0        0        0       25 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.936119 gempyp-1.0.70b6/gempyp/config/
+-rw-rw-rw-   0        0        0     1812 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/config/DefaultSettings.py
+-rw-rw-rw-   0        0        0     2145 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/config/GitLinkXML.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/config/__init__.py
+-rw-rw-rw-   0        0        0     7468 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/config/baseConfig.py
+-rw-rw-rw-   0        0        0      198 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/config/customParser.py
+-rw-rw-rw-   0        0        0     4003 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/config/xmlConfig.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.948409 gempyp-1.0.70b6/gempyp/data_compare/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.955723 gempyp-1.0.70b6/gempyp/data_compare/common/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/common/__init__.py
+-rw-rw-rw-   0        0        0     3627 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/common/common_functions.py
+-rw-rw-rw-   0        0        0      956 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/compare.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.970001 gempyp-1.0.70b6/gempyp/data_compare/configurator/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/configurator/__init__.py
+-rw-rw-rw-   0        0        0     4635 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/configurator/configurator.py
+-rw-rw-rw-   0        0        0      320 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/configurator/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.985220 gempyp-1.0.70b6/gempyp/data_compare/core/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/core/Compare.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/core/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/core/comparator.py
+-rw-rw-rw-   0        0        0    10157 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/core/python_obj_comparator.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.035693 gempyp-1.0.70b6/gempyp/data_compare/data/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/__init__.py
+-rw-rw-rw-   0        0        0     5498 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/data.py
+-rw-rw-rw-   0        0        0      869 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/database.py
+-rw-rw-rw-   0        0        0     1903 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/db_mysql.py
+-rw-rw-rw-   0        0        0     2646 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/db_oracle.py
+-rw-rw-rw-   0        0        0     2436 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/db_postgre.py
+-rw-rw-rw-   0        0        0     1999 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/db_sqlite.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data/file_processor.py
+-rw-rw-rw-   0        0        0    11161 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/data_comp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.038619 gempyp-1.0.70b6/gempyp/data_compare/report/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/report/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.044564 gempyp-1.0.70b6/gempyp/data_compare/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_compare/tools/__init__.py
+-rw-rw-rw-   0        0        0     6758 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/data_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.094304 gempyp-1.0.70b6/gempyp/dv/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/__init__.py
+-rw-rw-rw-   0        0        0     2285 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/dfOperations.py
+-rw-rw-rw-   0        0        0    10230 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/dvCompare.py
+-rw-rw-rw-   0        0        0      682 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/dvDatabases.py
+-rw-rw-rw-   0        0        0    10762 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/dv/dvDataframe.py
+-rw-rw-rw-   0        0        0     1441 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/dvObj.py
+-rw-rw-rw-   0        0        0     3789 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/dv/dvReporting.py
+-rw-rw-rw-   0        0        0    23252 2023-07-25 11:29:16.000000 gempyp-1.0.70b6/gempyp/dv/dvRunner.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.150733 gempyp-1.0.70b6/gempyp/engine/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/__init__.py
+-rw-rw-rw-   0        0        0     5092 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/baseTemplate.py
+-rw-rw-rw-   0        0        0     8428 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/engine/dataUpload.py
+-rw-rw-rw-   0        0        0    41280 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/engine/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.157163 gempyp-1.0.70b6/gempyp/engine/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/executors/__init__.py
+-rw-rw-rw-   0        0        0      443 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/executors/baseExecutor.py
+-rw-rw-rw-   0        0        0      656 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/gempypHelper.py
+-rw-rw-rw-   0        0        0     5483 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/runner.py
+-rw-rw-rw-   0        0        0     5537 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/simpleTestcase.py
+-rw-rw-rw-   0        0        0    12428 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/engine/testData.py
+-rw-rw-rw-   0        0        0     4566 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/gemPyp.py
+-rw-rw-rw-   0        0        0    14521 2023-07-25 11:29:16.000000 gempyp-1.0.70b6/gempyp/gempyp_plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.171524 gempyp-1.0.70b6/gempyp/jira/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/jira/__init__.py
+-rw-rw-rw-   0        0        0     2312 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/jira/jiraIntegration.py
+-rw-rw-rw-   0        0        0     4474 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/jira/jiraIntegrationCopy.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.191353 gempyp-1.0.70b6/gempyp/libs/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/libs/__init__.py
+-rw-rw-rw-   0        0        0     9011 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/libs/common.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.193707 gempyp-1.0.70b6/gempyp/libs/exceptions/
+-rw-rw-rw-   0        0        0       47 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/libs/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4352 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/libs/gem_s3_common.py
+-rw-rw-rw-   0        0        0     2642 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/libs/logConfig.py
+-rw-rw-rw-   0        0        0     1465 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/libs/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.266703 gempyp-1.0.70b6/gempyp/pyprest/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/__init__.py
+-rw-rw-rw-   0        0        0    11776 2023-07-25 11:29:16.000000 gempyp-1.0.70b6/gempyp/pyprest/apiCommon.py
+-rw-rw-rw-   0        0        0      491 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/beforeAfterSample.py
+-rw-rw-rw-   0        0        0    13694 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/compareFunctions.py
+-rw-rw-rw-   0        0        0    13567 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/keyCheck.py
+-rw-rw-rw-   0        0        0    15661 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/legacyComparison.py
+-rw-rw-rw-   0        0        0     1933 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/miscVariables.py
+-rw-rw-rw-   0        0        0    10792 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/postAssertion.py
+-rw-rw-rw-   0        0        0     4235 2023-07-25 10:59:19.000000 gempyp-1.0.70b6/gempyp/pyprest/postVariables.py
+-rw-rw-rw-   0        0        0     3889 2023-07-25 10:59:20.000000 gempyp-1.0.70b6/gempyp/pyprest/preVariables.py
+-rw-rw-rw-   0        0        0     8271 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/predefinedFunctions.py
+-rw-rw-rw-   0        0        0    36757 2023-07-25 10:59:20.000000 gempyp-1.0.70b6/gempyp/pyprest/pypRest.py
+-rw-rw-rw-   0        0        0     4333 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/reporting.py
+-rw-rw-rw-   0        0        0     2725 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/restEngine.py
+-rw-rw-rw-   0        0        0     1031 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/restObj.py
+-rw-rw-rw-   0        0        0     6308 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/utils.py
+-rw-rw-rw-   0        0        0     5463 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/pyprest/variableReplacement.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:41.273536 gempyp-1.0.70b6/gempyp/reporter/
+-rw-rw-rw-   0        0        0        0 2023-07-25 10:58:40.000000 gempyp-1.0.70b6/gempyp/reporter/__init__.py
+-rw-rw-rw-   0        0        0     8517 2023-07-25 10:59:20.000000 gempyp-1.0.70b6/gempyp/reporter/reportGenerator.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:57:40.910869 gempyp-1.0.70b6/gempyp.egg-info/
+-rw-rw-rw-   0        0        0       79 2023-07-25 11:57:40.000000 gempyp-1.0.70b6/gempyp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2645 2023-07-25 11:57:40.000000 gempyp-1.0.70b6/gempyp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:57:40.000000 gempyp-1.0.70b6/gempyp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-25 11:57:40.000000 gempyp-1.0.70b6/gempyp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 11:57:40.000000 gempyp-1.0.70b6/gempyp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1502 2023-07-25 11:57:30.000000 gempyp-1.0.70b6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:57:41.281618 gempyp-1.0.70b6/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-07-25 11:57:25.000000 gempyp-1.0.70b6/setup.py
```

### Comparing `gempyp-1.0.70b4/gempyp/config/baseConfig.py` & `gempyp-1.0.70b6/gempyp/config/baseConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/config/DefaultSettings.py` & `gempyp-1.0.70b6/gempyp/config/DefaultSettings.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/config/GitLinkXML.py` & `gempyp-1.0.70b6/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/config/xmlConfig.py` & `gempyp-1.0.70b6/gempyp/config/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.70b6/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/compare.py` & `gempyp-1.0.70b6/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.70b6/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.70b6/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.70b6/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/data.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/database.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.70b6/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_compare/data_comp.py` & `gempyp-1.0.70b6/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/data_uploader.py` & `gempyp-1.0.70b6/gempyp/data_uploader.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dfOperations.py` & `gempyp-1.0.70b6/gempyp/dv/dfOperations.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvCompare.py` & `gempyp-1.0.70b6/gempyp/dv/dvCompare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvDatabases.py` & `gempyp-1.0.70b6/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvDataframe.py` & `gempyp-1.0.70b6/gempyp/dv/dvDataframe.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvObj.py` & `gempyp-1.0.70b6/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvReporting.py` & `gempyp-1.0.70b6/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/dv/dvRunner.py` & `gempyp-1.0.70b6/gempyp/dv/dvRunner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/baseTemplate.py` & `gempyp-1.0.70b6/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/dataUpload.py` & `gempyp-1.0.70b6/gempyp/engine/dataUpload.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/engine.py` & `gempyp-1.0.70b6/gempyp/engine/engine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/gempypHelper.py` & `gempyp-1.0.70b6/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/runner.py` & `gempyp-1.0.70b6/gempyp/engine/runner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.70b6/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/engine/testData.py` & `gempyp-1.0.70b6/gempyp/engine/testData.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/gemPyp.py` & `gempyp-1.0.70b6/gempyp/gemPyp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/gempyp_plugin.py` & `gempyp-1.0.70b6/gempyp/gempyp_plugin.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.70b6/gempyp/jira/jiraIntegration.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.70b6/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/libs/common.py` & `gempyp-1.0.70b6/gempyp/libs/common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.70b6/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/libs/logConfig.py` & `gempyp-1.0.70b6/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/libs/parsers.py` & `gempyp-1.0.70b6/gempyp/libs/parsers.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.70b6/gempyp/pyprest/apiCommon.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.70b6/gempyp/pyprest/compareFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.70b6/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.70b6/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.70b6/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.70b6/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/postVariables.py` & `gempyp-1.0.70b6/gempyp/pyprest/postVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.70b6/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/preVariables.py` & `gempyp-1.0.70b6/gempyp/pyprest/preVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/pypRest.py` & `gempyp-1.0.70b6/gempyp/pyprest/pypRest.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/reporting.py` & `gempyp-1.0.70b6/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/restEngine.py` & `gempyp-1.0.70b6/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/restObj.py` & `gempyp-1.0.70b6/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/utils.py` & `gempyp-1.0.70b6/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.70b6/gempyp/pyprest/variableReplacement.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.70b6/gempyp/reporter/reportGenerator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b4/pyproject.toml` & `gempyp-1.0.70b6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.70b4"
+version = "1.0.70b6"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
@@ -50,7 +50,10 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 gempyp = "gempyp.gemPyp:main"
+
+[tool.poetry.plugins."pytest11"]
+"gempyp" = "gempyp.gempyp_plugin"
```

### Comparing `gempyp-1.0.70b4/README.md` & `gempyp-1.0.70b6/README.md`

 * *Files identical despite different names*

