# Comparing `tmp/hearthstone-7.2.2.tar.gz` & `tmp/hearthstone-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.2.2.tar", last modified: Fri Jul 14 10:43:39 2023, max compression
+gzip compressed data, was "hearthstone-7.3.0.tar", last modified: Tue Jul 25 19:24:43 2023, max compression
```

## Comparing `hearthstone-7.2.2.tar` & `hearthstone-7.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.641086 hearthstone-7.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-14 10:43:34.000000 hearthstone-7.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 10:43:39.641086 hearthstone-7.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 10:43:34.000000 hearthstone-7.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.637086 hearthstone-7.2.2/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    61035 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.641086 hearthstone-7.2.2/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.637086 hearthstone-7.2.2/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 10:43:39.641086 hearthstone-7.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-07-14 10:43:34.000000 hearthstone-7.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 19:24:32.000000 hearthstone-7.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 19:24:43.428986 hearthstone-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:24:32.000000 hearthstone-7.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61409 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 19:24:32.000000 hearthstone-7.3.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:24:43.428986 hearthstone-7.3.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:24:43.000000 hearthstone-7.3.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 19:24:43.428986 hearthstone-7.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-07-25 19:24:32.000000 hearthstone-7.3.0/setup.py
```

### Comparing `hearthstone-7.2.2/LICENSE` & `hearthstone-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/PKG-INFO` & `hearthstone-7.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.2.2
+Version: 7.3.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.2.2/README.md` & `hearthstone-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/bountyxml.py` & `hearthstone-7.3.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/cardxml.py` & `hearthstone-7.3.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/dbf.py` & `hearthstone-7.3.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/deckstrings.py` & `hearthstone-7.3.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/entities.py` & `hearthstone-7.3.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/enums.py` & `hearthstone-7.3.0/hearthstone/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,14 @@
 	DEATHRATTLE_RETURN_ZONE = 382
 	STEADY_SHOT_CAN_TARGET = 383
 	DISPLAYED_CREATOR = 385
 	POWERED_UP = 386
 	SPARE_PART = 388
 	FORGETFUL = 389
 	CAN_SUMMON_MAXPLUSONE_MINION = 390
-	OBFUSCATED = 391
 	BURNING = 392
 	OVERLOAD_LOCKED = 393
 	NUM_TIMES_HERO_POWER_USED_THIS_GAME = 394
 	CURRENT_HEROPOWER_DAMAGE_BONUS = 395
 	HEROPOWER_DAMAGE = 396
 	NUM_FRIENDLY_MINIONS_THAT_DIED_THIS_TURN = 398
 	NUM_CARDS_DRAWN_THIS_TURN = 399
@@ -530,15 +529,15 @@
 	TRANSFORMED_FROM_CARD_VISUAL_TYPE = 1719
 	TRADEABLE = 1720
 	TOOL = 1722
 	QUESTLINE = 1725
 	LETTUCE_MERCENARY_RESERVE = 1731
 	LETTUCE_SKIP_MERCENARY_RESERVE = 1732
 	PLAYER_ID_LOOKUP = 1740
-	TRADE_COST = 1743
+	DECK_ACTION_COST = 1743
 	BACON_AVALANCHE = 1744
 	SIGIL = 1749
 	LETTUCE_DISABLE_AUTO_SELECT_NEXT_MERC = 1753
 	PLAYED_CTHUN_EYE = 1764
 	PLAYED_CTHUN_BODY = 1765
 	PLAYED_CTHUN_MAW = 1766
 	PLAYED_CTHUN_HEART = 1767
@@ -760,33 +759,36 @@
 	DEATH_SPELL_OVERRIDE = 2722
 	BACON_IS_BOB_QUEST = 2732
 	BACON_HERO_REWARD_CARD_DBID = 2748
 	BACON_HERO_HEROPOWER_REWARD_CARD_DBID = 2749
 	BACON_HERO_REWARD_MINION_TYPE = 2750
 	BACON_HERO_HEROPOWER_REWARD_MINION_TYPE = 2751
 	MERCENARIES_DISCOVER_SOURCE = 2752
+	TITAN = 2772
 	HERO_ATTACK_GIVEN_ADDITIONAL = 2776
 	HERO_ARMOR_GIVEN_ADDITIONAL = 2778
 	LETTUCE_CHARGE = 2779
 	BACON_DIED_LAST_COMBAT_HINT = 2780
 	SHIFTING_LOCATION = 2783
+	FORGE = 2785
 	UNPLAYABLE_VISUALS = 2798
 	CARDTEXT_ENTITY_AS_NUMBERS = 2802
 	BACON_DOUBLE_QUEST_HERO_POWER = 2803
 	MERCENARIES_TREASURE_SCALE_LEVEL = 2810
 	CARD_COSTS_ARMOR = 2811
 	FINALE = 2820
 	OVERHEAL = 2821
 	BACON_BLOODGEMBUFFHEALTHVALUE = 2827
 	EMOTECHARACTER = 2839
 	HAS_ACTIVATE_POWER = 2840
 	EMOTECLASS = 2851
 	VENOMOUS = 2853
 	MAGNETIC_TO_RACE = 2859
 	BACON_MAX_LEADERBOARD_ARMOR = 2867
+	IS_USING_FORGE_OPTION = 2869
 	BACON_REBORN_TOOLTIP = 2870
 	BACON_PUTRICIDESCREATION_TOOLTIP = 2875
 	TAG_SCRIPT_DATA_NUM_3 = 2889
 	CARD_NAME_DATA_1 = 2890
 	BACON_COSTS_HEALTH_TO_BUY = 2911
 	TAG_SCRIPT_DATA_NUM_4 = 2919
 	TAG_SCRIPT_DATA_NUM_5 = 2920
