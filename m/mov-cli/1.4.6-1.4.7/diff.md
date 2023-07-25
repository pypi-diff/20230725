# Comparing `tmp/mov_cli-1.4.6.tar.gz` & `tmp/mov_cli-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.6.tar", max compression
+gzip compressed data, was "mov_cli-1.4.7.tar", max compression
```

## Comparing `mov_cli-1.4.6.tar` & `mov_cli-1.4.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2023-07-24 19:39:52.997461 mov_cli-1.4.6/LICENSE
--rw-r--r--   0        0        0     6933 2023-07-24 19:39:52.997461 mov_cli-1.4.6/README.md
--rw-r--r--   0        0        0      686 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/__init__.py
--rw-r--r--   0        0        0      809 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      906 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-07-24 19:39:52.997461 mov_cli-1.4.6/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0      341 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/extractors/tukipasti.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     3128 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     2772 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0      356 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ar.json
--rw-r--r--   0        0        0      356 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/de.json
--rw-r--r--   0        0        0      309 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/en.json
--rw-r--r--   0        0        0      348 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/fr.json
--rw-r--r--   0        0        0      338 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ko.json
--rw-r--r--   0        0        0      194 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/langs
--rw-r--r--   0        0        0      308 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/pl.json
--rw-r--r--   0        0        0      289 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/pt.json
--rw-r--r--   0        0        0      418 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ru.json
--rw-r--r--   0        0        0      660 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang/ta.json
--rw-r--r--   0        0        0     1752 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1563 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/player.py
--rw-r--r--   0        0        0     1171 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/props.py
--rw-r--r--   0        0        0     7383 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0     4630 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/utils/select.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/anime/__init__.py
--rw-r--r--   0        0        0     3286 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/anime/gogoanime.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/__init__.py
--rw-r--r--   0        0        0     3767 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/viewasian.py
--rw-r--r--   0        0        0     3394 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/asian/watchasian.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/cartoons/__init__.py
--rw-r--r--   0        0        0     3734 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/cartoons/kisscartoon.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.001461 mov_cli-1.4.6/mov_cli/websites/english/__init__.py
--rw-r--r--   0        0        0     7381 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/actvid.py
--rw-r--r--   0        0        0     3856 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/dopebox.py
--rw-r--r--   0        0        0     4242 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/remotestream.py
--rw-r--r--   0        0        0     3734 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/sflix.py
--rw-r--r--   0        0        0     1841 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/english/solar.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/__init__.py
--rw-r--r--   0        0        0     1943 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/einthusan.py
--rw-r--r--   0        0        0     2165 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/indian/tamilyogi.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/international/__init__.py
--rw-r--r--   0        0        0     3962 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/international/wlext.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/livetv/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/livetv/eja.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/sports/__init__.py
--rw-r--r--   0        0        0     4474 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/sports/scdn.py
--rw-r--r--   0        0        0        0 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/__init__.py
--rw-r--r--   0        0        0     2330 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/turkish123.py
--rw-r--r--   0        0        0     2921 2023-07-24 19:39:53.005462 mov_cli-1.4.6/mov_cli/websites/turkish/yoturkish.py
--rw-r--r--   0        0        0      736 2023-07-24 19:39:53.005462 mov_cli-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 mov_cli-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 17:14:27.983137 mov_cli-1.4.7/LICENSE
+-rw-r--r--   0        0        0     6540 2023-07-25 17:14:27.983137 mov_cli-1.4.7/README.md
+-rw-r--r--   0        0        0      687 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0      341 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/tukipasti.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2772 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0      356 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ar.json
+-rw-r--r--   0        0        0      356 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/de.json
+-rw-r--r--   0        0        0      309 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/en.json
+-rw-r--r--   0        0        0      348 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/fr.json
+-rw-r--r--   0        0        0      338 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ko.json
+-rw-r--r--   0        0        0      194 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/langs
+-rw-r--r--   0        0        0      308 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/pl.json
+-rw-r--r--   0        0        0      289 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/pt.json
+-rw-r--r--   0        0        0      418 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ru.json
+-rw-r--r--   0        0        0      660 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ta.json
+-rw-r--r--   0        0        0     1273 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1563 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1278 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/props.py
+-rw-r--r--   0        0        0     7472 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0     4900 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/select.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/anime/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/anime/gogoanime.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/viewasian.py
+-rw-r--r--   0        0        0     3382 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/watchasian.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/cartoons/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/cartoons/kisscartoon.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/__init__.py
+-rw-r--r--   0        0        0     6931 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/actvid.py
+-rw-r--r--   0        0        0     3274 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/dopebox.py
+-rw-r--r--   0        0        0     4242 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/remotestream.py
+-rw-r--r--   0        0        0     3273 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/english/sflix.py
+-rw-r--r--   0        0        0     1055 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/english/solar.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/__init__.py
+-rw-r--r--   0        0        0     1943 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/einthusan.py
+-rw-r--r--   0        0        0     2165 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/tamilyogi.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/international/__init__.py
+-rw-r--r--   0        0        0     3950 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/international/wlext.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/livetv/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/livetv/eja.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/sports/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/sports/scdn.py
+-rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/__init__.py
+-rw-r--r--   0        0        0     2318 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/turkish123.py
+-rw-r--r--   0        0        0     2909 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/yoturkish.py
+-rw-r--r--   0        0        0      736 2023-07-25 17:14:27.987137 mov_cli-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     7529 1970-01-01 00:00:00.000000 mov_cli-1.4.7/PKG-INFO
```

### Comparing `mov_cli-1.4.6/LICENSE` & `mov_cli-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/README.md` & `mov_cli-1.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         <li><a href="#ios">iOS</a></li>
       </ul>
     </ul>
   </li>
   <li><a href="#usage">Usage</a></li>
   <li><a href="#disclaimer">Disclaimer</a></li>
   <li><a href="#contributing">Contributing</a></li>
