# Comparing `tmp/gym_cas-0.0.7.tar.gz` & `tmp/gym_cas-0.0.8.tar.gz`

## Comparing `gym_cas-0.0.7.tar` & `gym_cas-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gym_cas-0.0.7/bitbucket-pipelines.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 gym_cas-0.0.7/examples/cheatsheet.ipynb
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/__init__.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/plot.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/trigonometry.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/test_abc.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/test_trigonometry.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 gym_cas-0.0.7/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.7/hatch.toml
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 gym_cas-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 gym_cas-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gym_cas-0.0.8/bitbucket-pipelines.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0   161524 2020-02-02 00:00:00.000000 gym_cas-0.0.8/examples/cheatsheet.ipynb
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.8/src/gym_cas/__about__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 gym_cas-0.0.8/src/gym_cas/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gym_cas-0.0.8/src/gym_cas/trigonometry.py
+-rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 gym_cas-0.0.8/src/gym_cas/vector.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 gym_cas-0.0.8/tests/test_abc.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 gym_cas-0.0.8/tests/test_trigonometry.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 gym_cas-0.0.8/tests/test_vector.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 gym_cas-0.0.8/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.8/hatch.toml
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 gym_cas-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 gym_cas-0.0.8/PKG-INFO
```

### Comparing `gym_cas-0.0.7/src/gym_cas/trigonometry.py` & `gym_cas-0.0.8/src/gym_cas/trigonometry.py`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.7/tests/test_trigonometry.py` & `gym_cas-0.0.8/tests/test_trigonometry.py`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.7/LICENSE.txt` & `gym_cas-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.7/hatch.toml` & `gym_cas-0.0.8/hatch.toml`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.7/pyproject.toml` & `gym_cas-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.7/PKG-INFO` & `gym_cas-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-cas
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to aid the use of Python as CAS in danish high schools.
 Project-URL: Homepage, https://jacs-mat.bitbucket.io/
 Author-email: JACS <jacs@zbc.dk>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: CAS, Matematik, Math, Gymnasium, HTX
 Classifier: Development Status :: 3 - Alpha
@@ -69,7 +69,34 @@
 Cos( vinkel )
 Tan( vinkel )
 aSin( forhold )
 aCos( forhold )
 aTan( forhold )
 ```
 
+### B4. Analytisk plangeometri
+
+```py
+plot_list( X_list ,Y_list, is_point=True)
+plot( funktion )
+plot_implicit( udtryk ,xlim=( x_min, x_max),ylim=( y_min, y_max))
+plot_geometry( Geometrisk objekt )
+```
+
+#### Flere grafer i en afbildning
+
+```py
+p1 = plot( udtryk1 )
+p2 = plot( udtryk2 )
+p = p1 + p2
+p.show()
+```
+
+### B5. Vektorer
+
+```py
+a = Matrix([x,y])
+a.dot(b)
+plot_vector( vektor )
+plot_vector( start, vektor )
+plot_vector( [vektor1, vektor2, ...])
+```
```

