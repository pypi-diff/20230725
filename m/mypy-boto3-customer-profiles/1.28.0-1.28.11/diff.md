# Comparing `tmp/mypy-boto3-customer-profiles-1.28.0.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.28.0.tar", last modified: Thu Jul  6 20:59:21 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.28.0.tar` & `mypy-boto3-customer-profiles-1.28.11.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.354271 mypy-boto3-customer-profiles-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-06 20:59:21.354271 mypy-boto3-customer-profiles-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.354271 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38754 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38697 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-06 20:37:17.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-06 20:37:17.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63019 2023-07-06 20:37:20.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-07-06 20:37:18.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.354271 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:21.000000 mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:21.354271 mypy-boto3-customer-profiles-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:37:16.000000 mypy-boto3-customer-profiles-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.833034 mypy-boto3-customer-profiles-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68581 2023-07-25 19:46:58.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68499 2023-07-25 19:46:57.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.833034 mypy-boto3-customer-profiles-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/LICENSE` & `mypy-boto3-customer-profiles-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.0/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.0
-Summary: Type annotations for boto3.CustomerProfiles 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.CustomerProfiles 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,27 +298,30 @@
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -332,179 +335,203 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
+    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
+    AttributeTypesSelectorOutputTypeDef,
+    AttributeTypesSelectorTypeDef,
+    ConflictResolutionOutputTypeDef,
+    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeOutputTypeDef,
+    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
+    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldTypeDef,
-    ObjectTypeKeyTypeDef,
+    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
+    GetSimilarProfilesRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
+    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
+    ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
-    MergeProfilesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
+    MatchingRuleOutputTypeDef,
+    MatchingRuleTypeDef,
+    ObjectTypeFieldTypeDef,
+    ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
+    AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
+    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingRequestTypeDef,
     MatchingResponseTypeDef,
+    RuleBasedMatchingResponseTypeDef,
+    MatchingRequestTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/README.md` & `mypy-boto3-customer-profiles-1.28.11/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,27 +266,30 @@
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -300,179 +303,203 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
+    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
+    AttributeTypesSelectorOutputTypeDef,
+    AttributeTypesSelectorTypeDef,
+    ConflictResolutionOutputTypeDef,
+    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeOutputTypeDef,
+    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
+    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldTypeDef,
-    ObjectTypeKeyTypeDef,
+    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
+    GetSimilarProfilesRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
+    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
+    ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
-    MergeProfilesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
+    MatchingRuleOutputTypeDef,
+    MatchingRuleTypeDef,
+    ObjectTypeFieldTypeDef,
+    ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
+    AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
+    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingRequestTypeDef,
     MatchingResponseTypeDef,