-  <li><a href="#add-a-language">Adding Languages</a></li>
   <li><a href="#license">License</a></li>
   <li><a href="#contact">Contact</a></li>
   <li><a href="#inspiration">inspiration</a></li>
 </ol>
 
 
 <!-- ABOUT THE PROJECT -->
@@ -123,19 +122,20 @@
     ```
 
 
 <!-- IOS -->
 ### iOS
   - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243) are installed.
 
-  - Run following commands (Note: this may take a while, it's iSH fault.)
+  - Run following commands (Note: this may take a while)
     ```
     apk update && apk upgrade
     apk add python3 fzf
     python3 -m ensurepip
+    mkdir /home/root
     pip3 install mov-cli
     ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
@@ -172,26 +172,14 @@
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
-<!-- ADDING LANGUAGES -->
-## Add a Language
-Please go to [mov-cli/translations](https://github.com/mov-cli/translations) there are instructions on how to add a Language.
-
-<!-- LICENSE -->
-## License
-
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
 <!-- CONTACT -->
 ## Contact
 
 Author: Poseidon444 | ```Discord: pain444```
 
 Maintainer: HLOAnanas | ```Discord: r3tr0ananas```
```

#### html2text {}

```diff
@@ -11,18 +11,17 @@
           o Installation
                 # Windows_/_Linux
                 # Android
                 # iOS
    3. Usage
    4. Disclaimer
    5. Contributing
-   6. Adding_Languages
-   7. License
-   8. Contact
-   9. inspiration
+   6. License
+   7. Contact
+   8. inspiration
  ## About The Project The new and improved mov-cli is here. mov-cli is a
 Commandline Tool to watch and download shows and movies. Shows and Movies are
 sourced from Streaming Sites.
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
 [`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
              (https://iina.io) - player used for MacOS - [`Outplayer`](https://
   outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
@@ -31,16 +30,16 @@
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
               ### Android - Make sure [MPV](https://play.google.com/store/apps/
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
   id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243)
- are installed. - Run following commands (Note: this may take a while, it's iSH
- fault.) ``` apk update && apk upgrade apk add python3 fzf python3 -m ensurepip
+  are installed. - Run following commands (Note: this may take a while) ``` apk
+update && apk upgrade apk add python3 fzf python3 -m ensurepip mkdir /home/root
                                                        pip3 install mov-cli ```
                                                                   (back_to_top)
  ## Usage Type: ```mov-cli``` into your Commandline.
                                                                   (back_to_top)
  ## Disclaimer This project is to be used at the userâs own risk, based on
 their government and laws. This project has no control on the content it is
 serving, using copyrighted content from the providers is not going to be
@@ -50,18 +49,14 @@
  ## Feature If you want a feature, create an [issue](https://github.com/mov-
 cli/mov-cli/issues/new) or create the feature and make a pull request.
                                                                   (back_to_top)
  ## Contributing Pull requests are welcome and _appreciated_. For major
 changes, please open an issue first to discuss what you would like to change.
 Contributors: [https://contrib.rocks/image?repo=mov-cli/mov-cli]
                                                                   (back_to_top)
- ## Add a Language Please go to [mov-cli/translations](https://github.com/mov-
-cli/translations) there are instructions on how to add a Language.  ## License
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
-                                                                  (back_to_top)
  ## Contact Author: Poseidon444 | ```Discord: pain444``` Maintainer: HLOAnanas
 | ```Discord: r3tr0ananas``` Project Link: [https://github.com/mov-cli/mov-cli]
 (https://github.com/mov-cli/mov-cli)
                                                                   (back_to_top)
  ## Inspiration Heavily inspired from [ani-cli](https://github.com/pystardust/
 ani-cli)
                                                                   (back_to_top)
```

### Comparing `mov_cli-1.4.6/mov_cli/__init__.py` & `mov_cli-1.4.7/mov_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 args_parser.add_argument("--debug", action="store_true", required=False)
 args_parser.add_argument("-p", required=False, help="Select Provider from Terminal")
 args_parser.add_argument("-s", required=False, help="Search from the Terminal")
 CMD_ARGS = args_parser.parse_args()
 
 if CMD_ARGS.pupdate:
     from .utils.select import updateProvider
+
     updateProvider()
 
 """Arguments parsed from the command line via argparse."""
```

### Comparing `mov_cli-1.4.6/mov_cli/__main__.py` & `mov_cli-1.4.7/mov_cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .utils.scraper import WebScraper
 from . import CMD_ARGS
 
 if platform.system() == "Windows":
     os.system("color FF")  # Fixes colour in Windows 10 CMD terminal
 
 
-def movcli(): # TODO add regex
+def movcli():  # TODO add regex
     if CMD_ARGS.debug:
         cl, url = ask(CMD_ARGS.p)
         provider: WebScraper = cl.Provider(url)
         provider.redo(CMD_ARGS.s)
     else:
         try:
             cl, url = ask(CMD_ARGS.p)
```

### Comparing `mov_cli-1.4.6/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.7/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.7/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/players/player.py` & `mov_cli-1.4.7/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/utils/httpclient.py` & `mov_cli-1.4.7/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/utils/lang/ta.json` & `mov_cli-1.4.7/mov_cli/utils/lang/ta.json`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/utils/lang.py` & `mov_cli-1.4.7/mov_cli/utils/lang.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,49 @@
-import httpx
 from fzf import fzf_prompt
 from .props import home
 import mov_cli.__main__ as mc
 from json import loads
 from .props import RestartNeeded, LanguageNotAOption
 from pkgutil import get_data
 
 langsfile = get_data(__name__, "lang/langs")
 
-sel = eval(langsfile)
+langsfile = loads(langsfile)
 
-def existing(language: str, g=False):
-    js = loads(langsfile)
+def existing(language: str, g: bool = False):
 
     exist = False
 
-    if g is False:
-        for _, value in js.items():
-            if value == language:
-                exist = True
-        if not exist:
-            raise LanguageNotAOption(language)
+    for _, value in langsfile.items():
+        if value == language:
+            exist = True
+    if not exist and not g:
+        raise LanguageNotAOption(language)
     else:
-        for _, value in js.items():
-            if value == language:
-                exist = True
         return exist
 
 def getlang():
     try:
-        with open(home() + "lang.mov-cli", "r") as f:
+        with open(f"{home()}/lang.mov-cli", "r") as f:
             lang = f.read()
         existing(lang)
         t = loads(get_data(__name__, f"lang/{lang}.json"))
-        ask = t["ASK"]
-        ex = t["EXIT"]
-        searcha = t["SEARCHA"]
-        download = t["DOWNLOAD"]
-        spro = t["SPROVIDER"]
-        dshow = t["DSHOW"]
-        dseason = t["DSEASON"]
-        season = t["SEASON"]
-        episode = t["EPISODE"]
-        change = t["CHANGE"]
-        t = [ask, ex, searcha, download, spro, dshow, dseason, season, episode, change]
-        return t
+        items = []
+        for _, value in t.items():
+            items.append(value)
+        return items
     except FileNotFoundError:
         import locale
 
         localLang = locale.getdefaultlocale()[0][:2]
         check = existing(localLang, True)
-        if check is True:
+        if check:
             lang = localLang
         else:
             lang = "en"
-        open(home() + "lang.mov-cli", "w").write(lang)
-        print(f"[?] Your Language was set to {lang}")
-        raise RestartNeeded
+        open(f"{home()}/lang.mov-cli", "w").write(lang)
+        return mc.movcli()
 
 def setlang():
-    s = fzf_prompt(sel)
-    selection = sel.get(s)
-    open(home() + "lang.mov-cli", "w").write(selection)
+    s = fzf_prompt(langsfile)
+    selection = langsfile.get(s)
+    open(f"{home()}/lang.mov-cli", "w").write(selection)
```

### Comparing `mov_cli-1.4.6/mov_cli/utils/player.py` & `mov_cli-1.4.7/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/utils/scraper.py` & `mov_cli-1.4.7/mov_cli/utils/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,19 @@
         subtitle: str = None,
         season="",
         episode=None,
         referrer: str = None,
     ):
         name = self.parse(name)
         fixname = re.sub(r"-+ +", " ", name)
-        if episode:
+        if episode and season:
             fixname = f"{fixname} S{season}E{episode}"
+        
+        if episode:
+            fixname = f"{fixname} E{episode}"
 
         if referrer:
             referrer = referrer
         else:
             referrer = self.base_url
         # args = shlex.split(f 'ffmpeg -i "{url}" -c copy {self.parse(name)}.mp4')
         args = [
```

### Comparing `mov_cli-1.4.6/mov_cli/utils/select.py` & `mov_cli-1.4.7/mov_cli/utils/select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 from fzf import fzf_prompt
 from importlib import import_module
 from .props import home, RestartNeeded
 from httpx import get
 import json
+from .props import firstStart
 
-base = {"eja": "https://eja.tv", "actvid": "https://actvid.rs", "sflix": "https://sflix.se", "solar": "https://solarmovie.pe", "dopebox": "https://dopebox.to", "viewasian": "https://viewasian.co", "gogoanime": "https://gogoanimehd.to/", "watchasian": "https://watchasian.mx", "wlext": "https://wlext.is", "streamblasters": "https://streamblasters.pro", "tamilyogi": "https://tamilyogi.email", "einthusan": "https://einthusan.tv", "turkish123": "https://turkish123.ac", "scdn": "", "remotestream": "https://remotestre.am", "kisscartoon": "https://thekisscartoon.com", "yoturkish": "https://www1.yoturkish.com"}
+base = {
+    "eja": "https://eja.tv",
+    "actvid": "https://actvid.rs",
+    "sflix": "https://sflix.se",
+    "solar": "https://solarmovie.pe",
+    "dopebox": "https://dopebox.to",
+    "viewasian": "https://viewasian.co",
+    "gogoanime": "https://gogoanimehd.to/",
+    "watchasian": "https://watchasian.mx",
+    "wlext": "https://wlext.is",
+    "streamblasters": "https://streamblasters.pro",
+    "tamilyogi": "https://tamilyogi.email",
+    "einthusan": "https://einthusan.tv",
+    "turkish123": "https://turkish123.ac",
+    "scdn": "",
+    "remotestream": "https://remotestre.am",
+    "kisscartoon": "https://thekisscartoon.com",
+    "yoturkish": "https://www1.yoturkish.com",
+}
 
 english = ["actvid", "sflix", "solar", "dopebox", "remotestream"]
 
 indian = [
     "tamilyogi",
     "einthusan",
     "streamblasters",
@@ -65,30 +84,35 @@
 
 def export(provider: str, typ: str, version: str = "mov_cli"):
     module = f"{version}.websites.{typ}.{provider}"
     return import_module(module)
 
 
 def p():
+    firstStart()
     try:
         js = open(f"{home()}/provider.mov-cli")
-        calls = json.load(js)
     except FileNotFoundError:
-        open(f"{home()}/provider.mov-cli", "w").write(json.dumps(base))
-        raise RestartNeeded
+        with open(f"{home()}/provider.mov-cli", "w") as f:
+            f.write(json.dumps(base))
+            js = f.read()
+    calls = json.load(js)
 
-    from porn_cli.__main__ import websites
-    if ph != []:
-        return dict(calls)
-    for main, sub in websites.items():
-        calls[main] = sub
-        ph.append(str(main))
-        preselction["Porn Providers"] = ph
-    return dict(calls)
+    try:
+        from porn_cli.__main__ import websites
 
+        if ph != []:
+            return dict(calls)
+        for main, sub in websites.items():
+            calls[main] = sub
+            ph.append(str(main))
+            preselction["Porn Providers"] = ph
+        return dict(calls)
+    except:
+        return dict(calls)
 
 
 def ask(provider: str = None):
     calls = p()
     if provider:
         provider = provider.replace(" ", "")
         get = calls.get(provider)
@@ -108,28 +132,30 @@
                 version = "porn_cli"
             else:
                 version = "mov_cli"
             cl = export(provider, typ, version)
             return cl, get
     else:
         init = fzf_prompt(preselction, header="Select:")
-        if init is None: exit(1)
+        if init is None:
+            exit(1)
         get = preselction.get(init)
         choice = fzf_prompt(get, header="Select:")
         typ = init.split(" ")[0].lower()
         if typ.__contains__("porn"):
             version = "porn_cli"
         else:
             version = "mov_cli"
         cl = export(choice, typ, version)
         return cl, calls.get(choice)
 
 
 def updateProvider():
     import tldextract
+
     DEFAULT_HEADERS: dict = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
         "Chrome/80.0.3987.163 "
         "Safari/537.36",
         "Accept-Language": "en-GB,en;q=0.5",
     }
 
@@ -143,15 +169,17 @@
             continue
         checkext = tldextract.extract(str(check.url))
         subext = tldextract.extract(sub)
         if checkext.registered_domain == subext.registered_domain:
             print(f"Checked: {main}")
         else:
             if checkext.subdomain:
-                updatedurl = "https://" + checkext.subdomain + "." + checkext.registered_domain
+                updatedurl = (
+                    "https://" + checkext.subdomain + "." + checkext.registered_domain
+                )
             else:
-                updatedurl = "https://" +  checkext.registered_domain
+                updatedurl = "https://" + checkext.registered_domain
             calls[main] = updatedurl
             print(f"Updated: {main} from {sub} to {updatedurl}")
     open(f"{home()}/provider.mov-cli", "w").write(json.dumps(calls))
     print("Provider Check: Done")
-    exit(0)
+    exit(0)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/anime/gogoanime.py` & `mov_cli-1.4.7/mov_cli/websites/anime/gogoanime.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,10 +76,10 @@
             )
             self.dl(url, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         name = t[self.title]
         url, episode = self.ask(t[self.url])
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/asian/viewasian.py` & `mov_cli-1.4.7/mov_cli/websites/asian/viewasian.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,10 +78,10 @@
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
         url, episode = self.ask(t[self.url])
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/asian/watchasian.py` & `mov_cli-1.4.7/mov_cli/websites/asian/watchasian.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,10 +78,10 @@
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
         link, episode = self.ask(t[self.url])
         url = self.doodstream(link)
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/cartoons/kisscartoon.py` & `mov_cli-1.4.7/mov_cli/websites/cartoons/kisscartoon.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,28 +78,22 @@
             + videoServer
             + "&d="
         )
         print(hls)
         return hls, inter_1
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
-        if state == "sd":
-            self.download(t)
-            return
         name = t[self.title]
         link, episode = self.ask(t[self.url])
         url, ref = self.cdn_url(link)
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name, referrer=ref)
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
         name = m[self.title]
         url, ref = self.cdn_url(m[self.url])
         if state == "d":
             self.dl(url, name)
             return
