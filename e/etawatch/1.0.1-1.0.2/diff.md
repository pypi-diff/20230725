# Comparing `tmp/etawatch-1.0.1.tar.gz` & `tmp/etawatch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etawatch-1.0.1.tar", last modified: Mon Jul 24 22:48:32 2023, max compression
+gzip compressed data, was "etawatch-1.0.2.tar", last modified: Tue Jul 25 00:24:44 2023, max compression
```

## Comparing `etawatch-1.0.1.tar` & `etawatch-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 22:48:32.006123 etawatch-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-23 16:38:43.000000 etawatch-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    42584 2023-07-24 22:48:32.005123 etawatch-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-07-23 16:59:01.000000 etawatch-1.0.1/README.md
--rw-rw-rw-   0        0        0      694 2023-07-24 22:47:39.000000 etawatch-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 22:48:32.007124 etawatch-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 22:48:31.989124 etawatch-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 22:48:31.997123 etawatch-1.0.1/src/etawatch/
--rw-rw-rw-   0        0        0      295 2023-07-24 22:47:30.000000 etawatch-1.0.1/src/etawatch/__init__.py
--rw-rw-rw-   0        0        0      907 2023-07-23 17:16:11.000000 etawatch-1.0.1/src/etawatch/etawatch.py
-drwxrwxrwx   0        0        0        0 2023-07-24 22:48:32.003124 etawatch-1.0.1/src/etawatch.egg-info/
--rw-rw-rw-   0        0        0    42584 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 22:48:31.000000 etawatch-1.0.1/src/etawatch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 00:24:44.404152 etawatch-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-23 16:38:43.000000 etawatch-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    42537 2023-07-25 00:24:44.402175 etawatch-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      729 2023-07-25 00:09:43.000000 etawatch-1.0.2/README.md
+-rw-rw-rw-   0        0        0      694 2023-07-25 00:24:25.000000 etawatch-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 00:24:44.404152 etawatch-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 00:24:44.385395 etawatch-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 00:24:44.394175 etawatch-1.0.2/src/etawatch/
+-rw-rw-rw-   0        0        0      295 2023-07-24 22:47:30.000000 etawatch-1.0.2/src/etawatch/__init__.py
+-rw-rw-rw-   0        0        0     1149 2023-07-25 00:22:26.000000 etawatch-1.0.2/src/etawatch/etawatch.py
+drwxrwxrwx   0        0        0        0 2023-07-25 00:24:44.401171 etawatch-1.0.2/src/etawatch.egg-info/
+-rw-rw-rw-   0        0        0    42537 2023-07-25 00:24:44.000000 etawatch-1.0.2/src/etawatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-25 00:24:44.000000 etawatch-1.0.2/src/etawatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 00:24:44.000000 etawatch-1.0.2/src/etawatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 00:24:44.000000 etawatch-1.0.2/src/etawatch.egg-info/top_level.txt
```

### Comparing `etawatch-1.0.1/LICENSE` & `etawatch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etawatch-1.0.1/PKG-INFO` & `etawatch-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etawatch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Like a stopwatch, but it also gives you an ETA
 Author-email: "Rick D. Gray" <rickdgray@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,34 +691,31 @@
 # Etawatch
 
 Like a stopwatch, but it also gives you an ETA.
 
 Example usage:
 
 ```python
-number_of_laps = 10
-
 # construction immediately starts timer
-eta = etawatch(number_of_laps)
-
+eta_watch = etawatch(5)
 for i in range(number_of_laps):
-    time.sleep(random.randint(1, 5))
-    eta, iteration_time = eta()
-    print(f'Time: {iteration_time:.2f} sec | Done in {eta:.2f} min')
+    # do some work
+    time.sleep(random.randint(1, 3))
+    eta, lap = eta_watch()
+    print(f'Lap: {i+1} | Time: {lap:.2f} sec | ETA: {eta:.2f} min')
 ```
 
 Another example:
 
 ```python
-number_of_laps = 10
-
-for i, eta, last_iter_time in enumerate(etawatch(number_of_laps)):
-    time.sleep(random.randint(1, 5))
-    print(f'Time: {iteration_time:.2f} sec | Done in {eta:.2f} min')
+for i, (eta, lap) in enumerate(etawatch(5)):
+    # do some work
+    time.sleep(random.randint(1, 3))
+    print(f'Lap: {i+1} | Time: {lap:.2f} sec | ETA: {eta:.2f} min')
 ```
 
 It can optionally predict ETA by only the last `n` number of runs.
 
 ```python
-# will run 10 laps but only return ETAs based on last 3
+# will only calculate ETAs based on last 3 lap times
 eta = etawatch(10, 3)
 ```
```

### Comparing `etawatch-1.0.1/pyproject.toml` & `etawatch-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "etawatch"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     {name = "Rick D. Gray", email = "rickdgray@outlook.com"},
 ]
 description = "Like a stopwatch, but it also gives you an ETA"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `etawatch-1.0.1/src/etawatch.egg-info/PKG-INFO` & `etawatch-1.0.2/src/etawatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etawatch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Like a stopwatch, but it also gives you an ETA
 Author-email: "Rick D. Gray" <rickdgray@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,34 +691,31 @@
 # Etawatch
 
 Like a stopwatch, but it also gives you an ETA.
 
 Example usage:
 
 ```python
-number_of_laps = 10
-
 # construction immediately starts timer
-eta = etawatch(number_of_laps)
-
+eta_watch = etawatch(5)
 for i in range(number_of_laps):
-    time.sleep(random.randint(1, 5))
-    eta, iteration_time = eta()
-    print(f'Time: {iteration_time:.2f} sec | Done in {eta:.2f} min')
+    # do some work
+    time.sleep(random.randint(1, 3))
+    eta, lap = eta_watch()
+    print(f'Lap: {i+1} | Time: {lap:.2f} sec | ETA: {eta:.2f} min')
 ```
 
 Another example:
 
 ```python
-number_of_laps = 10
-
-for i, eta, last_iter_time in enumerate(etawatch(number_of_laps)):
-    time.sleep(random.randint(1, 5))
-    print(f'Time: {iteration_time:.2f} sec | Done in {eta:.2f} min')
+for i, (eta, lap) in enumerate(etawatch(5)):
+    # do some work
+    time.sleep(random.randint(1, 3))
+    print(f'Lap: {i+1} | Time: {lap:.2f} sec | ETA: {eta:.2f} min')
 ```
 
 It can optionally predict ETA by only the last `n` number of runs.
 
 ```python
-# will run 10 laps but only return ETAs based on last 3
+# will only calculate ETAs based on last 3 lap times
 eta = etawatch(10, 3)
 ```
```

