# Comparing `tmp/dashvector-0.0.15-py3-none-any.whl.zip` & `tmp/dashvector-0.0.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,40 @@
-Zip file size: 72535 bytes, number of entries: 38
+Zip file size: 73007 bytes, number of entries: 38
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jul-12 09:23 dashvector/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 23-Jul-20 12:04 dashvector/version.py
+-rw-r--r--  2.0 unx      695 b- defN 23-Jul-24 08:00 dashvector/version.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/common/__init__.py
--rw-r--r--  2.0 unx      772 b- defN 23-Jul-12 09:23 dashvector/common/constants.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Jul-24 12:38 dashvector/common/constants.py
 -rw-r--r--  2.0 unx    10886 b- defN 23-Jul-17 06:53 dashvector/common/error.py
 -rw-r--r--  2.0 unx     4982 b- defN 23-Jul-12 09:23 dashvector/common/handler.py
 -rw-r--r--  2.0 unx     1659 b- defN 23-Jul-12 09:23 dashvector/common/logging.py
 -rw-r--r--  2.0 unx     4616 b- defN 23-Jul-12 09:23 dashvector/common/status.py
--rw-r--r--  2.0 unx    28048 b- defN 23-Jul-20 12:03 dashvector/common/types.py
+-rw-r--r--  2.0 unx    28048 b- defN 23-Jul-24 12:23 dashvector/common/types.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/__init__.py
 -rw-r--r--  2.0 unx    17041 b- defN 23-Jul-18 07:35 dashvector/core/client.py
--rw-r--r--  2.0 unx    33405 b- defN 23-Jul-20 09:19 dashvector/core/collection.py
+-rw-r--r--  2.0 unx    33405 b- defN 23-Jul-24 11:11 dashvector/core/collection.py
 -rw-r--r--  2.0 unx     5285 b- defN 23-Jul-20 11:49 dashvector/core/doc.py
 -rw-r--r--  2.0 unx    11772 b- defN 23-Jul-12 09:23 dashvector/core/partition.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/handler/__init__.py
 -rw-r--r--  2.0 unx    20176 b- defN 23-Jul-20 11:50 dashvector/core/handler/grpc_handler.py
 -rw-r--r--  2.0 unx    21454 b- defN 23-Jul-12 09:23 dashvector/core/handler/http_handler.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/models/__init__.py
--rw-r--r--  2.0 unx    10567 b- defN 23-Jul-13 11:16 dashvector/core/models/create_collection_request.py
--rw-r--r--  2.0 unx     2688 b- defN 23-Jul-12 09:23 dashvector/core/models/create_partition_request.py
--rw-r--r--  2.0 unx     5843 b- defN 23-Jul-12 09:23 dashvector/core/models/delete_doc_request.py
--rw-r--r--  2.0 unx     2139 b- defN 23-Jul-12 09:23 dashvector/core/models/describe_collection_request.py
--rw-r--r--  2.0 unx     2107 b- defN 23-Jul-12 09:23 dashvector/core/models/drop_collection_request.py
--rw-r--r--  2.0 unx     2667 b- defN 23-Jul-12 09:23 dashvector/core/models/drop_partition_request.py
--rw-r--r--  2.0 unx     6361 b- defN 23-Jul-20 01:56 dashvector/core/models/get_doc_request.py
+-rw-r--r--  2.0 unx    10581 b- defN 23-Jul-24 12:40 dashvector/core/models/create_collection_request.py
+-rw-r--r--  2.0 unx     2738 b- defN 23-Jul-24 12:40 dashvector/core/models/create_partition_request.py
+-rw-r--r--  2.0 unx     5893 b- defN 23-Jul-24 12:40 dashvector/core/models/delete_doc_request.py
+-rw-r--r--  2.0 unx     2189 b- defN 23-Jul-24 12:40 dashvector/core/models/describe_collection_request.py
+-rw-r--r--  2.0 unx     2157 b- defN 23-Jul-24 12:40 dashvector/core/models/drop_collection_request.py
+-rw-r--r--  2.0 unx     2717 b- defN 23-Jul-24 12:40 dashvector/core/models/drop_partition_request.py
+-rw-r--r--  2.0 unx     6411 b- defN 23-Jul-24 12:40 dashvector/core/models/get_doc_request.py
 -rw-r--r--  2.0 unx     1015 b- defN 23-Jul-12 09:23 dashvector/core/models/get_version_request.py
 -rw-r--r--  2.0 unx     1021 b- defN 23-Jul-12 09:23 dashvector/core/models/list_collection_request.py
