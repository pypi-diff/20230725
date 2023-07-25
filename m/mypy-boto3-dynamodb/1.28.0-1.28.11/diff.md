# Comparing `tmp/mypy-boto3-dynamodb-1.28.0.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.0.tar` & `mypy-boto3-dynamodb-1.28.11.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   152926 2023-07-06 20:38:33.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152773 2023-07-06 20:38:31.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.853034 mypy-boto3-dynamodb-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   152329 2023-07-25 19:47:09.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152192 2023-07-25 19:47:07.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.853034 mypy-boto3-dynamodb-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.0/LICENSE` & `mypy-boto3-dynamodb-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/PKG-INFO` & `mypy-boto3-dynamodb-1.28.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.0
-Summary: Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,30 +481,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -524,174 +528,199 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -709,82 +738,83 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.0/README.md` & `mypy-boto3-dynamodb-1.28.11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -449,30 +449,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -492,174 +496,199 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -677,82 +706,83 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.28.11\nVersion:         1.28.11\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.11")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AttributeActionType",
     "BackupStatusType",
     "BackupTypeFilterType",
     "BackupTypeType",
     "BatchStatementErrorCodeEnumType",
     "BillingModeType",
@@ -67,15 +66,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AttributeActionType = Literal["ADD", "DELETE", "PUT"]
 BackupStatusType = Literal["AVAILABLE", "CREATING", "DELETED"]
 BackupTypeFilterType = Literal["ALL", "AWS_BACKUP", "SYSTEM", "USER"]
 BackupTypeType = Literal["AWS_BACKUP", "SYSTEM", "USER"]
 BatchStatementErrorCodeEnumType = Literal[
     "AccessDenied",
     "ConditionalCheckFailed",
@@ -371,14 +369,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AttributeActionType",
     "BackupStatusType",
     "BackupTypeFilterType",
     "BackupTypeType",
     "BatchStatementErrorCodeEnumType",
     "BillingModeType",
@@ -66,14 +67,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AttributeActionType = Literal["ADD", "DELETE", "PUT"]
 BackupStatusType = Literal["AVAILABLE", "CREATING", "DELETED"]
 BackupTypeFilterType = Literal["ALL", "AWS_BACKUP", "SYSTEM", "USER"]
 BackupTypeType = Literal["AWS_BACKUP", "SYSTEM", "USER"]
 BatchStatementErrorCodeEnumType = Literal[
     "AccessDenied",
     "ConditionalCheckFailed",
@@ -369,14 +371,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,76 +53,70 @@
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
     "ScanPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListBackupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
-
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
-
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
-
 class QueryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
     """
 
     def paginate(
@@ -157,22 +151,21 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
-
 class ScanPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
     """
 
     def paginate(
@@ -206,13 +199,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,70 +53,76 @@
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
     "ScanPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListBackupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
+
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
+
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
+
 class QueryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
     """
 
     def paginate(
@@ -151,21 +157,22 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
+
 class ScanPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
     """
 
     def paginate(
@@ -199,13 +206,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,50 +35,51 @@
     ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeValueUpdateTableTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     ConditionTableTypeDef,
     DeleteItemOutputTableTypeDef,
     DeleteTableOutputTableTypeDef,
     ExpectedAttributeValueTableTypeDef,
     GetItemOutputTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableTypeDef,
+    KeySchemaElementTableOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     ProvisionedThroughputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     ScanOutputTableTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSESpecificationServiceResourceTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationServiceResourceTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
@@ -142,36 +143,36 @@
 
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: List[AttributeDefinitionTableTypeDef]
+    attribute_definitions: List[AttributeDefinitionTableOutputTypeDef]
     table_name: str
-    key_schema: List[KeySchemaElementTableTypeDef]
+    key_schema: List[KeySchemaElementTableOutputTypeDef]
     table_status: TableStatusType
     creation_date_time: datetime
-    provisioned_throughput: ProvisionedThroughputDescriptionResponseMetadataTypeDef
+    provisioned_throughput: ProvisionedThroughputDescriptionTableResponseMetadataTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
-    billing_mode_summary: BillingModeSummaryResponseMetadataTypeDef
+    billing_mode_summary: BillingModeSummaryTableResponseMetadataTypeDef
     local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
     global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
-    stream_specification: StreamSpecificationResponseMetadataTypeDef
+    stream_specification: StreamSpecificationTableResponseMetadataTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
     replicas: List[ReplicaDescriptionTableTypeDef]
-    restore_summary: RestoreSummaryResponseMetadataTypeDef
-    sse_description: SSEDescriptionResponseMetadataTypeDef
-    archival_summary: ArchivalSummaryResponseMetadataTypeDef
-    table_class_summary: TableClassSummaryResponseMetadataTypeDef
+    restore_summary: RestoreSummaryTableResponseMetadataTypeDef
+    sse_description: SSEDescriptionTableResponseMetadataTypeDef
+    archival_summary: ArchivalSummaryTableResponseMetadataTypeDef
+    table_class_summary: TableClassSummaryTableResponseMetadataTypeDef
     deletion_protection_enabled: bool
     name: str
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -35,50 +35,51 @@
     ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeValueUpdateTableTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     ConditionTableTypeDef,
     DeleteItemOutputTableTypeDef,
     DeleteTableOutputTableTypeDef,
     ExpectedAttributeValueTableTypeDef,
     GetItemOutputTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableTypeDef,
+    KeySchemaElementTableOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     ProvisionedThroughputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     ScanOutputTableTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSESpecificationServiceResourceTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationServiceResourceTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
@@ -135,36 +136,36 @@
 
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: List[AttributeDefinitionTableTypeDef]
+    attribute_definitions: List[AttributeDefinitionTableOutputTypeDef]
     table_name: str
-    key_schema: List[KeySchemaElementTableTypeDef]
+    key_schema: List[KeySchemaElementTableOutputTypeDef]
     table_status: TableStatusType
     creation_date_time: datetime
-    provisioned_throughput: ProvisionedThroughputDescriptionResponseMetadataTypeDef
+    provisioned_throughput: ProvisionedThroughputDescriptionTableResponseMetadataTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
-    billing_mode_summary: BillingModeSummaryResponseMetadataTypeDef
+    billing_mode_summary: BillingModeSummaryTableResponseMetadataTypeDef
     local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
     global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
-    stream_specification: StreamSpecificationResponseMetadataTypeDef
+    stream_specification: StreamSpecificationTableResponseMetadataTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
     replicas: List[ReplicaDescriptionTableTypeDef]
-    restore_summary: RestoreSummaryResponseMetadataTypeDef
-    sse_description: SSEDescriptionResponseMetadataTypeDef
-    archival_summary: ArchivalSummaryResponseMetadataTypeDef
-    table_class_summary: TableClassSummaryResponseMetadataTypeDef
+    restore_summary: RestoreSummaryTableResponseMetadataTypeDef
+    sse_description: SSEDescriptionTableResponseMetadataTypeDef
+    archival_summary: ArchivalSummaryTableResponseMetadataTypeDef
+    table_class_summary: TableClassSummaryTableResponseMetadataTypeDef
     deletion_protection_enabled: bool
     name: str
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ArchivalSummaryResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -58,32 +58,35 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "ArchivalSummaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
+    "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
+    "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
+    "AttributeValueServiceResourceTypeDef",
+    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -103,174 +106,199 @@
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "KeySchemaElementServiceResourceTypeDef",
     "ProvisionedThroughputServiceResourceTypeDef",
     "SSESpecificationServiceResourceTypeDef",
     "StreamSpecificationServiceResourceTypeDef",
     "TagServiceResourceTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "ExpectedAttributeValueTableTypeDef",
     "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
+    "DeleteRequestServiceResourceOutputTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
+    "KeySchemaElementTableOutputTypeDef",
+    "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
+    "KeySchemaElementOutputTypeDef",
+    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
+    "ReplicaOutputTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
+    "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
+    "StreamSpecificationOutputTypeDef",
+    "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
+    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
+    "DeleteRequestOutputTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
+    "KeysAndAttributesOutputTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
+    "PutRequestOutputTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexTypeDef",
-    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "GlobalTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "ReplicaGlobalSecondaryIndexTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
+    "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
+    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "UpdateTimeToLiveInputRequestTypeDef",
     "BatchStatementResponseTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
     "BatchGetItemInputRequestTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestOutputTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
@@ -288,118 +316,134 @@
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
     "GlobalSecondaryIndexUpdateTableTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "CreateTableInputRequestTypeDef",
     "RestoreTableFromBackupInputRequestTypeDef",
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "ListGlobalTablesOutputTypeDef",
-    "ReplicaDescriptionTableTypeDef",
     "CreateReplicationGroupMemberActionTableTypeDef",
     "UpdateReplicationGroupMemberActionTableTypeDef",
-    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "TableCreationParametersOutputTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
     "ListImportsOutputTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "ReplicaDescriptionTypeDef",
+    "ReplicaDescriptionTableTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
-    "TableDescriptionTableTypeDef",
     "ReplicationGroupUpdateTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "BackupDescriptionTypeDef",
+    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "ReplicationGroupUpdateTypeDef",
+    "TableDescriptionTableTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "UpdateTableInputRequestTypeDef",
     "DeleteBackupOutputTypeDef",
     "DescribeBackupOutputTypeDef",
     "DescribeImportOutputTypeDef",
     "ImportTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "UpdateTableInputRequestTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
+)
+
+AttributeDefinitionOutputTypeDef = TypedDict(
+    "AttributeDefinitionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
 )
 
 AttributeDefinitionServiceResourceTypeDef = TypedDict(
     "AttributeDefinitionServiceResourceTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeDefinitionTableOutputTypeDef = TypedDict(
+    "AttributeDefinitionTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
+)
+
 AttributeDefinitionTableTypeDef = TypedDict(
     "AttributeDefinitionTableTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
@@ -408,14 +452,46 @@
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeValueServiceResourceTypeDef = TypedDict(
+    "AttributeValueServiceResourceTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
+AttributeValueTableTypeDef = TypedDict(
+    "AttributeValueTableTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -449,38 +525,24 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
+        "TargetValue": float,
     },
-    total=False,
 )
 
-
-class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
-    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-):
-    pass
-
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -489,61 +551,47 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
-
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-
-_RequiredBackupDetailsTypeDef = TypedDict(
-    "_RequiredBackupDetailsTypeDef",
+BackupDetailsTypeDef = TypedDict(
+    "BackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
+        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-    },
-)
-_OptionalBackupDetailsTypeDef = TypedDict(
-    "_OptionalBackupDetailsTypeDef",
-    {
-        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
-    total=False,
 )
 
-
-class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
-    pass
-
-
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -552,15 +600,14 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -592,104 +639,80 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-
-ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
-    "ItemCollectionMetricsServiceResourceTypeDef",
+KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "SizeEstimateRangeGB": List[float],
+        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
     },
-    total=False,
 )
 
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
+ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
+    "ItemCollectionMetricsServiceResourceTypeDef",
     {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
+        "SizeEstimateRangeGB": List[float],
     },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -715,37 +738,33 @@
                 None,
             ]
         ],
     },
     total=False,
 )
 
