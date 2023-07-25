# Comparing `tmp/twitternewsbot-2.0.1.tar.gz` & `tmp/twitternewsbot-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitternewsbot-2.0.1.tar", last modified: Tue Jul 25 16:42:43 2023, max compression
+gzip compressed data, was "twitternewsbot-2.0.2.tar", last modified: Tue Jul 25 16:44:21 2023, max compression
```

## Comparing `twitternewsbot-2.0.1.tar` & `twitternewsbot-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:42:43.555605 twitternewsbot-2.0.1/
--rw-r--r--   0 arnavmarda   (501) staff       (20)     1068 2023-07-21 18:00:57.000000 twitternewsbot-2.0.1/LICENSE
--rw-r--r--   0 arnavmarda   (501) staff       (20)     3213 2023-07-25 16:42:43.555697 twitternewsbot-2.0.1/PKG-INFO
--rw-r--r--   0 arnavmarda   (501) staff       (20)     2461 2023-07-25 16:39:38.000000 twitternewsbot-2.0.1/README.md
--rw-r--r--   0 arnavmarda   (501) staff       (20)      131 2023-07-25 16:42:43.555916 twitternewsbot-2.0.1/setup.cfg
--rw-r--r--   0 arnavmarda   (501) staff       (20)     2049 2023-07-25 16:42:41.000000 twitternewsbot-2.0.1/setup.py
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:42:43.554633 twitternewsbot-2.0.1/twitternewsbot/
--rw-r--r--   0 arnavmarda   (501) staff       (20)      148 2023-07-25 16:38:08.000000 twitternewsbot-2.0.1/twitternewsbot/__init__.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)    13947 2023-07-23 21:03:02.000000 twitternewsbot-2.0.1/twitternewsbot/newsfinder.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)    14626 2023-07-23 21:06:50.000000 twitternewsbot-2.0.1/twitternewsbot/tweeter.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)     8096 2023-07-24 16:43:03.000000 twitternewsbot-2.0.1/twitternewsbot/twitternewsbot.py
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:42:43.555418 twitternewsbot-2.0.1/twitternewsbot.egg-info/
--rw-r--r--   0 arnavmarda   (501) staff       (20)     3213 2023-07-25 16:42:43.000000 twitternewsbot-2.0.1/twitternewsbot.egg-info/PKG-INFO
--rw-r--r--   0 arnavmarda   (501) staff       (20)      340 2023-07-25 16:42:43.000000 twitternewsbot-2.0.1/twitternewsbot.egg-info/SOURCES.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)        1 2023-07-25 16:42:43.000000 twitternewsbot-2.0.1/twitternewsbot.egg-info/dependency_links.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)      143 2023-07-25 16:42:43.000000 twitternewsbot-2.0.1/twitternewsbot.egg-info/requires.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)       15 2023-07-25 16:42:43.000000 twitternewsbot-2.0.1/twitternewsbot.egg-info/top_level.txt
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.289461 twitternewsbot-2.0.2/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     1068 2023-07-21 18:00:57.000000 twitternewsbot-2.0.2/LICENSE
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     3211 2023-07-25 16:44:21.289535 twitternewsbot-2.0.2/PKG-INFO
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     2459 2023-07-25 16:44:07.000000 twitternewsbot-2.0.2/README.md
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      131 2023-07-25 16:44:21.289721 twitternewsbot-2.0.2/setup.cfg
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     2049 2023-07-25 16:44:17.000000 twitternewsbot-2.0.2/setup.py
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.288487 twitternewsbot-2.0.2/twitternewsbot/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      148 2023-07-25 16:38:08.000000 twitternewsbot-2.0.2/twitternewsbot/__init__.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)    13947 2023-07-23 21:03:02.000000 twitternewsbot-2.0.2/twitternewsbot/newsfinder.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)    14626 2023-07-23 21:06:50.000000 twitternewsbot-2.0.2/twitternewsbot/tweeter.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     8096 2023-07-24 16:43:03.000000 twitternewsbot-2.0.2/twitternewsbot/twitternewsbot.py
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.289341 twitternewsbot-2.0.2/twitternewsbot.egg-info/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     3211 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/PKG-INFO
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      340 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)        1 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      143 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/requires.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)       15 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/top_level.txt
```

### Comparing `twitternewsbot-2.0.1/LICENSE` & `twitternewsbot-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitternewsbot-2.0.1/PKG-INFO` & `twitternewsbot-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitternewsbot
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python API allowing you to automize a personalized news delivery system.
 Home-page: https://github.com/arnavmarda/twitter-news-bot/
 Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz
 Author: Arnav Marda
 Author-email: arnavmarda@gmail.com
 License: MIT
 Keywords: AI,Twitter,News,Automation