+    RuleBasedMatchingResponseTypeDef,
+    MatchingRequestTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__init__.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__init__.pyi` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.28.11\nVersion:         1.28.11\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,22 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .literals import (
+    GenderType,
+    MatchTypeType,
+    PartyTypeType,
+    StatisticType,
+    StatusType,
+    logicalOperatorType,
+)
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
@@ -48,70 +55,69 @@
     GetDomainResponseTypeDef,
     GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CustomerProfilesClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class CustomerProfilesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/)
     """
 
     meta: ClientMeta
@@ -120,42 +126,38 @@
     def exceptions(self) -> Exceptions:
         """
         CustomerProfilesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#exceptions)
         """
-
     def add_profile_key(
         self, *, ProfileId: str, KeyName: str, Values: Sequence[str], DomainName: str
     ) -> AddProfileKeyResponseTypeDef:
         """
         Associates a new key value with a specific profile, such as a Contact Record
         ContactId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.add_profile_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#add_profile_key)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
-
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
@@ -166,44 +168,42 @@
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Creates a new calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_calculated_attribute_definition)
         """
-
     def create_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_domain)
         """
-
     def create_event_stream(
         self, *, DomainName: str, Uri: str, EventStreamName: str, Tags: Mapping[str, str] = ...
     ) -> CreateEventStreamResponseTypeDef:
         """
         Creates an event stream, which is a subscription to real-time events, such as
         when profiles are created and updated through Amazon Connect Customer Profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_event_stream)
         """
-
     def create_integration_workflow(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
@@ -212,15 +212,14 @@
     ) -> CreateIntegrationWorkflowResponseTypeDef:
         """
         Creates an integration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_integration_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_integration_workflow)
         """
-
     def create_profile(
         self,
         *,
         DomainName: str,
         AccountNumber: str = ...,
         AdditionalInformation: str = ...,
         PartyType: PartyTypeType = ...,
@@ -247,111 +246,100 @@
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
-
     def delete_calculated_attribute_definition(
         self, *, DomainName: str, CalculatedAttributeName: str
     ) -> Dict[str, Any]:
         """
         Deletes an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_calculated_attribute_definition)
         """
-
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         Deletes a specific domain and all of its customer data, such as customer profile
         attributes and their related objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_domain)
         """
-
     def delete_event_stream(self, *, DomainName: str, EventStreamName: str) -> Dict[str, Any]:
         """
         Disables and deletes the specified event stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_event_stream)
         """
-
     def delete_integration(self, *, DomainName: str, Uri: str) -> DeleteIntegrationResponseTypeDef:
         """
         Removes an integration from a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_integration)
         """
-
     def delete_profile(self, *, ProfileId: str, DomainName: str) -> DeleteProfileResponseTypeDef:
         """
         Deletes the standard customer profile and all data pertaining to the profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile)
         """
-
     def delete_profile_key(
         self, *, ProfileId: str, KeyName: str, Values: Sequence[str], DomainName: str
     ) -> DeleteProfileKeyResponseTypeDef:
         """
         Removes a searchable key from a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_key)
         """
-
     def delete_profile_object(
         self, *, ProfileId: str, ProfileObjectUniqueKey: str, ObjectTypeName: str, DomainName: str
     ) -> DeleteProfileObjectResponseTypeDef:
         """
         Removes an object associated with a profile of a given ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_object)
         """
-
     def delete_profile_object_type(
         self, *, DomainName: str, ObjectTypeName: str
     ) -> DeleteProfileObjectTypeResponseTypeDef:
         """
         Removes a ProfileObjectType from a specific domain as well as removes all the
         ProfileObjects of that type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_object_type)
         """
-
     def delete_workflow(self, *, DomainName: str, WorkflowId: str) -> Dict[str, Any]:
         """
         Deletes the specified workflow and all its corresponding resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_workflow)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
-
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
         Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
@@ -359,221 +347,217 @@
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_auto_merging_preview)
         """
-
     def get_calculated_attribute_definition(
         self, *, DomainName: str, CalculatedAttributeName: str
     ) -> GetCalculatedAttributeDefinitionResponseTypeDef:
         """
         Provides more information on a calculated attribute definition for Customer
         Profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_definition)
         """
-
     def get_calculated_attribute_for_profile(
         self, *, DomainName: str, ProfileId: str, CalculatedAttributeName: str
     ) -> GetCalculatedAttributeForProfileResponseTypeDef:
         """
         Retrieve a calculated attribute for a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_for_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_for_profile)
         """
-
     def get_domain(self, *, DomainName: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_domain)
         """
-
     def get_event_stream(
         self, *, DomainName: str, EventStreamName: str
     ) -> GetEventStreamResponseTypeDef:
         """
         Returns information about the specified event stream in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_event_stream)
         """
-
     def get_identity_resolution_job(
         self, *, DomainName: str, JobId: str
     ) -> GetIdentityResolutionJobResponseTypeDef:
         """
         Returns information about an Identity Resolution Job in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_identity_resolution_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_identity_resolution_job)
         """
-
     def get_integration(self, *, DomainName: str, Uri: str) -> GetIntegrationResponseTypeDef:
         """
         Returns an integration for a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_integration)
         """
-
     def get_matches(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetMatchesResponseTypeDef:
         """
         Before calling this API, use
         [CreateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateDomain.html)_
         or
         [UpdateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_UpdateDomain.html)_
         to enable identity resolution: set `Matching` to tr...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_matches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_matches)
         """
-
     def get_profile_object_type(
         self, *, DomainName: str, ObjectTypeName: str
     ) -> GetProfileObjectTypeResponseTypeDef:
         """
         Returns the object types for a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_profile_object_type)
         """
-
     def get_profile_object_type_template(
         self, *, TemplateId: str
     ) -> GetProfileObjectTypeTemplateResponseTypeDef:
         """
         Returns the template information for a specific object type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_profile_object_type_template)
         """
+    def get_similar_profiles(
+        self,
+        *,
+        DomainName: str,
+        MatchType: MatchTypeType,
+        SearchKey: str,
+        SearchValue: str,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetSimilarProfilesResponseTypeDef:
+        """
+        Returns a set of profiles that belong to the same matching group using the
+        `matchId` or `profileId`.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_similar_profiles)
+        """
     def get_workflow(self, *, DomainName: str, WorkflowId: str) -> GetWorkflowResponseTypeDef:
         """
         Get details of specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_workflow)
         """
-
     def get_workflow_steps(
         self, *, DomainName: str, WorkflowId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetWorkflowStepsResponseTypeDef:
         """
         Get granular list of steps in workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_workflow_steps)
         """
-
     def list_account_integrations(
         self, *, Uri: str, NextToken: str = ..., MaxResults: int = ..., IncludeHidden: bool = ...
     ) -> ListAccountIntegrationsResponseTypeDef:
         """
         Lists all of the integrations associated to a specific URI in the AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_account_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_account_integrations)
         """
-
     def list_calculated_attribute_definitions(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCalculatedAttributeDefinitionsResponseTypeDef:
         """
         Lists calculated attribute definitions for Customer Profiles See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/customer-
         profiles-2020-08-15/ListCalculatedAttributeDefinitions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attribute_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attribute_definitions)
         """
-
     def list_calculated_attributes_for_profile(
         self, *, DomainName: str, ProfileId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCalculatedAttributesForProfileResponseTypeDef:
         """
         Retrieve a list of calculated attributes for a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attributes_for_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attributes_for_profile)
         """
-
     def list_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Returns a list of all the domains for an AWS account that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_domains)
         """
-
     def list_event_streams(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventStreamsResponseTypeDef:
         """
         Returns a list of all the event streams in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_event_streams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_event_streams)
         """
-
     def list_identity_resolution_jobs(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIdentityResolutionJobsResponseTypeDef:
         """
         Lists all of the Identity Resolution Jobs in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_identity_resolution_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_identity_resolution_jobs)
         """
-
     def list_integrations(
         self,
         *,
         DomainName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeHidden: bool = ...
     ) -> ListIntegrationsResponseTypeDef:
         """
         Lists all of the integrations in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_integrations)
         """
-
     def list_profile_object_type_templates(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProfileObjectTypeTemplatesResponseTypeDef:
         """
         Lists all of the template information for object types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_type_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_object_type_templates)
         """
-
     def list_profile_object_types(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProfileObjectTypesResponseTypeDef:
         """
         Lists all of the templates available within the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_object_types)
         """
-
     def list_profile_objects(
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         ProfileId: str,
         NextToken: str = ...,
@@ -583,23 +567,30 @@
         """
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_objects)
         """
+    def list_rule_based_matches(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListRuleBasedMatchesResponseTypeDef:
+        """
+        Returns a set of `MatchIds` that belong to the given domain.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_rule_based_matches)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_rule_based_matches)
+        """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with an Amazon Connect Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_tags_for_resource)
         """
-
     def list_workflows(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
         QueryStartDate: Union[datetime, str] = ...,
@@ -609,15 +600,14 @@
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_workflows)
         """
-
     def merge_profiles(
         self,
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
         FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
@@ -625,15 +615,14 @@
         """
         Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#merge_profiles)
         """
-
     def put_integration(
         self,
         *,
         DomainName: str,
         Uri: str = ...,
         ObjectTypeName: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -643,25 +632,23 @@
         """
         Adds an integration between the service and a third-party service, which
         includes Amazon AppFlow and Amazon Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_integration)
         """
-
     def put_profile_object(
         self, *, ObjectTypeName: str, Object: str, DomainName: str
     ) -> PutProfileObjectResponseTypeDef:
         """
         Adds additional objects to customer profiles of a given ObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object)
         """
-
     def put_profile_object_type(
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         Description: str,
         TemplateId: str = ...,
@@ -675,15 +662,14 @@
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
         """
-
     def search_profiles(
         self,
         *,
         DomainName: str,
         KeyName: str,
         Values: Sequence[str],
         NextToken: str = ...,
@@ -695,33 +681,30 @@
         Searches for profiles within a specific domain using one or more predefined
         search keys (e.g., _fullName, _phone, _email, _account, etc.) and/or custom-
         defined search keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.search_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#search_profiles)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns one or more tags (key-value pairs) to the specified Amazon Connect
         Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified Amazon Connect Customer Profiles
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#untag_resource)
         """
-
     def update_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         DisplayName: str = ...,
         Description: str = ...,
@@ -729,33 +712,32 @@
     ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Updates an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_calculated_attribute_definition)
         """
-
     def update_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_domain)
         """
-
     def update_profile(
         self,
         *,
         DomainName: str,
         ProfileId: str,
         AdditionalInformation: str = ...,
         AccountNumber: str = ...,
@@ -783,15 +765,14 @@
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
-
     def get_paginator(
         self, operation_name: Literal["list_event_streams"]
     ) -> ListEventStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,22 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .literals import (
+    GenderType,
+    MatchTypeType,
+    PartyTypeType,
+    StatisticType,
+    StatusType,
+    logicalOperatorType,
+)
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
@@ -48,66 +55,73 @@
     GetDomainResponseTypeDef,
     GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CustomerProfilesClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class CustomerProfilesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/)
     """
 
     meta: ClientMeta
@@ -116,38 +130,42 @@
     def exceptions(self) -> Exceptions:
         """
         CustomerProfilesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#exceptions)
         """
+
     def add_profile_key(
         self, *, ProfileId: str, KeyName: str, Values: Sequence[str], DomainName: str
     ) -> AddProfileKeyResponseTypeDef:
         """
         Associates a new key value with a specific profile, such as a Contact Record
         ContactId.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.add_profile_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#add_profile_key)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
+
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
@@ -158,41 +176,45 @@
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Creates a new calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_calculated_attribute_definition)
         """
+
     def create_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_domain)
         """
+
     def create_event_stream(
         self, *, DomainName: str, Uri: str, EventStreamName: str, Tags: Mapping[str, str] = ...
     ) -> CreateEventStreamResponseTypeDef:
         """
         Creates an event stream, which is a subscription to real-time events, such as
         when profiles are created and updated through Amazon Connect Customer Profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_event_stream)
         """
+
     def create_integration_workflow(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
@@ -201,14 +223,15 @@
     ) -> CreateIntegrationWorkflowResponseTypeDef:
         """
         Creates an integration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_integration_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_integration_workflow)
         """
+
     def create_profile(
         self,
         *,
         DomainName: str,
         AccountNumber: str = ...,
         AdditionalInformation: str = ...,
         PartyType: PartyTypeType = ...,
@@ -235,100 +258,111 @@
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
+
     def delete_calculated_attribute_definition(
         self, *, DomainName: str, CalculatedAttributeName: str
     ) -> Dict[str, Any]:
         """
         Deletes an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_calculated_attribute_definition)
         """
+
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         Deletes a specific domain and all of its customer data, such as customer profile
         attributes and their related objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_domain)
         """
+
     def delete_event_stream(self, *, DomainName: str, EventStreamName: str) -> Dict[str, Any]:
         """
         Disables and deletes the specified event stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_event_stream)
         """
+
     def delete_integration(self, *, DomainName: str, Uri: str) -> DeleteIntegrationResponseTypeDef:
         """
         Removes an integration from a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_integration)
         """
+
     def delete_profile(self, *, ProfileId: str, DomainName: str) -> DeleteProfileResponseTypeDef:
         """
         Deletes the standard customer profile and all data pertaining to the profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile)
         """
+
     def delete_profile_key(
         self, *, ProfileId: str, KeyName: str, Values: Sequence[str], DomainName: str
     ) -> DeleteProfileKeyResponseTypeDef:
         """
         Removes a searchable key from a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_key)
         """
+
     def delete_profile_object(
         self, *, ProfileId: str, ProfileObjectUniqueKey: str, ObjectTypeName: str, DomainName: str
     ) -> DeleteProfileObjectResponseTypeDef:
         """
         Removes an object associated with a profile of a given ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_object)
         """
+
     def delete_profile_object_type(
         self, *, DomainName: str, ObjectTypeName: str
     ) -> DeleteProfileObjectTypeResponseTypeDef:
         """
         Removes a ProfileObjectType from a specific domain as well as removes all the
         ProfileObjects of that type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_profile_object_type)
         """
+
     def delete_workflow(self, *, DomainName: str, WorkflowId: str) -> Dict[str, Any]:
         """
         Deletes the specified workflow and all its corresponding resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_workflow)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
+
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
         Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
@@ -336,200 +370,239 @@
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_auto_merging_preview)
         """
+
     def get_calculated_attribute_definition(
         self, *, DomainName: str, CalculatedAttributeName: str
     ) -> GetCalculatedAttributeDefinitionResponseTypeDef:
         """
         Provides more information on a calculated attribute definition for Customer
         Profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_definition)
         """
+
     def get_calculated_attribute_for_profile(
         self, *, DomainName: str, ProfileId: str, CalculatedAttributeName: str
     ) -> GetCalculatedAttributeForProfileResponseTypeDef:
         """
         Retrieve a calculated attribute for a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_for_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_for_profile)
         """
+
     def get_domain(self, *, DomainName: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_domain)
         """
+
     def get_event_stream(
         self, *, DomainName: str, EventStreamName: str
     ) -> GetEventStreamResponseTypeDef:
         """
         Returns information about the specified event stream in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_event_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_event_stream)
         """
+
     def get_identity_resolution_job(
         self, *, DomainName: str, JobId: str
     ) -> GetIdentityResolutionJobResponseTypeDef:
         """
         Returns information about an Identity Resolution Job in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_identity_resolution_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_identity_resolution_job)
         """
+
     def get_integration(self, *, DomainName: str, Uri: str) -> GetIntegrationResponseTypeDef:
         """
         Returns an integration for a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_integration)
         """
+
     def get_matches(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetMatchesResponseTypeDef:
         """
         Before calling this API, use
         [CreateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateDomain.html)_
         or
         [UpdateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_UpdateDomain.html)_
         to enable identity resolution: set `Matching` to tr...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_matches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_matches)
         """
+
     def get_profile_object_type(
         self, *, DomainName: str, ObjectTypeName: str
     ) -> GetProfileObjectTypeResponseTypeDef:
         """
         Returns the object types for a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_profile_object_type)
         """
+
     def get_profile_object_type_template(
         self, *, TemplateId: str
     ) -> GetProfileObjectTypeTemplateResponseTypeDef:
         """
         Returns the template information for a specific object type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_profile_object_type_template)
         """
+
+    def get_similar_profiles(
+        self,
+        *,
+        DomainName: str,
+        MatchType: MatchTypeType,
+        SearchKey: str,
+        SearchValue: str,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetSimilarProfilesResponseTypeDef:
+        """
+        Returns a set of profiles that belong to the same matching group using the
+        `matchId` or `profileId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_similar_profiles)
+        """
+
     def get_workflow(self, *, DomainName: str, WorkflowId: str) -> GetWorkflowResponseTypeDef:
         """
         Get details of specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_workflow)
         """
+
     def get_workflow_steps(
         self, *, DomainName: str, WorkflowId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetWorkflowStepsResponseTypeDef:
         """
         Get granular list of steps in workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_workflow_steps)
         """
+
     def list_account_integrations(
         self, *, Uri: str, NextToken: str = ..., MaxResults: int = ..., IncludeHidden: bool = ...
     ) -> ListAccountIntegrationsResponseTypeDef:
         """
         Lists all of the integrations associated to a specific URI in the AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_account_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_account_integrations)
         """
+
     def list_calculated_attribute_definitions(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCalculatedAttributeDefinitionsResponseTypeDef:
         """
         Lists calculated attribute definitions for Customer Profiles See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/customer-
         profiles-2020-08-15/ListCalculatedAttributeDefinitions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attribute_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attribute_definitions)
         """
+
     def list_calculated_attributes_for_profile(
         self, *, DomainName: str, ProfileId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCalculatedAttributesForProfileResponseTypeDef:
         """
         Retrieve a list of calculated attributes for a customer profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attributes_for_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attributes_for_profile)
         """
+
     def list_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Returns a list of all the domains for an AWS account that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_domains)
         """