-
 class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
-
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
-    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
-    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -760,15 +779,15 @@
     },
 )
 
 ProjectionTableTypeDef = TypedDict(
     "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
+        "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTableTypeDef = TypedDict(
     "ProvisionedThroughputTableTypeDef",
     {
@@ -853,21 +872,19 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -908,35 +925,41 @@
     "_OptionalStreamSpecificationServiceResourceTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationServiceResourceTypeDef(
     _RequiredStreamSpecificationServiceResourceTypeDef,
     _OptionalStreamSpecificationServiceResourceTypeDef,
 ):
     pass
 
-
 TagServiceResourceTypeDef = TypedDict(
     "TagServiceResourceTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderList": List[str],
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": List[str],
+        "HeaderList": Sequence[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -1000,36 +1023,17 @@
     },
     total=False,
 )
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1045,14 +1049,21 @@
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
+DeleteRequestServiceResourceOutputTypeDef = TypedDict(
+    "DeleteRequestServiceResourceOutputTypeDef",
+    {
+        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
+    },
+)
+
 DeleteRequestServiceResourceTypeDef = TypedDict(
     "DeleteRequestServiceResourceTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1105,29 +1116,26 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1160,15 +1168,14 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
-    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1198,26 +1205,14 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
-    total=False,
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1248,31 +1243,22 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1288,22 +1274,20 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
-
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1332,54 +1316,106 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
+KeySchemaElementTableOutputTypeDef = TypedDict(
+    "KeySchemaElementTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionTableOutputTypeDef = TypedDict(
+    "ProjectionTableOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
+)
 
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+KeySchemaElementOutputTypeDef = TypedDict(
+    "KeySchemaElementOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionOutputTypeDef = TypedDict(
+    "ProjectionOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+    },
 )
 
 ProjectionServiceResourceTypeDef = TypedDict(
     "ProjectionServiceResourceTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
+ReplicaOutputTypeDef = TypedDict(
+    "ReplicaOutputTypeDef",
+    {
+        "RegionName": str,
+    },
+)
+
+S3BucketSourceOutputTypeDef = TypedDict(
+    "S3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+)
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1387,45 +1423,31 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
-
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1475,126 +1497,83 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
-
 TagTableTypeDef = TypedDict(
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideOutputTypeDef",
     {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+    },
+)
+
+PutRequestServiceResourceOutputTypeDef = TypedDict(
+    "PutRequestServiceResourceOutputTypeDef",
+    {
+        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
 )
 
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
@@ -1621,141 +1600,96 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
+RestoreSummaryTableTypeDef = TypedDict(
+    "RestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRestoreSummaryTableTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTableTypeDef",
-    {
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-    },
-)
-_OptionalRestoreSummaryTableTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTableTypeDef",
+RestoreSummaryTypeDef = TypedDict(
+    "RestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-    },
-    total=False,
-)
-
-
-class RestoreSummaryTableTypeDef(
-    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
-):
-    pass
-
-
-_RequiredRestoreSummaryTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTypeDef",
-    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-_OptionalRestoreSummaryTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-    },
-    total=False,
-)
-
-
-class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
-    pass
-
 
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
+SSEDescriptionTableTypeDef = TypedDict(
+    "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
+SSEDescriptionTypeDef = TypedDict(
+    "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-    total=False,
 )
 
-SSEDescriptionTypeDef = TypedDict(
-    "SSEDescriptionTypeDef",
+SSESpecificationOutputTypeDef = TypedDict(
+    "SSESpecificationOutputTypeDef",
     {
-        "Status": SSEStatusType,
+        "Enabled": bool,
         "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
+        "KMSMasterKeyId": str,
     },
-    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
+StreamSpecificationOutputTypeDef = TypedDict(
+    "StreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+    },
+)
+
+StreamSpecificationTableOutputTypeDef = TypedDict(
+    "StreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1765,35 +1699,32 @@
     "_OptionalStreamSpecificationTableTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
-
 TableBatchWriterRequestTypeDef = TypedDict(
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
+TimeToLiveSpecificationOutputTypeDef = TypedDict(
+    "TimeToLiveSpecificationOutputTypeDef",
     {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Enabled": bool,
+        "AttributeName": str,
     },
 )
 
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
@@ -1820,29 +1751,144 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    {
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
+    {
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1872,15 +1918,14 @@
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
@@ -1911,21 +1956,19 @@
         ],
         "ConsistentRead": bool,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
-
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -1978,19 +2021,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
-
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
@@ -2017,18 +2058,23 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
-
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
+DeleteRequestOutputTypeDef = TypedDict(
+    "DeleteRequestOutputTypeDef",
+    {
+        "Key": Dict[str, AttributeValueTypeDef],
+    },
+)
 
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
@@ -2110,19 +2156,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2154,21 +2198,19 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
-
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
             Union[
                 bytes,
@@ -2250,21 +2292,19 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2294,34 +2334,41 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
-
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
+)
+
+KeysAndAttributesOutputTypeDef = TypedDict(
+    "KeysAndAttributesOutputTypeDef",
+    {
+        "Keys": List[Dict[str, AttributeValueTypeDef]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
 )
 
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -2356,21 +2403,19 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
-
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
@@ -2398,20 +2443,25 @@
             ]
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
+PutRequestOutputTypeDef = TypedDict(
+    "PutRequestOutputTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+)
 
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
@@ -2493,19 +2543,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
-
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2559,28 +2607,25 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
-
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
-    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2591,44 +2636,42 @@
     "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-
 class AutoScalingPolicyUpdateTypeDef(
     _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
-
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2638,117 +2681,59 @@
     "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
-
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-    total=False,
 )
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2800,66 +2785,14 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2910,55 +2843,29 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_RequiredContinuousBackupsDescriptionTypeDef",
+ContinuousBackupsDescriptionTypeDef = TypedDict(
+    "ContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
-    },
-)
-_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_OptionalContinuousBackupsDescriptionTypeDef",
-    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
-    total=False,
 )
 
-
-class ContinuousBackupsDescriptionTypeDef(
-    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
-):
-    pass
-
-
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTableTypeDef],
@@ -2969,53 +2876,28 @@
     "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
     total=False,
 )
 
-
 class CreateGlobalSecondaryIndexActionTableTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
 ):
     pass
 
-
 UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-    },
-    total=False,
-)
-
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -3033,33 +2915,20 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
-
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -3068,49 +2937,19 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-)
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
-    {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
-    },
-    total=False,
-)
-
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
-
-
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
@@ -3119,101 +2958,68 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
-    {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaTypeDef],
-    },
-    total=False,
-)
-
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexTableTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
     _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
 ):
     pass
 
