# Comparing `tmp/cnvrg_experiment_chart-0.1.10.tar.gz` & `tmp/cnvrg_experiment_chart-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnvrg_experiment_chart-0.1.10.tar", last modified: Tue Jul 25 19:21:09 2023, max compression
+gzip compressed data, was "cnvrg_experiment_chart-0.1.6.tar", last modified: Sat Jul 22 19:41:20 2023, max compression
```

## Comparing `cnvrg_experiment_chart-0.1.10.tar` & `cnvrg_experiment_chart-0.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.366577 cnvrg_experiment_chart-0.1.10/
--rw-r--r--   0 root         (0) root         (0)      605 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/.gitignore
--rw-r--r--   0 root         (0) root         (0)      468 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      530 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)       74 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)    14009 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     1732 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/Jenkinsfile
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-25 19:21:09.367577 cnvrg_experiment_chart-0.1.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.364577 cnvrg_experiment_chart-0.1.10/docs/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.364577 cnvrg_experiment_chart-0.1.10/docs/_static/
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/_static/.gitignore
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     9844 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/readme.rst
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/docs/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1377 2023-07-25 19:21:09.367577 cnvrg_experiment_chart-0.1.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      717 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.359577 cnvrg_experiment_chart-0.1.10/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.365577 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart/
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4689 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart/chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.366577 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-25 19:21:09.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-25 19:21:09.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 19:21:09.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 19:20:47.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-25 19:21:09.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 19:21:09.000000 cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:21:09.366577 cnvrg_experiment_chart-0.1.10/tests/
--rw-r--r--   0 root         (0) root         (0)      290 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/tests/test_chart.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-07-25 19:19:57.000000 cnvrg_experiment_chart-0.1.10/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.450811 cnvrg_experiment_chart-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      530 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/.readthedocs.yml
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)    14009 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/Jenkinsfile
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-22 19:41:20.450811 cnvrg_experiment_chart-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.448811 cnvrg_experiment_chart-0.1.6/docs/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.448811 cnvrg_experiment_chart-0.1.6/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/_static/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     9844 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)     2373 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/readme.rst
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/docs/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-07-22 19:41:20.451811 cnvrg_experiment_chart-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      717 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.444811 cnvrg_experiment_chart-0.1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.449811 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4689 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart/chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.450811 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-07-22 19:41:20.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-22 19:41:20.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 19:41:20.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 19:41:00.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-22 19:41:20.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-22 19:41:20.000000 cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 19:41:20.450811 cnvrg_experiment_chart-0.1.6/tests/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/tests/test_chart.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-07-22 19:40:13.000000 cnvrg_experiment_chart-0.1.6/tox.ini
```

### Comparing `cnvrg_experiment_chart-0.1.10/.coveragerc` & `cnvrg_experiment_chart-0.1.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/.gitignore` & `cnvrg_experiment_chart-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/.readthedocs.yml` & `cnvrg_experiment_chart-0.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/CONTRIBUTING.rst` & `cnvrg_experiment_chart-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/Jenkinsfile` & `cnvrg_experiment_chart-0.1.6/Jenkinsfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,57 @@
-pipeline {
-    agent {
-        kubernetes {
-            defaultContainer 'python'
-            yaml '''
-            apiVersion: v1
-            kind: Pod
-            spec:
-              containers:
-              - name: python
-                image: nctiggy/python-build-image
-                command:
-                - sleep
-                args:
-                - 99d
-            '''
-        }
-    }
+podTemplate(yaml: '''
+    apiVersion: v1
+    kind: Pod
+    spec:
+      containers:
+      - name: python
+        image: nctiggy/python-build-image
+        command:
+        - sleep
+        args:
+        - 99d
+''')
 
-    stages {
-        stage('Print runtime versions') {
-            steps {
-                sh '''
-                    python --version
-                    ls -ltra
-                    printenv
-                    git --version
-                    git remote show origin
-                '''
-            }
+{
+  node(POD_LABEL) {
+      checkout scmGit(
+        branches: [[name: '*/tags/*']],
+        userRemoteConfigs: [[
+            refspec: '+refs/tags/*’:’refs/remotes/origin/tags/*',
+            url: 'https://github.com/nctiggy/cnvrg_experiment_chart.git']]
+        )
+      container('python') {
+        stage('Python version') {
+          sh '''
+            python --version
+            ls -ltra
+            printenv
+            git --version
+            git remote show origin
+            git tag -l
+            git describe
+          '''
         }
-        stage('Testing') {
-            environment {
-                COVERALLS_REPO_TOKEN = credentials('coverallsToken')
-            }
-            steps {
-                sh '''
-                    tox -e lint
-                    tox -- --junitxml=junit-result.xml
-                '''
-                junit 'junit-result.xml'
-            }
+        stage('Run Tests') {
+          sh '''
+            tox -e lint
+            tox
+          '''
         }
         stage('Build pypi package') {
-            when {
-                buildingTag()
-            }
-            steps {
-                sh 'tox -e build'
-            }
+          sh '''
+            tox -e build
+          '''
         }
-        stage('Publish pypi package') {
-            when {
-                buildingTag()
-            }
-            environment {
-                TWINE = credentials('pypi_user_pass')
-            }
-            steps {
-                sh '''
-                    export TWINE_PASSWORD=$TWINE_PSW
-                    export TWINE_USERNAME=$TWINE_USR
-                    tox -e publish -- --repository pypi
-                    tox -e clean
-                '''
-            }
+        withCredentials([usernamePassword(credentialsId: 'pypi_user_pass', passwordVariable: 'TWINE_PASSWORD', usernameVariable: 'TWINE_USERNAME')]) {
+          stage('Publish pypi package') {
+            sh '''
+              export TWINE_PASSWORD=$TWINE_PASSWORD
+              export TWINE_USERNAME=$TWINE_USERNAME
+              tox -e publish -- --repository pypi
+              tox -e clean
+            '''
+          }
         }
-    }
+      }
+  }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cnvrg_experiment_chart-0.1.10/LICENSE.txt` & `cnvrg_experiment_chart-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/README.rst` & `cnvrg_experiment_chart-0.1.6/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,47 @@
-.. image:: https://readthedocs.org/projects/cnvrg_experiment_chart/badge/?version=latest
-    :alt: ReadTheDocs
-    :target: https://cnvrg_experiment_chart.readthedocs.io/en/stable/
-.. image:: https://img.shields.io/coveralls/github/nctiggy/cnvrg_experiment_chart/main.svg
-    :alt: Coveralls
-    :target: https://coveralls.io/r/nctiggy/cnvrg_experiment_chart
-.. image:: https://img.shields.io/pypi/v/cnvrg_experiment_chart.svg
-    :alt: PyPI-Server
-    :target: https://pypi.org/project/cnvrg_experiment_chart/
-.. image:: https://static.pepy.tech/personalized-badge/cnvrg-experiment-chart?period=total&units=international_system&left_color=red&right_color=black&left_text=Downloads
-    :alt: Monthly Downloads
-    :target: https://pepy.tech/project/cnvrg_experiment_chart
+.. These are examples of badges you might want to add to your README:
+   please update the URLs accordingly
+
+    .. image:: https://api.cirrus-ci.com/github/<USER>/cnvrg_experiment_chart.svg?branch=main
+        :alt: Built Status
+        :target: https://cirrus-ci.com/github/<USER>/cnvrg_experiment_chart
+    .. image:: https://readthedocs.org/projects/cnvrg_experiment_chart/badge/?version=latest
+        :alt: ReadTheDocs
+        :target: https://cnvrg_experiment_chart.readthedocs.io/en/stable/
+    .. image:: https://img.shields.io/coveralls/github/<USER>/cnvrg_experiment_chart/main.svg
+        :alt: Coveralls
+        :target: https://coveralls.io/r/<USER>/cnvrg_experiment_chart
+    .. image:: https://img.shields.io/pypi/v/cnvrg_experiment_chart.svg
+        :alt: PyPI-Server
+        :target: https://pypi.org/project/cnvrg_experiment_chart/
+    .. image:: https://img.shields.io/conda/vn/conda-forge/cnvrg_experiment_chart.svg
+        :alt: Conda-Forge
+        :target: https://anaconda.org/conda-forge/cnvrg_experiment_chart
+    .. image:: https://pepy.tech/badge/cnvrg_experiment_chart/month
+        :alt: Monthly Downloads
+        :target: https://pepy.tech/project/cnvrg_experiment_chart
+    .. image:: https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter
+        :alt: Twitter
+        :target: https://twitter.com/cnvrg_experiment_chart
+
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
 |
 
 ======================
 cnvrg_experiment_chart
 ======================
 
 
-    This is a helper library to make using cnvrg charts a more intuitive
-    process. Currently line charts are the only supported kinds.
+    Add a short description here!
+
+
+A longer description of your project goes here...
 
 
 .. _pyscaffold-notes:
 
 Note
 ====
```

### Comparing `cnvrg_experiment_chart-0.1.10/docs/Makefile` & `cnvrg_experiment_chart-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/docs/conf.py` & `cnvrg_experiment_chart-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/setup.cfg` & `cnvrg_experiment_chart-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/setup.py` & `cnvrg_experiment_chart-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart/__init__.py` & `cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart/chart.py` & `cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart/chart.py`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/src/cnvrg_experiment_chart.egg-info/SOURCES.txt` & `cnvrg_experiment_chart-0.1.6/src/cnvrg_experiment_chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/tests/test_chart.py` & `cnvrg_experiment_chart-0.1.6/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `cnvrg_experiment_chart-0.1.10/tox.ini` & `cnvrg_experiment_chart-0.1.6/tox.ini`

 * *Files identical despite different names*