@@ -795,19 +797,27 @@
 	MAX_SIDEBOARD_CARDS = 2931
 	BONUSEFFECTS = 2934
 	BACON_USE_COIN_BASED_BUDDY_METER = 2935
 	BACON_BUY_BUDDY = 2937
 	BACON_BUY_BUDDY_2 = 2938
 	BACON_SHOW_HEROPOWER_BUDDY_AS_EVOLVING_BIG_CARD = 2943
 	HIDDEN_CHOICE_OVERRIDE = 2946
+	FORGED = 3011
 	BUILDING_UP = 3016
 	BACON_PAIR_CANDIDATE = 3031
 	BACON_TRIGGER_UPBEAT = 3046
 	BACON_TRIGGER_XY = 3047
 	FAN_LINK = 3052
+	FORGE_REVEALED = 3070
+	FORGES_INTO = 3074
+	SUMMONED_WHEN_DRAWN = 3128
+	IS_ALTERNATE_HEROPOWER = 3130
+	TITAN_ABILITY_USED_1 = 3140
+	TITAN_ABILITY_USED_2 = 3141
+	TITAN_ABILITY_USED_3 = 3142
 
 	InvisibleDeathrattle = 335
 	ImmuneToSpellpower = 349
 	AttackVisualType = 251
 	DevState = 268
 	GrantCharge = 355
 	HealTarget = 361
@@ -845,14 +855,15 @@
 	RECALL_OWED = OVERLOAD_OWED
 	RED_MANA_CRYSTALS = RED_MANA_GEM
 	TAG_HERO_POWER_DOUBLE = HERO_POWER_DOUBLE
 	TAG_AI_MUST_PLAY = AI_MUST_PLAY
 	# TREASURE = DISCOVER  # Added back
 	SHOWN_HERO_POWER = HERO_POWER
 	EVILZUG = MARK_OF_EVIL
+	TRADE_COST = DECK_ACTION_COST
 
 	# Deleted
 	IGNORE_DAMAGE = 1
 	GOLD_REWARD_STATE = 13
 	COPY_DEATHRATTLE = 55
 	COPY_DEATHRATTLE_INDEX = 56
 	CARD_ID = 186
@@ -879,14 +890,15 @@
 	OUTGOING_COMBAT_DAMAGE_MULTIPLIER = 287
 	OUTGOING_COMBAT_DAMAGE_CAP = 288
 	INCOMING_COMBAT_DAMAGE_MULTIPLIER = 289
 	INCOMING_COMBAT_DAMAGE_CAP = 290
 	DIVINE_SHIELD_READY = 314
 	IGNORE_DAMAGE_OFF = 354
 	NUM_OPTIONS = 359
+	OBFUSCATED = 391
 	LAST_CARD_PLAYED = 397
 	PENDING_EVOLUTIONS = 461
 	WEATHER = 1002
 	WEATHERSNOWSTORM = 1012
 	WEATHERTHUNDERSTORM = 1013
 	WEATHERFIRESTORM = 1014
 	EXTRA_SPELL_CASTS_BASE = 1140
@@ -1331,15 +1343,17 @@
 	REQ_CARD_TAVERN_TIER_LEVEL_TO_PLAY = 129
 	REQ_NOT_EXHAUSTED_LOCATION = 130
 	REQ_LOCATION_TARGET = 131
 	REQ_TARGET_SILVER_HAND_RECRUIT = 132
 	REQ_MINIMUM_CORPSES = 133
 	REQ_LOCATION_OR_MINION_TARGET = 134
 	REQ_CAN_BE_TARGETED_BY_LOCATIONS = 135
-	REQ_HAS_PLAYED_SPELL_THIS_GAME = 136
+	REQ_FORGE = 136
+	REQ_HAS_PLAYED_SPELL_THIS_GAME = 137
+	REQ_TARGET_IS_NON_TITAN = 141
 	REQ_DRAG_TO_PLAY = 999
 
 	# Renamed
 	REQ_ENCHANTED_TARGET = REQ_MAX_SECRETS
 	REQ_ENTIRE_ENTOURAGE_NOT_IN_PLAY = REQ_ALL_BASIC_TOTEMS_NOT_IN_PLAY
 	REQ_UNIQUE_SECRET = REQ_UNIQUE_SECRET_OR_QUEST
 	REQ_SECRET_CAP = REQ_SECRET_ZONE_CAP
@@ -1997,22 +2011,23 @@
 	DEATHS = 6
 	PLAY = 7
 	FATIGUE = 8
 	RITUAL = 9
 	REVEAL_CARD = 10
 	GAME_RESET = 11
 	MOVE_MINION = 12
-	TRADE = 13
+	DECK_ACTION = 13
 
 	# Removed
 	SCRIPT = 4
 	ACTION = 99
 
 	# Renamed
 	CONTINUOUS = 2
+	TRADE = DECK_ACTION
 
 
 class State(IntEnum):
 	"""TAG_STATE"""
 
 	INVALID = 0
 	LOADING = 1
```

### Comparing `hearthstone-7.2.2/hearthstone/mercenaryxml.py` & `hearthstone-7.3.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/stringsfile.py` & `hearthstone-7.3.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/utils/__init__.py` & `hearthstone-7.3.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone/xmlutils.py` & `hearthstone-7.3.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/hearthstone.egg-info/PKG-INFO` & `hearthstone-7.3.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.2.2
+Version: 7.3.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.2.2/hearthstone.egg-info/SOURCES.txt` & `hearthstone-7.3.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.2/setup.cfg` & `hearthstone-7.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.2.2
+version = 7.3.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

