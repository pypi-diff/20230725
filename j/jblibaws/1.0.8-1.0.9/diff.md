# Comparing `tmp/jblibaws-1.0.8.tar.gz` & `tmp/jblibaws-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jblibaws-1.0.8.tar", last modified: Mon Jan 10 16:50:51 2022, max compression
+gzip compressed data, was "jblibaws-1.0.9.tar", last modified: Tue May 24 22:04:37 2022, max compression
```

## Comparing `jblibaws-1.0.8.tar` & `jblibaws-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-01-10 16:50:51.590589 jblibaws-1.0.8/
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     1074 2021-07-13 00:13:07.000000 jblibaws-1.0.8/LICENSE
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     2320 2022-01-10 16:50:51.590589 jblibaws-1.0.8/PKG-INFO
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     1889 2022-01-09 04:27:22.000000 jblibaws-1.0.8/README.md
-drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-01-10 16:50:51.589589 jblibaws-1.0.8/jblibaws/
--rw-rw-r--   0 jbard     (1000) jbard     (1000)       63 2021-07-13 00:13:07.000000 jblibaws-1.0.8/jblibaws/__init__.py
-drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-01-10 16:50:51.590589 jblibaws-1.0.8/jblibaws/aws/
--rw-rw-r--   0 jbard     (1000) jbard     (1000)       46 2021-07-13 00:13:07.000000 jblibaws-1.0.8/jblibaws/aws/__init__.py
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     1215 2021-07-13 00:13:07.000000 jblibaws-1.0.8/jblibaws/aws/cognito.py
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     7283 2022-01-10 16:49:46.000000 jblibaws-1.0.8/jblibaws/aws/dynamodb.py
-drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-01-10 16:50:51.590589 jblibaws-1.0.8/jblibaws/dict_tools/
--rw-rw-r--   0 jbard     (1000) jbard     (1000)       25 2021-07-13 00:13:07.000000 jblibaws-1.0.8/jblibaws/dict_tools/__init__.py
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     1061 2021-07-13 00:13:07.000000 jblibaws-1.0.8/jblibaws/dict_tools/dict_tools.py
-drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-01-10 16:50:51.590589 jblibaws-1.0.8/jblibaws.egg-info/
--rw-rw-r--   0 jbard     (1000) jbard     (1000)     2320 2022-01-10 16:50:51.000000 jblibaws-1.0.8/jblibaws.egg-info/PKG-INFO
--rw-rw-r--   0 jbard     (1000) jbard     (1000)      315 2022-01-10 16:50:51.000000 jblibaws-1.0.8/jblibaws.egg-info/SOURCES.txt
--rw-rw-r--   0 jbard     (1000) jbard     (1000)        1 2022-01-10 16:50:51.000000 jblibaws-1.0.8/jblibaws.egg-info/dependency_links.txt
--rw-rw-r--   0 jbard     (1000) jbard     (1000)        9 2022-01-10 16:50:51.000000 jblibaws-1.0.8/jblibaws.egg-info/top_level.txt
--rw-rw-r--   0 jbard     (1000) jbard     (1000)       38 2022-01-10 16:50:51.591590 jblibaws-1.0.8/setup.cfg
--rw-rw-r--   0 jbard     (1000) jbard     (1000)      772 2022-01-10 16:49:55.000000 jblibaws-1.0.8/setup.py
+drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-05-24 22:04:37.781478 jblibaws-1.0.9/
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     1074 2021-07-13 00:13:07.000000 jblibaws-1.0.9/LICENSE
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     2266 2022-05-24 22:04:37.781478 jblibaws-1.0.9/PKG-INFO
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     1872 2022-05-24 22:01:22.000000 jblibaws-1.0.9/README.md
+drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-05-24 22:04:37.779478 jblibaws-1.0.9/jblibaws/
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)       63 2021-07-13 00:13:07.000000 jblibaws-1.0.9/jblibaws/__init__.py
+drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-05-24 22:04:37.780478 jblibaws-1.0.9/jblibaws/aws/
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)       46 2021-07-13 00:13:07.000000 jblibaws-1.0.9/jblibaws/aws/__init__.py
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     1215 2021-07-13 00:13:07.000000 jblibaws-1.0.9/jblibaws/aws/cognito.py
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     9137 2022-05-24 22:00:21.000000 jblibaws-1.0.9/jblibaws/aws/dynamodb.py
+drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-05-24 22:04:37.781478 jblibaws-1.0.9/jblibaws/dict_tools/
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)       25 2021-07-13 00:13:07.000000 jblibaws-1.0.9/jblibaws/dict_tools/__init__.py
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     1061 2021-07-13 00:13:07.000000 jblibaws-1.0.9/jblibaws/dict_tools/dict_tools.py
+drwxrwxr-x   0 jbard     (1000) jbard     (1000)        0 2022-05-24 22:04:37.780478 jblibaws-1.0.9/jblibaws.egg-info/
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)     2266 2022-05-24 22:04:37.000000 jblibaws-1.0.9/jblibaws.egg-info/PKG-INFO
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)      315 2022-05-24 22:04:37.000000 jblibaws-1.0.9/jblibaws.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)        1 2022-05-24 22:04:37.000000 jblibaws-1.0.9/jblibaws.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)        9 2022-05-24 22:04:37.000000 jblibaws-1.0.9/jblibaws.egg-info/top_level.txt
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)       38 2022-05-24 22:04:37.781478 jblibaws-1.0.9/setup.cfg
+-rw-rw-r--   0 jbard     (1000) jbard     (1000)      772 2022-05-24 22:00:41.000000 jblibaws-1.0.9/setup.py
```

### Comparing `jblibaws-1.0.8/LICENSE` & `jblibaws-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jblibaws-1.0.8/PKG-INFO` & `jblibaws-1.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: jblibaws
-Version: 1.0.8
+Version: 1.0.9
 Summary: JustBard's Python based AWS Utilities
 Home-page: http://justbard.com
 Author: Justin Bard
 Author-email: JustinBard@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jblib-aws
