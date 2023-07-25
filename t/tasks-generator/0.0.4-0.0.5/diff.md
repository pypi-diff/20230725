# Comparing `tmp/tasks_generator-0.0.4.tar.gz` & `tmp/tasks_generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasks_generator-0.0.4.tar", last modified: Fri Jul 21 22:40:17 2023, max compression
+gzip compressed data, was "tasks_generator-0.0.5.tar", last modified: Tue Jul 25 19:50:21 2023, max compression
```

## Comparing `tasks_generator-0.0.4.tar` & `tasks_generator-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 22:40:17.565599 tasks_generator-0.0.4/
--rw-rw-rw-   0        0        0     1084 2023-07-16 14:24:05.000000 tasks_generator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2100 2023-07-21 22:40:17.564599 tasks_generator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1615 2023-07-21 22:39:48.000000 tasks_generator-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 22:40:17.565599 tasks_generator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-07-21 22:40:05.000000 tasks_generator-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 22:40:17.560598 tasks_generator-0.0.4/tasks_generator/
--rw-rw-rw-   0        0        0        0 2023-07-16 14:18:45.000000 tasks_generator-0.0.4/tasks_generator/__init__.py
--rw-rw-rw-   0        0        0    25652 2023-07-21 22:28:44.000000 tasks_generator-0.0.4/tasks_generator/logarithms.py
--rw-rw-rw-   0        0        0      182 2023-07-20 14:02:35.000000 tasks_generator-0.0.4/tasks_generator/super_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 22:40:17.563599 tasks_generator-0.0.4/tasks_generator.egg-info/
--rw-rw-rw-   0        0        0     2100 2023-07-21 22:40:17.000000 tasks_generator-0.0.4/tasks_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-21 22:40:17.000000 tasks_generator-0.0.4/tasks_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 22:40:17.000000 tasks_generator-0.0.4/tasks_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 22:40:17.000000 tasks_generator-0.0.4/tasks_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 19:50:21.955290 tasks_generator-0.0.5/
+-rw-rw-rw-   0        0        0     1084 2023-07-16 14:24:05.000000 tasks_generator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2197 2023-07-25 19:50:21.954290 tasks_generator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1712 2023-07-25 19:49:54.000000 tasks_generator-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 19:50:21.955290 tasks_generator-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-07-25 19:47:30.000000 tasks_generator-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:50:21.948289 tasks_generator-0.0.5/tasks_generator/
+-rw-rw-rw-   0        0        0        0 2023-07-16 14:18:45.000000 tasks_generator-0.0.5/tasks_generator/__init__.py
+-rw-rw-rw-   0        0        0    42683 2023-07-25 19:47:09.000000 tasks_generator-0.0.5/tasks_generator/logarithms.py
+-rw-rw-rw-   0        0        0      182 2023-07-20 14:02:35.000000 tasks_generator-0.0.5/tasks_generator/super_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:50:21.953290 tasks_generator-0.0.5/tasks_generator.egg-info/
+-rw-rw-rw-   0        0        0     2197 2023-07-25 19:50:21.000000 tasks_generator-0.0.5/tasks_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-25 19:50:21.000000 tasks_generator-0.0.5/tasks_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:50:21.000000 tasks_generator-0.0.5/tasks_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 19:50:21.000000 tasks_generator-0.0.5/tasks_generator.egg-info/top_level.txt
```

### Comparing `tasks_generator-0.0.4/LICENSE` & `tasks_generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tasks_generator-0.0.4/PKG-INFO` & `tasks_generator-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasks_generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This module was written for education in math, by generating math tasks
 Home-page: https://github.com/XxXDeathmatchXxX/tasks_generator.git
 Author: Kirill Kudinov
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -31,15 +31,15 @@
 
     pip install tasks-generator
 
 # Usage
 
 Here is an example of how you would generate logarithm tasks:
     
-    import tasks_generator
+    from tasks_generator import logarithms
 #generate random task:
 
     answer, task = tasks_generator.logarithm_generator()
     print(task)
     print(answer)
 
 
@@ -66,14 +66,16 @@
     logarithms_addition()
     figure_in_logaritms_degree_addition()
     figures_in_logaritms_degree_addition()
     logarithms_subtraction()
     logarithms_subtraction_new()
     figure_in_logaritms_degree_subtarction()
     figures_in_logaritms_degree_subtarction()
+    logarithm_addition_of_divisions()
+    logarithm_subtraction_of_divisions()
     logarithm_generator()
 
 Use [answer, task] variables
```

### Comparing `tasks_generator-0.0.4/README.md` & `tasks_generator-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     pip install tasks-generator
 
 # Usage
 
 Here is an example of how you would generate logarithm tasks:
     
-    import tasks_generator
+    from tasks_generator import logarithms
 #generate random task:
 
     answer, task = tasks_generator.logarithm_generator()
     print(task)
     print(answer)
 
 
@@ -53,14 +53,16 @@
     logarithms_addition()
     figure_in_logaritms_degree_addition()
     figures_in_logaritms_degree_addition()
     logarithms_subtraction()
     logarithms_subtraction_new()
     figure_in_logaritms_degree_subtarction()
     figures_in_logaritms_degree_subtarction()
+    logarithm_addition_of_divisions()
+    logarithm_subtraction_of_divisions()
     logarithm_generator()
 
 Use [answer, task] variables
```

### Comparing `tasks_generator-0.0.4/setup.py` & `tasks_generator-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
         name='tasks_generator',
-        version='0.0.4',
+        version='0.0.5',
         description='This module was written for education in math, by generating math tasks',
         author='Kirill Kudinov',
         license='MIT',
         url='https://github.com/XxXDeathmatchXxX/tasks_generator.git',
         packages=find_packages(exclude=['random, math']),
         long_description=open('README.md').read(),
         long_description_content_type='text/markdown',
```

### Comparing `tasks_generator-0.0.4/tasks_generator.egg-info/PKG-INFO` & `tasks_generator-0.0.5/tasks_generator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasks-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This module was written for education in math, by generating math tasks
 Home-page: https://github.com/XxXDeathmatchXxX/tasks_generator.git
 Author: Kirill Kudinov
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -31,15 +31,15 @@
 
     pip install tasks-generator
 
 # Usage
 
 Here is an example of how you would generate logarithm tasks:
     
-    import tasks_generator
+    from tasks_generator import logarithms
 #generate random task:
 
     answer, task = tasks_generator.logarithm_generator()
     print(task)
     print(answer)
 
 
@@ -66,14 +66,16 @@
     logarithms_addition()
     figure_in_logaritms_degree_addition()
     figures_in_logaritms_degree_addition()
     logarithms_subtraction()
     logarithms_subtraction_new()
     figure_in_logaritms_degree_subtarction()
     figures_in_logaritms_degree_subtarction()
+    logarithm_addition_of_divisions()
+    logarithm_subtraction_of_divisions()
     logarithm_generator()
 
 Use [answer, task] variables
```