-
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+InputFormatOptionsOutputTypeDef = TypedDict(
+    "InputFormatOptionsOutputTypeDef",
+    {
+        "Csv": CsvOptionsOutputTypeDef,
+    },
+)
+
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -3272,21 +3078,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
-
 _RequiredPutItemInputTablePutItemTypeDef = TypedDict(
     "_RequiredPutItemInputTablePutItemTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -3337,21 +3141,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
     pass
 
-
 _RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
     "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -3404,21 +3206,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
     pass
 
-
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3429,48 +3229,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3480,91 +3280,153 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
-
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+)
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+    },
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+GlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "GlobalSecondaryIndexOutputTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+SourceTableDetailsTypeDef = TypedDict(
+    "SourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
 )
 
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
@@ -3575,96 +3437,274 @@
     "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
     },
     total=False,
 )
 
-
 class GlobalSecondaryIndexServiceResourceTypeDef(
     _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
     _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
 ):
     pass
 
-
 LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "LocalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
 )
 
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
+    {
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaOutputTypeDef],
+    },
+)
+
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
 
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+    },
+)
+
+ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+    },
+)
+
+WriteRequestServiceResourceOutputTypeDef = TypedDict(
+    "WriteRequestServiceResourceOutputTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceOutputTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+    },
+)
+
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
     },
     total=False,
 )
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
+        "TableName": str,
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
@@ -3673,22 +3713,20 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -3752,21 +3790,19 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
-
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
-
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -3829,19 +3865,17 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
-
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3899,21 +3933,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[
             str,
             Union[
@@ -3971,21 +4003,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -4045,21 +4075,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
-
 TransactGetItemTypeDef = TypedDict(
     "TransactGetItemTypeDef",
     {
         "Get": GetTypeDef,
     },
 )
 
@@ -4073,21 +4101,19 @@
     "_OptionalBatchGetItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchGetItemInputRequestTypeDef(
     _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -4095,20 +4121,26 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
+    {
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
+    },
+)
 
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
@@ -4131,15 +4163,14 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
-    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4149,404 +4180,221 @@
     },
     total=False,
 )
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Responses": Dict[
-            str,
-            List[
-                Dict[
-                    str,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ]
-            ],
-        ],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
-        "Item": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
     },
     total=False,
 )
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateTableInputRequestTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4563,21 +4411,19 @@
         "Tags": Sequence[TagTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-
 class CreateTableInputRequestTypeDef(
     _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
 ):
     pass
 
-
 _RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
     },
 )
