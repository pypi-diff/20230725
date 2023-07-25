# Comparing `tmp/french_cities-0.1.0a7.tar.gz` & `tmp/french_cities-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a7.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a8.tar", max compression
```

## Comparing `french_cities-0.1.0a7.tar` & `french_cities-0.1.0a8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      349 2023-07-23 12:10:10.458604 french_cities-0.1.0a7/french_cities/__init__.py
--rw-r--r--   0        0        0    19360 2023-07-23 12:06:30.774859 french_cities-0.1.0a7/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a7/french_cities/departement_finder.py
--rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a7/french_cities/utils.py
--rw-r--r--   0        0        0     7844 2023-07-23 11:38:50.970042 french_cities-0.1.0a7/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-23 12:10:22.989876 french_cities-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a7/README.fr.md
--rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a7/README.md
--rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0      349 2023-07-25 08:14:59.647042 french_cities-0.1.0a8/french_cities/__init__.py
+-rw-r--r--   0        0        0    19460 2023-07-25 08:05:14.837214 french_cities-0.1.0a8/french_cities/city_finder.py
+-rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a8/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      535 2023-07-25 08:14:16.766868 french_cities-0.1.0a8/french_cities/utils.py
+-rw-r--r--   0        0        0     7844 2023-07-23 11:38:50.970042 french_cities-0.1.0a8/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-25 08:14:55.193579 french_cities-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a8/README.fr.md
+-rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a8/README.md
+-rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a8/PKG-INFO
```

### Comparing `french_cities-0.1.0a7/french_cities/city_finder.py` & `french_cities-0.1.0a8/french_cities/city_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,16 +517,20 @@
 
     candidats = [f"candidat_{k+1}" for k in range(len(to_test_ok))]
     addresses["best"] = combine(addresses, candidats)
     addresses = addresses.drop(candidats, axis=1)
     addresses = addresses.drop("full", axis=1)
     addresses = addresses.drop_duplicates()
 
-    df = df.merge(
-        addresses.replace("", np.nan), how="left", on=components_kept
+    df = (
+        df
+        .reset_index(drop=False)
+        .merge(
+            addresses.replace("", np.nan), how="left", on=components_kept
+        )
     )
     candidats = ["candidat_0", "best"]
     df[field_output] = combine(df, candidats)
     df = df.drop(
         [x for x in candidats if x in set(df.columns)],
         axis=1,
     )
@@ -540,9 +544,9 @@
         df = df.merge(missing, on=[dep, "city_cleaned"], how="left")
 
         candidats = [field_output, "candidat_missing"]
         df[field_output] = combine(df, candidats)
         df = df.drop("candidat_missing", axis=1)
 
     df = df.drop("city_cleaned", axis=1)
-
+    df = df.set_index("index")
     return df
```

### Comparing `french_cities-0.1.0a7/french_cities/departement_finder.py` & `french_cities-0.1.0a8/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a7/french_cities/vintage.py` & `french_cities-0.1.0a8/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a7/pyproject.toml` & `french_cities-0.1.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a7"
+version = "0.1.0a8"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.0a7/README.fr.md` & `french_cities-0.1.0a8/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a7/README.md` & `french_cities-0.1.0a8/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a7/PKG-INFO` & `french_cities-0.1.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
```