@@ -35,15 +33,15 @@
     class talk_with_dynamo(table, boto_session, region='us-east-1')
 
         Example:
             table_name = "table-name"
             boto_session = boto3.session.Session()
             dynamo = talk_with_dynamo(table_name, boto_session) ## Generate Database Object
 
-            response = dynamo.query(partition_key=partition_key, partition_key_attribute=partition_key_attribute, sorting_key=sorting_key, sorting_key_attribute=sorting_key_attribute, index=index_key)
+            response = dynamo.query(self, partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False, index=False, queryOperator=False, betweenValue=False)
             print ("Resposne: {}".format(response))
 
 			getResponse = dynamo.getItem(partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False)
 
 			batch_keys = {'tableName': {'Keys': [{'PartitionKey': 'PartitionKeyAttribute', 'SortingKey': 'SortingKey'}]}}
 			batchResponse = dynamo.batchGetItem(batch_keys)
 
@@ -68,9 +66,7 @@
         Functions:
             get_user_email(cognito_user_id)
             - Gets User Email Address
 
 ```
 
 ### More Documentation To Come
-
-
```

### Comparing `jblibaws-1.0.8/README.md` & `jblibaws-1.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     class talk_with_dynamo(table, boto_session, region='us-east-1')
 
         Example:
             table_name = "table-name"
             boto_session = boto3.session.Session()
             dynamo = talk_with_dynamo(table_name, boto_session) ## Generate Database Object
 
-            response = dynamo.query(partition_key=partition_key, partition_key_attribute=partition_key_attribute, sorting_key=sorting_key, sorting_key_attribute=sorting_key_attribute, index=index_key)
+            response = dynamo.query(self, partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False, index=False, queryOperator=False, betweenValue=False)
             print ("Resposne: {}".format(response))
 
 			getResponse = dynamo.getItem(partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False)
 
 			batch_keys = {'tableName': {'Keys': [{'PartitionKey': 'PartitionKeyAttribute', 'SortingKey': 'SortingKey'}]}}
 			batchResponse = dynamo.batchGetItem(batch_keys)
```

### Comparing `jblibaws-1.0.8/jblibaws/aws/cognito.py` & `jblibaws-1.0.9/jblibaws/aws/cognito.py`

 * *Files identical despite different names*

### Comparing `jblibaws-1.0.8/jblibaws/aws/dynamodb.py` & `jblibaws-1.0.9/jblibaws/aws/dynamodb.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,15 +34,27 @@
 class talk_with_dynamo():
 	def __init__(self, table, boto_session, region='us-east-1', check_index=False, debug=False):
 		self.boto_session = boto_session
 		self.dynamodb = self.boto_session.resource('dynamodb', region_name=region)
 		self.table = self.dynamodb.Table(table)
 		self.check_index = check_index
 