@@ -4589,22 +4435,20 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
-
 class RestoreTableFromBackupInputRequestTypeDef(
     _RequiredRestoreTableFromBackupInputRequestTypeDef,
     _OptionalRestoreTableFromBackupInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
     },
 )
 _OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
@@ -4619,83 +4463,54 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
-
 class RestoreTableToPointInTimeInputRequestTypeDef(
     _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
     _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
-
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
-
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
-    {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4705,22 +4520,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMemberActionTableTypeDef(
     _RequiredCreateReplicationGroupMemberActionTableTypeDef,
     _OptionalCreateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-
 _RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4730,38 +4543,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class UpdateReplicationGroupMemberActionTableTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4771,22 +4566,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4796,30 +4589,52 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
+    {
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+)
+
+TableCreationParametersOutputTypeDef = TypedDict(
+    "TableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "SSESpecification": SSESpecificationOutputTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+)
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4836,28 +4651,75 @@
         "Tags": Sequence[TagServiceResourceTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-
 class CreateTableInputServiceResourceCreateTableTypeDef(
     _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
     _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
 ):
     pass
 
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
+    {
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+    },
+)
+
+ReplicaDescriptionTableTypeDef = TypedDict(
+    "ReplicaDescriptionTableTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+    },
+)
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4868,38 +4730,26 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-
 class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
     _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
 ):
     pass
 
-
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4909,20 +4759,28 @@
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
@@ -4931,31 +4789,19 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-
 class BatchWriteItemInputRequestTypeDef(
     _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
 _OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
@@ -4964,58 +4810,41 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
-
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
-    },
-)
-_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
-    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-
-class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-):
-    pass
-
-
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5032,22 +4861,20 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5064,58 +4891,20 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
-
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
     },
