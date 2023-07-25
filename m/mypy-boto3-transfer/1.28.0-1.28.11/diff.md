# Comparing `tmp/mypy-boto3-transfer-1.28.0.tar.gz` & `tmp/mypy-boto3-transfer-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.28.0.tar", last modified: Thu Jul  6 21:00:48 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.28.0.tar` & `mypy-boto3-transfer-1.28.11.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.794454 mypy-boto3-transfer-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46221 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46143 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-06 20:57:22.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-07-06 20:57:27.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59129 2023-07-06 20:57:26.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:48.794454 mypy-boto3-transfer-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:57:20.000000 mypy-boto3-transfer-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20953 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62188 2023-07-25 19:49:01.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62123 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/setup.py
```

### Comparing `mypy-boto3-transfer-1.28.0/LICENSE` & `mypy-boto3-transfer-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/PKG-INFO` & `mypy-boto3-transfer-1.28.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.0
-Summary: Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,37 +404,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
+    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
+    SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
+    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
+    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -443,146 +441,171 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    HomeDirectoryMapEntryOutputTypeDef,
+    PosixProfileOutputTypeDef,
+    TagOutputTypeDef,
+    SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    IdentityProviderDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
+    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
+    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
+    TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
+    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestConnectionResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
-    CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedConnectorTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateConnectorRequestRequestTypeDef,
+    UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
     DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
-    DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
+    CopyStepDetailsOutputTypeDef,
+    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_structure() -> As2ConnectorConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.0/README.md` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-transfer
+Version: 1.28.11
+Summary: Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,37 +404,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
+    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
+    SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
+    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
+    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -411,146 +441,171 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    HomeDirectoryMapEntryOutputTypeDef,
+    PosixProfileOutputTypeDef,
+    TagOutputTypeDef,
+    SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    IdentityProviderDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
+    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
+    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
+    TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
+    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestConnectionResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
-    CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedConnectorTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateConnectorRequestRequestTypeDef,
+    UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
     DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
-    DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
+    CopyStepDetailsOutputTypeDef,
+    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_structure() -> As2ConnectorConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Transfer 1.28.11\nVersion:         1.28.11\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,18 @@
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     PosixProfileTypeDef,
     ProtocolDetailsTypeDef,
+    SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
+    TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
@@ -203,22 +205,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_agreement)
         """
 
     def create_connector(
         self,
         *,
         Url: str,
-        As2Config: As2ConnectorConfigTypeDef,
         AccessRole: str,
+        As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
-        for the AS2 protocol.
+        for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
         """
 
     def create_profile(
         self,
@@ -324,15 +327,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_certificate)
         """
 
     def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the agreement that's specified in the provided `ConnectorId`.
+        Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_connector)
         """
 
     def delete_host_key(self, *, ServerId: str, HostKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -683,18 +686,25 @@
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
 
     def start_file_transfer(
-        self, *, ConnectorId: str, SendFilePaths: Sequence[str]
+        self,
+        *,
+        ConnectorId: str,
+        SendFilePaths: Sequence[str] = ...,
+        RetrieveFilePaths: Sequence[str] = ...,
+        LocalDirectoryPath: str = ...,
+        RemoteDirectoryPath: str = ...
     ) -> StartFileTransferResponseTypeDef:
         """
-        Begins an outbound file transfer to a remote AS2 server.
+        Begins a file transfer between local Amazon Web Services storage and a remote
+        AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_file_transfer)
         """
 
     def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -719,14 +729,22 @@
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#tag_resource)
         """
 
+    def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
+        """
+        Tests whether your SFTP connector is set up successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_connection)
+        """
+
     def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -807,15 +825,16 @@
     def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
-        LoggingRole: str = ...
+        LoggingRole: str = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,18 @@
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     PosixProfileTypeDef,
     ProtocolDetailsTypeDef,
+    SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
+    TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
@@ -194,22 +196,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_agreement)
         """
     def create_connector(
         self,
         *,
         Url: str,
-        As2Config: As2ConnectorConfigTypeDef,
         AccessRole: str,
+        As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
-        for the AS2 protocol.
+        for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
         """
     def create_profile(
         self,
         *,
@@ -307,15 +310,15 @@
         Deletes the certificate that's specified in the `CertificateId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_certificate)
         """
     def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the agreement that's specified in the provided `ConnectorId`.
+        Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_connector)
         """
     def delete_host_key(self, *, ServerId: str, HostKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the host key that's specified in the `HostKeyId` parameter.
@@ -631,18 +634,25 @@
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
     def start_file_transfer(
-        self, *, ConnectorId: str, SendFilePaths: Sequence[str]
+        self,
+        *,
+        ConnectorId: str,
+        SendFilePaths: Sequence[str] = ...,
+        RetrieveFilePaths: Sequence[str] = ...,
+        LocalDirectoryPath: str = ...,
+        RemoteDirectoryPath: str = ...
     ) -> StartFileTransferResponseTypeDef:
         """
-        Begins an outbound file transfer to a remote AS2 server.
+        Begins a file transfer between local Amazon Web Services storage and a remote
+        AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_file_transfer)
         """
     def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `OFFLINE` to
@@ -663,14 +673,21 @@
         """
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#tag_resource)
         """
+    def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
+        """
+        Tests whether your SFTP connector is set up successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_connection)
+        """
     def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -746,15 +763,16 @@
     def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
-        LoggingRole: str = ...
+        LoggingRole: str = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
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
@@ -506,14 +507,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,15 @@
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
@@ -504,14 +505,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,166 +87,163 @@
 class ListAccessesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listaccessespaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listaccessespaginator)
         """
 
 
 class ListAgreementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listagreementspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAgreementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listagreementspaginator)
         """
 
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listcertificatespaginator)
         """
 
 
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listconnectorspaginator)
         """
 
 
 class ListExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listexecutionspaginator)
         """
 
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ProfileType: ProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProfileType: ProfileTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listprofilespaginator)
         """
 
 
 class ListSecurityPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listsecuritypoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listsecuritypoliciespaginator)
         """
 
 
 class ListServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listserverspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listserverspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listuserspaginator)
         """
 
 
 class ListWorkflowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listworkflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -84,156 +84,153 @@
 class ListAccessesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listaccessespaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listaccessespaginator)
         """
 
 class ListAgreementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listagreementspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAgreementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listagreementspaginator)
         """
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listcertificatespaginator)
         """
 
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listconnectorspaginator)
         """
 
 class ListExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listexecutionspaginator)
         """
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ProfileType: ProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProfileType: ProfileTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listprofilespaginator)
         """
 
 class ListSecurityPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listsecuritypoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listsecuritypoliciespaginator)
         """
 
 class ListServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listserverspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listserverspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listtagsforresourcepaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listuserspaginator)
         """
 
 class ListWorkflowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listworkflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transfer service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
+    from mypy_boto3_transfer.type_defs import As2ConnectorConfigOutputTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -49,37 +49,35 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "As2ConnectorConfigOutputTypeDef",
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
-    "CreateAccessResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAgreementResponseTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateProfileResponseTypeDef",
+    "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CreateServerResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
+    "CustomStepDetailsOutputTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
     "DeleteSshPublicKeyRequestRequestTypeDef",
+    "DeleteStepDetailsOutputTypeDef",
     "DeleteStepDetailsTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DescribeAccessRequestRequestTypeDef",
     "DescribeAgreementRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -88,144 +86,184 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
+    "HomeDirectoryMapEntryOutputTypeDef",
+    "PosixProfileOutputTypeDef",
+    "TagOutputTypeDef",
+    "SftpConnectorConfigOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "EndpointDetailsOutputTypeDef",
+    "IdentityProviderDetailsOutputTypeDef",
+    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
+    "EfsFileLocationOutputTypeDef",
     "EfsFileLocationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "ImportSshPublicKeyResponseTypeDef",
+    "S3InputFileLocationOutputTypeDef",
     "S3InputFileLocationTypeDef",
-    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
-    "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListedCertificateTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListedConnectorTypeDef",
-    "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListExecutionsRequestRequestTypeDef",
     "ListHostKeysRequestRequestTypeDef",
     "ListedHostKeyTypeDef",
-    "ListProfilesRequestListProfilesPaginateTypeDef",
     "ListProfilesRequestRequestTypeDef",
     "ListedProfileTypeDef",
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
-    "ListSecurityPoliciesResponseTypeDef",
-    "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3TagOutputTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
-    "StartFileTransferResponseTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
+    "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
-    "TestIdentityProviderResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAccessResponseTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateAgreementResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
-    "UpdateCertificateResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
-    "UpdateHostKeyResponseTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "UpdateProfileResponseTypeDef",
-    "UpdateServerResponseTypeDef",
-    "UpdateUserResponseTypeDef",
+    "WorkflowDetailOutputTypeDef",
     "WorkflowDetailTypeDef",
