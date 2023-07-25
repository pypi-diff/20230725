# Comparing `tmp/routingfilter-1.6.2.tar.gz` & `tmp/routingfilter-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.6.2.tar", last modified: Thu Jun 15 16:58:53 2023, max compression
+gzip compressed data, was "routingfilter-1.6.3.tar", last modified: Tue Jul 25 10:30:37 2023, max compression
```

## Comparing `routingfilter-1.6.2.tar` & `routingfilter-1.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 16:58:40.000000 routingfilter-1.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:58:40.000000 routingfilter-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 16:58:53.319733 routingfilter-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 16:58:40.000000 routingfilter-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 16:58:40.000000 routingfilter-1.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:58:53.319733 routingfilter-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 16:58:40.000000 routingfilter-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:30:37.011131 routingfilter-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-25 10:30:25.000000 routingfilter-1.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:30:25.000000 routingfilter-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 10:30:37.011131 routingfilter-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 10:30:25.000000 routingfilter-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 10:30:25.000000 routingfilter-1.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:30:37.007131 routingfilter-1.6.3/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/routing_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-25 10:30:25.000000 routingfilter-1.6.3/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:30:37.011131 routingfilter-1.6.3/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 10:30:36.000000 routingfilter-1.6.3/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 10:30:37.000000 routingfilter-1.6.3/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:30:37.000000 routingfilter-1.6.3/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 10:30:37.000000 routingfilter-1.6.3/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 10:30:37.000000 routingfilter-1.6.3/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:30:37.011131 routingfilter-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-25 10:30:25.000000 routingfilter-1.6.3/setup.py
```

### Comparing `routingfilter-1.6.2/LICENSE.txt` & `routingfilter-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.2/PKG-INFO` & `routingfilter-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.2
+Version: 1.6.3
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.2/README.md` & `routingfilter-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.2/routingfilter/configfilter.py` & `routingfilter-1.6.3/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.2/routingfilter/dictquery.py` & `routingfilter-1.6.3/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.2/routingfilter/routing.py` & `routingfilter-1.6.3/routingfilter/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,20 @@
         :param type_: The event type (can be 'streams', 'customer' or everything else, as defined in the routing config). If the type does not exists, an empty list is returned
         :type type_: str
         :param tag_field_name: The event field to search into (default='tags')
         :type tag_field_name: str
         :return: A list of dicts containing the matched rules and the outputs in the following format: {"rules": [...], "output": {...}}; an empty list if no rule matched
         :rtype: List[dict]
         """
-        if not event.get("certego", {}).get("routing_history", {}):
-            event["certego"] = {"routing_history": {}}
+        # Creating routing_history if not present
+        if "certego" not in event:
+            event["certego"] = {}
+        if "routing_history" not in event["certego"]:
+            event["certego"]["routing_history"] = {}
+        # check for rules
         if not self.rules:
             self.logger.error("'rules_list' must be set before evaluating a match!")
             raise ValueError("'rules_list' must be set before evaluating a match!")
         if type_ not in self.rules:
             return []
 
         # iterate through the common set of tags
```

### Comparing `routingfilter-1.6.2/routingfilter/routing_benchmark.py` & `routingfilter-1.6.3/routingfilter/routing_benchmark.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.2/routingfilter/routing_test.py` & `routingfilter-1.6.3/routingfilter/routing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,17 +369,17 @@
                   "RacePro"
                 ]
               }
             ],
             "streams": {
             }
           }
-        self.assertFalse(self.routing.rule_in_routing_history(event, rule))
+        self.assertFalse(self.routing.rule_in_routing_history("streams", event, rule))
         event = {"certego": {"routing_history": {"Workshop": "2023-06-06T18:00:00.000Z"}}}
-        self.assertFalse(self.routing.rule_in_routing_history(event, rule))
+        self.assertFalse(self.routing.rule_in_routing_history("streams", event, rule))
         rule = {
             "filters": [
               {
                 "type": "EQUALS",
                 "key": "wheel_model",
                 "description": "Carbon fiber wheels needs manual truing",
                 "value": [
@@ -390,10 +390,10 @@
             ],
             "streams": {
                 "Workshop": {
                     "workers_needed": 1
                 }
             }
           }
-        self.assertTrue(self.routing.rule_in_routing_history(event, rule))
+        self.assertTrue(self.routing.rule_in_routing_history("streams", event, rule))
```

### Comparing `routingfilter-1.6.2/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.6.3/routingfilter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.2
+Version: 1.6.3
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.2/setup.py` & `routingfilter-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.6.2',
+    version='1.6.3',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