--rw-r--r--  2.0 unx    10042 b- defN 23-Jul-20 12:02 dashvector/core/models/query_doc_request.py
--rw-r--r--  2.0 unx     2114 b- defN 23-Jul-12 09:23 dashvector/core/models/stats_collection_request.py
--rw-r--r--  2.0 unx    17326 b- defN 23-Jul-20 12:02 dashvector/core/models/upsert_doc_request.py
+-rw-r--r--  2.0 unx    10083 b- defN 23-Jul-24 12:40 dashvector/core/models/query_doc_request.py
+-rw-r--r--  2.0 unx     2164 b- defN 23-Jul-24 12:40 dashvector/core/models/stats_collection_request.py
+-rw-r--r--  2.0 unx    17371 b- defN 23-Jul-24 12:40 dashvector/core/models/upsert_doc_request.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/proto/__init__.py
 -rw-r--r--  2.0 unx   136016 b- defN 23-Jul-12 09:23 dashvector/core/proto/centaur_pb2.py
 -rw-r--r--  2.0 unx    21819 b- defN 23-Jul-12 09:23 dashvector/core/proto/centaur_pb2_grpc.py
--rw-r--r--  2.0 unx    12090 b- defN 23-Jul-20 12:04 dashvector-0.0.15.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4366 b- defN 23-Jul-20 12:04 dashvector-0.0.15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 12:04 dashvector-0.0.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-20 12:04 dashvector-0.0.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3490 b- defN 23-Jul-20 12:04 dashvector-0.0.15.dist-info/RECORD
-38 files, 407139 bytes uncompressed, 66875 bytes compressed:  83.6%
+-rw-r--r--  2.0 unx    12090 b- defN 23-Jul-25 01:32 dashvector-0.0.16.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5086 b- defN 23-Jul-25 01:32 dashvector-0.0.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 01:32 dashvector-0.0.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-25 01:32 dashvector-0.0.16.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3490 b- defN 23-Jul-25 01:32 dashvector-0.0.16.dist-info/RECORD
+38 files, 408362 bytes uncompressed, 67347 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -93,23 +93,23 @@
 
 Filename: dashvector/core/proto/centaur_pb2.py
 Comment: 
 
 Filename: dashvector/core/proto/centaur_pb2_grpc.py
 Comment: 
 
-Filename: dashvector-0.0.15.dist-info/LICENSE.txt
+Filename: dashvector-0.0.16.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dashvector-0.0.15.dist-info/METADATA
+Filename: dashvector-0.0.16.dist-info/METADATA
 Comment: 
 
-Filename: dashvector-0.0.15.dist-info/WHEEL
+Filename: dashvector-0.0.16.dist-info/WHEEL
 Comment: 
 
-Filename: dashvector-0.0.15.dist-info/top_level.txt
+Filename: dashvector-0.0.16.dist-info/top_level.txt
 Comment: 
 
-Filename: dashvector-0.0.15.dist-info/RECORD
+Filename: dashvector-0.0.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashvector/version.py

```diff
@@ -13,8 +13,8 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
-__version__ = "0.0.15"
+__version__ = "0.0.16"
```

## dashvector/common/constants.py

```diff
@@ -15,7 +15,8 @@
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 DASHVECTOR_VECTOR_NAME = "proxima_vector"
 DASHVECTOR_LOGGING_LEVEL_ENV = 'DASHVECTOR_LOGGING_LEVEL'
+FIELD_NAME_PATTERN = '^[a-zA-Z][a-zA-Z0-9_-]{0,32}$'
```

## dashvector/core/models/create_collection_request.py

