# Comparing `tmp/mypy-boto3-securityhub-1.28.0.tar.gz` & `tmp/mypy-boto3-securityhub-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.28.0.tar` & `mypy-boto3-securityhub-1.28.11.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.706427 mypy-boto3-securityhub-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-07-06 21:00:35.702427 mypy-boto3-securityhub-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49455 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.698427 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-07-06 20:55:16.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   279880 2023-07-06 20:55:27.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   279813 2023-07-06 20:55:20.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.702427 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 21:00:35.000000 mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.706427 mypy-boto3-securityhub-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:55:15.000000 mypy-boto3-securityhub-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    82526 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    81023 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-07-25 19:48:45.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-25 19:48:45.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   508039 2023-07-25 19:48:57.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   507986 2023-07-25 19:48:51.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    82526 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/setup.py
```

### Comparing `mypy-boto3-securityhub-1.28.0/LICENSE` & `mypy-boto3-securityhub-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.28.11\nVersion:         1.28.11\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,26 +121,28 @@
     "REMOTE_ACCESS",
     "ROOTKIT",
     "SPYWARE",
     "TROJAN",
     "VIRUS",
     "WORM",
 ]
-MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
+MapFilterComparisonType = Literal["CONTAINS", "EQUALS", "NOT_CONTAINS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
 RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 RuleStatusType = Literal["DISABLED", "ENABLED"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
-StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
+StringFilterComparisonType = Literal[
+    "CONTAINS", "EQUALS", "NOT_CONTAINS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"
+]
 ThreatIntelIndicatorCategoryType = Literal[
     "BACKDOOR", "CARD_STEALER", "COMMAND_AND_CONTROL", "DROP_SITE", "EXPLOIT_SITE", "KEYLOGGER"
 ]
 ThreatIntelIndicatorTypeType = Literal[
     "DOMAIN",
     "EMAIL_ADDRESS",
     "HASH_MD5",
@@ -372,14 +374,15 @@
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

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -119,26 +119,28 @@
     "REMOTE_ACCESS",
     "ROOTKIT",
     "SPYWARE",
     "TROJAN",
     "VIRUS",
     "WORM",
 ]
-MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
+MapFilterComparisonType = Literal["CONTAINS", "EQUALS", "NOT_CONTAINS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
 RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 RuleStatusType = Literal["DISABLED", "ENABLED"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
-StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
+StringFilterComparisonType = Literal[
+    "CONTAINS", "EQUALS", "NOT_CONTAINS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"
+]
 ThreatIntelIndicatorCategoryType = Literal[
     "BACKDOOR", "CARD_STEALER", "COMMAND_AND_CONTROL", "DROP_SITE", "EXPLOIT_SITE", "KEYLOGGER"
 ]
 ThreatIntelIndicatorTypeType = Literal[
     "DOMAIN",
     "EMAIL_ADDRESS",
     "HASH_MD5",
@@ -370,14 +372,15 @@
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

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -88,256 +88,239 @@
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListSecurityControlDefinitionsPaginator",
     "ListStandardsControlAssociationsPaginator",
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
 class DescribeActionTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
-
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
-
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
-
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
-
 class GetEnabledStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
-
 class GetFindingHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
         """
 
-
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
-
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
-
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
-
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
-
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
-
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
-
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
-
 class ListSecurityControlDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
-
 class ListStandardsControlAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
         """
```

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,239 +88,256 @@
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListSecurityControlDefinitionsPaginator",
     "ListStandardsControlAssociationsPaginator",
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
 class DescribeActionTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeactiontargetspaginator)
         """
 
+
 class DescribeProductsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describeproductspaginator)
         """
 
+
 class DescribeStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardspaginator)
         """
 
+
 class DescribeStandardsControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
+
 class GetEnabledStandardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getenabledstandardspaginator)
         """
 
+
 class GetFindingHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindinghistorypaginator)
         """
 
+
 class GetFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
+
 class GetInsightsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getinsightspaginator)
         """
 
+
 class ListEnabledProductsForImportPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
+
 class ListFindingAggregatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
+
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listinvitationspaginator)
         """
 
+
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listmemberspaginator)
         """
 
+
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
+
 class ListSecurityControlDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
+
 class ListStandardsControlAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
         """
```

### Comparing `mypy-boto3-securityhub-1.28.0/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.0/setup.py` & `mypy-boto3-securityhub-1.28.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SecurityHub 1.28.11 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