@@ -5126,155 +4915,170 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
-
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
-
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
-    {
-        "AttributeDefinitions": List[AttributeDefinitionTableTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
 ReplicationGroupUpdateTableTypeDef = TypedDict(
     "ReplicationGroupUpdateTableTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTableTypeDef,
         "Update": UpdateReplicationGroupMemberActionTableTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
     },
     total=False,
 )
 
+ReplicationGroupUpdateTypeDef = TypedDict(
+    "ReplicationGroupUpdateTypeDef",
+    {
+        "Create": CreateReplicationGroupMemberActionTypeDef,
+        "Update": UpdateReplicationGroupMemberActionTypeDef,
+        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+    },
+    total=False,
+)
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+)
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
+    {
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersOutputTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
+    },
+)
+
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
-    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableStatus": TableStatusType,
         "CreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "TableSizeBytes": int,
         "ItemCount": int,
         "TableArn": str,
         "TableId": str,
         "BillingModeSummary": BillingModeSummaryTypeDef,
         "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
+        "StreamSpecification": StreamSpecificationOutputTypeDef,
         "LatestStreamLabel": str,
         "LatestStreamArn": str,
         "GlobalTableVersion": str,
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
-ReplicationGroupUpdateTypeDef = TypedDict(
-    "ReplicationGroupUpdateTypeDef",
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTableTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTableTypeDef],
+        "RestoreSummary": RestoreSummaryTableTypeDef,
+        "SSEDescription": SSEDescriptionTableTypeDef,
+        "ArchivalSummary": ArchivalSummaryTableTypeDef,
+        "TableClassSummary": TableClassSummaryTableTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
-    total=False,
 )
 
-_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaSettingsDescriptionTypeDef",
+ReplicaSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaSettingsDescriptionTypeDef",
-    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
-    total=False,
 )
 
-
-class ReplicaSettingsDescriptionTypeDef(
-    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
-):
-    pass
-
-
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5284,21 +5088,19 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
-
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -5310,203 +5112,198 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
-
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableTypeDef,
+        "SSESpecification": SSESpecificationTableTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
-    {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
-    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5518,22 +5315,20 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -5548,30 +5343,28 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
-
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ArchivalSummaryResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -58,31 +58,36 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "ArchivalSummaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
+    "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
+    "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
+    "AttributeValueServiceResourceTypeDef",
+    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -102,174 +107,199 @@
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "KeySchemaElementServiceResourceTypeDef",
     "ProvisionedThroughputServiceResourceTypeDef",
     "SSESpecificationServiceResourceTypeDef",
     "StreamSpecificationServiceResourceTypeDef",
     "TagServiceResourceTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "ExpectedAttributeValueTableTypeDef",
     "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
+    "DeleteRequestServiceResourceOutputTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
+    "KeySchemaElementTableOutputTypeDef",
+    "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
+    "KeySchemaElementOutputTypeDef",
+    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
+    "ReplicaOutputTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
+    "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
+    "StreamSpecificationOutputTypeDef",
+    "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
+    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
+    "DeleteRequestOutputTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
+    "KeysAndAttributesOutputTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
+    "PutRequestOutputTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexTypeDef",
-    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "GlobalTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "ReplicaGlobalSecondaryIndexTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
+    "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
+    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "UpdateTimeToLiveInputRequestTypeDef",
     "BatchStatementResponseTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
     "BatchGetItemInputRequestTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestOutputTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
@@ -287,118 +317,134 @@
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
     "GlobalSecondaryIndexUpdateTableTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "CreateTableInputRequestTypeDef",
     "RestoreTableFromBackupInputRequestTypeDef",
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "ListGlobalTablesOutputTypeDef",
-    "ReplicaDescriptionTableTypeDef",
     "CreateReplicationGroupMemberActionTableTypeDef",
     "UpdateReplicationGroupMemberActionTableTypeDef",
-    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "TableCreationParametersOutputTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
     "ListImportsOutputTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "ReplicaDescriptionTypeDef",
+    "ReplicaDescriptionTableTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
-    "TableDescriptionTableTypeDef",
     "ReplicationGroupUpdateTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "BackupDescriptionTypeDef",
+    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "ReplicationGroupUpdateTypeDef",
+    "TableDescriptionTableTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "UpdateTableInputRequestTypeDef",
     "DeleteBackupOutputTypeDef",
     "DescribeBackupOutputTypeDef",
     "DescribeImportOutputTypeDef",
     "ImportTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "UpdateTableInputRequestTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
+)
+
+AttributeDefinitionOutputTypeDef = TypedDict(
+    "AttributeDefinitionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
 )
 
 AttributeDefinitionServiceResourceTypeDef = TypedDict(
     "AttributeDefinitionServiceResourceTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeDefinitionTableOutputTypeDef = TypedDict(
+    "AttributeDefinitionTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
+)
+
 AttributeDefinitionTableTypeDef = TypedDict(
     "AttributeDefinitionTableTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
@@ -407,14 +453,46 @@
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeValueServiceResourceTypeDef = TypedDict(
+    "AttributeValueServiceResourceTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
+AttributeValueTableTypeDef = TypedDict(
+    "AttributeValueTableTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -448,36 +526,24 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
+        "TargetValue": float,
     },
-    total=False,
 )
 
-class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
-    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-):
-    pass
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -486,57 +552,49 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
+
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-_RequiredBackupDetailsTypeDef = TypedDict(
-    "_RequiredBackupDetailsTypeDef",
+
+BackupDetailsTypeDef = TypedDict(
+    "BackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
+        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-    },
-)
-_OptionalBackupDetailsTypeDef = TypedDict(
-    "_OptionalBackupDetailsTypeDef",
-    {
-        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
-    total=False,
 )
 
-class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
-    pass
-
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -545,15 +603,14 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -585,102 +642,82 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
-    "ItemCollectionMetricsServiceResourceTypeDef",
+
+KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "SizeEstimateRangeGB": List[float],
+        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
     },