-    "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
-    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "CreateAccessResponseTypeDef",
+    "CreateAgreementResponseTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "CreateServerResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "ImportHostKeyResponseTypeDef",
+    "ImportSshPublicKeyResponseTypeDef",
+    "ListSecurityPoliciesResponseTypeDef",
+    "StartFileTransferResponseTypeDef",
+    "TestConnectionResponseTypeDef",
+    "TestIdentityProviderResponseTypeDef",
+    "UpdateAccessResponseTypeDef",
+    "UpdateAgreementResponseTypeDef",
+    "UpdateCertificateResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
+    "UpdateHostKeyResponseTypeDef",
+    "UpdateProfileResponseTypeDef",
+    "UpdateServerResponseTypeDef",
+    "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
-    "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DescribedAgreementTypeDef",
-    "DescribedCertificateTypeDef",
-    "DescribedConnectorTypeDef",
-    "DescribedHostKeyTypeDef",
-    "DescribedProfileTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateConnectorRequestRequestTypeDef",
+    "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
+    "DescribedAccessTypeDef",
+    "DescribedAgreementTypeDef",
+    "DescribedCertificateTypeDef",
+    "DescribedHostKeyTypeDef",
+    "DescribedProfileTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DescribedConnectorTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "InputFileLocationOutputTypeDef",
     "InputFileLocationTypeDef",
+    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "ListAgreementsRequestListAgreementsPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListExecutionsRequestListExecutionsPaginateTypeDef",
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    "ListServersRequestListServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAccessesResponseTypeDef",
     "ListAgreementsResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
+    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
     "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
+    "CopyStepDetailsOutputTypeDef",
+    "DecryptStepDetailsOutputTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "CreateServerRequestRequestTypeDef",
     "DescribedServerTypeDef",
+    "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "DescribedExecutionTypeDef",
+    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
     "DescribeWorkflowResponseTypeDef",
 )
 
+As2ConnectorConfigOutputTypeDef = TypedDict(
+    "As2ConnectorConfigOutputTypeDef",
+    {
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "MessageSubject": str,
+        "Compression": CompressionEnumType,
+        "EncryptionAlgorithm": EncryptionAlgType,
+        "SigningAlgorithm": SigningAlgType,
+        "MdnSigningAlgorithm": MdnSigningAlgType,
+        "MdnResponse": MdnResponseType,
+        "BasicAuthSecretId": str,
+    },
+)
+
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
@@ -262,53 +300,40 @@
 )
 
 
 class PosixProfileTypeDef(_RequiredPosixProfileTypeDef, _OptionalPosixProfileTypeDef):
     pass
 
 