```diff
@@ -14,15 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
-from dashvector.common.constants import DASHVECTOR_VECTOR_NAME
+from dashvector.common.constants import DASHVECTOR_VECTOR_NAME, FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.types import DataParser
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
@@ -43,17 +43,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK CreateCollectionRequest name Type({name}) is Invalid")
 
         if len(name) < 3 or len(name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK CreateCollectionRequest name Length({len(name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', name) is None:
+        if re.search(FIELD_NAME_PATTERN, name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK CreateCollectionRequest name Characters({name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK CreateCollectionRequest name Characters({name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._name = name
 
         """
         dim: int
         """
         self._dimension = 0
         if not isinstance(dimension, int):
@@ -125,15 +125,15 @@
 
                 if len(field_name) < 1 or len(field_name) > 32:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f"DashVectorSDK CreateCollectionRequest field_name in fields_schema Length({len(field_name)}) is Invalid and must be in [1, 32]")
 
                 if re.search('^[a-zA-Z][a-zA-Z0-9_-]{0,32}$', field_name) is None:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                           reason=f"DashVectorSDK CreateCollectionRequest field_name in fields_schema Characters({field_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                           reason=f"DashVectorSDK CreateCollectionRequest field_name in fields_schema Characters({field_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
                 if field_name == DASHVECTOR_VECTOR_NAME:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f'DashVectorSDK CreateCollectionRequest field_name in fields_schema Value({DASHVECTOR_VECTOR_NAME}) is Reserved')
 
                 if not isinstance(field_dtype, type):
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
```

