# Comparing `tmp/gempyp-1.0.70b1.tar.gz` & `tmp/gempyp-1.0.70b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.70b1.tar", max compression
+gzip compressed data, was "gempyp-1.0.70b3.tar", max compression
```

## Comparing `gempyp-1.0.70b1.tar` & `gempyp-1.0.70b3.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0       25 2023-05-19 10:29:23.809487 gempyp-1.0.70b1/gempyp/__init__.py
--rw-r--r--   0        0        0      108 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/cli.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/__init__.py
--rw-r--r--   0        0        0     7387 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0      198 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/config/customParser.py
--rw-r--r--   0        0        0     1802 2023-05-19 10:29:23.812431 gempyp-1.0.70b1/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     4007 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0     6758 2023-05-19 10:29:23.813426 gempyp-1.0.70b1/gempyp/data_uploader.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/__init__.py
--rw-r--r--   0        0        0     2285 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dfOperations.py
--rw-r--r--   0        0        0    10230 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0     9470 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    23229 2023-05-19 10:29:23.814426 gempyp-1.0.70b1/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/__init__.py
--rw-r--r--   0        0        0     5092 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     8414 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    41041 2023-05-19 10:29:23.816426 gempyp-1.0.70b1/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2023-05-05 14:21:30.372942 gempyp-1.0.70b1/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2023-05-05 14:21:30.373956 gempyp-1.0.70b1/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5483 2023-05-19 10:29:23.818430 gempyp-1.0.70b1/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5537 2023-05-05 14:21:30.374954 gempyp-1.0.70b1/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    12428 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2023-05-05 14:21:30.376963 gempyp-1.0.70b1/gempyp/final_report.html
--rw-r--r--   0        0        0     4566 2023-05-19 10:29:23.819425 gempyp-1.0.70b1/gempyp/gemPyp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.379963 gempyp-1.0.70b1/gempyp/jira/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-05 14:21:30.380963 gempyp-1.0.70b1/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2023-05-05 14:21:30.380963 gempyp-1.0.70b1/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.381963 gempyp-1.0.70b1/gempyp/libs/__init__.py
--rw-r--r--   0        0        0     9045 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/libs/common.py
--rw-r--r--   0        0        0      131 2023-05-05 14:21:30.383963 gempyp-1.0.70b1/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2023-05-05 14:21:30.384963 gempyp-1.0.70b1/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2023-05-05 14:21:30.385646 gempyp-1.0.70b1/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2023-05-05 14:21:30.386656 gempyp-1.0.70b1/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1465 2023-05-05 14:21:30.386656 gempyp-1.0.70b1/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.387656 gempyp-1.0.70b1/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0     9844 2023-05-05 14:21:30.388723 gempyp-1.0.70b1/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2023-05-05 14:21:30.389602 gempyp-1.0.70b1/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    13694 2023-05-05 14:21:30.390435 gempyp-1.0.70b1/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13567 2023-05-05 14:21:30.391447 gempyp-1.0.70b1/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2023-05-05 14:21:30.392445 gempyp-1.0.70b1/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2023-05-05 14:21:30.393446 gempyp-1.0.70b1/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10792 2023-05-05 14:21:30.393446 gempyp-1.0.70b1/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     4195 2023-05-05 14:21:30.394437 gempyp-1.0.70b1/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2023-05-05 14:21:30.396448 gempyp-1.0.70b1/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     3873 2023-05-05 14:21:30.395446 gempyp-1.0.70b1/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    36175 2023-05-05 14:21:30.397446 gempyp-1.0.70b1/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4333 2023-05-05 14:21:30.398445 gempyp-1.0.70b1/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2023-05-05 14:21:30.398445 gempyp-1.0.70b1/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2023-05-05 14:21:30.399475 gempyp-1.0.70b1/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2023-05-05 14:21:30.400514 gempyp-1.0.70b1/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     5463 2023-05-05 14:21:30.400514 gempyp-1.0.70b1/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.401512 gempyp-1.0.70b1/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0     6959 2023-05-05 14:21:56.358422 gempyp-1.0.70b1/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    13086 2023-05-19 10:29:23.821450 gempyp-1.0.70b1/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     2490 2023-05-19 10:29:23.823426 gempyp-1.0.70b1/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2023-05-05 14:21:30.404588 gempyp-1.0.70b1/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/LICENSE
--rw-r--r--   0        0        0     1431 2023-05-19 10:53:48.974856 gempyp-1.0.70b1/pyproject.toml
--rw-r--r--   0        0        0     3161 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/README.md
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 gempyp-1.0.70b1/PKG-INFO
+-rw-r--r--   0        0        0    64741 2023-07-25 09:02:45.253390 gempyp-1.0.70b3/final_report.html
+-rw-r--r--   0        0        0       25 2023-07-25 09:02:47.561800 gempyp-1.0.70b3/gempyp/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-25 09:02:47.570571 gempyp-1.0.70b3/gempyp/cli.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.637331 gempyp-1.0.70b3/gempyp/config/__init__.py
+-rw-r--r--   0        0        0     7468 2023-07-25 09:02:47.645724 gempyp-1.0.70b3/gempyp/config/baseConfig.py
+-rw-r--r--   0        0        0      198 2023-07-25 09:02:47.661836 gempyp-1.0.70b3/gempyp/config/customParser.py
+-rw-r--r--   0        0        0     1812 2023-07-25 09:02:47.670573 gempyp-1.0.70b3/gempyp/config/DefaultSettings.py
+-rw-r--r--   0        0        0       62 2023-07-25 09:02:47.679027 gempyp-1.0.70b3/gempyp/config/gempyp.conf
+-rw-r--r--   0        0        0     2145 2023-07-25 09:02:47.696127 gempyp-1.0.70b3/gempyp/config/GitLinkXML.py
+-rw-r--r--   0        0        0    21143 2023-07-25 09:02:47.704817 gempyp-1.0.70b3/gempyp/config/Result.html
+-rw-r--r--   0        0        0       26 2023-07-25 09:02:47.721684 gempyp-1.0.70b3/gempyp/config/suite_conf.json
+-rw-r--r--   0        0        0       28 2023-07-25 09:02:47.730180 gempyp-1.0.70b3/gempyp/config/testcase_conf.json
+-rw-r--r--   0        0        0     4003 2023-07-25 09:02:47.738614 gempyp-1.0.70b3/gempyp/config/xmlConfig.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.755342 gempyp-1.0.70b3/gempyp/data_compare/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.797468 gempyp-1.0.70b3/gempyp/data_compare/common/__init__.py
+-rw-r--r--   0        0        0     3627 2023-07-25 09:02:47.803575 gempyp-1.0.70b3/gempyp/data_compare/common/common_functions.py
+-rw-r--r--   0        0        0      956 2023-07-25 09:02:47.763420 gempyp-1.0.70b3/gempyp/data_compare/compare.py
+-rw-r--r--   0        0        0      149 2023-07-25 09:02:47.820324 gempyp-1.0.70b3/gempyp/data_compare/config/dvm.json
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.837255 gempyp-1.0.70b3/gempyp/data_compare/configurator/__init__.py
+-rw-r--r--   0        0        0     4635 2023-07-25 09:02:47.853734 gempyp-1.0.70b3/gempyp/data_compare/configurator/configurator.py
+-rw-r--r--   0        0        0      320 2023-07-25 09:02:47.862000 gempyp-1.0.70b3/gempyp/data_compare/configurator/validator.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.878795 gempyp-1.0.70b3/gempyp/data_compare/core/__init__.py
+-rw-r--r--   0        0        0      589 2023-07-25 09:02:47.896258 gempyp-1.0.70b3/gempyp/data_compare/core/comparator.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.904378 gempyp-1.0.70b3/gempyp/data_compare/core/Compare.py
+-rw-r--r--   0        0        0    10157 2023-07-25 09:02:47.920782 gempyp-1.0.70b3/gempyp/data_compare/core/python_obj_comparator.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:47.937450 gempyp-1.0.70b3/gempyp/data_compare/data/__init__.py
+-rw-r--r--   0        0        0     5498 2023-07-25 09:02:47.954174 gempyp-1.0.70b3/gempyp/data_compare/data/data.py
+-rw-r--r--   0        0        0      869 2023-07-25 09:02:47.962540 gempyp-1.0.70b3/gempyp/data_compare/data/database.py
+-rw-r--r--   0        0        0     1903 2023-07-25 09:02:47.971012 gempyp-1.0.70b3/gempyp/data_compare/data/db_mysql.py
+-rw-r--r--   0        0        0     2646 2023-07-25 09:02:47.988463 gempyp-1.0.70b3/gempyp/data_compare/data/db_oracle.py
+-rw-r--r--   0        0        0     2436 2023-07-25 09:02:48.004315 gempyp-1.0.70b3/gempyp/data_compare/data/db_postgre.py
+-rw-r--r--   0        0        0     1999 2023-07-25 09:02:48.012725 gempyp-1.0.70b3/gempyp/data_compare/data/db_sqlite.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.021006 gempyp-1.0.70b3/gempyp/data_compare/data/file_processor.py
+-rw-r--r--   0        0        0    11161 2023-07-25 09:02:47.780448 gempyp-1.0.70b3/gempyp/data_compare/data_comp.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.045753 gempyp-1.0.70b3/gempyp/data_compare/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.062185 gempyp-1.0.70b3/gempyp/data_compare/tools/__init__.py
+-rw-r--r--   0        0        0     6758 2023-07-25 09:02:47.578786 gempyp-1.0.70b3/gempyp/data_uploader.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.078455 gempyp-1.0.70b3/gempyp/dv/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-25 09:02:48.087107 gempyp-1.0.70b3/gempyp/dv/dfOperations.py
+-rw-r--r--   0        0        0    10230 2023-07-25 09:02:48.096260 gempyp-1.0.70b3/gempyp/dv/dvCompare.py
+-rw-r--r--   0        0        0      682 2023-07-25 09:02:48.113148 gempyp-1.0.70b3/gempyp/dv/dvDatabases.py
+-rw-r--r--   0        0        0    10762 2023-07-25 09:02:48.121628 gempyp-1.0.70b3/gempyp/dv/dvDataframe.py
+-rw-r--r--   0        0        0     1441 2023-07-25 09:02:48.138148 gempyp-1.0.70b3/gempyp/dv/dvObj.py
+-rw-r--r--   0        0        0     3789 2023-07-25 09:02:48.146742 gempyp-1.0.70b3/gempyp/dv/dvReporting.py
+-rw-r--r--   0        0        0    23410 2023-07-25 09:02:48.154947 gempyp-1.0.70b3/gempyp/dv/dvRunner.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.171202 gempyp-1.0.70b3/gempyp/engine/__init__.py
+-rw-r--r--   0        0        0     5092 2023-07-25 09:02:48.187801 gempyp-1.0.70b3/gempyp/engine/baseTemplate.py
+-rw-r--r--   0        0        0     8428 2023-07-25 09:02:48.196579 gempyp-1.0.70b3/gempyp/engine/dataUpload.py
+-rw-r--r--   0        0        0    41280 2023-07-25 09:02:48.213827 gempyp-1.0.70b3/gempyp/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.272863 gempyp-1.0.70b3/gempyp/engine/executors/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-25 09:02:48.289433 gempyp-1.0.70b3/gempyp/engine/executors/baseExecutor.py
+-rw-r--r--   0        0        0      656 2023-07-25 09:02:48.222820 gempyp-1.0.70b3/gempyp/engine/gempypHelper.py
+-rw-r--r--   0        0        0     5483 2023-07-25 09:02:48.239675 gempyp-1.0.70b3/gempyp/engine/runner.py
+-rw-r--r--   0        0        0     5537 2023-07-25 09:02:48.248172 gempyp-1.0.70b3/gempyp/engine/simpleTestcase.py
+-rw-r--r--   0        0        0    12428 2023-07-25 09:02:48.256596 gempyp-1.0.70b3/gempyp/engine/testData.py
+-rw-r--r--   0        0        0    64741 2023-07-25 09:02:47.595428 gempyp-1.0.70b3/gempyp/final_report.html
+-rw-r--r--   0        0        0     4566 2023-07-25 09:02:47.612199 gempyp-1.0.70b3/gempyp/gemPyp.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.305625 gempyp-1.0.70b3/gempyp/jira/__init__.py
+-rw-r--r--   0        0        0     2312 2023-07-25 09:02:48.313575 gempyp-1.0.70b3/gempyp/jira/jiraIntegration.py
+-rw-r--r--   0        0        0     4474 2023-07-25 09:02:48.330188 gempyp-1.0.70b3/gempyp/jira/jiraIntegrationCopy.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.345465 gempyp-1.0.70b3/gempyp/libs/__init__.py
+-rw-r--r--   0        0        0     9011 2023-07-25 09:02:48.361846 gempyp-1.0.70b3/gempyp/libs/common.py
+-rw-r--r--   0        0        0      131 2023-07-25 09:02:48.422292 gempyp-1.0.70b3/gempyp/libs/enums/run_types.py
+-rw-r--r--   0        0        0      318 2023-07-25 09:02:48.438970 gempyp-1.0.70b3/gempyp/libs/enums/status.py
+-rw-r--r--   0        0        0       47 2023-07-25 09:02:48.455679 gempyp-1.0.70b3/gempyp/libs/exceptions/__init__.py
+-rw-r--r--   0        0        0     4352 2023-07-25 09:02:48.370566 gempyp-1.0.70b3/gempyp/libs/gem_s3_common.py
+-rw-r--r--   0        0        0     2642 2023-07-25 09:02:48.388175 gempyp-1.0.70b3/gempyp/libs/logConfig.py
+-rw-r--r--   0        0        0     1465 2023-07-25 09:02:48.397143 gempyp-1.0.70b3/gempyp/libs/parsers.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.471992 gempyp-1.0.70b3/gempyp/pyprest/__init__.py
+-rw-r--r--   0        0        0    11819 2023-07-25 09:02:48.488765 gempyp-1.0.70b3/gempyp/pyprest/apiCommon.py
+-rw-r--r--   0        0        0      491 2023-07-25 09:02:48.497200 gempyp-1.0.70b3/gempyp/pyprest/beforeAfterSample.py
+-rw-r--r--   0        0        0    13694 2023-07-25 09:02:48.514475 gempyp-1.0.70b3/gempyp/pyprest/compareFunctions.py
+-rw-r--r--   0        0        0    13567 2023-07-25 09:02:48.522672 gempyp-1.0.70b3/gempyp/pyprest/keyCheck.py
+-rw-r--r--   0        0        0    15661 2023-07-25 09:02:48.539506 gempyp-1.0.70b3/gempyp/pyprest/legacyComparison.py
+-rw-r--r--   0        0        0     1933 2023-07-25 09:02:48.547684 gempyp-1.0.70b3/gempyp/pyprest/miscVariables.py
+-rw-r--r--   0        0        0    10792 2023-07-25 09:02:48.555952 gempyp-1.0.70b3/gempyp/pyprest/postAssertion.py
+-rw-r--r--   0        0        0     4235 2023-07-25 09:02:48.572216 gempyp-1.0.70b3/gempyp/pyprest/postVariables.py
+-rw-r--r--   0        0        0     8271 2023-07-25 09:02:48.589019 gempyp-1.0.70b3/gempyp/pyprest/predefinedFunctions.py
+-rw-r--r--   0        0        0     3889 2023-07-25 09:02:48.605902 gempyp-1.0.70b3/gempyp/pyprest/preVariables.py
+-rw-r--r--   0        0        0    36757 2023-07-25 09:02:48.614021 gempyp-1.0.70b3/gempyp/pyprest/pypRest.py
+-rw-r--r--   0        0        0     4333 2023-07-25 09:02:48.630404 gempyp-1.0.70b3/gempyp/pyprest/reporting.py
+-rw-r--r--   0        0        0     2725 2023-07-25 09:02:48.638833 gempyp-1.0.70b3/gempyp/pyprest/restEngine.py
+-rw-r--r--   0        0        0     1031 2023-07-25 09:02:48.647046 gempyp-1.0.70b3/gempyp/pyprest/restObj.py
+-rw-r--r--   0        0        0     6308 2023-07-25 09:02:48.663514 gempyp-1.0.70b3/gempyp/pyprest/utils.py
+-rw-r--r--   0        0        0     5463 2023-07-25 09:02:48.671869 gempyp-1.0.70b3/gempyp/pyprest/variableReplacement.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:02:48.688494 gempyp-1.0.70b3/gempyp/reporter/__init__.py
+-rw-r--r--   0        0        0     8517 2023-07-25 09:02:48.697369 gempyp-1.0.70b3/gempyp/reporter/reportGenerator.py
+-rw-r--r--   0        0        0    13526 2023-07-25 09:02:48.713738 gempyp-1.0.70b3/gempyp/sdk/executor.py
+-rw-r--r--   0        0        0     1177 2023-07-25 09:02:48.720460 gempyp-1.0.70b3/gempyp/sdk/Gempytest.py
+-rw-r--r--   0        0        0     3128 2023-07-25 09:02:48.737367 gempyp-1.0.70b3/gempyp/sdk/worker.py
+-rw-r--r--   0        0        0    11547 2023-07-25 09:02:47.620545 gempyp-1.0.70b3/gempyp/testcase.html
+-rw-r--r--   0        0        0        2 2023-07-25 09:02:45.299942 gempyp-1.0.70b3/LICENSE
+-rw-r--r--   0        0        0     1431 2023-07-25 09:02:45.350223 gempyp-1.0.70b3/pyproject.toml
+-rw-r--r--   0        0        0     3161 2023-07-25 09:02:45.400285 gempyp-1.0.70b3/README.md
+-rw-r--r--   0        0        0    11547 2023-07-25 09:02:45.452797 gempyp-1.0.70b3/testcase.html
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 gempyp-1.0.70b3/PKG-INFO
```

### Comparing `gempyp-1.0.70b1/gempyp/config/baseConfig.py` & `gempyp-1.0.70b3/gempyp/config/baseConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 class AbstarctBaseConfig(ABC):
     def __init__(self, *args, **kwargs):
         self._CONFIG = {}
         self.cli_config ={}
         self.total_yflag_testcase =0
         
         try:
-            self.parse(*args, **kwargs)
+            self.log_file=self.parse(*args, **kwargs)
             # filter removed from here because we need to apply filter after updating data with cli input(if given)
             # self.update()
             logging.info("----------- Xml parsing completed ------------")
         except Exception as e:
             traceback.print_exc()
             logging.error("failed to parse the config: {e}".format(e=e))
+    
+    def getLogFilePath(self):
+        return self.log_file
 
     def getSuiteConfig(self) -> Dict:
         # logging.info("^^^^^^^^^^^^^ \n {suite_data} \n^^^^^^^^^".format(suite_data=self._CONFIG["SUITE_DATA"]))
         self.filter()
         return self._CONFIG["SUITE_DATA"]
 
     def getTestcaseConfig(self) -> Dict:
```

### Comparing `gempyp-1.0.70b1/gempyp/config/DefaultSettings.py` & `gempyp-1.0.70b3/gempyp/config/DefaultSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,19 @@
         url = checkUrl(url)
         response = dataUpload._sendData(" ", url, bridge_token, user_name,"GET")
         if response.status_code == 200:
             url_enter_point = response.json()
             urls["data"]=url_enter_point["data"]
             global apiSuccess
             apiSuccess = True
-        elif re.search('50[0-9]',str(response.status_code)):
-            logging.warning("Error Occurs While Getting the BASE_URLs")
-        else:
-            logging.info("Some Error From the Client Side, Maybe username or bridgeToken, Therefore terminating execution")
-            sys.exit()
+        # elif re.search('50[0-9]',str(response.status_code)):
+        #     logging.warning("Error Occurs While Getting the BASE_URLs")
+        # else:
+        #     logging.info("Some Error From the Client Side, Maybe username or bridgeToken, Therefore terminating execution")
+        #     sys.exit()
     except Exception as e:
             traceback.print_exc()
             logging.warning("Error Occurs While Getting the BASE_URLs")
             sys.exit()
 
 # for sending urls to dataupload file
 def getUrls(apiName):
