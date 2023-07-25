# Comparing `tmp/mypy-boto3-wisdom-1.28.0.tar.gz` & `tmp/mypy-boto3-wisdom-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.28.0.tar", last modified: Thu Jul  6 21:00:51 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.28.0.tar` & `mypy-boto3-wisdom-1.28.11.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.342459 mypy-boto3-wisdom-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-06 21:00:51.342459 mypy-boto3-wisdom-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.338459 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-06 20:58:06.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-06 20:58:06.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-06 20:58:07.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-06 20:58:07.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-06 20:58:07.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-06 20:58:07.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-07-06 20:58:08.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35511 2023-07-06 20:58:07.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.342459 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 21:00:51.000000 mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:51.342459 mypy-boto3-wisdom-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:58:02.000000 mypy-boto3-wisdom-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33923 2023-07-25 19:49:03.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/setup.py
```

### Comparing `mypy-boto3-wisdom-1.28.0/LICENSE` & `mypy-boto3-wisdom-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/PKG-INFO` & `mypy-boto3-wisdom-1.28.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,111 +354,117 @@
 ### Typed dictionaries
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
+    AssistantIntegrationConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
     HighlightTypeDef,
     FilterTypeDef,
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    RenderingConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
+    SessionIntegrationConfigurationTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
+    SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
     SearchContentRequestSearchContentPaginateTypeDef,
     SearchSessionsRequestRequestTypeDef,
     SearchSessionsRequestSearchSessionsPaginateTypeDef,
     RecommendationTriggerTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
     CreateKnowledgeBaseResponseTypeDef,
     GetKnowledgeBaseResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
     ListKnowledgeBasesResponseTypeDef,
     CreateAssistantAssociationResponseTypeDef,
     GetAssistantAssociationResponseTypeDef,
     ListAssistantAssociationsResponseTypeDef,
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.0/README.md` & `mypy-boto3-wisdom-1.28.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,111 +322,117 @@
 ### Typed dictionaries
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
+    AssistantIntegrationConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
     HighlightTypeDef,
     FilterTypeDef,
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    RenderingConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
+    SessionIntegrationConfigurationTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
+    SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
     SearchContentRequestSearchContentPaginateTypeDef,
     SearchSessionsRequestRequestTypeDef,
     SearchSessionsRequestSearchSessionsPaginateTypeDef,
     RecommendationTriggerTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
     CreateKnowledgeBaseResponseTypeDef,
     GetKnowledgeBaseResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
     ListKnowledgeBasesResponseTypeDef,
     CreateAssistantAssociationResponseTypeDef,
     GetAssistantAssociationResponseTypeDef,
     ListAssistantAssociationsResponseTypeDef,
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.28.11\nVersion:         1.28.11\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,15 @@
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

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,15 @@
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

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,129 +53,120 @@
     "ListContentsPaginator",
     "ListKnowledgeBasesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchSessionsPaginator",
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
 class ListAssistantAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
         """
 
-
 class ListAssistantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
         """
 
-
 class ListContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
         """
 
-
 class ListKnowledgeBasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
         """
 
-
 class QueryAssistantPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
         """
 
-
 class SearchContentPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
         """
 
-
 class SearchSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,120 +53,129 @@
     "ListContentsPaginator",
     "ListKnowledgeBasesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchSessionsPaginator",
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
 class ListAssistantAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
         """
 
+
 class ListAssistantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
         """
 
+
 class ListContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
         """
 
+
 class ListKnowledgeBasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
         """
 
+
 class QueryAssistantPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
         """
 
+
 class SearchContentPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
         """
 
+
 class SearchSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
+    from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -31,109 +31,123 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
-    "ServerSideEncryptionConfigurationTypeDef",
+    "AssistantIntegrationConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "HighlightTypeDef",
     "FilterTypeDef",
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "RenderingConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
+    "SessionIntegrationConfigurationTypeDef",
     "StartContentUploadRequestRequestTypeDef",
-    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
-    "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
+    "StartContentUploadResponseTypeDef",
+    "UpdateContentResponseTypeDef",
+    "CreateAssistantRequestRequestTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SessionDataTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     "RecommendationTriggerTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
+AppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "AppIntegrationsConfigurationOutputTypeDef",
+    {
+        "appIntegrationArn": str,
+        "objectFields": List[str],
+    },
+)
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -161,94 +175,95 @@
 
 KnowledgeBaseAssociationDataTypeDef = TypedDict(
     "KnowledgeBaseAssociationDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
-    total=False,
 )
 
-ServerSideEncryptionConfigurationTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationTypeDef",
+AssistantIntegrationConfigurationTypeDef = TypedDict(
+    "AssistantIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+)
+
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
-    total=False,
 )
 
-_RequiredContentDataTypeDef = TypedDict(
-    "_RequiredContentDataTypeDef",
+ContentDataTypeDef = TypedDict(
+    "ContentDataTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
+        "linkOutUri": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
+        "tags": Dict[str, str],
         "title": str,
         "url": str,
         "urlExpiry": datetime,
     },
 )
-_OptionalContentDataTypeDef = TypedDict(
-    "_OptionalContentDataTypeDef",
-    {
-        "linkOutUri": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ContentDataTypeDef(_RequiredContentDataTypeDef, _OptionalContentDataTypeDef):
-    pass
-
 
 ContentReferenceTypeDef = TypedDict(
     "ContentReferenceTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
-    total=False,
 )
 
-_RequiredContentSummaryTypeDef = TypedDict(
-    "_RequiredContentSummaryTypeDef",
+ContentSummaryTypeDef = TypedDict(
+    "ContentSummaryTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
+        "tags": Dict[str, str],
         "title": str,
     },
 )
-_OptionalContentSummaryTypeDef = TypedDict(
-    "_OptionalContentSummaryTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "tags": Dict[str, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
-    pass
-
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+    total=False,
+)
 
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
@@ -301,36 +316,14 @@
 
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSessionDataTypeDef = TypedDict(
-    "_RequiredSessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-    },
-)
-_OptionalSessionDataTypeDef = TypedDict(
-    "_OptionalSessionDataTypeDef",
-    {
-        "description": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
-    pass
-
-
 DeleteAssistantAssociationRequestRequestTypeDef = TypedDict(
     "DeleteAssistantAssociationRequestRequestTypeDef",
     {
         "assistantAssociationId": str,
         "assistantId": str,
     },
 )
@@ -359,15 +352,14 @@
 
 HighlightTypeDef = TypedDict(
     "HighlightTypeDef",
     {
         "beginOffsetInclusive": int,
         "endOffsetExclusive": int,
     },
-    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "field": Literal["NAME"],
         "operator": Literal["EQUALS"],
@@ -441,36 +433,31 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+RenderingConfigurationOutputTypeDef = TypedDict(
+    "RenderingConfigurationOutputTypeDef",
     {
-        "assistantId": str,
+        "templateUri": str,
     },
 )
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+
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
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -486,53 +473,23 @@
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -547,22 +504,14 @@
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
 
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -571,73 +520,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
-    total=False,
 )
 
 NotifyRecommendationsReceivedRequestRequestTypeDef = TypedDict(
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
-
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -658,61 +565,45 @@
 
 
 QueryRecommendationTriggerDataTypeDef = TypedDict(
     "QueryRecommendationTriggerDataTypeDef",
     {
         "text": str,
     },
-    total=False,
 )
 
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
     },
 )
 
-StartContentUploadRequestRequestTypeDef = TypedDict(
-    "StartContentUploadRequestRequestTypeDef",
+SessionIntegrationConfigurationTypeDef = TypedDict(
+    "SessionIntegrationConfigurationTypeDef",
     {
-        "contentType": str,
-        "knowledgeBaseId": str,
+        "topicIntegrationArn": str,
     },
 )
 
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
+StartContentUploadRequestRequestTypeDef = TypedDict(
+    "StartContentUploadRequestRequestTypeDef",
     {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": str,
+        "knowledgeBaseId": str,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -759,14 +650,21 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
+    },
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -797,66 +695,114 @@
 
 
 AssistantAssociationOutputDataTypeDef = TypedDict(
     "AssistantAssociationOutputDataTypeDef",
     {
         "knowledgeBaseAssociation": KnowledgeBaseAssociationDataTypeDef,
     },
-    total=False,
 )
 
-_RequiredAssistantDataTypeDef = TypedDict(
-    "_RequiredAssistantDataTypeDef",
+AssistantDataTypeDef = TypedDict(
+    "AssistantDataTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "name": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "status": AssistantStatusType,
+        "tags": Dict[str, str],
         "type": Literal["AGENT"],
     },
 )
-_OptionalAssistantDataTypeDef = TypedDict(
-    "_OptionalAssistantDataTypeDef",
+
+AssistantSummaryTypeDef = TypedDict(
+    "AssistantSummaryTypeDef",
     {
+        "assistantArn": str,
+        "assistantId": str,
         "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
+        "name": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "status": AssistantStatusType,
         "tags": Dict[str, str],
+        "type": Literal["AGENT"],
     },
-    total=False,
 )
 
+CreateContentResponseTypeDef = TypedDict(
+    "CreateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
-    pass
+GetContentResponseTypeDef = TypedDict(
+    "GetContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetContentSummaryResponseTypeDef = TypedDict(
+    "GetContentSummaryResponseTypeDef",
+    {
+        "contentSummary": ContentSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredAssistantSummaryTypeDef = TypedDict(
-    "_RequiredAssistantSummaryTypeDef",
+ListContentsResponseTypeDef = TypedDict(
+    "ListContentsResponseTypeDef",
     {
-        "assistantArn": str,
-        "assistantId": str,
-        "name": str,
-        "status": AssistantStatusType,
-        "type": Literal["AGENT"],
+        "contentSummaries": List[ContentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssistantSummaryTypeDef = TypedDict(
-    "_OptionalAssistantSummaryTypeDef",
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+SearchContentResponseTypeDef = TypedDict(
+    "SearchContentResponseTypeDef",
+    {
+        "contentSummaries": List[ContentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
-    pass
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssistantRequestRequestTypeDef",
     {
         "name": str,
         "type": Literal["AGENT"],
     },
@@ -875,306 +821,270 @@
 
 class CreateAssistantRequestRequestTypeDef(
     _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
 ):
     pass
 
 
-CreateContentResponseTypeDef = TypedDict(
-    "CreateContentResponseTypeDef",
+DocumentTextTypeDef = TypedDict(
+    "DocumentTextTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "highlights": List[HighlightTypeDef],
+        "text": str,
     },
 )
 
-GetContentResponseTypeDef = TypedDict(
-    "GetContentResponseTypeDef",
+SearchExpressionTypeDef = TypedDict(
+    "SearchExpressionTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
     },
 )
 
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assistantId": str,
     },
 )
-
-GetContentSummaryResponseTypeDef = TypedDict(
-    "GetContentSummaryResponseTypeDef",
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListContentsResponseTypeDef = TypedDict(
-    "ListContentsResponseTypeDef",
+
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
+
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     {
-        "contentSummaries": List[ContentSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SearchContentResponseTypeDef = TypedDict(
-    "SearchContentResponseTypeDef",
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
     {
-        "contentSummaries": List[ContentSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "knowledgeBaseId": str,
     },
 )
-
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
     {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
+
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
+
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DocumentTextTypeDef = TypedDict(
-    "DocumentTextTypeDef",
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "highlights": List[HighlightTypeDef],
-        "text": str,
+        "assistantId": str,
+        "queryText": str,
     },
-    total=False,
 )
-
-SearchExpressionTypeDef = TypedDict(
-    "SearchExpressionTypeDef",
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
+):
+    pass
+
+
 NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
     },
-    total=False,
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
-    {
-        "knowledgeBaseType": KnowledgeBaseTypeType,
-        "name": str,
-    },
-)
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+SessionDataTypeDef = TypedDict(
+    "SessionDataTypeDef",
     {
-        "clientToken": str,
         "description": str,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredKnowledgeBaseDataTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseDataTypeDef",
+KnowledgeBaseDataTypeDef = TypedDict(
+    "KnowledgeBaseDataTypeDef",
     {
+        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
+        "lastContentModificationTime": datetime,
         "name": str,
+        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "status": KnowledgeBaseStatusType,
+        "tags": Dict[str, str],
     },
 )
-_OptionalKnowledgeBaseDataTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseDataTypeDef",
+
+KnowledgeBaseSummaryTypeDef = TypedDict(
+    "KnowledgeBaseSummaryTypeDef",
     {
         "description": str,
-        "lastContentModificationTime": datetime,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "knowledgeBaseArn": str,
+        "knowledgeBaseId": str,
+        "knowledgeBaseType": KnowledgeBaseTypeType,
+        "name": str,
+        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
+        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class KnowledgeBaseDataTypeDef(
-    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
-):
-    pass
-
-
-_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseSummaryTypeDef",
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
-        "knowledgeBaseArn": str,
-        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
-        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseSummaryTypeDef",
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class KnowledgeBaseSummaryTypeDef(
-    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredAssistantAssociationDataTypeDef = TypedDict(
-    "_RequiredAssistantAssociationDataTypeDef",
+AssistantAssociationDataTypeDef = TypedDict(
+    "AssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
-    },
-)
-_OptionalAssistantAssociationDataTypeDef = TypedDict(
-    "_OptionalAssistantAssociationDataTypeDef",
-    {
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class AssistantAssociationDataTypeDef(
-    _RequiredAssistantAssociationDataTypeDef, _OptionalAssistantAssociationDataTypeDef
-):
-    pass
-
-
-_RequiredAssistantAssociationSummaryTypeDef = TypedDict(
-    "_RequiredAssistantAssociationSummaryTypeDef",
+AssistantAssociationSummaryTypeDef = TypedDict(
+    "AssistantAssociationSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
-    },
-)
-_OptionalAssistantAssociationSummaryTypeDef = TypedDict(
-    "_OptionalAssistantAssociationSummaryTypeDef",
-    {
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class AssistantAssociationSummaryTypeDef(
-    _RequiredAssistantAssociationSummaryTypeDef, _OptionalAssistantAssociationSummaryTypeDef
-):
-    pass
-
-
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDocumentTypeDef = TypedDict(
-    "_RequiredDocumentTypeDef",
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
-    },
-)
-_OptionalDocumentTypeDef = TypedDict(
-    "_OptionalDocumentTypeDef",
-    {
         "excerpt": DocumentTextTypeDef,
         "title": DocumentTextTypeDef,
     },
-    total=False,
 )
 
-
-class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
-    pass
-
-
 _RequiredSearchContentRequestRequestTypeDef = TypedDict(
     "_RequiredSearchContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
@@ -1200,15 +1110,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
@@ -1246,15 +1156,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1270,126 +1180,118 @@
         "id": str,
         "recommendationIds": List[str],
         "source": RecommendationSourceTypeType,
         "type": Literal["QUERY"],
     },
 )
 
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecommendationDataTypeDef = TypedDict(
-    "_RequiredRecommendationDataTypeDef",
+RecommendationDataTypeDef = TypedDict(
+    "RecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
         "recommendationId": str,
-    },
-)
-_OptionalRecommendationDataTypeDef = TypedDict(
-    "_OptionalRecommendationDataTypeDef",
-    {
         "relevanceLevel": RelevanceLevelType,
         "relevanceScore": float,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
-    total=False,
 )
 
-
-class RecommendationDataTypeDef(
-    _RequiredRecommendationDataTypeDef, _OptionalRecommendationDataTypeDef
-):
-    pass
-
-
-_RequiredResultDataTypeDef = TypedDict(
-    "_RequiredResultDataTypeDef",
+ResultDataTypeDef = TypedDict(
+    "ResultDataTypeDef",
     {
         "document": DocumentTypeDef,
-        "resultId": str,
-    },
-)
-_OptionalResultDataTypeDef = TypedDict(
-    "_OptionalResultDataTypeDef",
-    {
         "relevanceScore": float,
+        "resultId": str,
     },
-    total=False,
 )
 
-
-class ResultDataTypeDef(_RequiredResultDataTypeDef, _OptionalResultDataTypeDef):
-    pass
-
-
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
+    from mypy_boto3_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -30,109 +30,123 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
-    "ServerSideEncryptionConfigurationTypeDef",
+    "AssistantIntegrationConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "HighlightTypeDef",
     "FilterTypeDef",
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "RenderingConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
+    "SessionIntegrationConfigurationTypeDef",
     "StartContentUploadRequestRequestTypeDef",
-    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
-    "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
+    "StartContentUploadResponseTypeDef",
+    "UpdateContentResponseTypeDef",
+    "CreateAssistantRequestRequestTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SessionDataTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     "RecommendationTriggerTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
+AppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "AppIntegrationsConfigurationOutputTypeDef",
+    {
+        "appIntegrationArn": str,
+        "objectFields": List[str],
+    },
+)
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -158,91 +172,96 @@
 
 KnowledgeBaseAssociationDataTypeDef = TypedDict(
     "KnowledgeBaseAssociationDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
-    total=False,
 )
 
-ServerSideEncryptionConfigurationTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationTypeDef",
+AssistantIntegrationConfigurationTypeDef = TypedDict(
+    "AssistantIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+)
+
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
-    total=False,
 )
 
-_RequiredContentDataTypeDef = TypedDict(
-    "_RequiredContentDataTypeDef",
+ContentDataTypeDef = TypedDict(
+    "ContentDataTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
+        "linkOutUri": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
+        "tags": Dict[str, str],
         "title": str,
         "url": str,
         "urlExpiry": datetime,
     },
 )
-_OptionalContentDataTypeDef = TypedDict(
-    "_OptionalContentDataTypeDef",
-    {
-        "linkOutUri": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class ContentDataTypeDef(_RequiredContentDataTypeDef, _OptionalContentDataTypeDef):
-    pass
 
 ContentReferenceTypeDef = TypedDict(
     "ContentReferenceTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
-    total=False,
 )
 
-_RequiredContentSummaryTypeDef = TypedDict(
-    "_RequiredContentSummaryTypeDef",
+ContentSummaryTypeDef = TypedDict(
+    "ContentSummaryTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
+        "tags": Dict[str, str],
         "title": str,
     },
 )
-_OptionalContentSummaryTypeDef = TypedDict(
-    "_OptionalContentSummaryTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
     {
-        "tags": Dict[str, str],
+        "kmsKeyId": str,
     },
     total=False,
 )
 
-class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
-    pass
-
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -290,34 +309,14 @@
 )
 
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
-_RequiredSessionDataTypeDef = TypedDict(
-    "_RequiredSessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-    },
-)
-_OptionalSessionDataTypeDef = TypedDict(
-    "_OptionalSessionDataTypeDef",
-    {
-        "description": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
-    pass
-
 DeleteAssistantAssociationRequestRequestTypeDef = TypedDict(
     "DeleteAssistantAssociationRequestRequestTypeDef",
     {
         "assistantAssociationId": str,
         "assistantId": str,
     },
 )
@@ -346,15 +345,14 @@
 
 HighlightTypeDef = TypedDict(
     "HighlightTypeDef",
     {
         "beginOffsetInclusive": int,
         "endOffsetExclusive": int,
     },
-    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "field": Literal["NAME"],
         "operator": Literal["EQUALS"],
@@ -426,34 +424,31 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+RenderingConfigurationOutputTypeDef = TypedDict(
+    "RenderingConfigurationOutputTypeDef",
     {
-        "assistantId": str,
+        "templateUri": str,
     },
 )
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+
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
 
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -467,51 +462,23 @@
 
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -524,22 +491,14 @@
 )
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -548,71 +507,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
-    total=False,
 )
 
 NotifyRecommendationsReceivedRequestRequestTypeDef = TypedDict(
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -631,61 +550,45 @@
     pass
 
 QueryRecommendationTriggerDataTypeDef = TypedDict(
     "QueryRecommendationTriggerDataTypeDef",
     {
         "text": str,
     },
-    total=False,
 )
 
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
     },
 )
 
-StartContentUploadRequestRequestTypeDef = TypedDict(
-    "StartContentUploadRequestRequestTypeDef",
+SessionIntegrationConfigurationTypeDef = TypedDict(
+    "SessionIntegrationConfigurationTypeDef",
     {
-        "contentType": str,
-        "knowledgeBaseId": str,
+        "topicIntegrationArn": str,
     },
 )
 
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
+StartContentUploadRequestRequestTypeDef = TypedDict(
+    "StartContentUploadRequestRequestTypeDef",
     {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": str,
+        "knowledgeBaseId": str,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -730,14 +633,21 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
+    },
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -766,62 +676,114 @@
     pass
 
 AssistantAssociationOutputDataTypeDef = TypedDict(
     "AssistantAssociationOutputDataTypeDef",
     {
         "knowledgeBaseAssociation": KnowledgeBaseAssociationDataTypeDef,
     },
-    total=False,
 )
 
-_RequiredAssistantDataTypeDef = TypedDict(
-    "_RequiredAssistantDataTypeDef",
+AssistantDataTypeDef = TypedDict(
+    "AssistantDataTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "name": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "status": AssistantStatusType,
+        "tags": Dict[str, str],
         "type": Literal["AGENT"],
     },
 )
-_OptionalAssistantDataTypeDef = TypedDict(
-    "_OptionalAssistantDataTypeDef",
+
+AssistantSummaryTypeDef = TypedDict(
+    "AssistantSummaryTypeDef",
     {
+        "assistantArn": str,
+        "assistantId": str,
         "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
+        "name": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "status": AssistantStatusType,
         "tags": Dict[str, str],
+        "type": Literal["AGENT"],
     },
-    total=False,
 )
 
-class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
-    pass
+CreateContentResponseTypeDef = TypedDict(
+    "CreateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredAssistantSummaryTypeDef = TypedDict(
-    "_RequiredAssistantSummaryTypeDef",
+GetContentResponseTypeDef = TypedDict(
+    "GetContentResponseTypeDef",
     {
-        "assistantArn": str,
-        "assistantId": str,
-        "name": str,
-        "status": AssistantStatusType,
-        "type": Literal["AGENT"],
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContentSummaryResponseTypeDef = TypedDict(
+    "GetContentSummaryResponseTypeDef",
+    {
+        "contentSummary": ContentSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssistantSummaryTypeDef = TypedDict(
-    "_OptionalAssistantSummaryTypeDef",
+
+ListContentsResponseTypeDef = TypedDict(
+    "ListContentsResponseTypeDef",
+    {
+        "contentSummaries": List[ContentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
-    pass
+SearchContentResponseTypeDef = TypedDict(
+    "SearchContentResponseTypeDef",
+    {
+        "contentSummaries": List[ContentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssistantRequestRequestTypeDef",
     {
         "name": str,
         "type": Literal["AGENT"],
     },
@@ -838,294 +800,262 @@
 )
 
 class CreateAssistantRequestRequestTypeDef(
     _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
 ):
     pass
 
-CreateContentResponseTypeDef = TypedDict(
-    "CreateContentResponseTypeDef",
+DocumentTextTypeDef = TypedDict(
+    "DocumentTextTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "highlights": List[HighlightTypeDef],
+        "text": str,
     },
 )
 
-GetContentResponseTypeDef = TypedDict(
-    "GetContentResponseTypeDef",
+SearchExpressionTypeDef = TypedDict(
+    "SearchExpressionTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
     },
 )
 
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assistantId": str,
     },
 )
-
-GetContentSummaryResponseTypeDef = TypedDict(
-    "GetContentSummaryResponseTypeDef",
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListContentsResponseTypeDef = TypedDict(
-    "ListContentsResponseTypeDef",
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     {
-        "contentSummaries": List[ContentSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SearchContentResponseTypeDef = TypedDict(
-    "SearchContentResponseTypeDef",
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
     {
-        "contentSummaries": List[ContentSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "knowledgeBaseId": str,
     },
 )
-
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
     {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DocumentTextTypeDef = TypedDict(
-    "DocumentTextTypeDef",
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "highlights": List[HighlightTypeDef],
-        "text": str,
+        "assistantId": str,
+        "queryText": str,
     },
-    total=False,
 )
-
-SearchExpressionTypeDef = TypedDict(
-    "SearchExpressionTypeDef",
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
+):
+    pass
+
 NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
     },
-    total=False,
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
-    {
-        "knowledgeBaseType": KnowledgeBaseTypeType,
-        "name": str,
-    },
-)
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+SessionDataTypeDef = TypedDict(
+    "SessionDataTypeDef",
     {
-        "clientToken": str,
         "description": str,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
-):
-    pass
-
-_RequiredKnowledgeBaseDataTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseDataTypeDef",
+KnowledgeBaseDataTypeDef = TypedDict(
+    "KnowledgeBaseDataTypeDef",
     {
+        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
+        "lastContentModificationTime": datetime,
         "name": str,
+        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "status": KnowledgeBaseStatusType,
+        "tags": Dict[str, str],
     },
 )
-_OptionalKnowledgeBaseDataTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseDataTypeDef",
+
+KnowledgeBaseSummaryTypeDef = TypedDict(
+    "KnowledgeBaseSummaryTypeDef",
     {
         "description": str,
-        "lastContentModificationTime": datetime,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "knowledgeBaseArn": str,
+        "knowledgeBaseId": str,
+        "knowledgeBaseType": KnowledgeBaseTypeType,
+        "name": str,
+        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
+        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class KnowledgeBaseDataTypeDef(
-    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
-):
-    pass
-
-_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseSummaryTypeDef",
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
-        "knowledgeBaseArn": str,
-        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
-        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseSummaryTypeDef",
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class KnowledgeBaseSummaryTypeDef(
-    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAssistantAssociationDataTypeDef = TypedDict(
-    "_RequiredAssistantAssociationDataTypeDef",
+AssistantAssociationDataTypeDef = TypedDict(
+    "AssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
-    },
-)
-_OptionalAssistantAssociationDataTypeDef = TypedDict(
-    "_OptionalAssistantAssociationDataTypeDef",
-    {
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class AssistantAssociationDataTypeDef(
-    _RequiredAssistantAssociationDataTypeDef, _OptionalAssistantAssociationDataTypeDef
-):
-    pass
-
-_RequiredAssistantAssociationSummaryTypeDef = TypedDict(
-    "_RequiredAssistantAssociationSummaryTypeDef",
+AssistantAssociationSummaryTypeDef = TypedDict(
+    "AssistantAssociationSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
-    },
-)
-_OptionalAssistantAssociationSummaryTypeDef = TypedDict(
-    "_OptionalAssistantAssociationSummaryTypeDef",
-    {
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class AssistantAssociationSummaryTypeDef(
-    _RequiredAssistantAssociationSummaryTypeDef, _OptionalAssistantAssociationSummaryTypeDef
-):
-    pass
-
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDocumentTypeDef = TypedDict(
-    "_RequiredDocumentTypeDef",
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
-    },
-)
-_OptionalDocumentTypeDef = TypedDict(
-    "_OptionalDocumentTypeDef",
-    {
         "excerpt": DocumentTextTypeDef,
         "title": DocumentTextTypeDef,
     },
-    total=False,
 )
 
-class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
-    pass
-
 _RequiredSearchContentRequestRequestTypeDef = TypedDict(
     "_RequiredSearchContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
@@ -1149,15 +1079,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
     _OptionalSearchContentRequestSearchContentPaginateTypeDef,
@@ -1191,15 +1121,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
     _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1213,122 +1143,118 @@
         "id": str,
         "recommendationIds": List[str],
         "source": RecommendationSourceTypeType,
         "type": Literal["QUERY"],
     },
 )
 
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecommendationDataTypeDef = TypedDict(
-    "_RequiredRecommendationDataTypeDef",
+RecommendationDataTypeDef = TypedDict(
+    "RecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
         "recommendationId": str,
-    },
-)
-_OptionalRecommendationDataTypeDef = TypedDict(
-    "_OptionalRecommendationDataTypeDef",
-    {
         "relevanceLevel": RelevanceLevelType,
         "relevanceScore": float,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
-    total=False,
 )
 
-class RecommendationDataTypeDef(
-    _RequiredRecommendationDataTypeDef, _OptionalRecommendationDataTypeDef
-):
-    pass
-
-_RequiredResultDataTypeDef = TypedDict(
-    "_RequiredResultDataTypeDef",
+ResultDataTypeDef = TypedDict(
+    "ResultDataTypeDef",
     {
         "document": DocumentTypeDef,
-        "resultId": str,
-    },
-)
-_OptionalResultDataTypeDef = TypedDict(
-    "_OptionalResultDataTypeDef",
-    {
         "relevanceScore": float,
+        "resultId": str,
     },
-    total=False,
 )
 
-class ResultDataTypeDef(_RequiredResultDataTypeDef, _OptionalResultDataTypeDef):
-    pass
-
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,111 +354,117 @@
 ### Typed dictionaries
 
 `mypy_boto3_wisdom.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
+    AssistantIntegrationConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
     HighlightTypeDef,
     FilterTypeDef,
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    RenderingConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
+    SessionIntegrationConfigurationTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
+    SessionDataTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
     SearchContentRequestSearchContentPaginateTypeDef,
     SearchSessionsRequestRequestTypeDef,
     SearchSessionsRequestSearchSessionsPaginateTypeDef,
     RecommendationTriggerTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
     CreateKnowledgeBaseResponseTypeDef,
     GetKnowledgeBaseResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
     ListKnowledgeBasesResponseTypeDef,
     CreateAssistantAssociationResponseTypeDef,
     GetAssistantAssociationResponseTypeDef,
     ListAssistantAssociationsResponseTypeDef,
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_structure() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wisdom-1.28.0/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.0/setup.py` & `mypy-boto3-wisdom-1.28.11/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectWisdomService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