-    total=False,
 )
 
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
+ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
+    "ItemCollectionMetricsServiceResourceTypeDef",
     {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
+        "SizeEstimateRangeGB": List[float],
     },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -706,35 +743,35 @@
                 None,
             ]
         ],
     },
     total=False,
 )
 
+
 class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
+
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
-    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
-    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -749,15 +786,15 @@
     },
 )
 
 ProjectionTableTypeDef = TypedDict(
     "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
+        "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTableTypeDef = TypedDict(
     "ProvisionedThroughputTableTypeDef",
     {
@@ -842,19 +879,21 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -895,33 +934,43 @@
     "_OptionalStreamSpecificationServiceResourceTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationServiceResourceTypeDef(
     _RequiredStreamSpecificationServiceResourceTypeDef,
     _OptionalStreamSpecificationServiceResourceTypeDef,
 ):
     pass
 
+
 TagServiceResourceTypeDef = TypedDict(
     "TagServiceResourceTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderList": List[str],
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": List[str],
+        "HeaderList": Sequence[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -985,36 +1034,17 @@
     },
     total=False,
 )
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1030,14 +1060,21 @@
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
+DeleteRequestServiceResourceOutputTypeDef = TypedDict(
+    "DeleteRequestServiceResourceOutputTypeDef",
+    {
+        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
+    },
+)
+
 DeleteRequestServiceResourceTypeDef = TypedDict(
     "DeleteRequestServiceResourceTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1090,27 +1127,28 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1143,15 +1181,14 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
-    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1181,26 +1218,14 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
-    total=False,
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1231,31 +1256,22 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1271,20 +1287,22 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
+
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1313,52 +1331,108 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
+
+KeySchemaElementTableOutputTypeDef = TypedDict(
+    "KeySchemaElementTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionTableOutputTypeDef = TypedDict(
+    "ProjectionTableOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
+)
+
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+KeySchemaElementOutputTypeDef = TypedDict(
+    "KeySchemaElementOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionOutputTypeDef = TypedDict(
+    "ProjectionOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+    },
 )
 
 ProjectionServiceResourceTypeDef = TypedDict(
     "ProjectionServiceResourceTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
+ReplicaOutputTypeDef = TypedDict(
+    "ReplicaOutputTypeDef",
+    {
+        "RegionName": str,
+    },
+)
+
+S3BucketSourceOutputTypeDef = TypedDict(
+    "S3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+)
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1366,43 +1440,33 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
+
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1452,122 +1516,85 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
+
 TagTableTypeDef = TypedDict(
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+    },
+)
+
+ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
     {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRequestServiceResourceOutputTypeDef = TypedDict(
+    "PutRequestServiceResourceOutputTypeDef",
+    {
+        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
 )
 
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
@@ -1594,137 +1621,96 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
+RestoreSummaryTableTypeDef = TypedDict(
+    "RestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRestoreSummaryTableTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTableTypeDef",
-    {
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-    },
-)
-_OptionalRestoreSummaryTableTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTableTypeDef",
+RestoreSummaryTypeDef = TypedDict(
+    "RestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-    },
-    total=False,
-)
-
-class RestoreSummaryTableTypeDef(
-    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
-):
-    pass
-
-_RequiredRestoreSummaryTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTypeDef",
-    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-_OptionalRestoreSummaryTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-    },
-    total=False,
-)
 
-class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
-    pass
-
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
+SSEDescriptionTableTypeDef = TypedDict(
+    "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
+SSEDescriptionTypeDef = TypedDict(
+    "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-    total=False,
 )
 
-SSEDescriptionTypeDef = TypedDict(
-    "SSEDescriptionTypeDef",
+SSESpecificationOutputTypeDef = TypedDict(
+    "SSESpecificationOutputTypeDef",
     {
-        "Status": SSEStatusType,
+        "Enabled": bool,
         "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
+        "KMSMasterKeyId": str,
     },
-    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
+StreamSpecificationOutputTypeDef = TypedDict(
+    "StreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+    },
+)
+
+StreamSpecificationTableOutputTypeDef = TypedDict(
+    "StreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1734,33 +1720,34 @@
     "_OptionalStreamSpecificationTableTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
+
 TableBatchWriterRequestTypeDef = TypedDict(
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
+TimeToLiveSpecificationOutputTypeDef = TypedDict(
+    "TimeToLiveSpecificationOutputTypeDef",
     {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Enabled": bool,
+        "AttributeName": str,
     },
 )
 
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
@@ -1787,27 +1774,146 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    {
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
+    {
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1837,15 +1943,14 @@
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
@@ -1876,19 +1981,21 @@
         ],
         "ConsistentRead": bool,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
+
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -1941,17 +2048,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
+
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
@@ -1978,17 +2087,26 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
+
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
+
+DeleteRequestOutputTypeDef = TypedDict(
+    "DeleteRequestOutputTypeDef",
+    {
+        "Key": Dict[str, AttributeValueTypeDef],
+    },
+)
+
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2069,17 +2187,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
+
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2111,19 +2231,21 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
+
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
             Union[
                 bytes,
@@ -2205,19 +2327,21 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2247,32 +2371,43 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
+
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
+)
+
+KeysAndAttributesOutputTypeDef = TypedDict(
+    "KeysAndAttributesOutputTypeDef",
+    {
+        "Keys": List[Dict[str, AttributeValueTypeDef]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
 )
 
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -2307,19 +2442,21 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
+
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
@@ -2347,19 +2484,28 @@
             ]
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
+
+PutRequestOutputTypeDef = TypedDict(
+    "PutRequestOutputTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+)
+
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2440,17 +2586,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
+
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2504,26 +2652,27 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
+
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
-    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2534,42 +2683,44 @@
     "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
+
 class AutoScalingPolicyUpdateTypeDef(
     _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
+
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2579,113 +2730,61 @@
     "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
+
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-    total=False,
-)
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2737,64 +2836,14 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2845,55 +2894,31 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_RequiredContinuousBackupsDescriptionTypeDef",
+ContinuousBackupsDescriptionTypeDef = TypedDict(
+    "ContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
-    },
-)
-_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_OptionalContinuousBackupsDescriptionTypeDef",
-    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
-    total=False,
 )
 
-class ContinuousBackupsDescriptionTypeDef(
-    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
-):
-    pass
-
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTableTypeDef],
         "Projection": ProjectionTableTypeDef,
     },
@@ -2902,51 +2927,30 @@
     "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
     total=False,
 )
 
+
 class CreateGlobalSecondaryIndexActionTableTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
 ):
     pass
 
+
 UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-    },
-    total=False,
-)
-
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -2964,30 +2968,21 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
 
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
@@ -2997,44 +2992,20 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-)
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
-    {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
-    },
-    total=False,
-)
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
 
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
@@ -3044,60 +3015,35 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
-    {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaTypeDef],
-    },
-    total=False,
-)
-
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexTableTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
     _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
 ):
     pass
 
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-    },
-    total=False,
-)
 
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
@@ -3105,36 +3051,36 @@
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+InputFormatOptionsOutputTypeDef = TypedDict(
+    "InputFormatOptionsOutputTypeDef",
+    {
+        "Csv": CsvOptionsOutputTypeDef,
+    },
+)
+
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -3193,19 +3139,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
+
 _RequiredPutItemInputTablePutItemTypeDef = TypedDict(
     "_RequiredPutItemInputTablePutItemTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -3256,19 +3204,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
     pass
 
+
 _RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
     "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -3321,19 +3271,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
     pass
 
+
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3344,48 +3296,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3395,87 +3347,157 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
+
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+)
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+    },
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+GlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "GlobalSecondaryIndexOutputTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+SourceTableDetailsTypeDef = TypedDict(
+    "SourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
 )
 
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
@@ -3486,94 +3508,282 @@
     "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
     },
     total=False,
 )
 