-CreateAccessResponseTypeDef = TypedDict(
-    "CreateAccessResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAgreementResponseTypeDef = TypedDict(
-    "CreateAgreementResponseTypeDef",
+SftpConnectorConfigTypeDef = TypedDict(
+    "SftpConnectorConfigTypeDef",
     {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserSecretId": str,
+        "TrustedHostKeys": Sequence[str],
     },
+    total=False,
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
@@ -338,36 +363,21 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CreateServerResponseTypeDef = TypedDict(
-    "CreateServerResponseTypeDef",
+CustomStepDetailsOutputTypeDef = TypedDict(
+    "CustomStepDetailsOutputTypeDef",
     {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "Target": str,
+        "TimeoutSeconds": int,
+        "SourceFileLocation": str,
     },
 )
 
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
@@ -435,14 +445,22 @@
     {
         "ServerId": str,
         "SshPublicKeyId": str,
         "UserName": str,
     },
 )
 
+DeleteStepDetailsOutputTypeDef = TypedDict(
+    "DeleteStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "SourceFileLocation": str,
+    },
+)
+
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
     total=False,
@@ -519,39 +537,26 @@
 DescribeSecurityPolicyRequestRequestTypeDef = TypedDict(
     "DescribeSecurityPolicyRequestRequestTypeDef",
     {
         "SecurityPolicyName": str,
     },
 )
 
-_RequiredDescribedSecurityPolicyTypeDef = TypedDict(
-    "_RequiredDescribedSecurityPolicyTypeDef",
-    {
-        "SecurityPolicyName": str,
-    },
-)
-_OptionalDescribedSecurityPolicyTypeDef = TypedDict(
-    "_OptionalDescribedSecurityPolicyTypeDef",
+DescribedSecurityPolicyTypeDef = TypedDict(
+    "DescribedSecurityPolicyTypeDef",
     {
         "Fips": bool,
+        "SecurityPolicyName": str,
         "SshCiphers": List[str],
         "SshKexs": List[str],
         "SshMacs": List[str],
         "TlsCiphers": List[str],
     },
-    total=False,
 )
 
-
-class DescribedSecurityPolicyTypeDef(
-    _RequiredDescribedSecurityPolicyTypeDef, _OptionalDescribedSecurityPolicyTypeDef
-):
-    pass
-
-
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -575,46 +580,111 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
+HomeDirectoryMapEntryOutputTypeDef = TypedDict(
+    "HomeDirectoryMapEntryOutputTypeDef",
+    {
+        "Entry": str,
+        "Target": str,
+    },
+)
+
+PosixProfileOutputTypeDef = TypedDict(
+    "PosixProfileOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+        "SecondaryGids": List[int],
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+SftpConnectorConfigOutputTypeDef = TypedDict(
+    "SftpConnectorConfigOutputTypeDef",
+    {
+        "UserSecretId": str,
+        "TrustedHostKeys": List[str],
+    },
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
-    total=False,
+)
+
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
+    {
+        "AddressAllocationIds": List[str],
+        "SubnetIds": List[str],
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "SecurityGroupIds": List[str],
+    },
+)
+
+IdentityProviderDetailsOutputTypeDef = TypedDict(
+    "IdentityProviderDetailsOutputTypeDef",
+    {
+        "Url": str,
+        "InvocationRole": str,
+        "DirectoryId": str,
+        "Function": str,
+        "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
+    },
+)
+
+ProtocolDetailsOutputTypeDef = TypedDict(
+    "ProtocolDetailsOutputTypeDef",
+    {
+        "PassiveIp": str,
+        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
+        "SetStatOption": SetStatOptionType,
+        "As2Transports": List[Literal["HTTP"]],
+    },
 )
 
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
 )
 
-EfsFileLocationTypeDef = TypedDict(
-    "EfsFileLocationTypeDef",
+EfsFileLocationOutputTypeDef = TypedDict(
+    "EfsFileLocationOutputTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
-    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EfsFileLocationTypeDef = TypedDict(
+    "EfsFileLocationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileSystemId": str,
+        "Path": str,
     },
+    total=False,
 )
 
 ExecutionErrorTypeDef = TypedDict(
     "ExecutionErrorTypeDef",
     {
         "Type": ExecutionErrorTypeType,
         "Message": str,
@@ -625,84 +695,52 @@
     "S3FileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
-    total=False,
-)
-
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportHostKeyResponseTypeDef = TypedDict(
-    "ImportHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-ImportSshPublicKeyResponseTypeDef = TypedDict(
-    "ImportSshPublicKeyResponseTypeDef",
+S3InputFileLocationOutputTypeDef = TypedDict(
+    "S3InputFileLocationOutputTypeDef",
     {
-        "ServerId": str,
-        "SshPublicKeyId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Bucket": str,
+        "Key": str,
     },
 )
 
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
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
-class ListAccessesRequestListAccessesPaginateTypeDef(
-    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
-    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccessesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessesRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAccessesRequestRequestTypeDef = TypedDict(
@@ -725,39 +763,16 @@
     "ListedAccessTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
-    total=False,
 )
 
-_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAgreementsRequestListAgreementsPaginateTypeDef(
-    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
-    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAgreementsRequestRequestTypeDef = TypedDict(
@@ -783,23 +798,14 @@
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
-    total=False,
-)
-
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -815,23 +821,14 @@
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
-    total=False,
-)
-
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -842,39 +839,16 @@
 ListedConnectorTypeDef = TypedDict(
     "ListedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
-    total=False,
 )
 
-_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "WorkflowId": str,
-    },
-)
-_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExecutionsRequestListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 _OptionalListExecutionsRequestRequestTypeDef = TypedDict(
@@ -911,44 +885,24 @@
 
 class ListHostKeysRequestRequestTypeDef(
     _RequiredListHostKeysRequestRequestTypeDef, _OptionalListHostKeysRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListedHostKeyTypeDef = TypedDict(
-    "_RequiredListedHostKeyTypeDef",
+ListedHostKeyTypeDef = TypedDict(
+    "ListedHostKeyTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedHostKeyTypeDef = TypedDict(
-    "_OptionalListedHostKeyTypeDef",
-    {
         "HostKeyId": str,
         "Fingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
     },
-    total=False,
-)
-
-
-class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
-    pass
-
-
-ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListProfilesRequestListProfilesPaginateTypeDef",
-    {
-        "ProfileType": ProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -961,107 +915,48 @@
     "ListedProfileTypeDef",
     {
         "Arn": str,
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
-    total=False,
-)
-
-ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityPoliciesResponseTypeDef = TypedDict(
-    "ListSecurityPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecurityPolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServersRequestListServersPaginateTypeDef = TypedDict(
-    "ListServersRequestListServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListedServerTypeDef = TypedDict(
-    "_RequiredListedServerTypeDef",
+ListedServerTypeDef = TypedDict(
+    "ListedServerTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedServerTypeDef = TypedDict(
-    "_OptionalListedServerTypeDef",
-    {
         "Domain": DomainType,
         "IdentityProviderType": IdentityProviderTypeType,
         "EndpointType": EndpointTypeType,
         "LoggingRole": str,
         "ServerId": str,
         "State": StateType,
         "UserCount": int,
     },
-    total=False,
-)
-
-
-class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
-    pass
-
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1077,36 +972,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1121,43 +994,24 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListedUserTypeDef = TypedDict(
-    "_RequiredListedUserTypeDef",
+ListedUserTypeDef = TypedDict(
+    "ListedUserTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedUserTypeDef = TypedDict(
-    "_OptionalListedUserTypeDef",
-    {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "SshPublicKeyCount": int,
         "UserName": str,
     },
-    total=False,
-)
-
-
-class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
-    pass
-
-
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -1168,35 +1022,21 @@
 ListedWorkflowTypeDef = TypedDict(
     "ListedWorkflowTypeDef",
     {
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3TagOutputTypeDef = TypedDict(
+    "S3TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
@@ -1210,64 +1050,68 @@
         "WorkflowId": str,
         "ExecutionId": str,
         "Token": str,
         "Status": CustomStepStatusType,
     },
 )
 
-_RequiredUserDetailsTypeDef = TypedDict(
-    "_RequiredUserDetailsTypeDef",
+UserDetailsTypeDef = TypedDict(
+    "UserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
-    },
-)
-_OptionalUserDetailsTypeDef = TypedDict(
-    "_OptionalUserDetailsTypeDef",
-    {
         "SessionId": str,
     },
-    total=False,
 )
 
-
-class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
-    pass
-
-
-StartFileTransferRequestRequestTypeDef = TypedDict(
-    "StartFileTransferRequestRequestTypeDef",
+_RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
-        "SendFilePaths": Sequence[str],
     },
 )
-
-StartFileTransferResponseTypeDef = TypedDict(
-    "StartFileTransferResponseTypeDef",
+_OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFileTransferRequestRequestTypeDef",
     {
-        "TransferId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SendFilePaths": Sequence[str],
+        "RetrieveFilePaths": Sequence[str],
+        "LocalDirectoryPath": str,
+        "RemoteDirectoryPath": str,
     },
+    total=False,
 )
 
+
+class StartFileTransferRequestRequestTypeDef(
+    _RequiredStartFileTransferRequestRequestTypeDef, _OptionalStartFileTransferRequestRequestTypeDef
+):
+    pass
+
+
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
 StopServerRequestRequestTypeDef = TypedDict(
     "StopServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
+TestConnectionRequestRequestTypeDef = TypedDict(
+    "TestConnectionRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+
 _RequiredTestIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredTestIdentityProviderRequestRequestTypeDef",
     {
         "ServerId": str,
         "UserName": str,
     },
 )
@@ -1285,42 +1129,22 @@
 class TestIdentityProviderRequestRequestTypeDef(
     _RequiredTestIdentityProviderRequestRequestTypeDef,
     _OptionalTestIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-TestIdentityProviderResponseTypeDef = TypedDict(
-    "TestIdentityProviderResponseTypeDef",
-    {
-        "Response": str,
-        "StatusCode": int,
-        "Message": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAccessResponseTypeDef = TypedDict(
-    "UpdateAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAgreementRequestRequestTypeDef",
     {
         "AgreementId": str,
         "ServerId": str,
     },
 )
@@ -1340,22 +1164,14 @@
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAgreementResponseTypeDef = TypedDict(
-    "UpdateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
@@ -1371,48 +1187,23 @@
 
 class UpdateCertificateRequestRequestTypeDef(
     _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
 ):
     pass
 
 
-UpdateCertificateResponseTypeDef = TypedDict(
-    "UpdateCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
 )
 
-UpdateHostKeyResponseTypeDef = TypedDict(
-    "UpdateHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -1426,71 +1217,30 @@
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
 
-UpdateProfileResponseTypeDef = TypedDict(
-    "UpdateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateServerResponseTypeDef = TypedDict(
-    "UpdateServerResponseTypeDef",
+WorkflowDetailOutputTypeDef = TypedDict(
+    "WorkflowDetailOutputTypeDef",
     {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateUserResponseTypeDef = TypedDict(
-    "UpdateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WorkflowId": str,
+        "ExecutionRole": str,
     },
 )
 
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
 
-_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConnectorRequestRequestTypeDef",
-    {
-        "ConnectorId": str,
-    },
-)
-_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-    },
-    total=False,
-)
-
-
-class UpdateConnectorRequestRequestTypeDef(
-    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessRequestRequestTypeDef",
     {
         "Role": str,
         "ServerId": str,
         "ExternalId": str,
     },
@@ -1510,28 +1260,14 @@
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1578,249 +1314,287 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAgreementRequestRequestTypeDef",
+CreateAccessResponseTypeDef = TypedDict(
+    "CreateAccessResponseTypeDef",
     {
         "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateAgreementRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAgreementRequestRequestTypeDef",
+
+CreateAgreementResponseTypeDef = TypedDict(
+    "CreateAgreementResponseTypeDef",
     {
-        "Description": str,
-        "Status": AgreementStatusTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateAgreementRequestRequestTypeDef(
-    _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorRequestRequestTypeDef",
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
     {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorRequestRequestTypeDef",
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
     {
-        "LoggingRole": str,
-        "Tags": Sequence[TagTypeDef],
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateServerResponseTypeDef = TypedDict(
+    "CreateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateConnectorRequestRequestTypeDef(
-    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileRequestRequestTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
-        "As2Id": str,
-        "ProfileType": ProfileTypeType,
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileRequestRequestTypeDef",
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
     {
-        "CertificateIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "WorkflowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateProfileRequestRequestTypeDef(
-    _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
-):
-    pass
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ImportHostKeyResponseTypeDef = TypedDict(
+    "ImportHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredCreateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateUserRequestRequestTypeDef",
+ImportSshPublicKeyResponseTypeDef = TypedDict(
+    "ImportSshPublicKeyResponseTypeDef",
     {
-        "Role": str,
         "ServerId": str,
+        "SshPublicKeyId": str,
         "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateUserRequestRequestTypeDef",
+
+ListSecurityPoliciesResponseTypeDef = TypedDict(
+    "ListSecurityPoliciesResponseTypeDef",
     {
-        "HomeDirectory": str,
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "HomeDirectoryMappings": Sequence[HomeDirectoryMapEntryTypeDef],
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "SshPublicKeyBody": str,
-        "Tags": Sequence[TagTypeDef],
+        "NextToken": str,
+        "SecurityPolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+StartFileTransferResponseTypeDef = TypedDict(
+    "StartFileTransferResponseTypeDef",
+    {
+        "TransferId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateUserRequestRequestTypeDef(
-    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
-):
-    pass
-
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "Status": str,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribedAgreementTypeDef = TypedDict(
-    "_RequiredDescribedAgreementTypeDef",
+TestIdentityProviderResponseTypeDef = TypedDict(
+    "TestIdentityProviderResponseTypeDef",
     {
-        "Arn": str,
+        "Response": str,
+        "StatusCode": int,
+        "Message": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedAgreementTypeDef = TypedDict(
-    "_OptionalDescribedAgreementTypeDef",
+
+UpdateAccessResponseTypeDef = TypedDict(
+    "UpdateAccessResponseTypeDef",
     {
-        "AgreementId": str,
-        "Description": str,
-        "Status": AgreementStatusTypeType,
         "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
-        "Tags": List[TagTypeDef],
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class DescribedAgreementTypeDef(
-    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
-):
-    pass
-
-
-_RequiredDescribedCertificateTypeDef = TypedDict(
-    "_RequiredDescribedCertificateTypeDef",
+UpdateAgreementResponseTypeDef = TypedDict(
+    "UpdateAgreementResponseTypeDef",
     {
-        "Arn": str,
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedCertificateTypeDef = TypedDict(
-    "_OptionalDescribedCertificateTypeDef",
+
+UpdateCertificateResponseTypeDef = TypedDict(
+    "UpdateCertificateResponseTypeDef",
     {
         "CertificateId": str,
-        "Usage": CertificateUsageTypeType,
-        "Status": CertificateStatusTypeType,
-        "Certificate": str,
-        "CertificateChain": str,
-        "ActiveDate": datetime,
-        "InactiveDate": datetime,
-        "Serial": str,
-        "NotBeforeDate": datetime,
-        "NotAfterDate": datetime,
-        "Type": CertificateTypeType,
-        "Description": str,
-        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribedCertificateTypeDef(
-    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
-):
-    pass
+UpdateHostKeyResponseTypeDef = TypedDict(
+    "UpdateHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateProfileResponseTypeDef = TypedDict(
+    "UpdateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribedConnectorTypeDef = TypedDict(
-    "_RequiredDescribedConnectorTypeDef",
+UpdateServerResponseTypeDef = TypedDict(
+    "UpdateServerResponseTypeDef",
     {
-        "Arn": str,
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedConnectorTypeDef = TypedDict(
-    "_OptionalDescribedConnectorTypeDef",
+
+UpdateUserResponseTypeDef = TypedDict(
+    "UpdateUserResponseTypeDef",
     {
-        "ConnectorId": str,
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAgreementRequestRequestTypeDef",
+    {
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
         "AccessRole": str,
-        "LoggingRole": str,
-        "Tags": List[TagTypeDef],
+    },
+)
+_OptionalCreateAgreementRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAgreementRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class DescribedConnectorTypeDef(
-    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+class CreateAgreementRequestRequestTypeDef(
+    _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribedHostKeyTypeDef = TypedDict(
-    "_RequiredDescribedHostKeyTypeDef",
+_RequiredCreateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileRequestRequestTypeDef",
     {
-        "Arn": str,
+        "As2Id": str,
+        "ProfileType": ProfileTypeType,
     },
 )
-_OptionalDescribedHostKeyTypeDef = TypedDict(
-    "_OptionalDescribedHostKeyTypeDef",
+_OptionalCreateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileRequestRequestTypeDef",
     {
-        "HostKeyId": str,
-        "HostKeyFingerprint": str,
-        "Description": str,
-        "Type": str,
-        "DateImported": datetime,
-        "Tags": List[TagTypeDef],
+        "CertificateIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+class CreateProfileRequestRequestTypeDef(
+    _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
+):
     pass
 
 
-_RequiredDescribedProfileTypeDef = TypedDict(
-    "_RequiredDescribedProfileTypeDef",
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
     {
-        "Arn": str,
+        "Role": str,
+        "ServerId": str,
+        "UserName": str,
     },
 )
-_OptionalDescribedProfileTypeDef = TypedDict(
-    "_OptionalDescribedProfileTypeDef",
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
     {
-        "ProfileId": str,
-        "ProfileType": ProfileTypeType,
-        "As2Id": str,
-        "CertificateIds": List[str],
-        "Tags": List[TagTypeDef],
+        "HomeDirectory": str,
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "HomeDirectoryMappings": Sequence[HomeDirectoryMapEntryTypeDef],
+        "Policy": str,
+        "PosixProfile": PosixProfileTypeDef,
+        "SshPublicKeyBody": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
     pass
 
 
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
         "Usage": CertificateUsageTypeType,
@@ -1866,37 +1640,77 @@
 
 class ImportHostKeyRequestRequestTypeDef(
     _RequiredImportHostKeyRequestRequestTypeDef, _OptionalImportHostKeyRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
-        "NextToken": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorRequestRequestTypeDef",
     {
-        "Arn": str,
+        "Url": str,
+        "AccessRole": str,
+    },
+)
+_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorRequestRequestTypeDef",
+    {
+        "As2Config": As2ConnectorConfigTypeDef,
+        "LoggingRole": str,
         "Tags": Sequence[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateConnectorRequestRequestTypeDef(
+    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "SftpConfig": SftpConnectorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class UpdateConnectorRequestRequestTypeDef(
+    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
+):
+    pass
+
+
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeServerRequestServerOfflineWaitTypeDef = TypedDict(
     "_RequiredDescribeServerRequestServerOfflineWaitTypeDef",
     {
         "ServerId": str,
@@ -1936,150 +1750,411 @@
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
 
-_RequiredDescribedUserTypeDef = TypedDict(
-    "_RequiredDescribedUserTypeDef",
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileOutputTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+)
+
+DescribedAgreementTypeDef = TypedDict(
+    "DescribedAgreementTypeDef",
+    {
+        "Arn": str,
+        "AgreementId": str,
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
+        "AccessRole": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedCertificateTypeDef = TypedDict(
+    "DescribedCertificateTypeDef",
+    {
+        "Arn": str,
+        "CertificateId": str,
+        "Usage": CertificateUsageTypeType,
+        "Status": CertificateStatusTypeType,
+        "Certificate": str,
+        "CertificateChain": str,
+        "ActiveDate": datetime,
+        "InactiveDate": datetime,
+        "Serial": str,
+        "NotBeforeDate": datetime,
+        "NotAfterDate": datetime,
+        "Type": CertificateTypeType,
+        "Description": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedHostKeyTypeDef = TypedDict(
+    "DescribedHostKeyTypeDef",
+    {
+        "Arn": str,
+        "HostKeyId": str,
+        "HostKeyFingerprint": str,
+        "Description": str,
+        "Type": str,
+        "DateImported": datetime,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedProfileTypeDef = TypedDict(
+    "DescribedProfileTypeDef",
+    {
+        "Arn": str,
+        "ProfileId": str,
+        "ProfileType": ProfileTypeType,
+        "As2Id": str,
+        "CertificateIds": List[str],
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Arn": str,
+        "NextToken": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedUserTypeDef = TypedDict(
-    "_OptionalDescribedUserTypeDef",
+
+DescribedConnectorTypeDef = TypedDict(
+    "DescribedConnectorTypeDef",
     {
+        "Arn": str,
+        "ConnectorId": str,
+        "Url": str,
+        "As2Config": As2ConnectorConfigOutputTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "Tags": List[TagOutputTypeDef],
+        "SftpConfig": SftpConnectorConfigOutputTypeDef,
+    },
+)
+
+DescribedUserTypeDef = TypedDict(
+    "DescribedUserTypeDef",
+    {
+        "Arn": str,
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "UserName": str,
     },
-    total=False,
 )
 
-
-class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
-    pass
-
-
 ExecutionStepResultTypeDef = TypedDict(
     "ExecutionStepResultTypeDef",
     {
         "StepType": WorkflowStepTypeType,
         "Outputs": str,
         "Error": ExecutionErrorTypeDef,
     },
-    total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
-        "EfsFileLocation": EfsFileLocationTypeDef,
+        "EfsFileLocation": EfsFileLocationOutputTypeDef,
+    },
+)
+
+InputFileLocationOutputTypeDef = TypedDict(
+    "InputFileLocationOutputTypeDef",
+    {
+        "S3FileLocation": S3InputFileLocationOutputTypeDef,
+        "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
-    total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessesRequestListAccessesPaginateTypeDef(
+    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
+    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAgreementsRequestListAgreementsPaginateTypeDef(
+    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
+    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
+):
+    pass
+
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "WorkflowId": str,
+    },
+)
+_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExecutionsRequestListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
+):
+    pass
+
+
+ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    {
+        "ProfileType": ProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServersRequestListServersPaginateTypeDef = TypedDict(
+    "ListServersRequestListServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccessesResponseTypeDef = TypedDict(
     "ListAccessesResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Accesses": List[ListedAccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAgreementsResponseTypeDef = TypedDict(
     "ListAgreementsResponseTypeDef",
     {
         "NextToken": str,
         "Agreements": List[ListedAgreementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "NextToken": str,
         "Certificates": List[ListedCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "NextToken": str,
         "Connectors": List[ListedConnectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostKeysResponseTypeDef = TypedDict(
     "ListHostKeysResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "HostKeys": List[ListedHostKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "NextToken": str,
         "Profiles": List[ListedProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "NextToken": str,
         "Servers": List[ListedServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Users": List[ListedUserTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagStepDetailsOutputTypeDef = TypedDict(
+    "TagStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Tags": List[S3TagOutputTypeDef],
+        "SourceFileLocation": str,
     },
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
@@ -2092,88 +2167,116 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
+WorkflowDetailsOutputTypeDef = TypedDict(
+    "WorkflowDetailsOutputTypeDef",
+    {
+        "OnUpload": List[WorkflowDetailOutputTypeDef],
+        "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
+    },
+)
+
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
 DescribeAccessResponseTypeDef = TypedDict(
     "DescribeAccessResponseTypeDef",
     {
         "ServerId": str,
         "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeConnectorResponseTypeDef = TypedDict(
-    "DescribeConnectorResponseTypeDef",
-    {
-        "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfileResponseTypeDef = TypedDict(
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConnectorResponseTypeDef = TypedDict(
+    "DescribeConnectorResponseTypeDef",
+    {
+        "Connector": DescribedConnectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "ServerId": str,
         "User": DescribedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
-    total=False,
+)
+
+CopyStepDetailsOutputTypeDef = TypedDict(
+    "CopyStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+        "OverwriteExisting": OverwriteExistingType,
+        "SourceFileLocation": str,
+    },
+)
+
+DecryptStepDetailsOutputTypeDef = TypedDict(
+    "DecryptStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Type": Literal["PGP"],
+        "SourceFileLocation": str,
+        "OverwriteExisting": OverwriteExistingType,
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+    },
 )
 
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
@@ -2211,77 +2314,65 @@
     "ListedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
-    total=False,
 )
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
+DescribedServerTypeDef = TypedDict(
+    "DescribedServerTypeDef",
     {
+        "Arn": str,
         "Certificate": str,
+        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "HostKeyFingerprint": str,
+        "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
+        "ServerId": str,
+        "State": StateType,
+        "Tags": List[TagOutputTypeDef],
+        "UserCount": int,
+        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
+        "StructuredLogDestinations": List[str],
     },
-    total=False,
 )
 
-_RequiredDescribedServerTypeDef = TypedDict(
-    "_RequiredDescribedServerTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedServerTypeDef = TypedDict(
-    "_OptionalDescribedServerTypeDef",
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
-        "HostKeyFingerprint": str,
+        "HostKey": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
-        "Protocols": List[ProtocolType],
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
         "SecurityPolicyName": str,
-        "ServerId": str,
-        "State": StateType,
-        "Tags": List[TagTypeDef],
-        "UserCount": int,
+        "Tags": Sequence[TagTypeDef],
         "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": List[str],
+        "StructuredLogDestinations": Sequence[str],
     },
     total=False,
 )
 
-
-class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
-    pass
-
-
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2315,19 +2406,30 @@
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
-    total=False,
+)
+
+WorkflowStepOutputTypeDef = TypedDict(
+    "WorkflowStepOutputTypeDef",
+    {
+        "Type": WorkflowStepTypeType,
+        "CopyStepDetails": CopyStepDetailsOutputTypeDef,
+        "CustomStepDetails": CustomStepDetailsOutputTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
+        "TagStepDetails": TagStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
+    },
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
@@ -2341,32 +2443,44 @@
 
 ListExecutionsResponseTypeDef = TypedDict(
     "ListExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "WorkflowId": str,
         "Executions": List[ListedExecutionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServerResponseTypeDef = TypedDict(
     "DescribeServerResponseTypeDef",
     {
         "Server": DescribedServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExecutionResponseTypeDef = TypedDict(
     "DescribeExecutionResponseTypeDef",
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribedWorkflowTypeDef = TypedDict(
+    "DescribedWorkflowTypeDef",
+    {
+        "Arn": str,
+        "Description": str,
+        "Steps": List[WorkflowStepOutputTypeDef],
+        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
+        "WorkflowId": str,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Steps": Sequence[WorkflowStepTypeDef],
@@ -2385,39 +2499,14 @@
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribedWorkflowTypeDef = TypedDict(
-    "_RequiredDescribedWorkflowTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedWorkflowTypeDef = TypedDict(
-    "_OptionalDescribedWorkflowTypeDef",
-    {
-        "Description": str,
-        "Steps": List[WorkflowStepTypeDef],
-        "OnExceptionSteps": List[WorkflowStepTypeDef],
-        "WorkflowId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedWorkflowTypeDef(
-    _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
-):
-    pass
-
-
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transfer service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
+    from mypy_boto3_transfer.type_defs import As2ConnectorConfigOutputTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -48,37 +48,35 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "As2ConnectorConfigOutputTypeDef",
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
-    "CreateAccessResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAgreementResponseTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateProfileResponseTypeDef",
+    "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CreateServerResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
+    "CustomStepDetailsOutputTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
     "DeleteSshPublicKeyRequestRequestTypeDef",
+    "DeleteStepDetailsOutputTypeDef",
     "DeleteStepDetailsTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DescribeAccessRequestRequestTypeDef",
     "DescribeAgreementRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -87,144 +85,184 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
+    "HomeDirectoryMapEntryOutputTypeDef",
+    "PosixProfileOutputTypeDef",
+    "TagOutputTypeDef",
+    "SftpConnectorConfigOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "EndpointDetailsOutputTypeDef",
+    "IdentityProviderDetailsOutputTypeDef",
+    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
+    "EfsFileLocationOutputTypeDef",
     "EfsFileLocationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "ImportSshPublicKeyResponseTypeDef",
+    "S3InputFileLocationOutputTypeDef",
     "S3InputFileLocationTypeDef",
-    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
-    "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListedCertificateTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListedConnectorTypeDef",
-    "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListExecutionsRequestRequestTypeDef",
     "ListHostKeysRequestRequestTypeDef",
     "ListedHostKeyTypeDef",
-    "ListProfilesRequestListProfilesPaginateTypeDef",
     "ListProfilesRequestRequestTypeDef",
     "ListedProfileTypeDef",
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
-    "ListSecurityPoliciesResponseTypeDef",
-    "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3TagOutputTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
-    "StartFileTransferResponseTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
+    "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
-    "TestIdentityProviderResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAccessResponseTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateAgreementResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
-    "UpdateCertificateResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
-    "UpdateHostKeyResponseTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "UpdateProfileResponseTypeDef",
-    "UpdateServerResponseTypeDef",
-    "UpdateUserResponseTypeDef",
+    "WorkflowDetailOutputTypeDef",
     "WorkflowDetailTypeDef",
-    "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
-    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "CreateAccessResponseTypeDef",
+    "CreateAgreementResponseTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "CreateServerResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "ImportHostKeyResponseTypeDef",
+    "ImportSshPublicKeyResponseTypeDef",
+    "ListSecurityPoliciesResponseTypeDef",
+    "StartFileTransferResponseTypeDef",
+    "TestConnectionResponseTypeDef",
+    "TestIdentityProviderResponseTypeDef",
+    "UpdateAccessResponseTypeDef",
+    "UpdateAgreementResponseTypeDef",
+    "UpdateCertificateResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
+    "UpdateHostKeyResponseTypeDef",
+    "UpdateProfileResponseTypeDef",
+    "UpdateServerResponseTypeDef",
+    "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
-    "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DescribedAgreementTypeDef",
-    "DescribedCertificateTypeDef",
-    "DescribedConnectorTypeDef",
-    "DescribedHostKeyTypeDef",
-    "DescribedProfileTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateConnectorRequestRequestTypeDef",
+    "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
+    "DescribedAccessTypeDef",
+    "DescribedAgreementTypeDef",
+    "DescribedCertificateTypeDef",
+    "DescribedHostKeyTypeDef",
+    "DescribedProfileTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DescribedConnectorTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "InputFileLocationOutputTypeDef",
     "InputFileLocationTypeDef",
+    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "ListAgreementsRequestListAgreementsPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListExecutionsRequestListExecutionsPaginateTypeDef",
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    "ListServersRequestListServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAccessesResponseTypeDef",
     "ListAgreementsResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
+    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
     "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
+    "CopyStepDetailsOutputTypeDef",
+    "DecryptStepDetailsOutputTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "CreateServerRequestRequestTypeDef",
     "DescribedServerTypeDef",
+    "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "DescribedExecutionTypeDef",
+    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
     "DescribeWorkflowResponseTypeDef",
 )
 
+As2ConnectorConfigOutputTypeDef = TypedDict(
+    "As2ConnectorConfigOutputTypeDef",
+    {
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "MessageSubject": str,
+        "Compression": CompressionEnumType,
+        "EncryptionAlgorithm": EncryptionAlgType,
+        "SigningAlgorithm": SigningAlgType,
+        "MdnSigningAlgorithm": MdnSigningAlgType,
+        "MdnResponse": MdnResponseType,
+        "BasicAuthSecretId": str,
+    },
+)
+
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
@@ -259,53 +297,40 @@
     },
     total=False,
 )
 
 class PosixProfileTypeDef(_RequiredPosixProfileTypeDef, _OptionalPosixProfileTypeDef):
     pass
 
-CreateAccessResponseTypeDef = TypedDict(
-    "CreateAccessResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAgreementResponseTypeDef = TypedDict(
-    "CreateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
+SftpConnectorConfigTypeDef = TypedDict(
+    "SftpConnectorConfigTypeDef",
     {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserSecretId": str,
+        "TrustedHostKeys": Sequence[str],
     },
+    total=False,
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
@@ -335,36 +360,21 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CreateServerResponseTypeDef = TypedDict(
-    "CreateServerResponseTypeDef",
-    {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
+CustomStepDetailsOutputTypeDef = TypedDict(
+    "CustomStepDetailsOutputTypeDef",
     {
-        "WorkflowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "Target": str,
+        "TimeoutSeconds": int,
+        "SourceFileLocation": str,
     },
 )
 
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
@@ -432,14 +442,22 @@
     {
         "ServerId": str,
         "SshPublicKeyId": str,
         "UserName": str,
     },
 )
 
+DeleteStepDetailsOutputTypeDef = TypedDict(
+    "DeleteStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "SourceFileLocation": str,
+    },
+)
+
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
     total=False,
@@ -516,37 +534,26 @@
 DescribeSecurityPolicyRequestRequestTypeDef = TypedDict(
     "DescribeSecurityPolicyRequestRequestTypeDef",
     {
         "SecurityPolicyName": str,
     },
 )
 
-_RequiredDescribedSecurityPolicyTypeDef = TypedDict(
-    "_RequiredDescribedSecurityPolicyTypeDef",
-    {
-        "SecurityPolicyName": str,
-    },
-)
-_OptionalDescribedSecurityPolicyTypeDef = TypedDict(
-    "_OptionalDescribedSecurityPolicyTypeDef",
+DescribedSecurityPolicyTypeDef = TypedDict(
+    "DescribedSecurityPolicyTypeDef",
     {
         "Fips": bool,
+        "SecurityPolicyName": str,
         "SshCiphers": List[str],
         "SshKexs": List[str],
         "SshMacs": List[str],
         "TlsCiphers": List[str],
     },
-    total=False,
 )
 
-class DescribedSecurityPolicyTypeDef(
-    _RequiredDescribedSecurityPolicyTypeDef, _OptionalDescribedSecurityPolicyTypeDef
-):
-    pass
-
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -570,46 +577,111 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
+HomeDirectoryMapEntryOutputTypeDef = TypedDict(
+    "HomeDirectoryMapEntryOutputTypeDef",
+    {
+        "Entry": str,
+        "Target": str,
+    },
+)
+
+PosixProfileOutputTypeDef = TypedDict(
+    "PosixProfileOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+        "SecondaryGids": List[int],
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+SftpConnectorConfigOutputTypeDef = TypedDict(
+    "SftpConnectorConfigOutputTypeDef",
+    {
+        "UserSecretId": str,
+        "TrustedHostKeys": List[str],
+    },
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
-    total=False,
+)
+
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
+    {
+        "AddressAllocationIds": List[str],
+        "SubnetIds": List[str],
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "SecurityGroupIds": List[str],
+    },
+)
+
+IdentityProviderDetailsOutputTypeDef = TypedDict(
+    "IdentityProviderDetailsOutputTypeDef",
+    {
+        "Url": str,
+        "InvocationRole": str,
+        "DirectoryId": str,
+        "Function": str,
+        "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
+    },
+)
+
+ProtocolDetailsOutputTypeDef = TypedDict(
+    "ProtocolDetailsOutputTypeDef",
+    {
+        "PassiveIp": str,
+        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
+        "SetStatOption": SetStatOptionType,
+        "As2Transports": List[Literal["HTTP"]],
+    },
 )
 
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
 )
 
-EfsFileLocationTypeDef = TypedDict(
-    "EfsFileLocationTypeDef",
+EfsFileLocationOutputTypeDef = TypedDict(
+    "EfsFileLocationOutputTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
-    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EfsFileLocationTypeDef = TypedDict(
+    "EfsFileLocationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileSystemId": str,
+        "Path": str,
     },
+    total=False,
 )
 
 ExecutionErrorTypeDef = TypedDict(
     "ExecutionErrorTypeDef",
     {
         "Type": ExecutionErrorTypeType,
         "Message": str,
@@ -620,82 +692,52 @@
     "S3FileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
-    total=False,
-)
-
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportHostKeyResponseTypeDef = TypedDict(
-    "ImportHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-ImportSshPublicKeyResponseTypeDef = TypedDict(
-    "ImportSshPublicKeyResponseTypeDef",
+S3InputFileLocationOutputTypeDef = TypedDict(
+    "S3InputFileLocationOutputTypeDef",
     {
-        "ServerId": str,
-        "SshPublicKeyId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Bucket": str,
+        "Key": str,
     },
 )
 
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
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
 
-class ListAccessesRequestListAccessesPaginateTypeDef(
-    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
-    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessesRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAccessesRequestRequestTypeDef = TypedDict(
@@ -716,37 +758,16 @@
     "ListedAccessTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
-    total=False,
 )
 
-_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAgreementsRequestListAgreementsPaginateTypeDef(
-    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
-    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAgreementsRequestRequestTypeDef = TypedDict(
@@ -770,23 +791,14 @@
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
-    total=False,
-)
-
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -802,23 +814,14 @@
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
-    total=False,
-)
-
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -829,36 +832,15 @@
 ListedConnectorTypeDef = TypedDict(
     "ListedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
-    total=False,
-)
-
-_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "WorkflowId": str,
-    },
 )
-_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExecutionsRequestListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
@@ -892,42 +874,24 @@
 )
 
 class ListHostKeysRequestRequestTypeDef(
     _RequiredListHostKeysRequestRequestTypeDef, _OptionalListHostKeysRequestRequestTypeDef
 ):
     pass
 
-_RequiredListedHostKeyTypeDef = TypedDict(
-    "_RequiredListedHostKeyTypeDef",
+ListedHostKeyTypeDef = TypedDict(
+    "ListedHostKeyTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedHostKeyTypeDef = TypedDict(
-    "_OptionalListedHostKeyTypeDef",
-    {
         "HostKeyId": str,
         "Fingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
     },
-    total=False,
-)
-
-class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
-    pass
-
-ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListProfilesRequestListProfilesPaginateTypeDef",
-    {
-        "ProfileType": ProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -940,103 +904,48 @@
     "ListedProfileTypeDef",
     {
         "Arn": str,
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
-    total=False,
-)
-
-ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityPoliciesResponseTypeDef = TypedDict(
-    "ListSecurityPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecurityPolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServersRequestListServersPaginateTypeDef = TypedDict(
-    "ListServersRequestListServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListedServerTypeDef = TypedDict(
-    "_RequiredListedServerTypeDef",
+ListedServerTypeDef = TypedDict(
+    "ListedServerTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedServerTypeDef = TypedDict(
-    "_OptionalListedServerTypeDef",
-    {
         "Domain": DomainType,
         "IdentityProviderType": IdentityProviderTypeType,
         "EndpointType": EndpointTypeType,
         "LoggingRole": str,
         "ServerId": str,
         "State": StateType,
         "UserCount": int,
     },
-    total=False,
-)
-
-class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
-    pass
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1050,34 +959,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1090,41 +979,24 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-_RequiredListedUserTypeDef = TypedDict(
-    "_RequiredListedUserTypeDef",
+ListedUserTypeDef = TypedDict(
+    "ListedUserTypeDef",
     {
         "Arn": str,
-    },
-)
-_OptionalListedUserTypeDef = TypedDict(
-    "_OptionalListedUserTypeDef",
-    {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "SshPublicKeyCount": int,
         "UserName": str,
     },
-    total=False,
-)
-
-class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
-    pass
-
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -1135,35 +1007,21 @@
 ListedWorkflowTypeDef = TypedDict(
     "ListedWorkflowTypeDef",
     {
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+S3TagOutputTypeDef = TypedDict(
+    "S3TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
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
+        "Key": str,
+        "Value": str,
     },
 )
 
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
@@ -1177,62 +1035,66 @@
         "WorkflowId": str,
         "ExecutionId": str,
         "Token": str,
         "Status": CustomStepStatusType,
     },
 )
 
-_RequiredUserDetailsTypeDef = TypedDict(
-    "_RequiredUserDetailsTypeDef",
+UserDetailsTypeDef = TypedDict(
+    "UserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
-    },
-)
-_OptionalUserDetailsTypeDef = TypedDict(
-    "_OptionalUserDetailsTypeDef",
-    {
         "SessionId": str,
     },
-    total=False,
 )
 
-class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
-    pass
-
-StartFileTransferRequestRequestTypeDef = TypedDict(
-    "StartFileTransferRequestRequestTypeDef",
+_RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
-        "SendFilePaths": Sequence[str],
     },
 )
-
-StartFileTransferResponseTypeDef = TypedDict(
-    "StartFileTransferResponseTypeDef",
+_OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFileTransferRequestRequestTypeDef",
     {
-        "TransferId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SendFilePaths": Sequence[str],
+        "RetrieveFilePaths": Sequence[str],
+        "LocalDirectoryPath": str,
+        "RemoteDirectoryPath": str,
     },
+    total=False,
 )
 
+class StartFileTransferRequestRequestTypeDef(
+    _RequiredStartFileTransferRequestRequestTypeDef, _OptionalStartFileTransferRequestRequestTypeDef
+):
+    pass
+
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
 StopServerRequestRequestTypeDef = TypedDict(
     "StopServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
+TestConnectionRequestRequestTypeDef = TypedDict(
+    "TestConnectionRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+
 _RequiredTestIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredTestIdentityProviderRequestRequestTypeDef",
     {
         "ServerId": str,
         "UserName": str,
     },
 )
@@ -1248,42 +1110,22 @@
 
 class TestIdentityProviderRequestRequestTypeDef(
     _RequiredTestIdentityProviderRequestRequestTypeDef,
     _OptionalTestIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-TestIdentityProviderResponseTypeDef = TypedDict(
-    "TestIdentityProviderResponseTypeDef",
-    {
-        "Response": str,
-        "StatusCode": int,
-        "Message": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAccessResponseTypeDef = TypedDict(
-    "UpdateAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAgreementRequestRequestTypeDef",
     {
         "AgreementId": str,
         "ServerId": str,
     },
 )
@@ -1301,22 +1143,14 @@
 )
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
-UpdateAgreementResponseTypeDef = TypedDict(
-    "UpdateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
@@ -1330,48 +1164,23 @@
 )
 
 class UpdateCertificateRequestRequestTypeDef(
     _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
 ):
     pass
 
-UpdateCertificateResponseTypeDef = TypedDict(
-    "UpdateCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
 )
 
-UpdateHostKeyResponseTypeDef = TypedDict(
-    "UpdateHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -1383,69 +1192,30 @@
 )
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-UpdateProfileResponseTypeDef = TypedDict(
-    "UpdateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateServerResponseTypeDef = TypedDict(
-    "UpdateServerResponseTypeDef",
+WorkflowDetailOutputTypeDef = TypedDict(
+    "WorkflowDetailOutputTypeDef",
     {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateUserResponseTypeDef = TypedDict(
-    "UpdateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WorkflowId": str,
+        "ExecutionRole": str,
     },
 )
 
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
 
-_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConnectorRequestRequestTypeDef",
-    {
-        "ConnectorId": str,
-    },
-)
-_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-    },
-    total=False,
-)
-
-class UpdateConnectorRequestRequestTypeDef(
-    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessRequestRequestTypeDef",
     {
         "Role": str,
         "ServerId": str,
         "ExternalId": str,
     },
@@ -1463,28 +1233,14 @@
 )
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1527,232 +1283,282 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAgreementRequestRequestTypeDef",
+CreateAccessResponseTypeDef = TypedDict(
+    "CreateAccessResponseTypeDef",
     {
         "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateAgreementRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAgreementRequestRequestTypeDef",
+
+CreateAgreementResponseTypeDef = TypedDict(
+    "CreateAgreementResponseTypeDef",
     {
-        "Description": str,
-        "Status": AgreementStatusTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateAgreementRequestRequestTypeDef(
-    _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
-):
-    pass
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorRequestRequestTypeDef",
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
     {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorRequestRequestTypeDef",
+
+CreateServerResponseTypeDef = TypedDict(
+    "CreateServerResponseTypeDef",
     {
-        "LoggingRole": str,
-        "Tags": Sequence[TagTypeDef],
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateConnectorRequestRequestTypeDef(
-    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
-):
-    pass
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredCreateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileRequestRequestTypeDef",
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
     {
-        "As2Id": str,
-        "ProfileType": ProfileTypeType,
+        "WorkflowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileRequestRequestTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "CertificateIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateProfileRequestRequestTypeDef(
-    _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
-):
-    pass
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredCreateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateUserRequestRequestTypeDef",
+ImportHostKeyResponseTypeDef = TypedDict(
+    "ImportHostKeyResponseTypeDef",
     {
-        "Role": str,
         "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSshPublicKeyResponseTypeDef = TypedDict(
+    "ImportSshPublicKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "SshPublicKeyId": str,
         "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateUserRequestRequestTypeDef",
+
+ListSecurityPoliciesResponseTypeDef = TypedDict(
+    "ListSecurityPoliciesResponseTypeDef",
     {
-        "HomeDirectory": str,
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "HomeDirectoryMappings": Sequence[HomeDirectoryMapEntryTypeDef],
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "SshPublicKeyBody": str,
-        "Tags": Sequence[TagTypeDef],
+        "NextToken": str,
+        "SecurityPolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateUserRequestRequestTypeDef(
-    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
-):
-    pass
+StartFileTransferResponseTypeDef = TypedDict(
+    "StartFileTransferResponseTypeDef",
+    {
+        "TransferId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribedAgreementTypeDef = TypedDict(
-    "_RequiredDescribedAgreementTypeDef",
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
     {
-        "Arn": str,
+        "ConnectorId": str,
+        "Status": str,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedAgreementTypeDef = TypedDict(
-    "_OptionalDescribedAgreementTypeDef",
+
+TestIdentityProviderResponseTypeDef = TypedDict(
+    "TestIdentityProviderResponseTypeDef",
     {
-        "AgreementId": str,
-        "Description": str,
-        "Status": AgreementStatusTypeType,
-        "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
-        "Tags": List[TagTypeDef],
+        "Response": str,
+        "StatusCode": int,
+        "Message": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribedAgreementTypeDef(
-    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
-):
-    pass
+UpdateAccessResponseTypeDef = TypedDict(
+    "UpdateAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribedCertificateTypeDef = TypedDict(
-    "_RequiredDescribedCertificateTypeDef",
+UpdateAgreementResponseTypeDef = TypedDict(
+    "UpdateAgreementResponseTypeDef",
     {
-        "Arn": str,
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedCertificateTypeDef = TypedDict(
-    "_OptionalDescribedCertificateTypeDef",
+
+UpdateCertificateResponseTypeDef = TypedDict(
+    "UpdateCertificateResponseTypeDef",
     {
         "CertificateId": str,
-        "Usage": CertificateUsageTypeType,
-        "Status": CertificateStatusTypeType,
-        "Certificate": str,
-        "CertificateChain": str,
-        "ActiveDate": datetime,
-        "InactiveDate": datetime,
-        "Serial": str,
-        "NotBeforeDate": datetime,
-        "NotAfterDate": datetime,
-        "Type": CertificateTypeType,
-        "Description": str,
-        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribedCertificateTypeDef(
-    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
-):
-    pass
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribedConnectorTypeDef = TypedDict(
-    "_RequiredDescribedConnectorTypeDef",
+UpdateHostKeyResponseTypeDef = TypedDict(
+    "UpdateHostKeyResponseTypeDef",
     {
-        "Arn": str,
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribedConnectorTypeDef = TypedDict(
-    "_OptionalDescribedConnectorTypeDef",
+
+UpdateProfileResponseTypeDef = TypedDict(
+    "UpdateProfileResponseTypeDef",
     {
-        "ConnectorId": str,
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServerResponseTypeDef = TypedDict(
+    "UpdateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserResponseTypeDef = TypedDict(
+    "UpdateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAgreementRequestRequestTypeDef",
+    {
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
         "AccessRole": str,
-        "LoggingRole": str,
-        "Tags": List[TagTypeDef],
+    },
+)
+_OptionalCreateAgreementRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAgreementRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class DescribedConnectorTypeDef(
-    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+class CreateAgreementRequestRequestTypeDef(
+    _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribedHostKeyTypeDef = TypedDict(
-    "_RequiredDescribedHostKeyTypeDef",
+_RequiredCreateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileRequestRequestTypeDef",
     {
-        "Arn": str,
+        "As2Id": str,
+        "ProfileType": ProfileTypeType,
     },
 )
-_OptionalDescribedHostKeyTypeDef = TypedDict(
-    "_OptionalDescribedHostKeyTypeDef",
+_OptionalCreateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileRequestRequestTypeDef",
     {
-        "HostKeyId": str,
-        "HostKeyFingerprint": str,
-        "Description": str,
-        "Type": str,
-        "DateImported": datetime,
-        "Tags": List[TagTypeDef],
+        "CertificateIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+class CreateProfileRequestRequestTypeDef(
+    _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
+):
     pass
 
-_RequiredDescribedProfileTypeDef = TypedDict(
-    "_RequiredDescribedProfileTypeDef",
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
     {
-        "Arn": str,
+        "Role": str,
+        "ServerId": str,
+        "UserName": str,
     },
 )
-_OptionalDescribedProfileTypeDef = TypedDict(
-    "_OptionalDescribedProfileTypeDef",
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
     {
-        "ProfileId": str,
-        "ProfileType": ProfileTypeType,
-        "As2Id": str,
-        "CertificateIds": List[str],
-        "Tags": List[TagTypeDef],
+        "HomeDirectory": str,
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "HomeDirectoryMappings": Sequence[HomeDirectoryMapEntryTypeDef],
+        "Policy": str,
+        "PosixProfile": PosixProfileTypeDef,
+        "SshPublicKeyBody": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
     pass
 
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
         "Usage": CertificateUsageTypeType,
         "Certificate": str,
@@ -1793,37 +1599,73 @@
 )
 
 class ImportHostKeyRequestRequestTypeDef(
     _RequiredImportHostKeyRequestRequestTypeDef, _OptionalImportHostKeyRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
-        "NextToken": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorRequestRequestTypeDef",
     {
-        "Arn": str,
+        "Url": str,
+        "AccessRole": str,
+    },
+)
+_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorRequestRequestTypeDef",
+    {
+        "As2Config": As2ConnectorConfigTypeDef,
+        "LoggingRole": str,
         "Tags": Sequence[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateConnectorRequestRequestTypeDef(
+    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
     },
 )
+_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpdateConnectorRequestRequestTypeDef(
+    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
+):
+    pass
 
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeServerRequestServerOfflineWaitTypeDef = TypedDict(
     "_RequiredDescribeServerRequestServerOfflineWaitTypeDef",
     {
         "ServerId": str,
@@ -1859,148 +1701,401 @@
 
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
-_RequiredDescribedUserTypeDef = TypedDict(
-    "_RequiredDescribedUserTypeDef",
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileOutputTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+)
+
+DescribedAgreementTypeDef = TypedDict(
+    "DescribedAgreementTypeDef",
+    {
+        "Arn": str,
+        "AgreementId": str,
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
+        "AccessRole": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedCertificateTypeDef = TypedDict(
+    "DescribedCertificateTypeDef",
+    {
+        "Arn": str,
+        "CertificateId": str,
+        "Usage": CertificateUsageTypeType,
+        "Status": CertificateStatusTypeType,
+        "Certificate": str,
+        "CertificateChain": str,
+        "ActiveDate": datetime,
+        "InactiveDate": datetime,
+        "Serial": str,
+        "NotBeforeDate": datetime,
+        "NotAfterDate": datetime,
+        "Type": CertificateTypeType,
+        "Description": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedHostKeyTypeDef = TypedDict(
+    "DescribedHostKeyTypeDef",
+    {
+        "Arn": str,
+        "HostKeyId": str,
+        "HostKeyFingerprint": str,
+        "Description": str,
+        "Type": str,
+        "DateImported": datetime,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+DescribedProfileTypeDef = TypedDict(
+    "DescribedProfileTypeDef",
+    {
+        "Arn": str,
+        "ProfileId": str,
+        "ProfileType": ProfileTypeType,
+        "As2Id": str,
+        "CertificateIds": List[str],
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Arn": str,
+        "NextToken": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribedConnectorTypeDef = TypedDict(
+    "DescribedConnectorTypeDef",
     {
         "Arn": str,
+        "ConnectorId": str,
+        "Url": str,
+        "As2Config": As2ConnectorConfigOutputTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "Tags": List[TagOutputTypeDef],
+        "SftpConfig": SftpConnectorConfigOutputTypeDef,
     },
 )
-_OptionalDescribedUserTypeDef = TypedDict(
-    "_OptionalDescribedUserTypeDef",
+
+DescribedUserTypeDef = TypedDict(
+    "DescribedUserTypeDef",
     {
+        "Arn": str,
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "UserName": str,
     },
-    total=False,
 )
 
-class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
-    pass
-
 ExecutionStepResultTypeDef = TypedDict(
     "ExecutionStepResultTypeDef",
     {
         "StepType": WorkflowStepTypeType,
         "Outputs": str,
         "Error": ExecutionErrorTypeDef,
     },
-    total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
-        "EfsFileLocation": EfsFileLocationTypeDef,
+        "EfsFileLocation": EfsFileLocationOutputTypeDef,
+    },
+)
+
+InputFileLocationOutputTypeDef = TypedDict(
+    "InputFileLocationOutputTypeDef",
+    {
+        "S3FileLocation": S3InputFileLocationOutputTypeDef,
+        "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
-    total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessesRequestListAccessesPaginateTypeDef(
+    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
+    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAgreementsRequestListAgreementsPaginateTypeDef(
+    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
+    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
+):
+    pass
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "WorkflowId": str,
+    },
+)
+_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExecutionsRequestListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
+):
+    pass
+
+ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    {
+        "ProfileType": ProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServersRequestListServersPaginateTypeDef = TypedDict(
+    "ListServersRequestListServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccessesResponseTypeDef = TypedDict(
     "ListAccessesResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Accesses": List[ListedAccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAgreementsResponseTypeDef = TypedDict(
     "ListAgreementsResponseTypeDef",
     {
         "NextToken": str,
         "Agreements": List[ListedAgreementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "NextToken": str,
         "Certificates": List[ListedCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "NextToken": str,
         "Connectors": List[ListedConnectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostKeysResponseTypeDef = TypedDict(
     "ListHostKeysResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "HostKeys": List[ListedHostKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "NextToken": str,
         "Profiles": List[ListedProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "NextToken": str,
         "Servers": List[ListedServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Users": List[ListedUserTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagStepDetailsOutputTypeDef = TypedDict(
+    "TagStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Tags": List[S3TagOutputTypeDef],
+        "SourceFileLocation": str,
     },
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
@@ -2013,88 +2108,116 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
+WorkflowDetailsOutputTypeDef = TypedDict(
+    "WorkflowDetailsOutputTypeDef",
+    {
+        "OnUpload": List[WorkflowDetailOutputTypeDef],
+        "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
+    },
+)
+
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
 DescribeAccessResponseTypeDef = TypedDict(
     "DescribeAccessResponseTypeDef",
     {
         "ServerId": str,
         "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeConnectorResponseTypeDef = TypedDict(
-    "DescribeConnectorResponseTypeDef",
-    {
-        "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfileResponseTypeDef = TypedDict(
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConnectorResponseTypeDef = TypedDict(
+    "DescribeConnectorResponseTypeDef",
+    {
+        "Connector": DescribedConnectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "ServerId": str,
         "User": DescribedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
-    total=False,
+)
+
+CopyStepDetailsOutputTypeDef = TypedDict(
+    "CopyStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+        "OverwriteExisting": OverwriteExistingType,
+        "SourceFileLocation": str,
+    },
+)
+
+DecryptStepDetailsOutputTypeDef = TypedDict(
+    "DecryptStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Type": Literal["PGP"],
+        "SourceFileLocation": str,
+        "OverwriteExisting": OverwriteExistingType,
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+    },
 )
 
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
@@ -2130,75 +2253,65 @@
     "ListedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
-    total=False,
 )
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
+DescribedServerTypeDef = TypedDict(
+    "DescribedServerTypeDef",
     {
+        "Arn": str,
         "Certificate": str,
+        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "HostKeyFingerprint": str,
+        "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
+        "ServerId": str,
+        "State": StateType,
+        "Tags": List[TagOutputTypeDef],
+        "UserCount": int,
+        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
+        "StructuredLogDestinations": List[str],
     },
-    total=False,
 )
 
-_RequiredDescribedServerTypeDef = TypedDict(
-    "_RequiredDescribedServerTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedServerTypeDef = TypedDict(
-    "_OptionalDescribedServerTypeDef",
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
-        "HostKeyFingerprint": str,
+        "HostKey": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
-        "Protocols": List[ProtocolType],
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
         "SecurityPolicyName": str,
-        "ServerId": str,
-        "State": StateType,
-        "Tags": List[TagTypeDef],
-        "UserCount": int,
+        "Tags": Sequence[TagTypeDef],
         "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": List[str],
+        "StructuredLogDestinations": Sequence[str],
     },
     total=False,
 )
 
-class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
-    pass
-
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2230,19 +2343,30 @@
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
-    total=False,
+)
+
+WorkflowStepOutputTypeDef = TypedDict(
+    "WorkflowStepOutputTypeDef",
+    {
+        "Type": WorkflowStepTypeType,
+        "CopyStepDetails": CopyStepDetailsOutputTypeDef,
+        "CustomStepDetails": CustomStepDetailsOutputTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
+        "TagStepDetails": TagStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
+    },
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
@@ -2256,32 +2380,44 @@
 
 ListExecutionsResponseTypeDef = TypedDict(
     "ListExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "WorkflowId": str,
         "Executions": List[ListedExecutionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServerResponseTypeDef = TypedDict(
     "DescribeServerResponseTypeDef",
     {
         "Server": DescribedServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExecutionResponseTypeDef = TypedDict(
     "DescribeExecutionResponseTypeDef",
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribedWorkflowTypeDef = TypedDict(
+    "DescribedWorkflowTypeDef",
+    {
+        "Arn": str,
+        "Description": str,
+        "Steps": List[WorkflowStepOutputTypeDef],
+        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
+        "WorkflowId": str,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Steps": Sequence[WorkflowStepTypeDef],
@@ -2298,37 +2434,14 @@
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribedWorkflowTypeDef = TypedDict(
-    "_RequiredDescribedWorkflowTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedWorkflowTypeDef = TypedDict(
-    "_OptionalDescribedWorkflowTypeDef",
-    {
-        "Description": str,
-        "Steps": List[WorkflowStepTypeDef],
-        "OnExceptionSteps": List[WorkflowStepTypeDef],
-        "WorkflowId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class DescribedWorkflowTypeDef(
-    _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
-):
-    pass
-
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.11/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-transfer
-Version: 1.28.0
-Summary: Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,37 +372,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
+    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
+    SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
+    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
+    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -443,146 +409,171 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    HomeDirectoryMapEntryOutputTypeDef,
+    PosixProfileOutputTypeDef,
+    TagOutputTypeDef,
+    SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    IdentityProviderDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
+    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
+    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
+    TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
+    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestConnectionResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
-    CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedConnectorTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateConnectorRequestRequestTypeDef,
+    UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
     DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
-    DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
+    CopyStepDetailsOutputTypeDef,
+    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_structure() -> As2ConnectorConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.0/setup.py` & `mypy-boto3-transfer-1.28.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