+
     def list_event_streams(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventStreamsResponseTypeDef:
         """
         Returns a list of all the event streams in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_event_streams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_event_streams)
         """
+
     def list_identity_resolution_jobs(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIdentityResolutionJobsResponseTypeDef:
         """
         Lists all of the Identity Resolution Jobs in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_identity_resolution_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_identity_resolution_jobs)
         """
+
     def list_integrations(
         self,
         *,
         DomainName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeHidden: bool = ...
     ) -> ListIntegrationsResponseTypeDef:
         """
         Lists all of the integrations in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_integrations)
         """
+
     def list_profile_object_type_templates(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProfileObjectTypeTemplatesResponseTypeDef:
         """
         Lists all of the template information for object types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_type_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_object_type_templates)
         """
+
     def list_profile_object_types(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProfileObjectTypesResponseTypeDef:
         """
         Lists all of the templates available within the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_object_types)
         """
+
     def list_profile_objects(
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         ProfileId: str,
         NextToken: str = ...,
@@ -539,21 +612,33 @@
         """
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_profile_objects)
         """
+
+    def list_rule_based_matches(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListRuleBasedMatchesResponseTypeDef:
+        """
+        Returns a set of `MatchIds` that belong to the given domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_rule_based_matches)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_rule_based_matches)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with an Amazon Connect Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_tags_for_resource)
         """
+
     def list_workflows(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
         QueryStartDate: Union[datetime, str] = ...,
@@ -563,14 +648,15 @@
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_workflows)
         """
+
     def merge_profiles(
         self,
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
         FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
@@ -578,14 +664,15 @@
         """
         Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#merge_profiles)
         """
+
     def put_integration(
         self,
         *,
         DomainName: str,
         Uri: str = ...,
         ObjectTypeName: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -595,23 +682,25 @@
         """
         Adds an integration between the service and a third-party service, which
         includes Amazon AppFlow and Amazon Connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_integration)
         """
+
     def put_profile_object(
         self, *, ObjectTypeName: str, Object: str, DomainName: str
     ) -> PutProfileObjectResponseTypeDef:
         """
         Adds additional objects to customer profiles of a given ObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object)
         """
+
     def put_profile_object_type(
         self,
         *,
         DomainName: str,
         ObjectTypeName: str,
         Description: str,
         TemplateId: str = ...,
@@ -625,14 +714,15 @@
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
         """
+
     def search_profiles(
         self,
         *,
         DomainName: str,
         KeyName: str,
         Values: Sequence[str],
         NextToken: str = ...,
@@ -644,30 +734,33 @@
         Searches for profiles within a specific domain using one or more predefined
         search keys (e.g., _fullName, _phone, _email, _account, etc.) and/or custom-
         defined search keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.search_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#search_profiles)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns one or more tags (key-value pairs) to the specified Amazon Connect
         Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified Amazon Connect Customer Profiles
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#untag_resource)
         """
+
     def update_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
         DisplayName: str = ...,
         Description: str = ...,
@@ -675,31 +768,34 @@
     ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
         """
         Updates an existing calculated attribute definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_calculated_attribute_definition)
         """
+
     def update_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_domain)
         """
+
     def update_profile(
         self,
         *,
         DomainName: str,
         ProfileId: str,
         AdditionalInformation: str = ...,
         AccountNumber: str = ...,
@@ -727,14 +823,15 @@
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
+
     def get_paginator(
         self, operation_name: Literal["list_event_streams"]
     ) -> ListEventStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,44 @@
 Type annotations for customer-profiles service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_customer_profiles.literals import ConflictResolvingModelType
+    from mypy_boto3_customer_profiles.literals import AttributeMatchingModelType
 
-    data: ConflictResolvingModelType = "RECENCY"
+    data: AttributeMatchingModelType = "MANY_TO_MANY"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "AttributeMatchingModelType",
     "ConflictResolvingModelType",
     "DataPullModeType",
     "EventStreamDestinationStatusType",
     "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
     "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
+    "MatchTypeType",
     "OperatorPropertiesKeysType",
     "OperatorType",
     "PartyTypeType",
+    "RuleBasedMatchingStatusType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
     "StatisticType",
     "StatusType",
@@ -50,14 +53,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
 EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
 EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
@@ -81,14 +85,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+MatchTypeType = Literal["ML_BASED_MATCHING", "RULE_BASED_MATCHING"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "LOWER_BOUND",
     "MASK_LENGTH",
     "MASK_VALUE",
@@ -99,14 +104,15 @@
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
 OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
+RuleBasedMatchingStatusType = Literal["ACTIVE", "IN_PROGRESS", "PENDING"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
     "GREATER_THAN_OR_EQUAL_TO",
@@ -423,14 +429,15 @@
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

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 Type annotations for customer-profiles service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_customer_profiles.literals import ConflictResolvingModelType
+    from mypy_boto3_customer_profiles.literals import AttributeMatchingModelType
 
-    data: ConflictResolvingModelType = "RECENCY"
+    data: AttributeMatchingModelType = "MANY_TO_MANY"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AttributeMatchingModelType",
     "ConflictResolvingModelType",
     "DataPullModeType",
     "EventStreamDestinationStatusType",
     "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
     "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
+    "MatchTypeType",
     "OperatorPropertiesKeysType",
     "OperatorType",
     "PartyTypeType",
+    "RuleBasedMatchingStatusType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
     "StatisticType",
     "StatusType",
@@ -48,14 +51,15 @@
     "CustomerProfilesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
 EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
 EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
@@ -79,14 +83,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+MatchTypeType = Literal["ML_BASED_MATCHING", "RULE_BASED_MATCHING"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "LOWER_BOUND",
     "MASK_LENGTH",
     "MASK_VALUE",
@@ -97,14 +102,15 @@
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
 OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
+RuleBasedMatchingStatusType = Literal["ACTIVE", "IN_PROGRESS", "PENDING"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
     "GREATER_THAN_OR_EQUAL_TO",
@@ -421,14 +427,15 @@
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

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/paginator.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/paginator.pyi` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,29 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -49,165 +52,189 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "AddProfileKeyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
+    "AttributeItemOutputTypeDef",
     "AttributeItemTypeDef",
+    "AttributeTypesSelectorOutputTypeDef",
+    "AttributeTypesSelectorTypeDef",
+    "ConflictResolutionOutputTypeDef",
+    "ConsolidationOutputTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
+    "RangeOutputTypeDef",
+    "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
-    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
-    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
+    "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
-    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
-    "ObjectTypeFieldTypeDef",
-    "ObjectTypeKeyTypeDef",
+    "ObjectTypeFieldOutputTypeDef",
+    "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
+    "GetSimilarProfilesRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
+    "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
+    "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutIntegrationResponseTypeDef",
+    "MatchingRuleOutputTypeDef",
+    "MatchingRuleTypeDef",
+    "ObjectTypeFieldTypeDef",
+    "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
-    "PutProfileObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
+    "AddProfileKeyResponseTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteIntegrationResponseTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
+    "DeleteProfileResponseTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PutIntegrationResponseTypeDef",
+    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
+    "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
+    "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
+    "ExportingConfigOutputTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
-    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
-    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "ListEventStreamsResponseTypeDef",
-    "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
+    "MatchingRequestTypeDef",
+    "RuleBasedMatchingRequestTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainRequestRequestTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
     "AppflowIntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "IntegrationConfigTypeDef",
     "CreateIntegrationWorkflowRequestRequestTypeDef",
 )
@@ -218,31 +245,49 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "Address1": str,
+        "Address2": str,
+        "Address3": str,
+        "Address4": str,
+        "City": str,
+        "County": str,
+        "State": str,
+        "Province": str,
+        "Country": str,
+        "PostalCode": str,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
         "Address3": str,
         "Address4": str,
@@ -260,37 +305,23 @@
     "BatchTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-_RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
+AppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "AppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
-    },
-)
-_OptionalAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "_OptionalAppflowIntegrationWorkflowAttributesTypeDef",
-    {
         "RoleArn": str,
     },
-    total=False,
 )
 
-
-class AppflowIntegrationWorkflowAttributesTypeDef(
-    _RequiredAppflowIntegrationWorkflowAttributesTypeDef,
-    _OptionalAppflowIntegrationWorkflowAttributesTypeDef,
-):
-    pass
-
-
 AppflowIntegrationWorkflowMetricsTypeDef = TypedDict(
     "AppflowIntegrationWorkflowMetricsTypeDef",
     {
         "RecordsProcessed": int,
         "StepsCompleted": int,
         "TotalSteps": int,
     },
@@ -306,21 +337,76 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
+AttributeItemOutputTypeDef = TypedDict(
+    "AttributeItemOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
+AttributeTypesSelectorOutputTypeDef = TypedDict(
+    "AttributeTypesSelectorOutputTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+        "Address": List[str],
+        "PhoneNumber": List[str],
+        "EmailAddress": List[str],
+    },
+)
+
+_RequiredAttributeTypesSelectorTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorTypeDef",
+    {
+        "Address": Sequence[str],
+        "PhoneNumber": Sequence[str],
+        "EmailAddress": Sequence[str],
+    },
+    total=False,
+)
+
+
+class AttributeTypesSelectorTypeDef(
+    _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
+):
+    pass
+
+
+ConflictResolutionOutputTypeDef = TypedDict(
+    "ConflictResolutionOutputTypeDef",
+    {
+        "ConflictResolvingModel": ConflictResolvingModelType,
+        "SourceName": str,
+    },
+)
+
+ConsolidationOutputTypeDef = TypedDict(
+    "ConsolidationOutputTypeDef",
+    {
+        "MatchingAttributesList": List[List[str]],
+    },
+)
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -341,14 +427,30 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["DAYS"],
+    },
+)
+
+ThresholdOutputTypeDef = TypedDict(
+    "ThresholdOutputTypeDef",
+    {
+        "Value": str,
+        "Operator": OperatorType,
+    },
+)
+
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
 )
@@ -392,40 +494,14 @@
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
 
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -433,22 +509,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -457,153 +525,94 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
-_RequiredDestinationSummaryTypeDef = TypedDict(
-    "_RequiredDestinationSummaryTypeDef",
+DestinationSummaryTypeDef = TypedDict(
+    "DestinationSummaryTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
-    },
-)
-_OptionalDestinationSummaryTypeDef = TypedDict(
-    "_OptionalDestinationSummaryTypeDef",
-    {
         "UnhealthySince": datetime,
     },
-    total=False,
 )
 
-
-class DestinationSummaryTypeDef(
-    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
-):
-    pass
-
-
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
-    total=False,
 )
 
-_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
-    "_RequiredEventStreamDestinationDetailsTypeDef",
+EventStreamDestinationDetailsTypeDef = TypedDict(
+    "EventStreamDestinationDetailsTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
-    },
-)
-_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
-    "_OptionalEventStreamDestinationDetailsTypeDef",
-    {
         "UnhealthySince": datetime,
         "Message": str,
     },
-    total=False,
 )
 
-
-class EventStreamDestinationDetailsTypeDef(
-    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
-):
-    pass
-
+S3ExportingConfigOutputTypeDef = TypedDict(
+    "S3ExportingConfigOutputTypeDef",
+    {
+        "S3BucketName": str,
+        "S3KeyName": str,
+    },
+)
 
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
@@ -624,15 +633,14 @@
 
 S3ExportingLocationTypeDef = TypedDict(
     "S3ExportingLocationTypeDef",
     {
         "S3BucketName": str,
         "S3KeyName": str,
     },
-    total=False,
 )
 
 FieldSourceProfileIdsTypeDef = TypedDict(
     "FieldSourceProfileIdsTypeDef",
     {
         "AccountNumber": str,
         "AdditionalInformation": str,
@@ -661,26 +669,14 @@
 
 FoundByKeyValueTypeDef = TypedDict(
     "FoundByKeyValueTypeDef",
     {
         "KeyName": str,
         "Values": List[str],
     },
-    total=False,
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
@@ -692,25 +688,14 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -733,41 +718,24 @@
 JobStatsTypeDef = TypedDict(
     "JobStatsTypeDef",
     {
         "NumberOfProfilesReviewed": int,
         "NumberOfMatchesFound": int,
         "NumberOfMergesDone": int,
     },
-    total=False,
 )
 
 GetIntegrationRequestRequestTypeDef = TypedDict(
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -789,51 +757,74 @@
 MatchItemTypeDef = TypedDict(
     "MatchItemTypeDef",
     {
         "MatchId": str,
         "ProfileIds": List[str],
         "ConfidenceScore": float,
     },
-    total=False,
 )
 
 GetProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-ObjectTypeFieldTypeDef = TypedDict(
-    "ObjectTypeFieldTypeDef",
+ObjectTypeFieldOutputTypeDef = TypedDict(
+    "ObjectTypeFieldOutputTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
-    total=False,
 )
 
-ObjectTypeKeyTypeDef = TypedDict(
-    "ObjectTypeKeyTypeDef",
+ObjectTypeKeyOutputTypeDef = TypedDict(
+    "ObjectTypeKeyOutputTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
-    total=False,
 )
 
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
 )
 
+_RequiredGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "MatchType": MatchTypeType,
+        "SearchKey": str,
+        "SearchValue": str,
+    },
+)
+_OptionalGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetSimilarProfilesRequestRequestTypeDef(
+    _RequiredGetSimilarProfilesRequestRequestTypeDef,
+    _OptionalGetSimilarProfilesRequestRequestTypeDef,
+):
+    pass
+
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -865,14 +856,22 @@
     "IncrementalPullConfigTypeDef",
     {
         "DatetimeTypeFieldName": str,
     },
     total=False,
 )
 
+JobScheduleOutputTypeDef = TypedDict(
+    "JobScheduleOutputTypeDef",
+    {
+        "DayOfTheWeek": JobScheduleDayOfTheWeekType,
+        "Time": str,
+    },
+)
+
 JobScheduleTypeDef = TypedDict(
     "JobScheduleTypeDef",
     {
         "DayOfTheWeek": JobScheduleDayOfTheWeekType,
         "Time": str,
     },
 )
@@ -897,53 +896,39 @@
 class ListAccountIntegrationsRequestRequestTypeDef(
     _RequiredListAccountIntegrationsRequestRequestTypeDef,
     _OptionalListAccountIntegrationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListIntegrationItemTypeDef = TypedDict(
-    "_RequiredListIntegrationItemTypeDef",
+ListIntegrationItemTypeDef = TypedDict(
+    "ListIntegrationItemTypeDef",
     {
         "DomainName": str,
         "Uri": str,
+        "ObjectTypeName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-    },
-)
-_OptionalListIntegrationItemTypeDef = TypedDict(
-    "_OptionalListIntegrationItemTypeDef",
-    {
-        "ObjectTypeName": str,
         "Tags": Dict[str, str],
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
     },
-    total=False,
 )
 
-
-class ListIntegrationItemTypeDef(
-    _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
-):
-    pass
-
-
 ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -969,15 +954,14 @@
     "ListCalculatedAttributeForProfileItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "IsDataPartial": str,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
     {
         "DomainName": str,
         "ProfileId": str,
@@ -996,66 +980,43 @@
 class ListCalculatedAttributesForProfileRequestRequestTypeDef(
     _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
     _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListDomainItemTypeDef = TypedDict(
-    "_RequiredListDomainItemTypeDef",
+ListDomainItemTypeDef = TypedDict(
+    "ListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-    },
-)
-_OptionalListDomainItemTypeDef = TypedDict(
-    "_OptionalListDomainItemTypeDef",
-    {
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class ListDomainItemTypeDef(_RequiredListDomainItemTypeDef, _OptionalListDomainItemTypeDef):
-    pass
-
-
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1116,46 +1077,32 @@
 
 class ListIntegrationsRequestRequestTypeDef(
     _RequiredListIntegrationsRequestRequestTypeDef, _OptionalListIntegrationsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListProfileObjectTypeItemTypeDef = TypedDict(
-    "_RequiredListProfileObjectTypeItemTypeDef",
+ListProfileObjectTypeItemTypeDef = TypedDict(
+    "ListProfileObjectTypeItemTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
-    },
-)
-_OptionalListProfileObjectTypeItemTypeDef = TypedDict(
-    "_OptionalListProfileObjectTypeItemTypeDef",
-    {
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class ListProfileObjectTypeItemTypeDef(
-    _RequiredListProfileObjectTypeItemTypeDef, _OptionalListProfileObjectTypeItemTypeDef
-):
-    pass
-
-
 ListProfileObjectTypeTemplateItemTypeDef = TypedDict(
     "ListProfileObjectTypeTemplateItemTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
     },
-    total=False,
 )
 
 ListProfileObjectTypeTemplatesRequestRequestTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1189,37 +1136,51 @@
 ListProfileObjectsItemTypeDef = TypedDict(
     "ListProfileObjectsItemTypeDef",
     {
         "ObjectTypeName": str,
         "ProfileObjectUniqueKey": str,
         "Object": str,
     },
-    total=False,
 )
 
 ObjectFilterTypeDef = TypedDict(
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+_RequiredListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRuleBasedMatchesRequestRequestTypeDef",
     {
-        "resourceArn": str,
+        "DomainName": str,
+    },
+)
+_OptionalListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+
+class ListRuleBasedMatchesRequestRequestTypeDef(
+    _RequiredListRuleBasedMatchesRequestRequestTypeDef,
+    _OptionalListRuleBasedMatchesRequestRequestTypeDef,
+):
+    pass
+
+
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
     },
 )
 
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
@@ -1260,76 +1221,56 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
+MatchingRuleOutputTypeDef = TypedDict(
+    "MatchingRuleOutputTypeDef",
     {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rule": List[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+MatchingRuleTypeDef = TypedDict(
+    "MatchingRuleTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Rule": Sequence[str],
+    },
+)
+
+ObjectTypeFieldTypeDef = TypedDict(
+    "ObjectTypeFieldTypeDef",
+    {
+        "Source": str,
+        "Target": str,
+        "ContentType": FieldContentTypeType,
     },
     total=False,
 )
 
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
+ObjectTypeKeyTypeDef = TypedDict(
+    "ObjectTypeKeyTypeDef",
     {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StandardIdentifiers": Sequence[StandardIdentifierType],
+        "FieldNames": Sequence[str],
     },
+    total=False,
 )
 
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-)
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1438,19 +1379,202 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
+    {
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1520,41 +1644,56 @@
 
 
 WorkflowAttributesTypeDef = TypedDict(
     "WorkflowAttributesTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowAttributesTypeDef,
     },
-    total=False,
 )
 
 WorkflowMetricsTypeDef = TypedDict(
     "WorkflowMetricsTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowMetricsTypeDef,
     },
-    total=False,
 )
 
 WorkflowStepItemTypeDef = TypedDict(
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
-    total=False,
+)
+
+AttributeDetailsOutputTypeDef = TypedDict(
+    "AttributeDetailsOutputTypeDef",
+    {
+        "Attributes": List[AttributeItemOutputTypeDef],
+        "Expression": str,
+    },
 )
 
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
+AutoMergingOutputTypeDef = TypedDict(
+    "AutoMergingOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Consolidation": ConsolidationOutputTypeDef,
+        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "MinAllowedConfidenceScoreForMerging": float,
+    },
+)
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1592,14 +1731,23 @@
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
 
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "Range": RangeOutputTypeDef,
+        "ObjectCount": int,
+        "Threshold": ThresholdOutputTypeDef,
+    },
+)
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -1624,51 +1772,45 @@
 )
 
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
 
-_RequiredEventStreamSummaryTypeDef = TypedDict(
-    "_RequiredEventStreamSummaryTypeDef",
+EventStreamSummaryTypeDef = TypedDict(
+    "EventStreamSummaryTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
         "EventStreamArn": str,
         "State": EventStreamStateType,
-    },
-)
-_OptionalEventStreamSummaryTypeDef = TypedDict(
-    "_OptionalEventStreamSummaryTypeDef",
-    {
         "StoppedSince": datetime,
         "DestinationSummary": DestinationSummaryTypeDef,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class EventStreamSummaryTypeDef(
-    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
-):
-    pass
-
-
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportingConfigOutputTypeDef = TypedDict(
+    "ExportingConfigOutputTypeDef",
+    {
+        "S3Exporting": S3ExportingConfigOutputTypeDef,
     },
 )
 
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
@@ -1677,15 +1819,14 @@
 )
 
 ExportingLocationTypeDef = TypedDict(
     "ExportingLocationTypeDef",
     {
         "S3Exporting": S3ExportingLocationTypeDef,
     },
-    total=False,
 )
 
 _RequiredMergeProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredMergeProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
         "MainProfileId": str,
@@ -1723,189 +1864,179 @@
         "PhoneNumber": str,
         "MobilePhoneNumber": str,
         "HomePhoneNumber": str,
         "BusinessPhoneNumber": str,
         "EmailAddress": str,
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
-        "Address": AddressTypeDef,
-        "ShippingAddress": AddressTypeDef,
-        "MailingAddress": AddressTypeDef,
-        "BillingAddress": AddressTypeDef,
+        "Address": AddressOutputTypeDef,
+        "ShippingAddress": AddressOutputTypeDef,
+        "MailingAddress": AddressOutputTypeDef,
+        "BillingAddress": AddressOutputTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
-    total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
-
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
+
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1932,18 +2063,49 @@
 
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
+    },
+)
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
+
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
+    pass
+
+
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2011,136 +2173,160 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
-        "DomainName": str,
         "CalculatedAttributeName": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Statistic": StatisticType,
-    },
-)
-_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
-    {
         "DisplayName": str,
         "Description": str,
-        "Conditions": ConditionsTypeDef,
-        "Tags": Mapping[str, str],
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Conditions": ConditionsOutputTypeDef,
+        "Statistic": StatisticType,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
-CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Conditions": ConditionsTypeDef,
-        "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeDefinitionResponseTypeDef",
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
-        "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsTypeDef,
+        "Conditions": ConditionsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
     },
 )
-_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
+        "DomainName": str,
         "CalculatedAttributeName": str,
+    },
+)
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
         "DisplayName": str,
         "Description": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MatchingResponseTypeDef = TypedDict(
+    "MatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "JobSchedule": JobScheduleOutputTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
+        "ExportingConfig": ExportingConfigOutputTypeDef,
+    },
+)
+
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleOutputTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
+        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "ExportingConfig": ExportingConfigOutputTypeDef,
     },
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
@@ -2157,40 +2343,55 @@
 )
 
 
 class MatchingRequestTypeDef(_RequiredMatchingRequestTypeDef, _OptionalMatchingRequestTypeDef):
     pass
 
 
-MatchingResponseTypeDef = TypedDict(
-    "MatchingResponseTypeDef",
+_RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_RequiredRuleBasedMatchingRequestTypeDef",
     {
         "Enabled": bool,
-        "JobSchedule": JobScheduleTypeDef,
-        "AutoMerging": AutoMergingTypeDef,
+    },
+)
+_OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_OptionalRuleBasedMatchingRequestTypeDef",
+    {
+        "MatchingRules": Sequence[MatchingRuleTypeDef],
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
+
+class RuleBasedMatchingRequestTypeDef(
+    _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
+):
+    pass
+
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
-        "AutoMerging": AutoMergingTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2198,23 +2399,22 @@
         "Status": IdentityResolutionJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "JobStats": JobStatsTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "Message": str,
     },
-    total=False,
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2250,27 +2450,77 @@
 )
 
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Stats": DomainStatsTypeDef,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainResponseTypeDef = TypedDict(
+    "UpdateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateDomainRequestRequestTypeDef(
@@ -2288,78 +2538,33 @@
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainRequestRequestTypeDef",
     {
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class UpdateDomainRequestRequestTypeDef(
     _RequiredUpdateDomainRequestRequestTypeDef, _OptionalUpdateDomainRequestRequestTypeDef
 ):
     pass
 
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Stats": DomainStatsTypeDef,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainResponseTypeDef = TypedDict(
-    "UpdateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,29 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -48,165 +51,189 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "AddProfileKeyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
+    "AttributeItemOutputTypeDef",
     "AttributeItemTypeDef",
+    "AttributeTypesSelectorOutputTypeDef",
+    "AttributeTypesSelectorTypeDef",
+    "ConflictResolutionOutputTypeDef",
+    "ConsolidationOutputTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
+    "RangeOutputTypeDef",
+    "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
-    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
-    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
+    "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
-    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
-    "ObjectTypeFieldTypeDef",
-    "ObjectTypeKeyTypeDef",
+    "ObjectTypeFieldOutputTypeDef",
+    "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
+    "GetSimilarProfilesRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
+    "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
+    "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutIntegrationResponseTypeDef",
+    "MatchingRuleOutputTypeDef",
+    "MatchingRuleTypeDef",
+    "ObjectTypeFieldTypeDef",
+    "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
-    "PutProfileObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
+    "AddProfileKeyResponseTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteIntegrationResponseTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
+    "DeleteProfileResponseTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PutIntegrationResponseTypeDef",
+    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
+    "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
+    "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
+    "ExportingConfigOutputTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
-    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
-    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "ListEventStreamsResponseTypeDef",
-    "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
+    "MatchingRequestTypeDef",
+    "RuleBasedMatchingRequestTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainRequestRequestTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
     "AppflowIntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "IntegrationConfigTypeDef",
     "CreateIntegrationWorkflowRequestRequestTypeDef",
 )
@@ -217,31 +244,49 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "Address1": str,
+        "Address2": str,
+        "Address3": str,
+        "Address4": str,
+        "City": str,
+        "County": str,
+        "State": str,
+        "Province": str,
+        "Country": str,
+        "PostalCode": str,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
         "Address3": str,
         "Address4": str,
@@ -259,35 +304,23 @@
     "BatchTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-_RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
+AppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "AppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
-    },
-)
-_OptionalAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "_OptionalAppflowIntegrationWorkflowAttributesTypeDef",
-    {
         "RoleArn": str,
     },
-    total=False,
 )
 
-class AppflowIntegrationWorkflowAttributesTypeDef(
-    _RequiredAppflowIntegrationWorkflowAttributesTypeDef,
-    _OptionalAppflowIntegrationWorkflowAttributesTypeDef,
-):
-    pass
-
 AppflowIntegrationWorkflowMetricsTypeDef = TypedDict(
     "AppflowIntegrationWorkflowMetricsTypeDef",
     {
         "RecordsProcessed": int,
         "StepsCompleted": int,
         "TotalSteps": int,
     },
@@ -303,21 +336,74 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
+AttributeItemOutputTypeDef = TypedDict(
+    "AttributeItemOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
+AttributeTypesSelectorOutputTypeDef = TypedDict(
+    "AttributeTypesSelectorOutputTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+        "Address": List[str],
+        "PhoneNumber": List[str],
+        "EmailAddress": List[str],
+    },
+)
+
+_RequiredAttributeTypesSelectorTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorTypeDef",
+    {
+        "Address": Sequence[str],
+        "PhoneNumber": Sequence[str],
+        "EmailAddress": Sequence[str],
+    },
+    total=False,
+)
+
+class AttributeTypesSelectorTypeDef(
+    _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
+):
+    pass
+
+ConflictResolutionOutputTypeDef = TypedDict(
+    "ConflictResolutionOutputTypeDef",
+    {
+        "ConflictResolvingModel": ConflictResolvingModelType,
+        "SourceName": str,
+    },
+)
+
+ConsolidationOutputTypeDef = TypedDict(
+    "ConsolidationOutputTypeDef",
+    {
+        "MatchingAttributesList": List[List[str]],
+    },
+)
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -336,14 +422,30 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["DAYS"],
+    },
+)
+
+ThresholdOutputTypeDef = TypedDict(
+    "ThresholdOutputTypeDef",
+    {
+        "Value": str,
+        "Operator": OperatorType,
+    },
+)
+
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
 )
@@ -385,40 +487,14 @@
 )
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -426,22 +502,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -450,149 +518,94 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
-_RequiredDestinationSummaryTypeDef = TypedDict(
-    "_RequiredDestinationSummaryTypeDef",
+DestinationSummaryTypeDef = TypedDict(
+    "DestinationSummaryTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
-    },
-)
-_OptionalDestinationSummaryTypeDef = TypedDict(
-    "_OptionalDestinationSummaryTypeDef",
-    {
         "UnhealthySince": datetime,
     },
-    total=False,
 )
 
-class DestinationSummaryTypeDef(
-    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
-):
-    pass
-
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
-    total=False,
 )
 
-_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
-    "_RequiredEventStreamDestinationDetailsTypeDef",
+EventStreamDestinationDetailsTypeDef = TypedDict(
+    "EventStreamDestinationDetailsTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
-    },
-)
-_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
-    "_OptionalEventStreamDestinationDetailsTypeDef",
-    {
         "UnhealthySince": datetime,
         "Message": str,
     },
-    total=False,
 )
 
-class EventStreamDestinationDetailsTypeDef(
-    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
-):
-    pass
+S3ExportingConfigOutputTypeDef = TypedDict(
+    "S3ExportingConfigOutputTypeDef",
+    {
+        "S3BucketName": str,
+        "S3KeyName": str,
+    },
+)
 
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
@@ -611,15 +624,14 @@
 
 S3ExportingLocationTypeDef = TypedDict(
     "S3ExportingLocationTypeDef",
     {
         "S3BucketName": str,
         "S3KeyName": str,
     },
-    total=False,
 )
 
 FieldSourceProfileIdsTypeDef = TypedDict(
     "FieldSourceProfileIdsTypeDef",
     {
         "AccountNumber": str,
         "AdditionalInformation": str,
@@ -648,26 +660,14 @@
 
 FoundByKeyValueTypeDef = TypedDict(
     "FoundByKeyValueTypeDef",
     {
         "KeyName": str,
         "Values": List[str],
     },
-    total=False,
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
@@ -679,25 +679,14 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -720,41 +709,24 @@
 JobStatsTypeDef = TypedDict(
     "JobStatsTypeDef",
     {
         "NumberOfProfilesReviewed": int,
         "NumberOfMatchesFound": int,
         "NumberOfMergesDone": int,
     },
-    total=False,
 )
 
 GetIntegrationRequestRequestTypeDef = TypedDict(
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -774,51 +746,72 @@
 MatchItemTypeDef = TypedDict(
     "MatchItemTypeDef",
     {
         "MatchId": str,
         "ProfileIds": List[str],
         "ConfidenceScore": float,
     },
-    total=False,
 )
 
 GetProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-ObjectTypeFieldTypeDef = TypedDict(
-    "ObjectTypeFieldTypeDef",
+ObjectTypeFieldOutputTypeDef = TypedDict(
+    "ObjectTypeFieldOutputTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
-    total=False,
 )
 
-ObjectTypeKeyTypeDef = TypedDict(
-    "ObjectTypeKeyTypeDef",
+ObjectTypeKeyOutputTypeDef = TypedDict(
+    "ObjectTypeKeyOutputTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
-    total=False,
 )
 
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
 )
 
+_RequiredGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "MatchType": MatchTypeType,
+        "SearchKey": str,
+        "SearchValue": str,
+    },
+)
+_OptionalGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetSimilarProfilesRequestRequestTypeDef(
+    _RequiredGetSimilarProfilesRequestRequestTypeDef,
+    _OptionalGetSimilarProfilesRequestRequestTypeDef,
+):
+    pass
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -848,14 +841,22 @@
     "IncrementalPullConfigTypeDef",
     {
         "DatetimeTypeFieldName": str,
     },
     total=False,
 )
 
+JobScheduleOutputTypeDef = TypedDict(
+    "JobScheduleOutputTypeDef",
+    {
+        "DayOfTheWeek": JobScheduleDayOfTheWeekType,
+        "Time": str,
+    },
+)
+
 JobScheduleTypeDef = TypedDict(
     "JobScheduleTypeDef",
     {
         "DayOfTheWeek": JobScheduleDayOfTheWeekType,
         "Time": str,
     },
 )
@@ -878,51 +879,39 @@
 
 class ListAccountIntegrationsRequestRequestTypeDef(
     _RequiredListAccountIntegrationsRequestRequestTypeDef,
     _OptionalListAccountIntegrationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListIntegrationItemTypeDef = TypedDict(
-    "_RequiredListIntegrationItemTypeDef",
+ListIntegrationItemTypeDef = TypedDict(
+    "ListIntegrationItemTypeDef",
     {
         "DomainName": str,
         "Uri": str,
+        "ObjectTypeName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-    },
-)
-_OptionalListIntegrationItemTypeDef = TypedDict(
-    "_OptionalListIntegrationItemTypeDef",
-    {
-        "ObjectTypeName": str,
         "Tags": Dict[str, str],
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
     },
-    total=False,
 )
 
-class ListIntegrationItemTypeDef(
-    _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
-):
-    pass
-
 ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -946,15 +935,14 @@
     "ListCalculatedAttributeForProfileItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "IsDataPartial": str,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
     {
         "DomainName": str,
         "ProfileId": str,
@@ -971,62 +959,43 @@
 
 class ListCalculatedAttributesForProfileRequestRequestTypeDef(
     _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
     _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDomainItemTypeDef = TypedDict(
-    "_RequiredListDomainItemTypeDef",
+ListDomainItemTypeDef = TypedDict(
+    "ListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-    },
-)
-_OptionalListDomainItemTypeDef = TypedDict(
-    "_OptionalListDomainItemTypeDef",
-    {
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class ListDomainItemTypeDef(_RequiredListDomainItemTypeDef, _OptionalListDomainItemTypeDef):
-    pass
-
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1081,44 +1050,32 @@
 )
 
 class ListIntegrationsRequestRequestTypeDef(
     _RequiredListIntegrationsRequestRequestTypeDef, _OptionalListIntegrationsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListProfileObjectTypeItemTypeDef = TypedDict(
-    "_RequiredListProfileObjectTypeItemTypeDef",
+ListProfileObjectTypeItemTypeDef = TypedDict(
+    "ListProfileObjectTypeItemTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
-    },
-)
-_OptionalListProfileObjectTypeItemTypeDef = TypedDict(
-    "_OptionalListProfileObjectTypeItemTypeDef",
-    {
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class ListProfileObjectTypeItemTypeDef(
-    _RequiredListProfileObjectTypeItemTypeDef, _OptionalListProfileObjectTypeItemTypeDef
-):
-    pass
-
 ListProfileObjectTypeTemplateItemTypeDef = TypedDict(
     "ListProfileObjectTypeTemplateItemTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
     },
-    total=False,
 )
 
 ListProfileObjectTypeTemplatesRequestRequestTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1150,37 +1107,49 @@
 ListProfileObjectsItemTypeDef = TypedDict(
     "ListProfileObjectsItemTypeDef",
     {
         "ObjectTypeName": str,
         "ProfileObjectUniqueKey": str,
         "Object": str,
     },
-    total=False,
 )
 
 ObjectFilterTypeDef = TypedDict(
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+_RequiredListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRuleBasedMatchesRequestRequestTypeDef",
     {
-        "resourceArn": str,
+        "DomainName": str,
     },
 )
+_OptionalListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+class ListRuleBasedMatchesRequestRequestTypeDef(
+    _RequiredListRuleBasedMatchesRequestRequestTypeDef,
+    _OptionalListRuleBasedMatchesRequestRequestTypeDef,
+):
+    pass
+
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
     },
 )
 
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
@@ -1219,76 +1188,56 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
+MatchingRuleOutputTypeDef = TypedDict(
+    "MatchingRuleOutputTypeDef",
     {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rule": List[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+MatchingRuleTypeDef = TypedDict(
+    "MatchingRuleTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Rule": Sequence[str],
+    },
+)
+
+ObjectTypeFieldTypeDef = TypedDict(
+    "ObjectTypeFieldTypeDef",
+    {
+        "Source": str,
+        "Target": str,
+        "ContentType": FieldContentTypeType,
     },
     total=False,
 )
 
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
+ObjectTypeKeyTypeDef = TypedDict(
+    "ObjectTypeKeyTypeDef",
     {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StandardIdentifiers": Sequence[StandardIdentifierType],
+        "FieldNames": Sequence[str],
     },
+    total=False,
 )
 
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-)
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1391,19 +1340,202 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
+    {
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1469,41 +1601,56 @@
     pass
 
 WorkflowAttributesTypeDef = TypedDict(
     "WorkflowAttributesTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowAttributesTypeDef,
     },
-    total=False,
 )
 
 WorkflowMetricsTypeDef = TypedDict(
     "WorkflowMetricsTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowMetricsTypeDef,
     },
-    total=False,
 )
 
 WorkflowStepItemTypeDef = TypedDict(
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
-    total=False,
+)
+
+AttributeDetailsOutputTypeDef = TypedDict(
+    "AttributeDetailsOutputTypeDef",
+    {
+        "Attributes": List[AttributeItemOutputTypeDef],
+        "Expression": str,
+    },
 )
 
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
+AutoMergingOutputTypeDef = TypedDict(
+    "AutoMergingOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Consolidation": ConsolidationOutputTypeDef,
+        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "MinAllowedConfidenceScoreForMerging": float,
+    },
+)
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1537,14 +1684,23 @@
 
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "Range": RangeOutputTypeDef,
+        "ObjectCount": int,
+        "Threshold": ThresholdOutputTypeDef,
+    },
+)
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -1567,49 +1723,45 @@
     },
     total=False,
 )
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-_RequiredEventStreamSummaryTypeDef = TypedDict(
-    "_RequiredEventStreamSummaryTypeDef",
+EventStreamSummaryTypeDef = TypedDict(
+    "EventStreamSummaryTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
         "EventStreamArn": str,
         "State": EventStreamStateType,
-    },
-)
-_OptionalEventStreamSummaryTypeDef = TypedDict(
-    "_OptionalEventStreamSummaryTypeDef",
-    {
         "StoppedSince": datetime,
         "DestinationSummary": DestinationSummaryTypeDef,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class EventStreamSummaryTypeDef(
-    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
-):
-    pass
-
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportingConfigOutputTypeDef = TypedDict(
+    "ExportingConfigOutputTypeDef",
+    {
+        "S3Exporting": S3ExportingConfigOutputTypeDef,
     },
 )
 
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
@@ -1618,15 +1770,14 @@
 )
 
 ExportingLocationTypeDef = TypedDict(
     "ExportingLocationTypeDef",
     {
         "S3Exporting": S3ExportingLocationTypeDef,
     },
-    total=False,
 )
 
 _RequiredMergeProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredMergeProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
         "MainProfileId": str,
@@ -1662,187 +1813,177 @@
         "PhoneNumber": str,
         "MobilePhoneNumber": str,
         "HomePhoneNumber": str,
         "BusinessPhoneNumber": str,
         "EmailAddress": str,
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
-        "Address": AddressTypeDef,
-        "ShippingAddress": AddressTypeDef,
-        "MailingAddress": AddressTypeDef,
-        "BillingAddress": AddressTypeDef,
+        "Address": AddressOutputTypeDef,
+        "ShippingAddress": AddressOutputTypeDef,
+        "MailingAddress": AddressOutputTypeDef,
+        "BillingAddress": AddressOutputTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
-    total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
+        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1867,18 +2008,47 @@
     pass
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
+    },
+)
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
+    pass
+
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -1944,132 +2114,156 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
-        "DomainName": str,
         "CalculatedAttributeName": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Statistic": StatisticType,
-    },
-)
-_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
-    {
         "DisplayName": str,
         "Description": str,
-        "Conditions": ConditionsTypeDef,
-        "Tags": Mapping[str, str],
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Conditions": ConditionsOutputTypeDef,
+        "Statistic": StatisticType,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-):
-    pass
-
-CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Conditions": ConditionsTypeDef,
-        "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeDefinitionResponseTypeDef",
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
-        "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsTypeDef,
+        "Conditions": ConditionsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
     },
 )
-_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
 ):
     pass
 
-UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
+        "DomainName": str,
         "CalculatedAttributeName": str,
+    },
+)
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
         "DisplayName": str,
         "Description": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MatchingResponseTypeDef = TypedDict(
+    "MatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "JobSchedule": JobScheduleOutputTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
+        "ExportingConfig": ExportingConfigOutputTypeDef,
+    },
+)
+
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleOutputTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
+        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "ExportingConfig": ExportingConfigOutputTypeDef,
     },
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
@@ -2084,40 +2278,53 @@
     },
     total=False,
 )
 
 class MatchingRequestTypeDef(_RequiredMatchingRequestTypeDef, _OptionalMatchingRequestTypeDef):
     pass
 
-MatchingResponseTypeDef = TypedDict(
-    "MatchingResponseTypeDef",
+_RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_RequiredRuleBasedMatchingRequestTypeDef",
     {
         "Enabled": bool,
-        "JobSchedule": JobScheduleTypeDef,
-        "AutoMerging": AutoMergingTypeDef,
+    },
+)
+_OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_OptionalRuleBasedMatchingRequestTypeDef",
+    {
+        "MatchingRules": Sequence[MatchingRuleTypeDef],
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
+class RuleBasedMatchingRequestTypeDef(
+    _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
+):
+    pass
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
-        "AutoMerging": AutoMergingTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2125,23 +2332,22 @@
         "Status": IdentityResolutionJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "JobStats": JobStatsTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "Message": str,
     },
-    total=False,
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2173,27 +2379,77 @@
     },
     total=False,
 )
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Stats": DomainStatsTypeDef,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainResponseTypeDef = TypedDict(
+    "UpdateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
@@ -2209,76 +2465,31 @@
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainRequestRequestTypeDef",
     {
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class UpdateDomainRequestRequestTypeDef(
     _RequiredUpdateDomainRequestRequestTypeDef, _OptionalUpdateDomainRequestRequestTypeDef
 ):
     pass
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Stats": DomainStatsTypeDef,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainResponseTypeDef = TypedDict(
-    "UpdateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.0
-Summary: Type annotations for boto3.CustomerProfiles 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.CustomerProfiles 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,27 +298,30 @@
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -332,179 +335,203 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
+    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
+    AttributeTypesSelectorOutputTypeDef,
+    AttributeTypesSelectorTypeDef,
+    ConflictResolutionOutputTypeDef,
+    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeOutputTypeDef,
+    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
+    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldTypeDef,
-    ObjectTypeKeyTypeDef,
+    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
+    GetSimilarProfilesRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
+    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
+    ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
-    MergeProfilesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
+    MatchingRuleOutputTypeDef,
+    MatchingRuleTypeDef,
+    ObjectTypeFieldTypeDef,
+    ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
+    AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
+    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingRequestTypeDef,
     MatchingResponseTypeDef,
+    RuleBasedMatchingResponseTypeDef,
+    MatchingRequestTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.0/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.0/setup.py` & `mypy-boto3-customer-profiles-1.28.11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CustomerProfiles 1.28.11 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

