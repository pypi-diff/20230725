# Comparing `tmp/oms-mqclient-2.3.3.tar.gz` & `tmp/oms-mqclient-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.3.3.tar", last modified: Tue Jul 25 17:23:55 2023, max compression
+gzip compressed data, was "oms-mqclient-2.3.4.tar", last modified: Tue Jul 25 18:56:48 2023, max compression
```

## Comparing `oms-mqclient-2.3.3.tar` & `oms-mqclient-2.3.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.596529 oms-mqclient-2.3.3/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-25 17:23:52.000000 oms-mqclient-2.3.3/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6667 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14402 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    14188 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    17161 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    23781 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2722 2023-07-25 17:23:55.604529 oms-mqclient-2.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.596529 oms-mqclient-2.3.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    38854 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-25 18:56:46.000000 oms-mqclient-2.3.4/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6667 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14402 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    17161 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23781 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      502 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    38812 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.3.3/LICENSE` & `oms-mqclient-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/PKG-INFO` & `oms-mqclient-2.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.3
+Version: 2.3.4
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
@@ -21,14 +21,15 @@
 Provides-Extra: all
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
 Provides-Extra: nats
 Provides-Extra: telemetry
 Provides-Extra: dev
 Provides-Extra: integration
+Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/oms-mqclient)](https://pypi.org/project/oms-mqclient/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/MQClient?include_prereleases)](https://github.com/Observation-Management-Service/MQClient/) [![PyPI - License](https://img.shields.io/pypi/l/oms-mqclient)](https://github.com/Observation-Management-Service/MQClient/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # MQClient
```

### Comparing `oms-mqclient-2.3.3/README.md` & `oms-mqclient-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/__init__.py` & `oms-mqclient-2.3.4/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.3.3"
+__version__ = "2.3.4"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.3.3/mqclient/broker_client_interface.py` & `oms-mqclient-2.3.4/mqclient/broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/broker_client_manager.py` & `oms-mqclient-2.3.4/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.3.4/mqclient/broker_clients/apachepulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/broker_clients/nats.py` & `oms-mqclient-2.3.4/mqclient/broker_clients/nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.3.4/mqclient/broker_clients/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/broker_clients/utils.py` & `oms-mqclient-2.3.4/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/log_msgs.py` & `oms-mqclient-2.3.4/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/queue.py` & `oms-mqclient-2.3.4/mqclient/queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/mqclient/telemetry.py` & `oms-mqclient-2.3.4/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.3.4/oms_mqclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.3
+Version: 2.3.4
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
@@ -21,14 +21,15 @@
 Provides-Extra: all
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
 Provides-Extra: nats
 Provides-Extra: telemetry
 Provides-Extra: dev
 Provides-Extra: integration
+Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/oms-mqclient)](https://pypi.org/project/oms-mqclient/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/MQClient?include_prereleases)](https://github.com/Observation-Management-Service/MQClient/) [![PyPI - License](https://img.shields.io/pypi/l/oms-mqclient)](https://github.com/Observation-Management-Service/MQClient/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # MQClient
```

### Comparing `oms-mqclient-2.3.3/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.3.4/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/setup.cfg` & `oms-mqclient-2.3.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 	pytest-mock
 	mock
 	coloredlogs
 integration = 
 	wipac-keycloak-rest-services
 	wipac-rest-tools
 	pytest-xdist
+mypy = 
+	%(all)s
+	%(telemetry)s
+	%(dev)s
+	%(integration)s
 
 [options.package_data]
 * = py.typed
 
 [options.packages.find]
 exclude = 
 	test
```

### Comparing `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,17 @@
 
         n_subs_that_got_msgs = 0
         for sublist in received_data:
             if sublist:
                 n_subs_that_got_msgs += 1
                 all_recvd.extend(sublist)
         # since threads are mixed, can't test like test_020
-        if num_subs < len(DATA_LIST):
-            assert n_subs_that_got_msgs == num_subs
-        else:
-            logging.debug(f"{n_subs_that_got_msgs=}")
-            assert n_subs_that_got_msgs == len(DATA_LIST)
+        # the threading makes us not able to assert how many, but it should be >= 1
+        logging.debug(f"{n_subs_that_got_msgs=}")
+        assert n_subs_that_got_msgs > 2
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_030(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
```

### Comparing `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/integrate/conftest.py` & `oms-mqclient-2.3.4/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/integrate/test_nats.py` & `oms-mqclient-2.3.4/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/integrate/test_pulsar.py` & `oms-mqclient-2.3.4/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.3.4/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.3.4/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.3/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.3.4/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

