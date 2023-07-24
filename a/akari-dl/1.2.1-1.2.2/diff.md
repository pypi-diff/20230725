# Comparing `tmp/akari-dl-1.2.1.tar.gz` & `tmp/akari-dl-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-dl-1.2.1.tar", last modified: Mon Jul 24 23:39:47 2023, max compression
+gzip compressed data, was "akari-dl-1.2.2.tar", last modified: Mon Jul 24 23:43:33 2023, max compression
```

## Comparing `akari-dl-1.2.1.tar` & `akari-dl-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.852800 akari-dl-1.2.1/
--rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      589 2023-07-24 23:39:47.851804 akari-dl-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.782778 akari-dl-1.2.1/akari_dl/
--rw-rw-rw-   0        0        0     2792 2023-07-24 23:39:30.000000 akari-dl-1.2.1/akari_dl/__init__.py
--rw-rw-rw-   0        0        0     1829 2023-07-24 23:32:08.000000 akari-dl-1.2.1/akari_dl/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.850801 akari-dl-1.2.1/akari_dl/src/
--rw-rw-rw-   0        0        0     2983 2023-07-24 23:38:21.000000 akari-dl-1.2.1/akari_dl/src/download_anime.py
--rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.1/akari_dl/src/log_response.py
--rw-rw-rw-   0        0        0     1106 2023-07-24 23:38:25.000000 akari-dl-1.2.1/akari_dl/src/resolve_anime.py
--rw-rw-rw-   0        0        0     1155 2023-07-24 23:33:26.000000 akari-dl-1.2.1/akari_dl/src/website.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.847799 akari-dl-1.2.1/akari_dl.egg-info/
--rw-rw-rw-   0        0        0      589 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 23:39:47.852800 akari-dl-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-07-24 23:39:39.000000 akari-dl-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.354812 akari-dl-1.2.2/
+-rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:43:33.353812 akari-dl-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.337814 akari-dl-1.2.2/akari_dl/
+-rw-rw-rw-   0        0        0     2792 2023-07-24 23:43:21.000000 akari-dl-1.2.2/akari_dl/__init__.py
+-rw-rw-rw-   0        0        0     1829 2023-07-24 23:32:08.000000 akari-dl-1.2.2/akari_dl/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.352812 akari-dl-1.2.2/akari_dl/src/
+-rw-rw-rw-   0        0        0        0 2023-07-24 23:42:55.000000 akari-dl-1.2.2/akari_dl/src/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-07-24 23:38:21.000000 akari-dl-1.2.2/akari_dl/src/download_anime.py
+-rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.2/akari_dl/src/log_response.py
+-rw-rw-rw-   0        0        0     1106 2023-07-24 23:38:25.000000 akari-dl-1.2.2/akari_dl/src/resolve_anime.py
+-rw-rw-rw-   0        0        0     1231 2023-07-24 23:38:29.000000 akari-dl-1.2.2/akari_dl/src/resolve_website.py
+-rw-rw-rw-   0        0        0     1155 2023-07-24 23:33:26.000000 akari-dl-1.2.2/akari_dl/src/website.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:43:33.347811 akari-dl-1.2.2/akari_dl.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 23:43:33.000000 akari-dl-1.2.2/akari_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 23:43:33.354812 akari-dl-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-24 23:43:27.000000 akari-dl-1.2.2/setup.py
```

### Comparing `akari-dl-1.2.1/LICENSE` & `akari-dl-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/PKG-INFO` & `akari-dl-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.1
+Version: 1.2.2
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.2.1/README.md` & `akari-dl-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/akari_dl/__init__.py` & `akari-dl-1.2.2/akari_dl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 
 arg_parser.add_argument("website", type=str, help="Specify the name of what website to direct-download anime from (see supported websites: https://github.com/keisanng/akari-dl#supported-websites.)", nargs="?")
 arg_parser.add_argument("anime", type=str, help="Specify what anime to download by title (in Romaji {https://en.wikipedia.org/wiki/Romanization_of_Japanese}.)")
 arg_parser.add_argument("output", type=str, help="Specify path to output downloaded video files to.", nargs="?")
 arg_parser.add_argument("-e", "--episodes", type=int, help="Specify the amount of episodes to download (downloads all if not specified) [NOT YET IMPLEMENTED.]")
 arg_parser.add_argument("-s", "--specials", action="store_true", help="Enable downloading of special episodes (only works with websites that list the specials on the same page as the episodes.)")
 arg_parser.add_argument("-d", "--debug", action="store_true", help="Run akari-dl in debug mode; log each connections html body and http headers and prints logging messages.")
-arg_parser.add_argument("-v", "--version", action="version", version="1.2.1", help="Print the current version of akari-dl.")
+arg_parser.add_argument("-v", "--version", action="version", version="1.2.2", help="Print the current version of akari-dl.")
 
 logger = logging
```

### Comparing `akari-dl-1.2.1/akari_dl/__main__.py` & `akari-dl-1.2.2/akari_dl/__main__.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/akari_dl/src/download_anime.py` & `akari-dl-1.2.2/akari_dl/src/download_anime.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/akari_dl/src/resolve_anime.py` & `akari-dl-1.2.2/akari_dl/src/resolve_anime.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/akari_dl/src/website.py` & `akari-dl-1.2.2/akari_dl/src/website.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.1/akari_dl.egg-info/PKG-INFO` & `akari-dl-1.2.2/akari_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.1
+Version: 1.2.2
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.2.1/setup.py` & `akari-dl-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
   name="akari-dl",
-  version="1.2.1",
+  version="1.2.2",
   author="keisan",
   author_email="<keisan@skiff.com>",
   description="A lightweight and open-source anime downloading CLI.",
   long_description="akari-dl downloads anime video files from direct download websites based on user configuration to avoid more annoying downloading methods like torrenting and manually downloading.",
   url="https://github.com/keisanng/akari-dl",
   project_urls={
     "Documentation": "https://github.com/keisanng/akari-dl#readme",
```

