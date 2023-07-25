# Comparing `tmp/gogo_cli-0.0.6.tar.gz` & `tmp/gogo_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.6.tar", max compression
+gzip compressed data, was "gogo_cli-0.0.7.tar", max compression
```

## Comparing `gogo_cli-0.0.6.tar` & `gogo_cli-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/LICENSE
--rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2894 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0      981 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1054 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1054 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.7/PKG-INFO
```

### Comparing `gogo_cli-0.0.6/LICENSE` & `gogo_cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.6/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.0.7/gogo_cli/core/__gogo_cli__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
 query = query.replace(' ', '%20')
 
 url = f"https://api.consumet.org/anime/gogoanime/{query}"
 
 
 
-def play(anime, episode, playNext):
-    if playNext == 1:
-        episode = episode + 1
+def play(anime, episode):
     play_url = f"https://api.consumet.org/anime/gogoanime/watch/{anime}-episode-{episode}"
     data = client.get(play_url, params = { "server": "gogocdn" },).text
     parsed_data = json.loads(data)
     referrer = parsed_data["headers"]["Referer"]
     quality_options = [source["quality"] for source in parsed_data["sources"]]
    
     if len(quality_options) > 1:
@@ -71,16 +69,15 @@
     data = client.get(info_url).text
     parsed_data = json.loads(data)
     total_episodes = parsed_data['totalEpisodes']
     if total_episodes > 1:
         ch = int(input(f"Total Episodes: {total_episodes}, Enter episode to play: "))
     else:
         ch = 1
-    playNext = 0
-    uwu = play(anime, ch, playNext)
+    uwu = play(anime, ch)
 
 def search():
     try:
         result = client.get(url).text
         parsed_data = json.loads(result)
         result_ids = [result['id'] for result in parsed_data['results']]
         for idx, result_id in enumerate(result_ids, start=1):
```

### Comparing `gogo_cli-0.0.6/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.0.7/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.6/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.0.7/gogo_cli/core/utils/__player__.py`

 * *Files identical despite different names*

