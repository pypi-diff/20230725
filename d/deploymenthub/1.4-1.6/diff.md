# Comparing `tmp/deploymenthub-1.4.tar.gz` & `tmp/deploymenthub-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-1.4.tar", last modified: Fri Apr  8 01:10:42 2022, max compression
+gzip compressed data, was "deploymenthub-1.6.tar", last modified: Tue Jul 25 04:52:50 2023, max compression
```

## Comparing `deploymenthub-1.4.tar` & `deploymenthub-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2022-04-08 01:10:42.372868 deploymenthub-1.4/
--rw-r--r--   0 jared      (501) staff       (20)     1050 2021-06-14 05:14:23.000000 deploymenthub-1.4/LICENSE.txt
--rw-r--r--   0 jared      (501) staff       (20)      452 2022-04-08 01:10:42.372759 deploymenthub-1.4/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)      124 2021-06-26 03:49:44.000000 deploymenthub-1.4/README.md
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2022-04-08 01:10:42.372060 deploymenthub-1.4/bin/
--rw-r--r--   0 jared      (501) staff       (20)     1169 2022-04-08 00:50:08.000000 deploymenthub-1.4/bin/deploymenthub
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2022-04-08 01:10:42.372632 deploymenthub-1.4/deploymenthub.egg-info/
--rw-r--r--   0 jared      (501) staff       (20)      452 2022-04-08 01:10:42.000000 deploymenthub-1.4/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)      196 2022-04-08 01:10:42.000000 deploymenthub-1.4/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jared      (501) staff       (20)        1 2022-04-08 01:10:42.000000 deploymenthub-1.4/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jared      (501) staff       (20)        1 2022-04-08 01:10:42.000000 deploymenthub-1.4/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jared      (501) staff       (20)       38 2022-04-08 01:10:42.372902 deploymenthub-1.4/setup.cfg
--rw-r--r--   0 jared      (501) staff       (20)      683 2022-04-08 01:06:56.000000 deploymenthub-1.4/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 04:52:50.228038 deploymenthub-1.6/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-1.6/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-25 04:52:50.227874 deploymenthub-1.6/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-1.6/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 04:52:50.226860 deploymenthub-1.6/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1170 2023-07-25 04:40:51.000000 deploymenthub-1.6/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 04:52:50.227643 deploymenthub-1.6/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-25 04:52:50.000000 deploymenthub-1.6/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-25 04:52:50.000000 deploymenthub-1.6/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-25 04:52:50.000000 deploymenthub-1.6/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-25 04:52:50.000000 deploymenthub-1.6/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-25 04:52:50.228080 deploymenthub-1.6/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      683 2023-07-25 04:52:36.000000 deploymenthub-1.6/setup.py
```

### Comparing `deploymenthub-1.4/LICENSE.txt` & `deploymenthub-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-1.4/bin/deploymenthub` & `deploymenthub-1.6/bin/deploymenthub`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                         help='Branch you want to deploy.')
     parser.parse_args()
     args = parser.parse_args()
 
     project = args.project
     action = args.action
     branch = args.branch
-    url = "http://192.168.1.254:5000"
+    url = "http://192.168.0.216/:5000"
 
     list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops']
 
     if project in list_of_projects:
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
```

### Comparing `deploymenthub-1.4/setup.py` & `deploymenthub-1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version=1.4,
+    version=1.6,
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