```

### Comparing `gempyp-1.0.70b1/gempyp/config/GitLinkXML.py` & `gempyp-1.0.70b3/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/config/Result.html` & `gempyp-1.0.70b3/gempyp/config/Result.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/config/xmlConfig.py` & `gempyp-1.0.70b3/gempyp/config/xmlConfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,27 +50,28 @@
             self.unique_id = self._CONFIG["SUITE_DATA"]["S_RUN_ID"]
         os.environ['unique_id'] = self.unique_id
         os.environ['log_dir'] = self.log_dir
         warnings.filterwarnings('ignore')
         suiteLogsLoc = str(os.path.join(self.log_dir, 'Suite_' + self.unique_id + '.txt'))  ## replacing log with txt for UI compatibility
         LoggingConfig(os.path.join(self.log_dir, 'Suite_' + self.unique_id + '.txt'))  ## replacing log with txt for UI compatibility
         # LoggingConfig(suiteLogsLoc)
-        logging.info("------suite logs------"+ str(suiteLogsLoc))
+        logging.info("suite logs : "+ str(suiteLogsLoc))
         self._CONFIG["TESTCASE_DATA"] = self._getTestCaseData(data)
         self._CONFIG["SUITE_DATA"]['LOG_DIR'] = self.log_dir
         self._CONFIG["SUITE_DATA"]['UNIQUE_ID'] = self.unique_id
+        return suiteLogsLoc
 
     def _getSuiteData(self, data) -> Dict:
 
         suite_data = data.find("suite")
 
         suite_dict = xmlToDict(suite_data)
         suite_dict={key.replace('-','_'):value for key,value in suite_dict.items()}
         suite_dict["SUITE_VARS"] = {}
-        logging.info("--------suite_dict--------\n {suite_dict} \n----------".format(suite_dict=suite_dict))
+        logging.info("suite_dict: \n {suite_dict} \n".format(suite_dict=suite_dict))
         # do your validations here
 
         return suite_dict
 
     def _getTestCaseData(self, data) -> Dict:
 
         testcase_data = data.find("testcases")
```

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.70b3/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/compare.py` & `gempyp-1.0.70b3/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.70b3/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.70b3/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.70b3/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/data.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/database.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.70b3/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_compare/data_comp.py` & `gempyp-1.0.70b3/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/data_uploader.py` & `gempyp-1.0.70b3/gempyp/data_uploader.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dfOperations.py` & `gempyp-1.0.70b3/gempyp/dv/dfOperations.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvCompare.py` & `gempyp-1.0.70b3/gempyp/dv/dvCompare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvDatabases.py` & `gempyp-1.0.70b3/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvDataframe.py` & `gempyp-1.0.70b3/gempyp/dv/dvDataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,23 +109,48 @@
 
     def dbOperations(self, cred, db):
         try:
             log = f"----Connecting to {db}DB----"
             self.logger.info(log)
             myDB = self.connectingDB(db, cred)
         except Exception as e:
+            print("DB Operations..........................................")
             self.reporter.addRow(
                 f"Connection to {db}DB: ", "Exception Occurred", status.ERR)
             self.logger.error(str(e))
-            
-            # self.reporter.addMisc(
-            #         "REASON OF FAILURE", get_reason_of_failure(traceback.format_exc(), e))
-
             raise Exception(e)
+        
+        try:
+            db_1, columns = self.executeQuery(db, myDB)
+        except Exception as e:
+            self.logger.error(str(e))
+            self.reporter.addRow(
+                f"Executing {db} SQL", "Exception Occurred", status.ERR)
+            raise e
+        return db_1,columns
+    
+    def fetch_data_with_retries(self, cred, db):
+        retry_limit = 3  # Maximum number of connection retry attempts
+        retry_delay = 10  # Delay between retry attempts in seconds
+        retries = 0
+        while retries < retry_limit:
+            try:
+                return self.dbOperations(cred, db)
+            except Exception as e:
+                print(f"Connection failed: {str(e)}")
+                print("Retrying...")
+                print("fetch_data_with_retries...........................")
+                time.sleep(retry_delay)
+                retries += 1
+
+        print("Maximum number of retries exceeded. Failed to fetch data.")
+        return None, None
 
+    
+    def executeQuery(self,db,myDB):
         try:
             self.logger.info(f"----Executing the {db}SQL----")
             # checking whether it is mongodb object by checking mongoclient in starting of the object
             x = re.search("^MongoClient.*", str(myDB))
             if x:
                 try:
                     db_name = f'{db}_DB'
@@ -144,16 +169,20 @@
                 except Exception:
                     self.reporter.addRow("Fetching Query","Not Present in JSON Format",status.ERR)
                     raise Exception("Mongo Query not Present in JSON Format")
                 results = list(conn.find(query))
                 db_1 = pd.DataFrame(results)
                 columns = list(db_1.columns)
             else:
+                # try:
                 myCursor = myDB.cursor()
                 sql = f"{db}_SQL"
+                statement_timeout = 0
+                myDB.cursor().execute(f"ALTER SESSION SET STATEMENT_TIMEOUT_IN_SECONDS = {statement_timeout}")
+                myDB.cursor().execute(f"alter warehouse COMPUTE_WH set statement_timeout_in_seconds = {statement_timeout}")
                 myCursor.execute(self.configData[sql])
                 self.reporter.addRow(
                     f"Executing {db} SQL", f"{self.configData[sql]}<br>{db} SQL executed Successfull", status.PASS)
                 columns = [i[0] for i in myCursor.description]
                 results = myCursor.fetchall()
                 db_1 = pd.DataFrame(results,columns=columns)
         except Exception as e:
```

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvObj.py` & `gempyp-1.0.70b3/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvReporting.py` & `gempyp-1.0.70b3/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/dv/dvRunner.py` & `gempyp-1.0.70b3/gempyp/dv/dvRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,17 @@
             target_duplicates_df, tgt_dup_len = self.getDuplicateKeysDf(self.target_df, "TARGET")
             dup_keys_length = src_dup_len + tgt_dup_len
             duplicate_keys_df = pd.concat([source_duplicates_df , target_duplicates_df ], axis=0, ignore_index=True)
 
             if self.source_columns == self.target_columns:
                 pass
             else:
+                print(self.source_columns)
+                print(self.target_columns)
+                print("___________________________________________")
                 self.logger.info(
                     "--------Same Column not Present in Both Table--------")
                 self.reporter.addRow(
                     "Same Columns in Table", "Not Found", status.ERR)
                 raise Exception("Same Columns Not Found")
 
             """deleting duplicates from df and keeping last ones"""
@@ -473,14 +476,15 @@
             value=config.get(key)
             if(type(value)!=logging.Logger):
                 if re.search("mysql.connector.connect",value) or re.search("^{",value):
                     config[key] = re.sub(pattern, lambda match: f"'{os.environ.get(match.group(1), '')}'", value)
                 else:
                     if("ENV." in value):
                         config[key]=os.environ.get(value.replace("ENV.",""))
+        print(config)
         return config
     
     def parseConfigDict(self,conf):
         for key in conf.keys():
             if("ENV." in conf.get(key) and os.environ.get(conf.get(key).replace("ENV.",""))):
                 conf[key]=os.environ.get(conf.get(key).replace("ENV.",""))
         return conf
```

### Comparing `gempyp-1.0.70b1/gempyp/engine/baseTemplate.py` & `gempyp-1.0.70b3/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/engine/dataUpload.py` & `gempyp-1.0.70b3/gempyp/engine/dataUpload.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,21 @@
                 DefaultSettings.project_id = json.loads(response.text)["data"]["p_id"]
             except Exception as e:
                 logging.info(traceback.format_exc())
             if payload in suite_data:
                 suite_data.remove(payload)
         elif response and response.status_code == 200:
             logging.info("Suite Data updated Successfully")
-        elif re.search('50[0-9]',str(response.status_code)):
-            logging.info("Suite data is not uploaded")
-            if payload not in suite_data:
-                suite_data.append(payload)
-        else:
-            logging.info("Some Error From the Client Side, Terminating Execution")
-            sys.exit()
+        # elif re.search('50[0-9]',str(response.status_code)):
+        #     logging.info("Suite data is not uploaded")
+        #     if payload not in suite_data:
+        #         suite_data.append(payload)
+        # else:
+        #     logging.info("Some Error From the Client Side, Terminating Execution")
+        #     sys.exit()
         # else:
         #     logging.info("Suite data is not uploaded")
         #     if payload not in suite_data:
         #         suite_data.append(payload)
                 
     except Exception as e:
         logging.error(traceback.format_exc())
```

### Comparing `gempyp-1.0.70b1/gempyp/engine/engine.py` & `gempyp-1.0.70b3/gempyp/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             #     w.write(listToStr)
             unuploaded_path=self.DATA.WriteSuiteFile(self.base_url,self.ouput_folder,self.username,self.bridgetoken)
             
         if("EMAIL_TO" in self.PARAMS.keys()):
             sendMail(self.s_run_id,self.mail,self.bridgetoken, self.username)
 
         self.repJson = TemplateData().makeSuiteReport(self.DATA.getJSONData(), self.testcase_data, self.ouput_folder,self.jewel_user)
-        TemplateData().repSummary(self.repJson, jewel, unuploaded_path)
+        TemplateData().repSummary(self.repJson, jewel, unuploaded_path,self.testcase_log_folder,self.complete_logs,self.bridgetoken,self.username,self.suite_log_file)
 
     def makeOutputFolder(self):
         """
         make outputFolder for report named as gempyp_reports in user home directory if not given by the user and makes log fplder for log files
         if given by user than set user given path for reports file   
         """
 
@@ -234,30 +234,32 @@
 
         os.makedirs(self.ouput_folder)
         self.testcase_folder = os.path.join(self.ouput_folder, "testcases")
         os.makedirs(self.testcase_folder)
         self.testcase_log_folder = os.path.join(self.ouput_folder, "logs")
         os.environ['TESTCASE_LOG_FOLDER'] = self.testcase_log_folder
         os.makedirs(self.testcase_log_folder)
+        self.complete_logs = os.path.join(self.testcase_log_folder,self.s_run_id + '.txt')
     def verify(self,value):
-        if(re.search(r'[^a-zA-Z0-9_ ]',value)):
+        if(re.search(r'[^a-zA-Z0-9_ .-]',value)):
                 logging.info("Some Error From the Client Side. May be s_run_id, project_name or ENV is not in a correct format")
                 sys.exit()
         else:
                 return value
 
     def setUP(self, config: Type[AbstarctBaseConfig]):
 
         """
 
         assigning values to some attributes which will be used in method makeSuiteDetails
 
         """
         
         self.PARAMS = config.getSuiteConfig()
+        self.suite_log_file=config.getLogFilePath()
         self.ENV = os.getenv("appenv", "BETA").upper()
 
         #checking if url is present in file and calling get api
         # if self.PARAMS.get("BASE_URL", None):
         #     DefaultSettings.getEnterPoint(self.PARAMS["BASE_URL"] ,self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"] )
         self.CONFIG = config
 
@@ -314,15 +316,15 @@
 
             if self.PARAMS.get("S_ID", None):
                 self.jewel_run = True
             else:
                 try:
                     if DefaultSettings.apiSuccess:
                         self.s3_url = upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=self.bridgetoken, username=self.username, file=self.PARAMS["config"])[0]["Url"]
-                        logging.info("--------- url" + str(self.s3_url))
+                        logging.info("S3 Url: " + str(self.s3_url))
                     else:
                         self.s3_url = self.PARAMS["config"]
                 except Exception as e:
                     logging.info(e)
         #add suite_vars here 
 
     # def parseMails(self):
@@ -340,15 +342,15 @@
             self.s_run_id = self.verify(self.PARAMS["S_RUN_ID"])
         else:
             if not self.unique_id:
                 self.unique_id = uuid.uuid4()
             self.s_run_id = f"{self.project_name}_{self.project_env}_{self.unique_id}"
             self.s_run_id = self.s_run_id.upper()
         # self.s_run_id = re.sub(r'[^\w\s]', '',self.s_run_id)
