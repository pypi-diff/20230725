# Comparing `tmp/french_cities-0.1.0a8.tar.gz` & `tmp/french_cities-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a8.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a9.tar", max compression
```

## Comparing `french_cities-0.1.0a8.tar` & `french_cities-0.1.0a9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      349 2023-07-25 08:14:59.647042 french_cities-0.1.0a8/french_cities/__init__.py
--rw-r--r--   0        0        0    19460 2023-07-25 08:05:14.837214 french_cities-0.1.0a8/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a8/french_cities/departement_finder.py
--rw-r--r--   0        0        0      535 2023-07-25 08:14:16.766868 french_cities-0.1.0a8/french_cities/utils.py
--rw-r--r--   0        0        0     7844 2023-07-23 11:38:50.970042 french_cities-0.1.0a8/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-25 08:14:55.193579 french_cities-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a8/README.fr.md
--rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a8/README.md
--rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      349 2023-07-25 14:34:53.551368 french_cities-0.1.0a9/french_cities/__init__.py
+-rw-r--r--   0        0        0    19611 2023-07-25 12:18:31.033911 french_cities-0.1.0a9/french_cities/city_finder.py
+-rw-r--r--   0        0        0     7464 2023-07-25 14:33:59.441164 french_cities-0.1.0a9/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      535 2023-07-25 08:14:16.766868 french_cities-0.1.0a9/french_cities/utils.py
+-rw-r--r--   0        0        0     7844 2023-07-23 11:38:50.970042 french_cities-0.1.0a9/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-25 14:35:07.329769 french_cities-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     9426 2023-07-25 14:15:49.284414 french_cities-0.1.0a9/README.fr.md
+-rw-r--r--   0        0        0     7918 2023-07-25 14:15:36.692406 french_cities-0.1.0a9/README.md
+-rw-r--r--   0        0        0    18350 1970-01-01 00:00:00.000000 french_cities-0.1.0a9/PKG-INFO
```

### Comparing `french_cities-0.1.0a8/french_cities/city_finder.py` & `french_cities-0.1.0a9/french_cities/city_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,20 +445,24 @@
                 total=len(args), desc="Queuing download", leave=False
             ) as pbar:
                 with ThreadPool(10) as pool:
                     future = pool.map(get, args)
                     results_iterator = future.result()
                     while True:
                         try:
-                            results.append(next(results_iterator))
+                            this_result = next(results_iterator)
+                            if this_result:
+                                results.append(this_result)
                         except StopIteration:
                             break
                         finally:
                             pbar.update(1)
 
+            logger.info("résultat obtenu")
+
             results_api = (
                 gpd.GeoDataFrame.from_features(np.array(results).flatten())
                 .loc[:, ["full", "score", "city", "citycode"]]
                 .rename(
                     {
                         "score": "result_score",
                         "city": "result_city",
```

### Comparing `french_cities-0.1.0a8/french_cities/utils.py` & `french_cities-0.1.0a9/french_cities/utils.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a8/french_cities/vintage.py` & `french_cities-0.1.0a9/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a8/pyproject.toml` & `french_cities-0.1.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a8"
+version = "0.1.0a9"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.0a8/README.fr.md` & `french_cities-0.1.0a9/README.fr.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,21 @@
 de gros volumes de données que ne le feraient des appels multiples à des API.
 
 ### Trouver les départements
 `french-cities` peut retrouver un code département à partir de codes postaux ou 
 de codes communes officiels (COG/INSEE).
 
 Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
-Adresse Nationale) et devrait fournir des résultats corrects.
+Adresse Nationale) et devrait fournir des résultats corrects. Le cas des codes
+Cedex n'étant que partiellement géré par la BAN, un appel est fait dans un
+second temps à l'[API d'OpenDataSoft](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr)
+construite sur la base des [travaux de Christian Quest](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+Cette utilisation s'appuie sur un accès freemium non authentifié; l'utilisateur 
+du package est invité à contrôler les conditions générales d'utilisation de l'API auprès du
+fournisseur.
 
 Travailler à partir de codes communes officiels peut entraîner des résultats
 erronés pour des données anciennes, dans le cas de communes ayant changé de
 département (ce qui est relativement rare).
 Ce choix est délibéré : seuls les premiers caractères des codes commune sont
 utilisés pour la reconnaissance du département (algorithme rapide et qui donne
 des résultats corrects pour 99% des cas), par opposition à un requêtage
```

### Comparing `french_cities-0.1.0a8/README.md` & `french_cities-0.1.0a9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,20 @@
 calls and will optimize the call to each endpoints.
 
 ### Retrieve departements' codes
 `french-cities` can retrieve departement's codes from postal codes or official
 (COG/INSEE) codes. 
 
 Working from postal codes will make use of the BAN (Base Adresse Nationale)
-and should return correct results.
+and should return correct results. The case of "Cedex" codes is only partially
+covered by the BAN, so [OpenDataSoft's API](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr),
+constructed upon [Christian Quest works](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+This consumes the freemium API and no authentication is included:
+the user of the present package should check the current API's legal terms
+directly on OpenDataSoft's website.
 
 Working from official codes may give wrong results when working on an old
 dataset and with cities which have changed of departments (which is rarely seen). 
 This is deliberate: it will use the first characters of the cities' codes 
 (which is a fast process and 99% accurate) instead of using an API (which is
 lengthy though foolproof).
```

### Comparing `french_cities-0.1.0a8/PKG-INFO` & `french_cities-0.1.0a9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
@@ -84,15 +84,20 @@
 calls and will optimize the call to each endpoints.
 
 ### Retrieve departements' codes
 `french-cities` can retrieve departement's codes from postal codes or official
 (COG/INSEE) codes. 
 
 Working from postal codes will make use of the BAN (Base Adresse Nationale)
-and should return correct results.
+and should return correct results. The case of "Cedex" codes is only partially
+covered by the BAN, so [OpenDataSoft's API](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr),
+constructed upon [Christian Quest works](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+This consumes the freemium API and no authentication is included:
+the user of the present package should check the current API's legal terms
+directly on OpenDataSoft's website.
 
 Working from official codes may give wrong results when working on an old
 dataset and with cities which have changed of departments (which is rarely seen). 
 This is deliberate: it will use the first characters of the cities' codes 
 (which is a fast process and 99% accurate) instead of using an API (which is
 lengthy though foolproof).
 
@@ -305,15 +310,21 @@
 de gros volumes de données que ne le feraient des appels multiples à des API.
 
 ### Trouver les départements
 `french-cities` peut retrouver un code département à partir de codes postaux ou 
 de codes communes officiels (COG/INSEE).
 
 Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
-Adresse Nationale) et devrait fournir des résultats corrects.
+Adresse Nationale) et devrait fournir des résultats corrects. Le cas des codes
+Cedex n'étant que partiellement géré par la BAN, un appel est fait dans un
+second temps à l'[API d'OpenDataSoft](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/api/?flg=fr&q=code%3D68013&lang=fr)
+construite sur la base des [travaux de Christian Quest](https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr).
+Cette utilisation s'appuie sur un accès freemium non authentifié; l'utilisateur 
+du package est invité à contrôler les conditions générales d'utilisation de l'API auprès du
+fournisseur.
 
 Travailler à partir de codes communes officiels peut entraîner des résultats
 erronés pour des données anciennes, dans le cas de communes ayant changé de
 département (ce qui est relativement rare).
 Ce choix est délibéré : seuls les premiers caractères des codes commune sont
 utilisés pour la reconnaissance du département (algorithme rapide et qui donne
 des résultats corrects pour 99% des cas), par opposition à un requêtage
```

