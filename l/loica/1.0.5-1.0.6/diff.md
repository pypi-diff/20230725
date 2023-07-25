# Comparing `tmp/loica-1.0.5.tar.gz` & `tmp/loica-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loica-1.0.5.tar", last modified: Sat Mar 19 02:06:49 2022, max compression
+gzip compressed data, was "loica-1.0.6.tar", last modified: Tue Jul 25 14:17:21 2023, max compression
```

## Comparing `loica-1.0.5.tar` & `loica-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2022-03-19 02:06:49.889720 loica-1.0.5/
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     1073 2022-03-19 01:57:25.000000 loica-1.0.5/LICENSE
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     2278 2022-03-19 02:06:49.889352 loica-1.0.5/PKG-INFO
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     1802 2022-03-19 01:57:25.000000 loica-1.0.5/README.md
-drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2022-03-19 02:06:49.880593 loica-1.0.5/loica/
--rw-r--r--   0 gonzalovidal   (501) staff       (20)      220 2022-01-31 21:43:07.000000 loica-1.0.5/loica/__init__.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     6487 2022-03-19 01:57:26.000000 loica-1.0.5/loica/assay.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     2846 2022-01-31 21:43:07.000000 loica-1.0.5/loica/colony.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     2491 2022-03-19 01:57:26.000000 loica-1.0.5/loica/geneproduct.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)    20044 2022-03-19 01:57:26.000000 loica-1.0.5/loica/genetic_network.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     3763 2022-03-19 01:57:26.000000 loica-1.0.5/loica/metabolism.py
-drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2022-03-19 02:06:49.888485 loica-1.0.5/loica/operators/
--rw-r--r--   0 gonzalovidal   (501) staff       (20)      112 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/__init__.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     6752 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/hill1.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     9430 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/hill2.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)      869 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/operator.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     5538 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/receiver.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     4409 2022-03-19 01:57:26.000000 loica-1.0.5/loica/operators/source.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     2430 2022-01-31 21:43:07.000000 loica-1.0.5/loica/sample.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     1080 2022-03-19 01:57:26.000000 loica-1.0.5/loica/supplement.py
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     3402 2022-01-31 21:43:07.000000 loica-1.0.5/loica/util.py
-drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2022-03-19 02:06:49.884296 loica-1.0.5/loica.egg-info/
--rw-r--r--   0 gonzalovidal   (501) staff       (20)     2278 2022-03-19 02:06:49.000000 loica-1.0.5/loica.egg-info/PKG-INFO
--rw-r--r--   0 gonzalovidal   (501) staff       (20)      495 2022-03-19 02:06:49.000000 loica-1.0.5/loica.egg-info/SOURCES.txt
--rw-r--r--   0 gonzalovidal   (501) staff       (20)        1 2022-03-19 02:06:49.000000 loica-1.0.5/loica.egg-info/dependency_links.txt
--rw-r--r--   0 gonzalovidal   (501) staff       (20)       44 2022-03-19 02:06:49.000000 loica-1.0.5/loica.egg-info/requires.txt
--rw-r--r--   0 gonzalovidal   (501) staff       (20)        6 2022-03-19 02:06:49.000000 loica-1.0.5/loica.egg-info/top_level.txt
--rw-r--r--   0 gonzalovidal   (501) staff       (20)       38 2022-03-19 02:06:49.889873 loica-1.0.5/setup.cfg
--rw-r--r--   0 gonzalovidal   (501) staff       (20)      940 2022-03-19 01:57:26.000000 loica-1.0.5/setup.py
+drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2023-07-25 14:17:21.677709 loica-1.0.6/
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     1073 2023-06-30 13:24:37.000000 loica-1.0.6/LICENSE
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     4452 2023-07-25 14:17:21.677299 loica-1.0.6/PKG-INFO
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     2504 2023-06-30 13:24:37.000000 loica-1.0.6/README.md
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     1033 2023-07-25 14:17:06.000000 loica-1.0.6/pyproject.toml
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)       38 2023-07-25 14:17:21.677928 loica-1.0.6/setup.cfg
+drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2023-07-25 14:17:21.656613 loica-1.0.6/src/
+drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2023-07-25 14:17:21.664361 loica-1.0.6/src/loica/
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)      220 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/__init__.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     6513 2023-07-25 12:13:54.000000 loica-1.0.6/src/loica/assay.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     2846 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/colony.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     2491 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/geneproduct.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)    20044 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/genetic_network.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     3763 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/metabolism.py
+drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2023-07-25 14:17:21.676174 loica-1.0.6/src/loica/operators/
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)      131 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/operators/__init__.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     6752 2023-07-25 12:13:54.000000 loica-1.0.6/src/loica/operators/hill1.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     9430 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/operators/hill2.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)      869 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/operators/operator.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     5538 2023-07-25 12:13:54.000000 loica-1.0.6/src/loica/operators/receiver.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     4409 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/operators/source.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)      799 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/operators/sum.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     2573 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/sample.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     1080 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/supplement.py
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     3402 2023-06-30 13:24:37.000000 loica-1.0.6/src/loica/util.py
+drwxr-xr-x   0 gonzalovidal   (501) staff       (20)        0 2023-07-25 14:17:21.669399 loica-1.0.6/src/loica.egg-info/
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)     4452 2023-07-25 14:17:21.000000 loica-1.0.6/src/loica.egg-info/PKG-INFO
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)      608 2023-07-25 14:17:21.000000 loica-1.0.6/src/loica.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)        1 2023-07-25 14:17:21.000000 loica-1.0.6/src/loica.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)       81 2023-07-25 14:17:21.000000 loica-1.0.6/src/loica.egg-info/requires.txt
+-rw-r--r--   0 gonzalovidal   (501) staff       (20)        6 2023-07-25 14:17:21.000000 loica-1.0.6/src/loica.egg-info/top_level.txt
```

### Comparing `loica-1.0.5/LICENSE` & `loica-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/assay.py` & `loica-1.0.6/src/loica/assay.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     if stochastic:
                         time = t * self.interval
                         sample.step(time, self.interval, stochastic=True)
                     else:
                         for tt in range(substeps):
                             time = t * self.interval + tt * dt
                             sample.step(time, dt)
