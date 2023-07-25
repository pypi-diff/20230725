# Comparing `tmp/hearthstone-7.3.0.tar.gz` & `tmp/hearthstone-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.3.0.tar", last modified: Tue Jul 25 19:24:43 2023, max compression
+gzip compressed data, was "hearthstone-7.4.0.tar", last modified: Tue Jul 25 20:07:57 2023, max compression
```

## Comparing `hearthstone-7.3.0.tar` & `hearthstone-7.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 19:24:32.000000 hearthstone-7.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 19:24:43.428986 hearthstone-7.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:24:32.000000 hearthstone-7.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    61409 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 19:24:43.428986 hearthstone-7.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-07-25 19:24:32.000000 hearthstone-7.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:57.074354 hearthstone-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 20:07:51.000000 hearthstone-7.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 20:07:57.074354 hearthstone-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 20:07:51.000000 hearthstone-7.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:57.074354 hearthstone-7.4.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61409 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:57.074354 hearthstone-7.4.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 20:07:51.000000 hearthstone-7.4.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:57.074354 hearthstone-7.4.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:57.000000 hearthstone-7.4.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 20:07:57.074354 hearthstone-7.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-07-25 20:07:51.000000 hearthstone-7.4.0/setup.py
```

### Comparing `hearthstone-7.3.0/LICENSE` & `hearthstone-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/PKG-INFO` & `hearthstone-7.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.3.0
+Version: 7.4.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.3.0/README.md` & `hearthstone-7.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/bountyxml.py` & `hearthstone-7.4.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/cardxml.py` & `hearthstone-7.4.0/hearthstone/cardxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,15 @@
 	discover = prop(GameTag.DISCOVER, bool)
 	divine_shield = prop(GameTag.DIVINE_SHIELD, bool)
 	double_spelldamage_bonus = prop(GameTag.RECEIVES_DOUBLE_SPELLDAMAGE_BONUS, bool)
 	dredge = prop(GameTag.DREDGE, bool)
 	echo = prop(GameTag.ECHO, bool)
 	elite = prop(GameTag.ELITE, bool)
 	evil_glow = prop(GameTag.EVIL_GLOW, bool)
+	forge = prop(GameTag.FORGE, bool)
 	forgetful = prop(GameTag.FORGETFUL, bool)
 	ghostly = prop(GameTag.GHOSTLY, bool)
 	hide_health = prop(GameTag.HIDE_HEALTH, bool)
 	hide_stats = prop(GameTag.HIDE_STATS, bool)
 	hide_cost = prop(GameTag.HIDE_COST, bool)
 	immune = prop(GameTag.IMMUNE, bool)
 	inspire = prop(GameTag.INSPIRE, bool)
@@ -361,14 +362,15 @@
 	rush = prop(GameTag.RUSH, bool)
 	secret = prop(GameTag.SECRET, bool)
 	sidequest = prop(GameTag.SIDEQUEST, bool)
 	spare_part = prop(GameTag.SPARE_PART, bool)
 	spellburst = prop(GameTag.SPELLBURST, bool)
 	start_of_game = prop(GameTag.START_OF_GAME, bool)
 	taunt = prop(GameTag.TAUNT, bool)
+	titan = prop(GameTag.TITAN, bool)
 	topdeck = prop(GameTag.TOPDECK, bool)
 	tradeable = prop(GameTag.TRADEABLE, bool)
 	twinspell = prop(GameTag.TWINSPELL, bool)
 	untouchable = prop(GameTag.UNTOUCHABLE, bool)
 	venomous = prop(GameTag.VENOMOUS, bool)
 
 	##
```

### Comparing `hearthstone-7.3.0/hearthstone/dbf.py` & `hearthstone-7.4.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/deckstrings.py` & `hearthstone-7.4.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/entities.py` & `hearthstone-7.4.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/enums.py` & `hearthstone-7.4.0/hearthstone/enums.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/mercenaryxml.py` & `hearthstone-7.4.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/stringsfile.py` & `hearthstone-7.4.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/utils/__init__.py` & `hearthstone-7.4.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone/xmlutils.py` & `hearthstone-7.4.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-7.4.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.3.0
+Version: 7.4.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.3.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-7.4.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.3.0/setup.cfg` & `hearthstone-7.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.3.0
+version = 7.4.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