+
 class GlobalSecondaryIndexServiceResourceTypeDef(
     _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
     _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
 ):
     pass
 
+
 LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "LocalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
 )
 
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
+    {
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaOutputTypeDef],
+    },
+)
+
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
 
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+    },
+)
+
+ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+    },
+)
+
+WriteRequestServiceResourceOutputTypeDef = TypedDict(
+    "WriteRequestServiceResourceOutputTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceOutputTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+    },
+)
+
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
     },
     total=False,
 )
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
+        "TableName": str,
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
@@ -3582,20 +3792,22 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -3659,19 +3871,21 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
+
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
+
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -3734,17 +3948,19 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
+
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3802,19 +4018,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[
             str,
             Union[
@@ -3872,19 +4090,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3944,19 +4164,21 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
+
 TransactGetItemTypeDef = TypedDict(
     "TransactGetItemTypeDef",
     {
         "Get": GetTypeDef,
     },
 )
 
@@ -3970,19 +4192,21 @@
     "_OptionalBatchGetItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchGetItemInputRequestTypeDef(
     _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -3990,19 +4214,29 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
+    {
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
+    },
+)
+
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
     total=False,
@@ -4024,15 +4258,14 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
-    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4042,404 +4275,221 @@
     },
     total=False,
 )
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Responses": Dict[
-            str,
-            List[
-                Dict[
-                    str,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ]
-            ],
-        ],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
-        "Item": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
     },
     total=False,
 )
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateTableInputRequestTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4456,19 +4506,21 @@
         "Tags": Sequence[TagTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
+
 class CreateTableInputRequestTypeDef(
     _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
 ):
     pass
 
+
 _RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
     },
 )
