# Comparing `tmp/animegifs-0.7.1.tar.gz` & `tmp/animegifs-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.7.1.tar", last modified: Tue Jul 18 17:27:53 2023, max compression
+gzip compressed data, was "animegifs-0.7.2.tar", last modified: Tue Jul 25 11:43:31 2023, max compression
```

## Comparing `animegifs-0.7.1.tar` & `animegifs-0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.175184 animegifs-0.7.1/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     4949 2023-07-18 17:27:53.174184 animegifs-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4132 2023-07-18 17:24:40.000000 animegifs-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.152657 animegifs-0.7.1/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.7.1/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-07-18 17:09:32.000000 animegifs-0.7.1/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.172186 animegifs-0.7.1/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.7.1/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-18 17:09:32.000000 animegifs-0.7.1/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1157 2023-06-14 16:22:51.000000 animegifs-0.7.1/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.162758 animegifs-0.7.1/animegifs.egg-info/
--rw-rw-rw-   0        0        0     4949 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:27:53.175184 animegifs-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1283 2023-07-18 17:25:55.000000 animegifs-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:43:31.464934 animegifs-0.7.2/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     4952 2023-07-25 11:43:31.463932 animegifs-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4135 2023-07-25 11:41:50.000000 animegifs-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:43:31.442464 animegifs-0.7.2/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.7.2/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-07-18 17:09:32.000000 animegifs-0.7.2/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:43:31.461933 animegifs-0.7.2/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.7.2/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-07-18 17:38:58.000000 animegifs-0.7.2/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1157 2023-06-14 16:22:51.000000 animegifs-0.7.2/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:43:31.452382 animegifs-0.7.2/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     4952 2023-07-25 11:43:31.000000 animegifs-0.7.2/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-25 11:43:31.000000 animegifs-0.7.2/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:43:31.000000 animegifs-0.7.2/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-25 11:43:31.000000 animegifs-0.7.2/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 11:43:31.000000 animegifs-0.7.2/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:43:31.465933 animegifs-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2023-07-25 11:39:31.000000 animegifs-0.7.2/setup.py
```

### Comparing `animegifs-0.7.1/LICENSE` & `animegifs-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.7.1/PKG-INFO` & `animegifs-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.7.1
+Version: 0.7.2
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -28,15 +28,15 @@
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MarcoSa-2000/animegifs?style=for-the-badge"></a>
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.7 will not have the gifs library updated anymore.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
@@ -65,15 +65,15 @@
 
 gifs = animegifs.Animegifs()
 
 user_input = input() #let user send any input and search if that input matches a category.
 #if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
 #   user_input = "bite"
 try:
-    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+    gif = gifs.get_gif(user_input) #return the url of the gif if the category exists.
 except animegifs.errors.CategoryError:
     print("not a valid gif category.")
 ```
 
 ## Category list:
 
 **A**
@@ -115,15 +115,15 @@
 **P**
 * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
 
 **R**
 * Run
 
 **S**
-* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+* Sad, Scared, Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
 
 **T**
 * Tease, Threat, Tickle, Tired
 
 **W**
 * Wave
```

#### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.7.1 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.2 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
-flawlessly or at all. Version below v0.6 will not have the gifs library updated
+flawlessly or at all. Version below v0.7 will not have the gifs library updated
 anymore. For troubleshoots, known errors and categories list, check below. `pip
 install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
 the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
 return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
 myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
 anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
 page. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() user_input = input() #let user send any input and search
 if that input matches a category. #if user_input == "nom": #nom as category
 doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
-except animegifs.errors.CategoryError: print("not a valid gif category.") ```
-## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
-**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
-Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
-Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
-Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
-**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
-Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
-Category List** * Random, Steal-magic # Live API You can test out the API (and
-lib functionality) on my bot's website here: https://enkidu-app.github.io/
-animegifs # Submit a GIF If you also want to contribute to the gifs collection,
-you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
-and other The first call (only!) in the session is expected to have a slower
-reaction time (5-15s) because of the authentication process. If you encounter
-an error, please raise an issue on the issue page: https://github.com/MarcoSa-
-2000/animegifs/issues. Alternatively, you can join my Discord server (https://
-discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
-feedback, or report any errors. I do also have a multi-function Discord bot.
-Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
-Copyright This repository doesn't include any copyrighted material. If you
-happen to come across any copyrighted content within this repository (but
-hosted elsewhere) that you own or represent, email me at
-**grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+gif = gifs.get_gif(user_input) #return the url of the gif if the category
+exists. except animegifs.errors.CategoryError: print("not a valid gif
+category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Submit a GIF If you also want to
+contribute to the gifs collection, you can submit a gif at: https://forms.gle/
+wxWmRuy5VCdDCZWp8 # Troubleshooting and other The first call (only!) in the
+session is expected to have a slower reaction time (5-15s) because of the
+authentication process. If you encounter an error, please raise an issue on the
+issue page: https://github.com/MarcoSa-2000/animegifs/issues. Alternatively,
+you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to
+request new categories, functions, provide feedback, or report any errors. I do
+also have a multi-function Discord bot. Feel free to check out the web
+dashboard here: https://enkidu-app.github.io. # Copyright This repository
+doesn't include any copyrighted material. If you happen to come across any
+copyrighted content within this repository (but hosted elsewhere) that you own
+or represent, email me at **grest0grest@gmail.com**. Please provide specific
+details about the copyrighted material and where it can be found. Once I
+confirm your claim, I'll take immediate action to remove the identified
+material.
```

### Comparing `animegifs-0.7.1/README.md` & `animegifs-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MarcoSa-2000/animegifs?style=for-the-badge"></a>
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.7 will not have the gifs library updated anymore.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
@@ -45,15 +45,15 @@
 
 gifs = animegifs.Animegifs()
 
 user_input = input() #let user send any input and search if that input matches a category.
 #if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
 #   user_input = "bite"
 try:
-    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+    gif = gifs.get_gif(user_input) #return the url of the gif if the category exists.
 except animegifs.errors.CategoryError:
     print("not a valid gif category.")
 ```
 
 ## Category list:
 
 **A**
@@ -95,15 +95,15 @@
 **P**
 * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
 
 **R**
 * Run
 
 **S**
-* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+* Sad, Scared, Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
 
 **T**
 * Tease, Threat, Tickle, Tired
 
 **W**
 * Wave
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
 # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
-flawlessly or at all. Version below v0.6 will not have the gifs library updated
+flawlessly or at all. Version below v0.7 will not have the gifs library updated
 anymore. For troubleshoots, known errors and categories list, check below. `pip
 install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
 the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
 return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
 myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
 anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
 page. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() user_input = input() #let user send any input and search
 if that input matches a category. #if user_input == "nom": #nom as category
 doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
-except animegifs.errors.CategoryError: print("not a valid gif category.") ```
-## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
-**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
-Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
-Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
-Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
-**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
-Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
-Category List** * Random, Steal-magic # Live API You can test out the API (and
-lib functionality) on my bot's website here: https://enkidu-app.github.io/
-animegifs # Submit a GIF If you also want to contribute to the gifs collection,
-you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
-and other The first call (only!) in the session is expected to have a slower
-reaction time (5-15s) because of the authentication process. If you encounter
-an error, please raise an issue on the issue page: https://github.com/MarcoSa-
-2000/animegifs/issues. Alternatively, you can join my Discord server (https://
-discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
-feedback, or report any errors. I do also have a multi-function Discord bot.
-Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
-Copyright This repository doesn't include any copyrighted material. If you
-happen to come across any copyrighted content within this repository (but
-hosted elsewhere) that you own or represent, email me at
-**grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+gif = gifs.get_gif(user_input) #return the url of the gif if the category
+exists. except animegifs.errors.CategoryError: print("not a valid gif
+category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Submit a GIF If you also want to
+contribute to the gifs collection, you can submit a gif at: https://forms.gle/
+wxWmRuy5VCdDCZWp8 # Troubleshooting and other The first call (only!) in the
+session is expected to have a slower reaction time (5-15s) because of the
+authentication process. If you encounter an error, please raise an issue on the
+issue page: https://github.com/MarcoSa-2000/animegifs/issues. Alternatively,
+you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to
+request new categories, functions, provide feedback, or report any errors. I do
+also have a multi-function Discord bot. Feel free to check out the web
+dashboard here: https://enkidu-app.github.io. # Copyright This repository
+doesn't include any copyrighted material. If you happen to come across any
+copyrighted content within this repository (but hosted elsewhere) that you own
+or represent, email me at **grest0grest@gmail.com**. Please provide specific
+details about the copyrighted material and where it can be found. Once I
+confirm your claim, I'll take immediate action to remove the identified
+material.
```

### Comparing `animegifs-0.7.1/animegifs/animegifs.py` & `animegifs-0.7.2/animegifs/animegifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.7.1/animegifs/distutils/errors.py` & `animegifs-0.7.2/animegifs/distutils/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 class CategoryIntegral(Exception):
     """
     Category can't be an integral, only a string.
-    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs
+    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs#category-list
     """
 
     def __init__(self, category, error="Category can't be an integral."):
         self.category = category
         self.error = error
         super().__init__(self.error)
 
 class CategoryError(Exception):
     """
     Not a valid category. Category must be a string.
-    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs
+    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs#category-list
     """
 
     def __init__(self, category, error="Not a valid category."):
         self.category = category
         self.error = error
         super().__init__(self.error)
 
 class CategoryUnknown(Exception):
     """
     This is a not handled error, probably the category type is neither an int nor a str.
     Make sure to check category is a string and is a valid category.
-    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs
+    You can check valid categories at: https://github.com/MarcoSa-2000/animegifs#category-list
     """
 
     def __init__(self, category, error="Not a valid category."):
         self.category = category
         self.error = error
         super().__init__(self.error)
```

### Comparing `animegifs-0.7.1/animegifs/distutils/gifs.py` & `animegifs-0.7.2/animegifs/distutils/gifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.7.1/animegifs.egg-info/PKG-INFO` & `animegifs-0.7.2/animegifs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.7.1
+Version: 0.7.2
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -28,15 +28,15 @@
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MarcoSa-2000/animegifs?style=for-the-badge"></a>
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.7 will not have the gifs library updated anymore.
 For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
@@ -65,15 +65,15 @@
 
 gifs = animegifs.Animegifs()
 
 user_input = input() #let user send any input and search if that input matches a category.
 #if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
 #   user_input = "bite"
 try:
-    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+    gif = gifs.get_gif(user_input) #return the url of the gif if the category exists.
 except animegifs.errors.CategoryError:
     print("not a valid gif category.")
 ```
 
 ## Category list:
 
 **A**
@@ -115,15 +115,15 @@
 **P**
 * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
 
 **R**
 * Run
 
 **S**
-* Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
+* Sad, Scared, Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank, Stare
 
 **T**
 * Tease, Threat, Tickle, Tired
 
 **W**
 * Wave
```

#### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.7.1 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.2 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
-flawlessly or at all. Version below v0.6 will not have the gifs library updated
+flawlessly or at all. Version below v0.7 will not have the gifs library updated
 anymore. For troubleshoots, known errors and categories list, check below. `pip
 install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
 gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
 the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
 return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
 myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
 anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
 page. ``` ```py #v0.6> from animegifs import animegifs gifs =
 animegifs.Animegifs() user_input = input() #let user send any input and search
 if that input matches a category. #if user_input == "nom": #nom as category
 doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
-gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
-except animegifs.errors.CategoryError: print("not a valid gif category.") ```
-## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
-**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
-Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
-Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
-Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
-**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
-Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
-Category List** * Random, Steal-magic # Live API You can test out the API (and
-lib functionality) on my bot's website here: https://enkidu-app.github.io/
-animegifs # Submit a GIF If you also want to contribute to the gifs collection,
-you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
-and other The first call (only!) in the session is expected to have a slower
-reaction time (5-15s) because of the authentication process. If you encounter
-an error, please raise an issue on the issue page: https://github.com/MarcoSa-
-2000/animegifs/issues. Alternatively, you can join my Discord server (https://
-discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
-feedback, or report any errors. I do also have a multi-function Discord bot.
-Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
-Copyright This repository doesn't include any copyrighted material. If you
-happen to come across any copyrighted content within this repository (but
-hosted elsewhere) that you own or represent, email me at
-**grest0grest@gmail.com**. Please provide specific details about the
-copyrighted material and where it can be found. Once I confirm your claim, I'll
-take immediate action to remove the identified material.
+gif = gifs.get_gif(user_input) #return the url of the gif if the category
+exists. except animegifs.errors.CategoryError: print("not a valid gif
+category.") ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
+Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
+Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
+Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
+Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
+Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, Shoot, Shrug,
+Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
+**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
+Live API You can test out the API (and lib functionality) on my bot's website
+here: https://enkidu-app.github.io/animegifs # Submit a GIF If you also want to
+contribute to the gifs collection, you can submit a gif at: https://forms.gle/
+wxWmRuy5VCdDCZWp8 # Troubleshooting and other The first call (only!) in the
+session is expected to have a slower reaction time (5-15s) because of the
+authentication process. If you encounter an error, please raise an issue on the
+issue page: https://github.com/MarcoSa-2000/animegifs/issues. Alternatively,
+you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to
+request new categories, functions, provide feedback, or report any errors. I do
+also have a multi-function Discord bot. Feel free to check out the web
+dashboard here: https://enkidu-app.github.io. # Copyright This repository
+doesn't include any copyrighted material. If you happen to come across any
+copyrighted content within this repository (but hosted elsewhere) that you own
+or represent, email me at **grest0grest@gmail.com**. Please provide specific
+details about the copyrighted material and where it can be found. Once I
+confirm your claim, I'll take immediate action to remove the identified
+material.
```

### Comparing `animegifs-0.7.1/setup.py` & `animegifs-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.7.1'
+VERSION = '0.7.2'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Marco-Sa2000',
     author_email='grest0grest@gmail.com',
     license='MIT',
     url="https://github.com/MarcoSa-2000/animegifs",
     install_requires=[
-       'requests>=2.28.2,<=2.29.0',
+       'requests==2.31.0',
        'mal-api==0.5.3',
-       'PyJWT>=2.4.0,<=2.7.0'
+       'PyJWT>=2.4.0,<=2.8.0'
     ],
     python_requires='>=3.8',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