@@ -33,15 +33,15 @@
 5. Pipeline and automate the scraping and tweeting procedure using a `cron` job.
 
 # Quick Start
 For complete documentation and examples, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 ## Installation
 ```bash
-pip install twitter-news-bot
+pip install twitternewsbot
 ```
 
 ## Requirements - before using the API
 For more information on how to generate the following keys and tokens, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 1. To use the `tweepy` API to post tweets, you must have a Twitter developer account and create an app. You can create an app [here](https://developer.twitter.com/en/apps). Don't worry, Twitter gives you 1 free app. Once you have created an app, you will need to generate the following keys and tokens:
     - Consumer API key
```

### Comparing `twitternewsbot-2.0.1/README.md` & `twitternewsbot-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 5. Pipeline and automate the scraping and tweeting procedure using a `cron` job.
 
 # Quick Start
 For complete documentation and examples, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 ## Installation
 ```bash
-pip install twitter-news-bot
+pip install twitternewsbot
 ```
 
 ## Requirements - before using the API
 For more information on how to generate the following keys and tokens, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 1. To use the `tweepy` API to post tweets, you must have a Twitter developer account and create an app. You can create an app [here](https://developer.twitter.com/en/apps). Don't worry, Twitter gives you 1 free app. Once you have created an app, you will need to generate the following keys and tokens:
     - Consumer API key
```

### Comparing `twitternewsbot-2.0.1/setup.py` & `twitternewsbot-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'twitternewsbot',         # How you named your package folder (MyLib)
   packages = ['twitternewsbot'],   # Chose the same as "name"
-  version = '2.0.1',      # Start with a small number and increase it with every change you make
+  version = '2.0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python API allowing you to automize a personalized news delivery system.',   # Give a short description about your library
   author = 'Arnav Marda',                   # Type in your name
   author_email = 'arnavmarda@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/arnavmarda/twitter-news-bot/',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz',    # I explain this later on
   keywords = ['AI', 'Twitter', 'News', 'Automation'],   # Keywords that define your package best
```

### Comparing `twitternewsbot-2.0.1/twitternewsbot/newsfinder.py` & `twitternewsbot-2.0.2/twitternewsbot/newsfinder.py`

 * *Files identical despite different names*

### Comparing `twitternewsbot-2.0.1/twitternewsbot/tweeter.py` & `twitternewsbot-2.0.2/twitternewsbot/tweeter.py`

 * *Files identical despite different names*

### Comparing `twitternewsbot-2.0.1/twitternewsbot/twitternewsbot.py` & `twitternewsbot-2.0.2/twitternewsbot/twitternewsbot.py`

 * *Files identical despite different names*

### Comparing `twitternewsbot-2.0.1/twitternewsbot.egg-info/PKG-INFO` & `twitternewsbot-2.0.2/twitternewsbot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitternewsbot
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python API allowing you to automize a personalized news delivery system.
 Home-page: https://github.com/arnavmarda/twitter-news-bot/
 Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz
 Author: Arnav Marda
 Author-email: arnavmarda@gmail.com
 License: MIT
 Keywords: AI,Twitter,News,Automation
@@ -33,15 +33,15 @@
 5. Pipeline and automate the scraping and tweeting procedure using a `cron` job.
 
 # Quick Start
 For complete documentation and examples, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 ## Installation
 ```bash
-pip install twitter-news-bot
+pip install twitternewsbot
 ```
 
 ## Requirements - before using the API
 For more information on how to generate the following keys and tokens, please refer to the [documentation](https://arnavmarda.github.io/twitter-news-bot/).
 
 1. To use the `tweepy` API to post tweets, you must have a Twitter developer account and create an app. You can create an app [here](https://developer.twitter.com/en/apps). Don't worry, Twitter gives you 1 free app. Once you have created an app, you will need to generate the following keys and tokens:
     - Consumer API key
```