@@ -4480,20 +4532,22 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+
 class RestoreTableFromBackupInputRequestTypeDef(
     _RequiredRestoreTableFromBackupInputRequestTypeDef,
     _OptionalRestoreTableFromBackupInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
     },
 )
 _OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
@@ -4508,79 +4562,58 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+
 class RestoreTableToPointInTimeInputRequestTypeDef(
     _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
     _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
+
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
+
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
-    {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4590,20 +4623,22 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMemberActionTableTypeDef(
     _RequiredCreateReplicationGroupMemberActionTableTypeDef,
     _OptionalCreateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
+
 _RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4613,35 +4648,21 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class UpdateReplicationGroupMemberActionTableTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
@@ -4652,20 +4673,22 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4675,28 +4698,54 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
+    {
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+)
+
+TableCreationParametersOutputTypeDef = TypedDict(
+    "TableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "SSESpecification": SSESpecificationOutputTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+)
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4713,26 +4762,77 @@
         "Tags": Sequence[TagServiceResourceTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
+
 class CreateTableInputServiceResourceCreateTableTypeDef(
     _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
     _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
 ):
     pass
 
+
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
+    {
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+    },
+)
+
+ReplicaDescriptionTableTypeDef = TypedDict(
+    "ReplicaDescriptionTableTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+    },
+)
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4743,36 +4843,28 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
+
 class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
     _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
 ):
     pass
 
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4782,19 +4874,31 @@
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
+
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
 _OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
@@ -4802,28 +4906,20 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
+
 class BatchWriteItemInputRequestTypeDef(
     _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
@@ -4833,54 +4929,43 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
-    },
-)
-_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
-    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-):
-    pass
-
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4897,20 +4982,22 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
+
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4927,55 +5014,21 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
 
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
@@ -4987,151 +5040,172 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
+
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
-    {
-        "AttributeDefinitions": List[AttributeDefinitionTableTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
 
 ReplicationGroupUpdateTableTypeDef = TypedDict(
     "ReplicationGroupUpdateTableTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTableTypeDef,
         "Update": UpdateReplicationGroupMemberActionTableTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
     },
     total=False,
 )
 
+ReplicationGroupUpdateTypeDef = TypedDict(
+    "ReplicationGroupUpdateTypeDef",
+    {
+        "Create": CreateReplicationGroupMemberActionTypeDef,
+        "Update": UpdateReplicationGroupMemberActionTypeDef,
+        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+    },
+    total=False,
+)
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+)
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
+    {
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersOutputTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
+    },
+)
+
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
-    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableStatus": TableStatusType,
         "CreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "TableSizeBytes": int,
         "ItemCount": int,
         "TableArn": str,
         "TableId": str,
         "BillingModeSummary": BillingModeSummaryTypeDef,
         "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
+        "StreamSpecification": StreamSpecificationOutputTypeDef,
         "LatestStreamLabel": str,
         "LatestStreamArn": str,
         "GlobalTableVersion": str,
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
-ReplicationGroupUpdateTypeDef = TypedDict(
-    "ReplicationGroupUpdateTypeDef",
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTableTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTableTypeDef],
+        "RestoreSummary": RestoreSummaryTableTypeDef,
+        "SSEDescription": SSEDescriptionTableTypeDef,
+        "ArchivalSummary": ArchivalSummaryTableTypeDef,
+        "TableClassSummary": TableClassSummaryTableTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
-    total=False,
 )
 
-_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaSettingsDescriptionTypeDef",
+ReplicaSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaSettingsDescriptionTypeDef",
-    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
-    total=False,
 )
 
-class ReplicaSettingsDescriptionTypeDef(
-    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
-):
-    pass
-
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5141,19 +5215,21 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
+
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -5165,199 +5241,202 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
+
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableTypeDef,
+        "SSESpecification": SSESpecificationTableTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
+
+
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
-    {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
-    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5369,20 +5448,22 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -5397,28 +5478,30 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
+
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.0
-Summary: Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,30 +481,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -524,174 +528,199 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -709,82 +738,83 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.0/setup.py` & `mypy-boto3-dynamodb-1.28.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

