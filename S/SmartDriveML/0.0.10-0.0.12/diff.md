# Comparing `tmp/SmartDriveML-0.0.10.tar.gz` & `tmp/SmartDriveML-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartDriveML-0.0.10.tar", last modified: Fri Jun 23 19:24:50 2023, max compression
+gzip compressed data, was "SmartDriveML-0.0.12.tar", last modified: Tue Jul 25 13:59:35 2023, max compression
```

## Comparing `SmartDriveML-0.0.10.tar` & `SmartDriveML-0.0.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:50.965348 SmartDriveML-0.0.10/
--rw-rw-rw-   0        0        0     1791 2023-06-23 19:24:50.965348 SmartDriveML-0.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:50.934082 SmartDriveML-0.0.10/SmartDriveML/
--rw-rw-rw-   0        0        0        0 2023-06-23 19:23:23.000000 SmartDriveML-0.0.10/SmartDriveML/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-23 19:21:16.000000 SmartDriveML-0.0.10/SmartDriveML/mlFunctions.py
--rw-rw-rw-   0        0        0      238 2023-06-23 19:14:37.000000 SmartDriveML-0.0.10/SmartDriveML/priceAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:50.965348 SmartDriveML-0.0.10/SmartDriveML.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-06-23 19:24:50.000000 SmartDriveML-0.0.10/SmartDriveML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-23 19:24:50.000000 SmartDriveML-0.0.10/SmartDriveML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:24:50.000000 SmartDriveML-0.0.10/SmartDriveML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 19:24:50.000000 SmartDriveML-0.0.10/SmartDriveML.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 19:24:50.000000 SmartDriveML-0.0.10/SmartDriveML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 19:24:50.965348 SmartDriveML-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0     2989 2023-06-23 19:24:44.000000 SmartDriveML-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:59:35.331858 SmartDriveML-0.0.12/
+-rw-rw-rw-   0        0        0     1791 2023-07-25 13:59:35.331858 SmartDriveML-0.0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 13:59:35.316234 SmartDriveML-0.0.12/SmartDriveML/
+-rw-rw-rw-   0        0        0        0 2023-06-23 19:23:23.000000 SmartDriveML-0.0.12/SmartDriveML/__init__.py
+-rw-rw-rw-   0        0        0      284 2023-07-25 13:57:17.000000 SmartDriveML-0.0.12/SmartDriveML/mlFunctions.py
+-rw-rw-rw-   0        0        0      238 2023-06-23 19:14:37.000000 SmartDriveML-0.0.12/SmartDriveML/priceAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:59:35.331858 SmartDriveML-0.0.12/SmartDriveML.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-07-25 13:59:35.000000 SmartDriveML-0.0.12/SmartDriveML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-25 13:59:35.000000 SmartDriveML-0.0.12/SmartDriveML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:59:35.000000 SmartDriveML-0.0.12/SmartDriveML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 13:59:35.000000 SmartDriveML-0.0.12/SmartDriveML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 13:59:35.000000 SmartDriveML-0.0.12/SmartDriveML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:59:35.331858 SmartDriveML-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0     2989 2023-07-25 13:58:48.000000 SmartDriveML-0.0.12/setup.py
```

### Comparing `SmartDriveML-0.0.10/PKG-INFO` & `SmartDriveML-0.0.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.10
+Version: 0.0.12
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.10/SmartDriveML.egg-info/PKG-INFO` & `SmartDriveML-0.0.12/SmartDriveML.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.10
+Version: 0.0.12
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.10/setup.py` & `SmartDriveML-0.0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.10'
+VERSION = '0.0.12'
 DESCRIPTION = 'SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices'
 LONG_DESCRIPTION = 'SmartDriveML is a state-of-the-art Python library created to revolutionize the way industries drive projects using machine learning. This advanced application serves as a comprehensive tool, assisting users in making informed decisions regarding cloud service providers, framework selection, and project feasibility, all while maintaining a cost-effective approach. One of the core functionalities of SmartDriveML is its ability to compare costs among various cloud service providers. By leveraging its integrated algorithms and extensive data on cloud service pricing, this tool enables users to evaluate the financial implications of different providers such as AWS or Azure. With this crucial information at their disposal, industries can optimize their budget allocation, ensuring that their machine learning projects remain economically viable. Another essential feature of SmartDriveML is its framework analysis capability. The library provides comprehensive insights into popular frameworks like Pandas and PySpark, aiding users in choosing the most suitable option for their specific project requirements. By considering factors such as data volume, computational needs, and ease of implementation, SmartDriveML helps industries make informed decisions that align with their objectives and resource constraints. Moreover, SmartDriveML goes beyond cost and framework analysis by providing essential functions for exploratory data analysis and executing fundamental machine learning algorithms on sample datasets. These functions enable users to assess the potential of their projects, allowing them to evaluate whether machine learning can effectively drive their initiatives. By providing this accessible yet powerful toolset, SmartDriveML empowers industries to make data-driven decisions and confidently embark on machine learning-driven projects.'
 
 # Setting up
 setup(
     name="SmartDriveML",
     version=VERSION,
```