-	def query(self, partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False, index=False):
+	def query(self, partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False, index=False, queryOperator=False, betweenValue=False):
+		"""
+		Query a DynamoDB Table.\n
+		queryOperator can now be set to one of the following: gt, gte, lt, lte, between
+		\tgt: greater than (>)
+		\tgte: greater than or equal to (>=)
+		\tlt: less than (<)
+		\tlte: less than or equal to (<=)
+		\tbetween: condition where the attribute is greater than or equal to the low value and less than or equal to the high value.
+
+		betweenValue: Expecting a tuple of two values and is intended to be used with the between queryOperator
+		"""
+
 		if self.check_index:
 			# When adding a global secondary index to an existing table, you cannot query the index until it has been backfilled.
 			# This portion of the script waits until the index is in the “ACTIVE” status, indicating it is ready to be queried.
 			while True:
 				if not self.table.global_secondary_indexes or self.table.global_secondary_indexes[0]['IndexStatus'] != 'ACTIVE':
 					print('[{}]  Waiting for index to backfill...'.format('INFO'))
 					sleep(5)
@@ -56,18 +68,47 @@
 				KeyConditionExpression=Key(partition_key).eq(partition_key_attribute),
 			)
 		elif index and sorting_key and sorting_key_attribute:
 			response = self.table.query(
 				IndexName=index,
 				KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).eq(sorting_key_attribute),
 			)
-		elif partition_key and partition_key_attribute and sorting_key and sorting_key_attribute:
+		elif partition_key and partition_key_attribute and sorting_key and sorting_key_attribute and not queryOperator:
 			response = self.table.query(
 				KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).eq(sorting_key_attribute),
 			)
+		elif partition_key and partition_key_attribute and sorting_key and sorting_key_attribute and queryOperator and not betweenValue:
+			if queryOperator == 'gt': 
+				response = self.table.query(
+					KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).gt(sorting_key_attribute),
+				)
+			elif queryOperator == 'gte': 
+				response = self.table.query(
+					KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).gte(sorting_key_attribute),
+				)
+			elif queryOperator == 'lt': 
+				response = self.table.query(
+					KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).lt(sorting_key_attribute),
+				)
+			elif queryOperator == 'lte': 
+				response = self.table.query(
+					KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).lte(sorting_key_attribute),
+				)
+			else:
+				response = ""
+
+		elif partition_key and partition_key_attribute and sorting_key and queryOperator and betweenValue:
+			if queryOperator == 'between' and betweenValue: 
+				lowValue, highValue = betweenValue
+
+				response = self.table.query(
+					KeyConditionExpression=Key(partition_key).eq(partition_key_attribute) & Key(sorting_key).between(lowValue, highValue),
+				)
+			else:
+				response = ""
 		elif partition_key and partition_key_attribute:
 			response = self.table.query(
 				KeyConditionExpression=Key(partition_key).eq(partition_key_attribute),
 			)
 		else:
 			response = ""
```

### Comparing `jblibaws-1.0.8/jblibaws/dict_tools/dict_tools.py` & `jblibaws-1.0.9/jblibaws/dict_tools/dict_tools.py`

 * *Files identical despite different names*

### Comparing `jblibaws-1.0.8/jblibaws.egg-info/PKG-INFO` & `jblibaws-1.0.9/jblibaws.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: jblibaws
-Version: 1.0.8
+Version: 1.0.9
 Summary: JustBard's Python based AWS Utilities
 Home-page: http://justbard.com
 Author: Justin Bard
 Author-email: JustinBard@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jblib-aws
@@ -35,15 +33,15 @@
     class talk_with_dynamo(table, boto_session, region='us-east-1')
 
         Example:
             table_name = "table-name"
             boto_session = boto3.session.Session()
             dynamo = talk_with_dynamo(table_name, boto_session) ## Generate Database Object
 
-            response = dynamo.query(partition_key=partition_key, partition_key_attribute=partition_key_attribute, sorting_key=sorting_key, sorting_key_attribute=sorting_key_attribute, index=index_key)
+            response = dynamo.query(self, partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False, index=False, queryOperator=False, betweenValue=False)
             print ("Resposne: {}".format(response))
 
 			getResponse = dynamo.getItem(partition_key, partition_key_attribute, sorting_key=False, sorting_key_attribute=False)
 
 			batch_keys = {'tableName': {'Keys': [{'PartitionKey': 'PartitionKeyAttribute', 'SortingKey': 'SortingKey'}]}}
 			batchResponse = dynamo.batchGetItem(batch_keys)
 
@@ -68,9 +66,7 @@
         Functions:
             get_user_email(cognito_user_id)
             - Gets User Email Address
 
 ```
 
 ### More Documentation To Come
-
-
```

### Comparing `jblibaws-1.0.8/setup.py` & `jblibaws-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='jblibaws',
-                version='1.0.8',
+                version='1.0.9',
                 description='JustBard\'s Python based AWS Utilities',
                 long_description=long_description,
                 long_description_content_type="text/markdown",
                 author='Justin Bard',
                 author_email='JustinBard@gmail.com',
                 url='http://justbard.com',
                 packages=setuptools.find_packages(),
```