## dashvector/core/models/create_partition_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class CreatePartitionRequest(RPCRequest):
@@ -44,17 +45,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK CreatePartitionRequest name Type({partition_name}) is Invalid")
 
         if len(partition_name) < 3 or len(partition_name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK CreatePartitionRequest name Length({len(partition_name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', partition_name) is None:
+        if re.search(FIELD_NAME_PATTERN, partition_name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK CreatePartitionRequest name Characters({partition_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK CreatePartitionRequest name Characters({partition_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._partition_name = partition_name
 
         """
         CreatePartitionRequest: google.protobuf.Message
         """
         create_request = centaur_pb2.CreatePartitionRequest()
         create_request.collection_name = self._collection_name
```

## dashvector/core/models/delete_doc_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class DeleteDocRequest(RPCRequest):
@@ -98,17 +99,17 @@
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK DeleteDocRequest partition Type({type(partition)}) is Invalid")
 
             if len(partition) < 3 or len(partition) > 32:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK DeleteDocRequest partition Length({len(partition)}) is Invalid and must be in [3, 32]")
 
-            if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', partition) is None:
+            if re.search(FIELD_NAME_PATTERN, partition) is None:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                       reason=f"DashVectorSDK DeleteDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                       reason=f"DashVectorSDK DeleteDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
             self._partition = partition
 
         """
         DeleteDocRequest: google.protobuf.Message
         """
         delete_request = centaur_pb2.DeleteDocRequest()
```

## dashvector/core/models/describe_collection_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class DescribeCollectionRequest(RPCRequest):
     def __init__(self, *,
@@ -35,17 +36,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DescribeCollectionRequest name Type({name}) is Invalid")
 
         if len(name) < 3 or len(name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DescribeCollectionRequest name Length({len(name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', name) is None:
+        if re.search(FIELD_NAME_PATTERN, name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK DescribeCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK DescribeCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._name = name
 
         """
         DescribeCollectionRequest: google.protobuf.Message
         """
         describe_request = centaur_pb2.DescribeCollectionRequest(collection_name=self._name)
```

## dashvector/core/models/drop_collection_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class DropCollectionRequest(RPCRequest):
     def __init__(self, *,
@@ -35,17 +36,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DropCollectionRequest name Type({name}) is Invalid")
 
         if len(name) < 3 or len(name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DropCollectionRequest name Length({len(name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', name) is None:
+        if re.search(FIELD_NAME_PATTERN, name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK DropCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK DropCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._name = name
 
         """
         DropCollectionRequest: google.protobuf.Message
         """
         drop_request = centaur_pb2.DropCollectionRequest(collection_name=self._name)
```

## dashvector/core/models/drop_partition_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class DropPartitionRequest(RPCRequest):
@@ -44,17 +45,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DropPartitionRequest name Type({partition_name}) is Invalid")
 
         if len(partition_name) < 3 or len(partition_name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK DropPartitionRequest name Length({len(partition_name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', partition_name) is None:
+        if re.search(FIELD_NAME_PATTERN, partition_name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK DropPartitionRequest name Characters({partition_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK DropPartitionRequest name Characters({partition_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._partition_name = partition_name
 
         """
         DropPartitionRequest: google.protobuf.Message
         """
         drop_request = centaur_pb2.DropPartitionRequest()
         drop_request.collection_name = self._collection_name
```

## dashvector/core/models/get_doc_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class GetDocRequest(RPCRequest):
@@ -104,17 +105,17 @@
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK GetDocRequest partition Type({type(partition)}) is Invalid")
 
             if len(partition) < 3 or len(partition) > 32:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK GetDocRequest partition Length({len(partition)}) is Invalid and must be in [3, 32]")
 
-            if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$',partition) is None:
+            if re.search(FIELD_NAME_PATTERN,partition) is None:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                       reason=f"DashVectorSDK GetDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                       reason=f"DashVectorSDK GetDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
             self._partition = partition
 
         """
         GetDocRequest: google.protobuf.Message
         """
         get_request = centaur_pb2.GetDocRequest()
```

## dashvector/core/models/query_doc_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class QueryDocRequest(RPCRequest):
@@ -144,17 +145,17 @@
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK QueryDocRequest partition Type({type(partition)}) is Invalid")
 
             if len(partition) < 3 or len(partition) > 32:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK QueryDocRequest partition Length({len(partition)}) is Invalid and must be in [3, 32]")
 
-            if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', partition) is None:
+            if re.search(FIELD_NAME_PATTERN, partition) is None:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                       reason=f"DashVectorSDK QueryDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                       reason=f"DashVectorSDK QueryDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
             self._partition = partition
         if self._partition is not None:
             query_request.partition = self._partition
 
         '''
         output_fields: Optional[List[str]] = None
@@ -170,17 +171,17 @@
                         raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                                reason=f"DashVectorSDK QueryDocRequest output_field in output_fields Type({type(output_field)}) is Invalid")
                     
                     if len(output_field) < 1 or len(output_field) > 32:
                         raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                                reason=f"DashVectorSDK QueryDocRequest output_field in output_fields Length({len(output_field)}) is Invalid and must be in [1, 32]")
 
-                    if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', output_field) is None:
+                    if re.search(FIELD_NAME_PATTERN, output_field) is None:
                         raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                               reason=f"DashVectorSDK QueryDocRequest output_field in output_fields Characters({output_field}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                               reason=f"DashVectorSDK QueryDocRequest output_field in output_fields Characters({output_field}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
                     
                 self.output_fields = output_fields
             else:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK QueryDocRequest output_fields Type({type(output_fields)}) is Invalid")
         if self.output_fields is not None:
             query_request.query_fields.extend(self.output_fields)
```

## dashvector/core/models/stats_collection_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 
 
 class StatsCollectionRequest(RPCRequest):
     def __init__(self, *,
@@ -35,17 +36,17 @@
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK StatsCollectionRequest name Type({name}) is Invalid")
 
         if len(name) < 3 or len(name) > 32:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK StatsCollectionRequest name Length({len(name)}) is Invalid and must be in [3, 32]")
 
-        if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', name) is None:
+        if re.search(FIELD_NAME_PATTERN, name) is None:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK StatsCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                   reason=f"DashVectorSDK StatsCollectionRequest name Characters({len(name)}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
         self._name = name
 
         """
         StatsCollectionRequest: google.protobuf.Message
         """
         stats_request = centaur_pb2.StatsCollectionRequest(collection_name=self._name)
```

## dashvector/core/models/upsert_doc_request.py

```diff
@@ -14,14 +14,15 @@
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
 import re
+from dashvector.common.constants import FIELD_NAME_PATTERN
 from dashvector.common.types import *
 from dashvector.common.error import DashVectorCode, DashVectorException
 from dashvector.common.handler import RPCRequest
 from dashvector.core.proto import centaur_pb2
 from dashvector.core.doc import Doc
 
 
@@ -53,27 +54,27 @@
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK UpsertDocRequest partition Type({type(partition)}) is Invalid")
 
             if len(partition) < 3 or len(partition) > 32:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                        reason=f"DashVectorSDK UpsertDocRequest partition Length({len(partition)}) is Invalid and must be in [3, 32]")
 
-            if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', partition) is None:
+            if re.search(FIELD_NAME_PATTERN, partition) is None:
                 raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                       reason=f"DashVectorSDK UpsertDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                       reason=f"DashVectorSDK UpsertDocRequest partition Characters({partition}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
             self._partition = partition
 
         """
         action: str
         """
         self._action = ""
         if not isinstance(action, str):
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK UpsertDocRequest action Type({type(pt)}) is Invalid")
+                                   reason=f"DashVectorSDK UpsertDocRequest action Type({type(action)}) is Invalid")
         if action != "upsert" and action != "insert" and action != "update":
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK UpsertDocRequest action Value({action}) is Invalid and must be in ['insert', 'update', 'upsert']")
         self._action = action
 
         """
         InsertDocRequest: google.protobuf.Message
@@ -155,17 +156,17 @@
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f"DashVectorSDK UpsertDocRequest field name Type({type(field_name)}) is Invalid")
 
                 if len(field_name) < 1 or len(field_name) > 32:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f"DashVectorSDK UpsertDocRequest field name Length({len(field_name)}) is Invalid and must be in [1, 32]")
 
-                if re.search('^[a-zA-Z][a-zA-Z0-9_]{0,32}$', field_name) is None:
+                if re.search(FIELD_NAME_PATTERN, field_name) is None:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                           reason=f"DashVectorSDK UpsertDocRequest field name Characters({field_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
+                                           reason=f"DashVectorSDK UpsertDocRequest field name Characters({field_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_, -]")
 
                 new_field = new_doc.fields.add()
                 new_field.name = field_name
 
                 if field_name in self._collection_field_map:
                     field_schema = self._collection_field_map[field_name]
                     field_schema_is_invalid = False
```

## Comparing `dashvector-0.0.15.dist-info/LICENSE.txt` & `dashvector-0.0.16.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dashvector-0.0.15.dist-info/METADATA` & `dashvector-0.0.16.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashvector
-Version: 0.0.15
+Version: 0.0.16
 Summary: DashVector Client Python Sdk Library
 Home-page: https://github.com/alibaba/proxima
 Author: Alibaba
 Author-email: dashvector@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -31,20 +31,47 @@
 ## Installation
 To install the DashVector client Python SDK, simply run:
 ```shell
 pip install dashvector
 ```
 
 ## QuickStart
-You can use `Client` api to communicate with DashVector service.
 
 ```python
+import numpy as np
 import dashvector
 
+# You can use `Client` api to communicate with DashVector service.
 client = dashvector.Client(api_key='YOUR-DASHVECTOR-API-KEY')
+
+# Create a collection named "quickstart" with dimension of 4, using the default Euclidean distance metric
+client.create(name='quickstart', dimension=4)
+
+# Get a collection by name
+collection = client.get(name='quickstart')
+
+# You can use 'Collection' api to Inert/Query/Upsert/Update/Delete/Fetch docs
+# Insert sample data (10 * 4-dimensional vectors)
+collection.insert(
+    [
+        dashvector.Doc(id=str(i), vector=np.random.rand(4), fields={'anykey': 'anyvalue'}) 
+        for i in range(10)
+    ]
+)
+
+# Performs approximate nearest-neighbor search
+docs = collection.query([0.1, 0.2, 0.3, 0.4], topk=5)
+print(docs)
+
+# Get statistics about collection
+stats = collection.stats()
+print(stats)
+
+# Delete a collection by name
+client.delete(name='quickstart')
 ```
 
 ## Sample Code
 
 ### Create a Collection
 `Client` host various `Collection` APIs for interacting with DashVector service.
 
@@ -108,26 +135,24 @@
 
 ### Insert/Update/Upsert Docs
 ```python
 import dashvector
 
 client = dashvector.Client(api_key='YOUR-DASHVECTOR-API-KEY')
 collection = client.get('YOUR-COLLECTION-NAME')
-collection.upsert(('YOUR-DOC-ID', [0.1, 0.2], {'price': 100, 'type': 'dress'}))
+collection.insert(('YOUR-DOC-ID', [0.1, 0.2, 0.3, 0.4], {'price': 100, 'type': 'dress'}))
 ```
 
 ### Query a Collection
 ```python
 import dashvector
 
 client = dashvector.Client(api_key='YOUR-DASHVECTOR-API-KEY')
 collection = client.get('YOUR-COLLECTION-NAME')
-match_docs = collection.query([0.1, 0.2, 0.3, 0.4], 
-                       topk=100, 
-                       include_vector=True)
+match_docs = collection.query([0.1, 0.2, 0.3, 0.4], topk=100)
 if match_docs:
     for doc in match_docs:
         print(doc)
 ```
 
 ### Delete Docs
 ```python
```

## Comparing `dashvector-0.0.15.dist-info/RECORD` & `dashvector-0.0.16.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 dashvector/__init__.py,sha256=Cpl05fQAaj_mlaecjl7OA8Us1Nd80DPI0kt9enNHNsM,1224
-dashvector/version.py,sha256=TGhi5GQDujqWa-eIMjnlIL8Uee-H6r0TkDRUGUEahxM,695
+dashvector/version.py,sha256=B-hediEKIFe19Tg4CfBMu6-B8llAnni1YBH6fv0PIMk,695
 dashvector/common/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
-dashvector/common/constants.py,sha256=zpBWhp04ESp60M7Zj9HHXcOMk8Q_jH7dmanE4V1gfTI,772
+dashvector/common/constants.py,sha256=N7tAhz--U3pXclVrfZ7-FbjJBmSLmS_xmnmP7q5F7VI,825
 dashvector/common/error.py,sha256=3Zq8ru1A582ZHypgpPPS81DSp23rGr7-bU2hgT76eI8,10886
 dashvector/common/handler.py,sha256=347-RKVaaF829PrnmcAWldVcCF8ivFFi5OMba53PsWw,4982
 dashvector/common/logging.py,sha256=Cw-KMQ_y94VfKxw4QEJ1HbjZVH2AIkkUuhsTC-9O_4c,1659
 dashvector/common/status.py,sha256=JvJI2-Yk8eimGjWOHotzYPY8DmjeVUW02zk_dGm954Q,4616
 dashvector/common/types.py,sha256=OP8IQhJPZMaK-lCvplUoDjkhk8ncnNDn7JkhIEl6dUk,28048
 dashvector/core/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/core/client.py,sha256=YxVSSC3hDk5MwG70RcgVpWAGw8KymtHXiFY92VLmCag,17041
 dashvector/core/collection.py,sha256=JTXJOQfd4DNA33nMJKjDyQ4nq6qTwDtKFNQqpW0o7Jc,33405
 dashvector/core/doc.py,sha256=nSBmNInoE_5dzVnSdWBcGQ5WKd227hJ-6GlRhBLvUTo,5285
 dashvector/core/partition.py,sha256=G6WdshhvqoYrObe7yj2lCI2r3QUt5bNeA2BozvmPZwY,11772
 dashvector/core/handler/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/core/handler/grpc_handler.py,sha256=EZ7YQsaZdl93qSAquiVKcrga2JbJ04G9fuQGhOkDNu4,20176
 dashvector/core/handler/http_handler.py,sha256=rysglKNvNMM55-UbR1jKkgHr4FsUpHh_bEhdU_AOfvA,21454
 dashvector/core/models/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
-dashvector/core/models/create_collection_request.py,sha256=F4t76iivpIbE-e217jzptGt67VZ554KidVl3hDLqvII,10567
-dashvector/core/models/create_partition_request.py,sha256=2Yow2FYjfht2uSmkoVEbG3uwgUthCuQB1ISuGadG5xY,2688
-dashvector/core/models/delete_doc_request.py,sha256=Ey2m0CfLH2iJRw4DJtODA_RJJi7qM_8xJS2MxYZFBS0,5843
-dashvector/core/models/describe_collection_request.py,sha256=DD8tef7Pm0oJUXkydbY0R10ZMPzt6fbBREq2aH3givw,2139
-dashvector/core/models/drop_collection_request.py,sha256=94TiA0cnymFPewc2U1IsDPp-TCnQmZG9_x-sk-tstC0,2107
-dashvector/core/models/drop_partition_request.py,sha256=Wdrn0Y7CaaXe2OKt-ryLXkjxog1ppgcr0oDaUpnE3dU,2667
-dashvector/core/models/get_doc_request.py,sha256=rbq2qRtsb0UCP2HatXWAVDd8M8NzZ5EKsYS0U51mJhE,6361
+dashvector/core/models/create_collection_request.py,sha256=pqU_v2cAriMu9N4CQfK4ZpnpMfxtA676R9XeRcHZQks,10581
+dashvector/core/models/create_partition_request.py,sha256=L4fNFKC7U0M1C40QYaFCigGTwXPKWeHcBQr-j2K9xmA,2738
+dashvector/core/models/delete_doc_request.py,sha256=vKYTdM8mq4u3nXcjcvECM7-oXQ_zXusSVup87ugaDIc,5893
+dashvector/core/models/describe_collection_request.py,sha256=o18b1ez3mM14VtgpgG68S2FOm1zuIlFQU1soSDSUsng,2189
+dashvector/core/models/drop_collection_request.py,sha256=4i4QXOXzGKJtdJ0ZFJ53znXeGAzFYinWGWyculZJ93w,2157
+dashvector/core/models/drop_partition_request.py,sha256=Tpls7AAkWozkNsc9hfKx6KkHkRFKLhmysvlxeJC7MJw,2717
+dashvector/core/models/get_doc_request.py,sha256=JQXov2UbOtpvp2wXc8CvEYLyIouQgeUAAXlA5bwxnVc,6411
 dashvector/core/models/get_version_request.py,sha256=MJIU8UJ1heNJ09rpy_kXwSyPLsy0TA7GDJuTeBDdqVU,1015
 dashvector/core/models/list_collection_request.py,sha256=CoVqnp4HpfZ9co8Sf2L_AXG2G-GnSzTWMEdmLdx8xoQ,1021
-dashvector/core/models/query_doc_request.py,sha256=Hlvu9rXLJVd4U-4nDYBNyuPLimB_zeZjjXYvwJwFNCk,10042
-dashvector/core/models/stats_collection_request.py,sha256=CO8mzBbZ0OqXfZj1Ja49bjYuRyA8i1ss8LfTRc9oy9w,2114
-dashvector/core/models/upsert_doc_request.py,sha256=KVsdL61pRB-NKx1vySRiejsXfDHOrAJTWCrIjfqtAoY,17326
+dashvector/core/models/query_doc_request.py,sha256=Uq3mfRsCSzrXkbNwZE9AN7bNtc2a0qzcccCON2Nyrfk,10083
+dashvector/core/models/stats_collection_request.py,sha256=5t906fiO5xlgCb8QAzkJWyOerEoWid6rTm3oFlbfQos,2164
+dashvector/core/models/upsert_doc_request.py,sha256=1K4iy-N68La3WLpTNMamQ7kuL3-O1QliehdwDLFaz3A,17371
 dashvector/core/proto/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/core/proto/centaur_pb2.py,sha256=JqO3G1qYgTr7JSPhrcS652Q_dEVoCMh6PDj-4gopCEo,136016
 dashvector/core/proto/centaur_pb2_grpc.py,sha256=a2ED6WA43pi7BWe5-g3v9uj-RV4qRZeGYO6k96zPVzk,21819
-dashvector-0.0.15.dist-info/LICENSE.txt,sha256=GYJChq297x8HRI7yfGLcHdK-evsn6Sv7k68UCeGTu9w,12090
-dashvector-0.0.15.dist-info/METADATA,sha256=WDkROT_qeL36cSNXN6r_jM-xf4Uep0Mfn4R_vNyBkY8,4366
-dashvector-0.0.15.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-dashvector-0.0.15.dist-info/top_level.txt,sha256=Ynh6NVKjpSk3PBj82cAq0AEs9j_KIV3ANXLCiLHntVk,11
-dashvector-0.0.15.dist-info/RECORD,,
+dashvector-0.0.16.dist-info/LICENSE.txt,sha256=GYJChq297x8HRI7yfGLcHdK-evsn6Sv7k68UCeGTu9w,12090
+dashvector-0.0.16.dist-info/METADATA,sha256=pku2u_peWoCoJ6z8vMX4Bo5wZ_XyYpKRUh-0vReO_XQ,5086
+dashvector-0.0.16.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+dashvector-0.0.16.dist-info/top_level.txt,sha256=Ynh6NVKjpSk3PBj82cAq0AEs9j_KIV3ANXLCiLHntVk,11
+dashvector-0.0.16.dist-info/RECORD,,
```