-        if state == "sd":
-            print("You can download only Shows with 'sd'")
-            return
         self.play(url, name, referrer=ref)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/english/actvid.py` & `mov_cli-1.4.7/mov_cli/websites/english/actvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,63 +36,48 @@
             for i in soup.select(".film-poster-ahref")
         ]
         title = [i.text for i in soup.select(".film-name > a")]
         ids = [i.split("-")[-1] for i in urls]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, series_id: str) -> tuple:
-        r = self.client.get(f"{self.base_url}/ajax/season/list/{series_id}") # self.ajax_season
+        r = self.client.get(
+            f"{self.base_url}/ajax/season/list/{series_id}"
+        )  # self.ajax_season
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
         z = f"{self.base_url}/ajax/season/episodes/{season_ids[int(season) - 1]}"
         rf = self.client.get(z)
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
-        episode = episodes[int(self.askepisode(len(episodes))) - 1]
-        ep = self.getep(
-            url=f"{self.base_url}/ajax/season/episodes/{season_ids[int(season) - 1]}",
-            data_id=f"{episode}",
-        )
+        ep = self.askepisode(len(episodes))
+        episode = episodes[int(ep) - 1]
         return episode, season, ep
-
-    def getep(self, url, data_id):
-        source = self.client.get(f"{url}").text
-
-        soup = BS(source, self.scraper)
-
-        unformated = soup.find("a", {"data-id": f"{data_id}"})["title"]
-
-        formated = unformated.split("Eps")[1]
-        formated = formated.split(":")[0]
-
-        return formated
-
+    
     def cdn_url(self, final_link: str, rabb_id: str) -> str:
         self.client.set_headers({"X-Requested-With": "XMLHttpRequest"})
         data = self.client.get(f"{final_link}getSources?id={rabb_id}").json()
         n = json.loads(self.decrypt(data["sources"], self.gh_key()))
         return n[0]["file"]
 
     def server_id(self, mov_id: str) -> str:
         req = self.client.get(f"{self.base_url}/ajax/episode/list/{mov_id}")
         soup = BS(req, self.scraper)
         return [i["data-linkid"] for i in soup.select(".nav-item > a")][0]
 
     def ep_server_id(self, ep_id: str) -> str:
-        req = self.client.get(
-            f"{self.base_url}/ajax/episode/servers/{ep_id}"
-        )
+        req = self.client.get(f"{self.base_url}/ajax/episode/servers/{ep_id}")
         soup = BS(req, self.scraper)
         return [i["data-id"] for i in soup.select(".nav-item > a")][0]
 
     def get_link(self, thing_id: str) -> tuple:
-        req = self.client.get(f"{self.base_url}/ajax/episode/sources/{thing_id}").json()[
-            "link"
-        ]
+        req = self.client.get(
+            f"{self.base_url}/ajax/episode/sources/{thing_id}"
+        ).json()["link"]
         print(req)
         return req, self.rabbit_id(req)
 
     def rabbit_id(self, url: str) -> tuple:
         parts = p.urlparse(url, allow_fragments=True, scheme="/").path.split("/")
         return (
             re.findall(r"(https:\/\/.*\/embed-4)", url)[0].replace(
@@ -122,15 +107,15 @@
         return s[: -ord(s[len(s) - 1 :])]
 
     def decrypt(self, data, key):
         k = self.get_key(base64.b64decode(data)[8:16], key)
         dec_key = k[:32]
         iv = k[32:]
         p = AES.new(dec_key, AES.MODE_CBC, iv=iv).decrypt(base64.b64decode(data)[16:])
-        return self.unpad(p).decode()   
+        return self.unpad(p).decode()
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/english/dopebox.py` & `mov_cli-1.4.7/mov_cli/websites/english/dopebox.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,45 +15,26 @@
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
-        episode = episodes[int(self.askepisode(len(episodes))) - 1]
-        ep = self.getep(
-            f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
-            data_id=episode,
-        )
+        ep = self.askepisode(len(episodes))
+        episode = episodes[int(ep) - 1]
         return episode, season, ep
 
-    def getep(self, url, data_id):
-        source = self.client.get(f"{url}").text
-        soup = BS(source, self.scraper)
-
-        unformated = soup.find("div", {"data-id": f"{data_id}"})
-
-        children = unformated.findChildren("div", {"class": "episode-number"})
-        for child in children:
-            text = child.text
-
-        text = text.split("Episode")[1]
-        text = text.split(":")[0]
-
-        return text
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def get_link(self, thing_id: str) -> tuple:
-        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()[
-            "link"
-        ]
+        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()["link"]
         print(req)
         return req, self.rabbit_id(req)
 
     def ep_server_id(self, ep_id):
         rem = self.client.get(
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/english/remotestream.py` & `mov_cli-1.4.7/mov_cli/websites/english/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/english/sflix.py` & `mov_cli-1.4.7/mov_cli/websites/english/sflix.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,35 +20,18 @@
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         ep = self.askepisode(len(episodes))
         episode = episodes[int(ep) - 1]
         return episode, season, ep
 
     def get_link(self, thing_id: str) -> tuple:
-        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()[
-            "link"
-        ]
+        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()["link"]
         print(req)
         return req, self.rabbit_id(req)
 
-
-    def getep(self, url, data_id):
-        source = self.client.get(f"{url}").text
-        soup = BS(source, self.scraper)
-
-        unformated = soup.find("div", {"data-id": f"{data_id}"})
-
-        children = unformated.findChildren("div", {"class": "episode-number"})
-        for child in children:
-            text = child.text
-            text = text.split("Episode")[1]
-            text = text.split(":")[0]
-
-            return text
-
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ep_server_id(self, ep_id):
         rem = self.client.get(
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/indian/einthusan.py` & `mov_cli-1.4.7/mov_cli/websites/indian/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/indian/streamblasters.py` & `mov_cli-1.4.7/mov_cli/websites/indian/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/indian/tamilyogi.py` & `mov_cli-1.4.7/mov_cli/websites/indian/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/international/wlext.py` & `mov_cli-1.4.7/mov_cli/websites/international/wlext.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             self.dl(url, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         name = t[self.title]
         url, episode = self.ask(t[self.url])
         url = str(self.cdn_url(url))
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name)
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
         name = m[self.title]
         url, episode = self.ask(m[self.url])
         url = self.cdn_url(url)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/livetv/eja.py` & `mov_cli-1.4.7/mov_cli/websites/livetv/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/sports/scdn.py` & `mov_cli-1.4.7/mov_cli/websites/sports/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.6/mov_cli/websites/turkish/turkish123.py` & `mov_cli-1.4.7/mov_cli/websites/turkish/turkish123.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     def TV_PandDP(self, t: list, state: str):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
         url, episode, ref = self.ask(t[self.url])
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name, referrer=ref)
```

### Comparing `mov_cli-1.4.6/mov_cli/websites/turkish/yoturkish.py` & `mov_cli-1.4.7/mov_cli/websites/turkish/yoturkish.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,10 +67,10 @@
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd" or "ds"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
         url, episode, ref = self.ask(t[self.url])
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name, episode=episode)
             return
         self.play(url, name, referrer=ref)
```

### Comparing `mov_cli-1.4.6/pyproject.toml` & `mov_cli-1.4.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.6"
+version = "1.4.7"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@r3tr0ananas.lol>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.6/PKG-INFO` & `mov_cli-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.6
+Version: 1.4.7
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@r3tr0ananas.lol
@@ -84,15 +84,14 @@
         <li><a href="#ios">iOS</a></li>
       </ul>
     </ul>
   </li>
   <li><a href="#usage">Usage</a></li>
   <li><a href="#disclaimer">Disclaimer</a></li>
   <li><a href="#contributing">Contributing</a></li>
-  <li><a href="#add-a-language">Adding Languages</a></li>
   <li><a href="#license">License</a></li>
   <li><a href="#contact">Contact</a></li>
   <li><a href="#inspiration">inspiration</a></li>
 </ol>
 
 
 <!-- ABOUT THE PROJECT -->
@@ -149,19 +148,20 @@
     ```
 
 
 <!-- IOS -->
 ### iOS
   - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243) are installed.
 
-  - Run following commands (Note: this may take a while, it's iSH fault.)
+  - Run following commands (Note: this may take a while)
     ```
     apk update && apk upgrade
     apk add python3 fzf
     python3 -m ensurepip
+    mkdir /home/root
     pip3 install mov-cli
     ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
@@ -198,26 +198,14 @@
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
-<!-- ADDING LANGUAGES -->
-## Add a Language
-Please go to [mov-cli/translations](https://github.com/mov-cli/translations) there are instructions on how to add a Language.
-
-<!-- LICENSE -->
-## License
-
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
 <!-- CONTACT -->
 ## Contact
 
 Author: Poseidon444 | ```Discord: pain444```
 
 Maintainer: HLOAnanas | ```Discord: r3tr0ananas```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.6 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.7 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@r3tr0ananas.lol Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
@@ -24,18 +24,17 @@
           o Installation
                 # Windows_/_Linux
                 # Android
                 # iOS
    3. Usage
    4. Disclaimer
    5. Contributing
-   6. Adding_Languages
-   7. License
-   8. Contact
-   9. inspiration
+   6. License
+   7. Contact
+   8. inspiration
  ## About The Project The new and improved mov-cli is here. mov-cli is a
 Commandline Tool to watch and download shows and movies. Shows and Movies are
 sourced from Streaming Sites.
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
 [`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
              (https://iina.io) - player used for MacOS - [`Outplayer`](https://
   outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
@@ -44,16 +43,16 @@
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
               ### Android - Make sure [MPV](https://play.google.com/store/apps/
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
   id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243)
- are installed. - Run following commands (Note: this may take a while, it's iSH
- fault.) ``` apk update && apk upgrade apk add python3 fzf python3 -m ensurepip
+  are installed. - Run following commands (Note: this may take a while) ``` apk
+update && apk upgrade apk add python3 fzf python3 -m ensurepip mkdir /home/root
                                                        pip3 install mov-cli ```
                                                                   (back_to_top)
  ## Usage Type: ```mov-cli``` into your Commandline.
                                                                   (back_to_top)
  ## Disclaimer This project is to be used at the userâs own risk, based on
 their government and laws. This project has no control on the content it is
 serving, using copyrighted content from the providers is not going to be
@@ -63,18 +62,14 @@
  ## Feature If you want a feature, create an [issue](https://github.com/mov-
 cli/mov-cli/issues/new) or create the feature and make a pull request.
                                                                   (back_to_top)
  ## Contributing Pull requests are welcome and _appreciated_. For major
 changes, please open an issue first to discuss what you would like to change.
 Contributors: [https://contrib.rocks/image?repo=mov-cli/mov-cli]
                                                                   (back_to_top)
- ## Add a Language Please go to [mov-cli/translations](https://github.com/mov-
-cli/translations) there are instructions on how to add a Language.  ## License
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
-                                                                  (back_to_top)
  ## Contact Author: Poseidon444 | ```Discord: pain444``` Maintainer: HLOAnanas
 | ```Discord: r3tr0ananas``` Project Link: [https://github.com/mov-cli/mov-cli]
 (https://github.com/mov-cli/mov-cli)
                                                                   (back_to_top)
  ## Inspiration Heavily inspired from [ani-cli](https://github.com/pystardust/
 ani-cli)
                                                                   (back_to_top)
```