-                pbar.update(1 / n_samples * 100)
+                    pbar.update(1 / self.n_measurements / n_samples * 100)
             pbar.close()
                 
     def upload(self, flapjack, study):
         assay = flapjack.create('assay', 
                                     name=self.name, 
                                     study=study, 
                                     temperature=0,
```

### Comparing `loica-1.0.5/loica/colony.py` & `loica-1.0.6/src/loica/colony.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/geneproduct.py` & `loica-1.0.6/src/loica/geneproduct.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/genetic_network.py` & `loica-1.0.6/src/loica/genetic_network.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/metabolism.py` & `loica-1.0.6/src/loica/metabolism.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/operators/hill1.py` & `loica-1.0.6/src/loica/operators/hill1.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/operators/hill2.py` & `loica-1.0.6/src/loica/operators/hill2.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/operators/operator.py` & `loica-1.0.6/src/loica/operators/operator.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/operators/receiver.py` & `loica-1.0.6/src/loica/operators/receiver.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/operators/source.py` & `loica-1.0.6/src/loica/operators/source.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/sample.py` & `loica-1.0.6/src/loica/sample.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,16 +40,20 @@
         if metabolism:
             self.biomass = self.metabolism.biomass
         self.supplements = {}
 
     def initialize(self):
         self.genetic_network.initialize()
 
-    def set_supplement(self, supplement, concentration):
-        self.supplements[supplement] = concentration
+    def set_supplement(self, supplement, concentration, profile=None):
+        if not profile:
+            def prof(t):
+                return 1
+            profile = prof
+        self.supplements[supplement] = (concentration, profile)
 
     def set_regulator(self, name, concentration):
         for reg in self.genetic_network.regulators:
             if reg.name == name:
                 reg.init_concentration = concentration
             else: pass
 
@@ -58,16 +62,16 @@
             if rep.name == name:
                 rep.init_concentration = concentration
             else: pass
 
     def step(self, t, dt, stochastic=False):
         if self.genetic_network and self.metabolism:
             growth_rate = self.metabolism.growth_rate(t)
-            for supp,conc in self.supplements.items():
-                supp.concentration = conc
+            for supp,(conc,prof) in self.supplements.items():
+                supp.concentration = conc * prof(t)
             if stochastic:
                 self.genetic_network.step_stochastic(growth_rate, t, dt)
             else:
                 self.genetic_network.step(growth_rate, t, dt)
             self.reporters = self.genetic_network.reporters
```

### Comparing `loica-1.0.5/loica/supplement.py` & `loica-1.0.6/src/loica/supplement.py`

 * *Files identical despite different names*

### Comparing `loica-1.0.5/loica/util.py` & `loica-1.0.6/src/loica/util.py`

 * *Files identical despite different names*