-        self.s_run_id=re.sub(r'\s+', '_',self.s_run_id)
+        # self.s_run_id=re.sub(r'\s+', '_',self.s_run_id)
         logging.info("S_RUN_ID: {}".format(self.s_run_id))
         suite_details = {
             "s_run_id": self.s_run_id,
             "s_start_time": self.start_time,
             "s_end_time": None,
             "s_id": self.PARAMS.get("S_ID", "test_id"),
             "status": status.EXE.name,
```

### Comparing `gempyp-1.0.70b1/gempyp/engine/gempypHelper.py` & `gempyp-1.0.70b3/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/engine/runner.py` & `gempyp-1.0.70b3/gempyp/engine/runner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.70b3/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/engine/testData.py` & `gempyp-1.0.70b3/gempyp/engine/testData.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/final_report.html` & `gempyp-1.0.70b3/final_report.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/gemPyp.py` & `gempyp-1.0.70b3/gempyp/gemPyp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.70b3/gempyp/jira/jiraIntegration.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,13 +51,13 @@
     if not title:
         del jira_body["title"]  # adding title  ######################### post 1.0.4
     jira_body = json.loads(json.dumps(str(jira_body).replace("'", '"')))
     try:
         logging.info("----------- Requesting JIRA API ------------")
         jira_id = createJira(jira_body, bridge_token, user_name)
         if jira_id:
-            logging.info(f"----------- Jira Id - {jira_id} ------------")
+            logging.info(f"Jira Id - {jira_id}")
         return jira_id
     except Exception as e:
         traceback.print_exc()
         return None
```

### Comparing `gempyp-1.0.70b1/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.70b3/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/libs/common.py` & `gempyp-1.0.70b3/gempyp/libs/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def readPath(file_name):
         try:
             conf = file_name.split(os.sep)
             if conf[0] == ".." or conf[0]==".":
                 script_path, script_name = importFromPath(file_name)
                 for each in sys.path:
                     if isinstance(each,dict) and each is not None:
-                        logging.info("--------- Fetching config path - {} ------".format( each['XMLConfigDir']))
+                        logging.info("Fetching config path - {}".format( each['XMLConfigDir']))
                         lib_path = os.path.join(each['XMLConfigDir'], file_name)
                         return lib_path
             else:
                 return file_name
         except Exception as e:
             traceback.print_exc()
 
@@ -135,15 +135,15 @@
             try:
                 dynamicTestcase = importlib.import_module(script_name) 
             except Exception:
                 logging.info("when absolute and module import both failed")
                 try:
                     for each in sys.path:
                         if isinstance(each,dict) and each is not None:
-                            logging.info("--------- Fetching config path - {} ------".format( each['XMLConfigDir']))
+                            logging.info("Fetching config path - {}".format( each['XMLConfigDir']))
                             lib_path = os.path.join(each['XMLConfigDir'], script_path)
                     sys.path.append(lib_path)
                     dynamicTestcase = importlib.import_module(script_name.split(".")[0])
                     import_flag = 1 
                 except Exception:
                     traceback.print_exc()
                 if import_flag != 1:
```

### Comparing `gempyp-1.0.70b1/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.70b3/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/libs/logConfig.py` & `gempyp-1.0.70b3/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/libs/parsers.py` & `gempyp-1.0.70b3/gempyp/libs/parsers.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.70b3/gempyp/pyprest/apiCommon.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,28 +12,65 @@
 import os
 
 
 class Api:
     def __init__(self):
         pass
 
+    def convert_quotes_boolean(self,data):
+        if isinstance(data, bool):
+            return str(data).lower()
+        elif isinstance(data, list):
+            return [self.convert_quotes_boolean(item) for item in data]
+        elif isinstance(data, dict):
+            return {self.convert_quotes_boolean(key): self.convert_quotes_boolean(value) for key, value in data.items()}
+        else:
+            return data
+
     def execute(self, request):
         encrypt_key = "Y4irRsiBmyGMBie5gAZ8va3IOHVOYZFxC5L1-jNydZk="
         result = Response()
         # if not request.file:
         header_dict = {key.upper(): value.upper() for key, value in request.headers.items()}
         if header_dict.get("CONTENT-TYPE", "") == "APPLICATION/JSON":
                 try:
                     if not isinstance(request.body, str):
                         request.body = json.dumps(request.body)
                 except Exception as e:
                     logging.info("JSON object can not be serialized")
                     logging.info(str(e))
             # write code for authentication 
             # decrypt password
+        else:
+                try:
+                    newFile=[]
+                    newBody={}
+                    for key,value in request.body.items():
+                        newFileTuple=tuple()
+                        if(isinstance(value,str) and os.path.isfile(value)):
+                            newFileTuple+=(key,open(value,'rb'))
+                            # newFile[key]=open(value,'rb')
+                            newFile.append(newFileTuple)
+                        else:
+                            if(isinstance(value,dict)):
+                                newBody[key]=str(json.dumps(value))
+                            else:
+                                newBody[key]=value
+                    request.file=newFile
+                    request.body=newBody
+                    # request.body = self.convert_quotes_boolean(request.body)
+                    print(type(request.body))
+                    print(request.body)
+                    print("__________________________________")
+                    pass
+                except Exception as e:
+                    logging.info("JSON object can not be serialized")
+                    logging.info(str(e))
+            # write code for authentication 
+            # decrypt password
         auth = None
         try:
                 if request.auth.upper() == "PASSWORD":
                     password = self.decrypt_(request.credentials.get("password", ""), encrypt_key)
                     auth = HttpNtlmAuth(request.credentials.get("username", " "), password)
         except Exception as e:
                 logging.info("Error occured while creating the auth object- " + str(e))
@@ -54,111 +91,117 @@
                         resp = requests.post(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
                             auth=auth,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     else:
                         
                         resp = requests.post(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
+                        print(request.body)
+                        print(resp.text)
+                        print("posttttttttttttttttttttttttttttttttttttttttt")
                     end_time = datetime.now()
                 elif str.upper(request.method) == "GET":
                     start_time = datetime.now()
                     if request.auth.upper() == "PASSWORD": 
                         resp = requests.get(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             verify=request.SSLVerify,
                             auth=auth,
-                            timeout=request.timeout // 1000,
+                            timeout=request.timeout,
                         )
                     else:
                         resp = requests.get(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000,
+                            timeout=request.timeout,
                         )
                     end_time = datetime.now()
                 elif str.upper(request.method) == "PUT":
                     start_time = datetime.now()
                     if request.auth.upper() == "PASSWORD": 
                         resp = requests.put(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             auth=auth,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     else:
                         resp = requests.put(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
+                        print(request.body)
+                        print(resp.text)
+                        print("putttttttttttttttttttttt________________________")
                     end_time = datetime.now()
                 elif str.upper(request.method) == "PATCH":
                     start_time = datetime.now()
                     if request.auth.upper() == "PASSWORD": 
                         resp = requests.patch(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
                             auth=auth,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     else:
                         resp = requests.patch(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     end_time = datetime.now()
                 elif str.upper(request.method) == "DELETE":
                     start_time = datetime.now()
                     if request.auth.upper() == "PASSWORD":
                         resp = requests.delete(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
                             auth=auth,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     else:
                         resp = requests.delete(
                             request.api,
                             headers=request.headers,
                             files=request.file,
                             data=request.body,
                             verify=request.SSLVerify,
-                            timeout=request.timeout // 1000
+                            timeout=request.timeout
                         )
                     end_time = datetime.now()
                 else:
                     raise Exception("invalid method")
 
                 obj.status_code = resp.status_code
                 obj.response_body = resp.text
```

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.70b3/gempyp/pyprest/compareFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.70b3/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.70b3/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.70b3/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.70b3/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/postVariables.py` & `gempyp-1.0.70b3/gempyp/pyprest/postVariables.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,39 +37,39 @@
                     # find suite variables
                     if "SUITE." in key.upper():
                         scope = "suite"
                         key = key.replace(".", "_")     
                     if "SUITE." in str(each_item[0].strip(" ")):
                         key = "SUITE_" + each_item[0].strip(" ").strip("set $[#SUITE.").strip("]").upper()
                         
-                        self.pyprest_obj.variables["suite"][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1])
+                        self.pyprest_obj.variables["suite"][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1].strip())
         
 
                     
                     # check for postdefined functions and response variables
                     if "$[#" in each_item[1].strip(" "):    
                         # check for predefined function
-                        self.pyprest_obj.variables[scope][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1])
+                        self.pyprest_obj.variables[scope][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1].strip())
                         
                         # if not found in predefined functions, check in response
-                        response_key = each_item[1].strip("$[#").strip("]")
+                        response_key = each_item[1].strip().strip("$[#").strip("]")
                         # find key in response  
                         # call keycheck
                         response_key_partition = response_key.split(".")
                         response_json = utils.formatRespBody(self.pyprest_obj.res_obj.response_body)
                         if self.isLegacyPresent and 'legacy' in response_key_partition:
                             response_json = utils.formatRespBody(self.pyprest_obj.legacy_res.response_body)    
                         result = KeyCheck(self.pyprest_obj).findKeys(response_json, deepcopy(response_key_partition), deepcopy(response_key_partition))
                         # if result is not "FOUND" then can't set value
                         if result.upper() != "FOUND":
                             self.logger.info("====== Key Not Found in response =======")
-                            self.logger.info("'" + each_item[1] + "' is not found")
+                            self.logger.info("'" + each_item[1].strip() + "' is not found")
 
                             # check predefined functions
-                            self.pyprest_obj.variables[scope][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1])
+                            self.pyprest_obj.variables[scope][key] = PreVariables(self.pyprest_obj).getFunctionValues(each_item[1].strip())
                         else:
                             new_list = utils.fetchValueOfKey(response_json, response_key_partition, result)
                             self.pyprest_obj.variables[scope][key] = new_list[response_key]
 
                     # key not found in response, checking pre variables and pre variables
                     if "$[#" in each_item[1].strip(" "):
                         var_replacement(self.pyprest_obj).variableReplacement()
```

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.70b3/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/preVariables.py` & `gempyp-1.0.70b3/gempyp/pyprest/preVariables.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
                     # find suite variables
                     if "SUITE." in key.upper():
                         scope = "suite"
                         key = key.replace(".", "_")
                     if "SUITE." in str(each_item[0].strip(" ")):
                         key = "SUITE_" + each_item[0].strip(" ").strip("set $[#SUITE.").strip("]").upper()
                         
-                        self.pyprest_obj.variables["suite"][key] = self.getFunctionValues(each_item[1])
+                        self.pyprest_obj.variables["suite"][key] = self.getFunctionValues(each_item[1].strip())
 
-                    self.pyprest_obj.variables[scope][key] = self.getFunctionValues(each_item[1])
+                    self.pyprest_obj.variables[scope][key] = self.getFunctionValues(each_item[1].strip())
 
                     
             self.pyprest_obj.logger.info(f"Setting PRE VARIABLES: -------- {str(self.pyprest_obj.variables)}")
 
     def getFunctionValues(self, var_name):
         if re.match(self.regex_func, var_name):
             functions_list = [x[0] for x in getmembers(Prefunc, isfunction)]
```

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/pypRest.py` & `gempyp-1.0.70b3/gempyp/pyprest/pypRest.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,16 @@
         
         # get body
         self.body = self.data["config_data"].get("BODY", {})
 
         # get file
         self.file = self.data["config_data"].get("REQUEST_FILE", None)
 
+        self.formData=self.data["config_data"].get("REQUEST_FILE", None)
+
         # get pre variables, not mandatory
         self.pre_variables = self.data["config_data"].get("PRE_VARIABLES", "")
 
         self.key_check = self.data["config_data"].get("KEY_CHECK", None)
 
         self.exp_status_code = self.getExpectedStatusCode("EXPECTED_STATUS_CODE") 
 
@@ -195,55 +197,59 @@
         self.post_variables = self.data["config_data"].get("POST_VARIABLES", "")
 
         self.auth_type = self.data["config_data"].get("AUTHENTICATION", "")
 
         self.username = self.data["config_data"].get("USERNAME", self.data.get("USER", None))
 
         self.password = self.data["config_data"].get("PASSWORD", None)
+        self.timeout=int(self.data["config_data"].get("TIMEOUT", 1000))
 
         #get values of mandatory keys of legacy apis
         # if self.isLegacyPresent and len(["LEGACY_API", "LEGACY_METHOD", "LEGACY_HEADERS", "LEGACY_BODY"] - self.data["config_data"].keys()) == 0:
         self.legacy_api = self.data["config_data"].get("LEGACY_API",None)
         self.legacy_method = self.data["config_data"].get("LEGACY_METHOD", "GET")
         self.legacy_headers = self.data["config_data"].get("LEGACY_HEADERS", {})
         self.legacy_body = self.data["config_data"].get("LEGACY_BODY", {})
         self.legacy_exp_status_code = self.getExpectedStatusCode("LEGACY_EXPECTED_STATUS_CODE")
         self.legacy_auth_type = self.data["config_data"].get("LEGACY_AUTHENTICATION", "")
         self.legacy_file=self.data["config_data"].get("LEGACY_REQUEST_FILE", None)
+        self.legacy_timeout=int(self.data["config_data"].get("LEGACY_TIMEOUT", 1000))
         #setting variables and variable replacement
-        print(self.variables)
-        print("###############################")
         
         PreVariables(self).preVariable()
         VarReplacement(self).variableReplacement()
         try:
             self.pollnwait=json.loads(self.pollnwait)
         except:
             pass
-        try:
-            self.legacy_body=json.loads(str(self.legacy_body))
-        except Exception as e:
-            self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
-            self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
-        try:
-            self.legacy_headers=json.loads(str(self.legacy_headers))
-        except Exception as e:
-            self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
-            self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
-        try:
-            self.body = json.loads(str(self.body))
+        self.legacy_body=json.loads(str(self.legacy_body))
+        self.legacy_headers=json.loads(str(self.legacy_headers))
+        self.body = json.loads(str(self.body))
+        self.headers=json.loads(str(self.headers))
+        # try:
+        #     self.legacy_body=json.loads(str(self.legacy_body))
+        # except Exception as e:
+        #     self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
+        #     self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
+        # try:
+        #     self.legacy_headers=json.loads(str(self.legacy_headers))
+        # except Exception as e:
+        #     self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
+        #     self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
+        # try:
+        #     self.body = json.loads(str(self.body))
             
-        except Exception as e:
-            self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
-            self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
-        try:
-            self.headers=json.loads(str(self.headers))
-        except Exception as e:
-            self.reporter.addRow("Loading Headers", f"Exception occured while parsing headers - {str(e)}Headers - " + str(self.headers), status.FAIL)
-            self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
+        # except Exception as e:
+        #     self.reporter.addRow("Loading Body", f"Exception occured while parsing body - {str(e)}Body - " + str(self.body), status.FAIL)
+        #     self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
+        # try:
+        #     self.headers=json.loads(self.headers)
+        # except Exception as e:
+        #     self.reporter.addRow("Loading Headers", f"Exception occured while parsing headers - {str(e)}Headers - " + str(self.headers), status.FAIL)
+        #     self.reporter.addMisc("REASON OF FAILURE", common.get_reason_of_failure(traceback.format_exc(), e))
 
     def file_upload(self,json_form_data): 
         files_data=[]
         json_form_data_1={}  
         for key,value in json_form_data.items():
             files_data_tuple=tuple()
             if(os.path.exists(json_form_data[key])):
@@ -265,14 +271,20 @@
         else:
             self.req_obj = api.Request()
             # create request
             self.req_obj.api = self.api
             self.req_obj.method = self.method
             self.req_obj.body = self.body
             self.req_obj.headers = self.headers
+            self.req_obj.timeout=self.timeout
+            # if(self.file is not None):
+            #     self.file=json.loads(self.file)
+            #     if(len(self.file)>0):
+            #         for item in self.file:
+            #             self.req_obj.file = self.file_upload(item)
             if(self.file is not None):
                 self.req_obj.file = self.file_upload(json.loads(self.file))
             if self.auth_type == "NTLM":
                 self.req_obj.credentials = {"username": self.username, "password": self.password}
                 self.req_obj.auth = "PASSWORD"
 
 
@@ -280,16 +292,15 @@
         # create legacy request
         if hasattr(self,'legacy_api'):
             self.legacy_req = api.Request()
             self.legacy_req.api = self.legacy_api
             self.legacy_req.method = self.legacy_method
             self.legacy_req.headers = self.legacy_headers
             self.legacy_req.body = self.legacy_body  
-            print(self.legacy_file)
-            print("##############################")
+            self.legacy_req.timeout=self.legacy_timeout
             if(self.legacy_file is not None):
                 self.legacy_req.file=self.file_upload(json.loads(self.legacy_file))
         # calling the before method after creating the request object.
         self.beforeMethod()
         self.logRequest()
         # calling variable replacement after before method
         
@@ -384,16 +395,14 @@
             self.loopList=self.parseLoop(self.loop)
             print(self.loopList)
             print("###############################")
         # self.product_type = self.data["PRODUCT_TYPE"]
 
     def logRequest(self):
         if self.legacy_req is not None and self.legacy_req.api is not None:
-            print(self.legacy_req.api)
-            print("@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@")
             self.logger.info(f"{self.legacy_req.__dict__}")
             self.logger.info(f"{self.req_obj.__dict__}")
             
 
             legacy_request_body = f"REQUEST BODY: {self.legacy_req.body}" if self.legacy_req.method.upper() != "GET" else ""
             current_request_body = f"REQUEST BODY: {self.req_obj.body}" if self.req_obj.method.upper() != "GET" else ""
```

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/reporting.py` & `gempyp-1.0.70b3/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/restEngine.py` & `gempyp-1.0.70b3/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/restObj.py` & `gempyp-1.0.70b3/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/utils.py` & `gempyp-1.0.70b3/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.70b3/gempyp/pyprest/variableReplacement.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.70b3/gempyp/reporter/reportGenerator.py`

 * *Files 14% similar despite different names*

```diff
@@ -117,43 +117,72 @@
         reportJson = json.dumps(reportJson)
         suiteReport = suiteReport.replace("DATA_1", reportJson)
         
         # if not len(testcase_data) > 0:   ##TODO
         #     return repJson, None
         ouput_file_path=""
         # if not jewel_user:
-        #     ResultFile = os.path.join(ouput_folder, "Result_{}.html".format(date))
-        #     ouput_file_path = ResultFile
-        #     with open(ResultFile, "w+") as f:
-        #         f.write(suiteReport)
+        ResultFile = os.path.join(ouput_folder, "Result_{}.html".format(date))
+        ouput_file_path = ResultFile
+        with open(ResultFile, "w+") as f:
+            f.write(suiteReport)
         # return repJson, ouput_file_path
         return repJson
     
     def makeTestcaseReport(self):
         index_path = os.path.dirname(__file__)
         index_path = os.path.join(os.path.split(index_path)[0], "testcase.html")
         with open(index_path, "r") as f:
             Result_data = f.read()
         json_data = self._toJSON()
         return json.loads(json_data)
+    
+    def createLogFile(self,folder_path,output_file,suite_log_file):
+        with open(output_file, 'a') as outfile:
+            with open(suite_log_file, 'r') as infile:
+                        # Read the contents of the file
+                    file_contents = infile.read()
+                    outfile.write(file_contents)
+                    outfile.write('\n')
+            # Iterate over all files in the folder
+            for file_name in os.listdir(folder_path):
+                if file_name.endswith('.txt'):
+                    file_path = os.path.join(folder_path, file_name)
+                    
+                    # Open each file in the folder
+                    with open(file_path, 'r') as infile:
+                        # Read the contents of the file
+                        file_contents = infile.read()
+                        
+                        # Append the contents to the output file
+                        outfile.write(file_contents)
+                        outfile.write('\n')  # Add a newline after each file (optional)
+        return output_file
+
 
-    def repSummary(self, repJson,jewel_link, unuploaded_path):
+    def repSummary(self, repJson,jewel_link, unuploaded_path,folder_path,output_file,bridgeToken,username,suite_log):
         """
         logging some information
         """
         try:
             logging.info("---------- Finalised the report --------------")
             logging.info("============== Run Summary =============")
             count_info = {key.lower(): val for key, val in repJson['suits_details']['testcase_info'].items()}
             log_str = f"Total Testcases: {str(count_info.get('total', 0))} | Passed Testcases: {str(count_info.get('pass', 0))} | Failed Testcases: {str(count_info.get('fail', 0))} | "
             status_dict = {"info": "Info", "warn": "WARN", "exe": "Exe", "err":"ERR"}
             for key, val in count_info.items():
                 if key in status_dict.keys():
                     log_str += f"{status_dict[key.lower()]} Testcases: {val} | "
             logging.info(log_str.strip(" | "))
+            output_file=self.createLogFile(folder_path,output_file,suite_log)
+            s3_log_file_url=None
+            try:
+                s3_log_file_url = create_s3_link(url=upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=bridgeToken, username=username, file=output_file,tag="public")[0]["Url"])
+            except Exception as e:
+                logging.warn(str(e))
 
             if unuploaded_path != None:
                 logging.info(f"Unuploaded Data File Path:{unuploaded_path}")
             #  we will check if output report is None, then display report not created
             if len(jewel_link)>0:
 #                 s3_report_file_url= create_s3_link(url=upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=bridgetoken, username=username, file=output_file_path.split('/')[-1],tag="public")[0]["Url"]) 
                 logging.info('Report at Jewel: {link}'.format(link = jewel_link))
```

### Comparing `gempyp-1.0.70b1/gempyp/sdk/executor.py` & `gempyp-1.0.70b3/gempyp/sdk/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,56 +16,54 @@
 import tempfile
 import subprocess
 import sys
 import os
 import pandas as pd
 from gempyp.libs.enums.status import status
 from gempyp.libs.common import *
+import glob
 from gempyp.engine.engine import Engine
 
 
 class Executor(TestcaseReporter):
     def __init__(self, **kwargs):
         self.method = kwargs.get("tc_name", self.getMethodName())
         self.log_file = tempfile.gettempdir() + "\logs.log"
         # os.makedirs("testcase_log_folder")
-        sys.stdout = sys.stderr =  open(self.log_file, 'w')
+        # sys.stdout = sys.stderr =  open(self.log_file, 'w')
         logging.basicConfig(filename="logs.log", filemode='w', format='%(name)s - %(levelname)s - %(message)s',level=logging.DEBUG)
         # custom_logger = my_custom_logger("logs.log")
-        logging.info("inside constructor here--------------------")
+        logging.info("--------inside constructor here-----------")
         logging.info(f"-------Executing testcase - {self.getMethodName()}---------")
         self.data = self.getTestcaseData()
         self.reporter = TestcaseReporter(self.data["PROJECT_NAME"], self.data["NAME"])
-       
         
-
         path = __file__
         path = path.rsplit(os.sep, 1)[0]
         self.DATA = TestData()
         # make suite details and upload it
         self.makeSuiteDetails()
         runBaseUrls(self.jewel_user,self.data["ENTER_POINT"],self.data["JEWEL_USER"],self.data["JEWEL_BRIDGE_TOKEN"])
         if not os.getenv("PID"):
             self.makeOutputFolder()
             os.environ["PID"] = str(os.getpid())
-            subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True)
+            subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True, stdout=subprocess.PIPE)
             try:
-                logging.info(f"---------------S_RUN_ID-------------{self.s_run_id}")
+                logging.info(f"S_RUN_ID : {self.s_run_id}")
                 dataUpload.sendSuiteData((self.DATA.toSuiteJson()), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"]) # check with deamon, should insert only once
                   # logging not working
             except Exception as e:
                 print(f"Exception occured - {e}")
                 pass
 
     def __del__(self):
-        self.final()
+            self.final()
 
     def final(self):       
         output = []
-        
         # destructor of reporter object called
         
         self.reporter.finalizeReport()
         
         # create testcase reporter json
         self.reporter.json_data = self.reporter.template_data.makeTestcaseReport()
         # serializing data, adding suite data
@@ -79,19 +77,19 @@
         for i in output:
             i["testcase_dict"]["steps"] = i["json_data"]["steps"]
             dict_ = {}
             dict_["testcases"] = {}
             dict_["REPORT_LOCATION"] = os.getenv("REPORT_LOCATION")
             dict_["misc_data"] = {}
             tmp_dir = os.path.join(tempfile.gettempdir(), self.s_run_id + ".txt")
-            
 
             self.DATA.testcase_details = self.DATA.testcase_details.append(
                 i["testcase_dict"], ignore_index=True
             )
+            print("\n\n ------------------------- {} \n\n----------------------".format(output))    
             # self.DATA.testcaseDetails = pd.concat([self.DATA.testcaseDetails, pd.DataFrame(list(i["testcase_dict"].items()))])
             self.updateTestcaseMiscData(i["misc"], tc_run_id=i["testcase_dict"].get("tc_run_id"))
             suite_data = self.DATA.getJSONData()
             if isinstance(suite_data, str):
                 suite_data = json.loads(suite_data)
             if isinstance(self.DATA.toSuiteJson(), str):
                 suite_temp = json.loads(self.DATA.toSuiteJson())
@@ -104,38 +102,41 @@
                 with open(tmp_dir, "r+") as f:
                     data = f.read()
                     data = json.loads(data)
                     data[self.s_run_id] = self.updateSuiteData(suite_data, data[self.s_run_id])
                     data["testcases"][i["testcase_dict"].get("tc_run_id")] = i["json_data"]
                     f.seek(0)
                     f.write(json.dumps(data))
-            logging.info("---------------TC_RUN_ID-----------------"+i["testcase_dict"]["tc_run_id"].upper())
-            dataUpload.sendTestcaseData((self.DATA.totestcaseJson(i["testcase_dict"]["tc_run_id"].upper(), self.data["S_RUN_ID"])), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"])  # instead of output, I need to pass s_run id and  tc_run_id
+            # for k in range(count):
+            updatedData=json.loads(self.DATA.totestcaseJson(i["testcase_dict"]["tc_run_id"].upper(), self.data["S_RUN_ID"]))
+            logging.info("TC_RUN_ID : "+i["testcase_dict"]["tc_run_id"].upper())
+            dataUpload.sendTestcaseData(json.dumps(updatedData), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"])  # instead of output, I need to pass s_run id and  tc_run_id
             path = __file__
             path = path.rsplit(os.sep, 1)[0]
-            subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True)
+            # subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True)
             # sys.stdout.close()
         
             # os.rename(self.log_file, tmp_dir.rsplit(".", 1)[0] + ".log")
 
-            
-
     def getTestcaseData(self):
         self.jewel_user=False
         config_file = configparser.ConfigParser()
-        directory_path = os.getcwd()
+        file_path = glob.glob("**/gempyp.conf", recursive=True)
+        # directory_path = os.getcwd()
 
-        if not os.path.exists(directory_path + os.sep + "gempyp.conf"):
+        # if not os.path.exists(directory_path + os.sep + "gempyp.conf"):
+        if not file_path:
             print("Config file is missing. Aborting  gempyp report......")
             sys.exit()
-        config_file.read("gempyp.conf")
+        # config_file.read("gempyp.conf")
+        config_file.read(file_path)
         data = {}
-        self.projectName = data["PROJECT_NAME"] = config_file['ReportSetting']["project_name"]
-        self.testcaseName = data["NAME"] = self.method
+        self.projectName = data["PROJECT_NAME"] =config_file['ReportSetting']["project_name"]
         self.env = data["ENVIRONMENT"] = config_file['ReportSetting'].get("environment", "PROD")
+        self.testcaseName = data["NAME"] = self.method
         data["JEWEL_USER"] = config_file['ReportSetting'].get("jewel_user", getpass.getuser())
         data["JEWEL_BRIDGE_TOKEN"] = config_file['ReportSetting'].get("jewel_bridge_token", None)
         data["REPORT_LOCATION"] = config_file['ReportSetting'].get("report_location", None)
         data["MACHINE"] = platform.node()
         data["MAIL_TO"] = config_file['ReportSetting'].get("mail_to", None)
         data["MAIL_CC"] = config_file['ReportSetting'].get("mail_cc", None)
         data["MAIL_BCC"] = config_file['ReportSetting'].get("mail_bcc", None)
@@ -198,15 +199,15 @@
             "status": status.EXE.name,
             "project_name": self.data["PROJECT_NAME"],
             "report_name": self.data["REPORT_NAME"],
             "run_type": "ON DEMAND",
             "user": self.data["JEWEL_USER"],
             "env": self.data["ENVIRONMENT"],
             "machine": self.data["MACHINE"],
-            "initiated_by": self.data["JEWEL_USER"],
+            # "initiated_by": self.data["JEWEL_USER"],
             "run_mode": run_mode,
             "os": platform.system().upper(),
             "meta_data": [],
             "testcase_info": None,
             "expected_testcases":1,
             "framework_name": "GEMPYP",
         }
@@ -291,8 +292,13 @@
                 del statusDict[key]
             else:
                 count += statusDict[key]
         statusDict["total"] = count
         current_data["suits_details"]["expected_testcases"]=count
         current_data["suits_details"]["testcase_info"] = statusDict
 
-        return current_data
+        return current_data
+    
+    def delete_env_variables_with_string(string):
+        for key in os.environ.keys():
+            if string in key:
+                del os.environ[key]
```

### Comparing `gempyp-1.0.70b1/gempyp/sdk/worker.py` & `gempyp-1.0.70b3/gempyp/sdk/worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import configparser
 import psutil
 import sys
 from gempyp.engine import dataUpload
 from gempyp.reporter.reportGenerator import TemplateData
 import logging
 from gempyp.libs.common import *
+import glob
 
 
 def pid_running(pid):
     if not pid:
         return False
     if psutil.pid_exists(int(pid)):
         return True
@@ -19,30 +20,34 @@
         return False
 
 def create_report(data, s_run_id):
      # read bridgetoken
     try:
         jewel=False
         config_file = configparser.ConfigParser()
-        config_file.read("gempyp.conf")
+        file_path = glob.glob("**/gempyp.conf", recursive=True)
+        # config_file.read("gempyp.conf")
+        config_file.read(file_path)
         bridgetoken = config_file['ReportSetting'].get("jewel_bridge_token", None)
         username=config_file['ReportSetting'].get("jewel_user", None)
         if username and bridgetoken:
             jewel=True
     except Exception as e:
         bridgetoken = None
     data = json.loads(data)
+    logging.info("-------------------{}-----------------".format(data))
     runBaseUrls(jewel,config_file['ReportSetting'].get("enter_point", None),username,bridgetoken)
     json_data = data[s_run_id]
     testcaseData = data["testcases"]
     output_folder = data["REPORT_LOCATION"]
     repJson = TemplateData().makeSuiteReport(json.dumps(json_data), testcaseData,output_folder,jewel)
     suite_data = json_data["suits_details"]
     suite_data["misc_data"] = data["misc_data"]
-    username = suite_data["initiated_by"]
+    username = suite_data["user"]
+    # jewel_link=f"{data['urls']['jewel-url']}/#/autolytics/execution-report?s_run_id={s_run_id}"
     del suite_data["testcase_details"]
     del suite_data["testcase_info"]
     dataUpload.sendSuiteData(json.dumps(suite_data), bridgetoken, username, mode="PUT")
     return output_folder
 
 
 if __name__ == "__main__":
@@ -54,12 +59,16 @@
                 file_path = os.path.join(tempfile.gettempdir(), s_run_id + ".txt")
                 if os.path.exists(file_path):
                     with open(file_path, "r+") as f:
                         data = str(f.read())
                         output_file_path = create_report(data, s_run_id)
                         # where to get this json data from
                         current_pid = os.getpid()
+                        jewelLink = DefaultSettings.getUrls('jewel-url')
+                        if jewelLink is not None:
+                            jewel_link = f'{jewelLink}/#/autolytics/execution-report?s_run_id={s_run_id}&p_id={DefaultSettings.project_id}'
+                            logging.info(f"Jewel link of gempyp report - {jewel_link}")
                         logging.info(f"Find Gempyp logs at - {s_run_id + '.log'}")
                         logging.info(f"Find Gempyp Report at - {output_file_path}")
                         # os.rename("logs.log",f"{s_run_id}.log")
                         os.kill(current_pid, 19)
-                        sys.exit()
+                        sys.exit()
```

### Comparing `gempyp-1.0.70b1/gempyp/testcase.html` & `gempyp-1.0.70b3/gempyp/testcase.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/pyproject.toml` & `gempyp-1.0.70b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.70b1"
+version = "1.0.70b3"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
```

### Comparing `gempyp-1.0.70b1/README.md` & `gempyp-1.0.70b3/README.md`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b1/PKG-INFO` & `gempyp-1.0.70b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempyp
-Version: 1.0.70b1
+Version: 1.0.70b3
 Summary: An ecosystem of libraries useful for software development
 Home-page: https://github.com/Gemini-Solutions/gempyp
 License: MIT
 Author: Gemini Solutions-QA
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gempyp Version: 1.0.70b1 Summary: An ecosystem of
+Metadata-Version: 2.1 Name: gempyp Version: 1.0.70b3 Summary: An ecosystem of
 libraries useful for software development Home-page: https://github.com/Gemini-
 Solutions/gempyp License: MIT Author: Gemini Solutions-QA Requires-Python:
 >=3.6.8,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

