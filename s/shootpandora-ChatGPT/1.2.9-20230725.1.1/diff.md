# Comparing `tmp/shootpandora-ChatGPT-1.2.9.tar.gz` & `tmp/shootpandora-ChatGPT-20230725.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootpandora-ChatGPT-1.2.9.tar", last modified: Tue Jul 25 04:09:18 2023, max compression
+gzip compressed data, was "shootpandora-ChatGPT-20230725.1.1.tar", last modified: Tue Jul 25 06:00:48 2023, max compression
```

## Comparing `shootpandora-ChatGPT-1.2.9.tar` & `shootpandora-ChatGPT-20230725.1.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.456402 shootpandora-ChatGPT-1.2.9/
--rw-rw-rw-   0        0        0    18431 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/LICENSE
--rw-rw-rw-   0        0        0      192 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     7055 2023-07-25 04:09:18.455404 shootpandora-ChatGPT-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5472 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-1.2.9/README.md
--rw-rw-rw-   0        0        0      288 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/requirements.txt
--rw-rw-rw-   0        0        0       70 2023-07-25 04:08:05.000000 shootpandora-ChatGPT-1.2.9/requirements_api.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 04:09:18.456402 shootpandora-ChatGPT-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2540 2023-07-25 04:08:05.000000 shootpandora-ChatGPT-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.034400 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/
--rw-rw-rw-   0        0        0     7055 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4634 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      386 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 04:09:17.000000 shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.949404 shootpandora-ChatGPT-1.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.069402 shootpandora-ChatGPT-1.2.9/src/shootpandora/
--rw-rw-rw-   0        0        0       50 2023-07-25 04:08:05.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/__init__.py
--rw-rw-rw-   0        0        0      112 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.083401 shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/__init__.py
--rw-rw-rw-   0        0        0    17946 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/legacy.py
--rw-rw-rw-   0        0        0    10683 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/server.py
--rw-rw-rw-   0        0        0     2232 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/cloud_launcher.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.111401 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/__init__.py
--rw-rw-rw-   0        0        0      540 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/config.py
--rw-rw-rw-   0        0        0      968 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/hooks.py
--rw-rw-rw-   0        0        0      502 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/sentry.py
--rw-rw-rw-   0        0        0     1841 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/token.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.975399 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.128404 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.957402 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.963400 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.222400 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/
--rw-rw-rw-   0        0        0   905465 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-rw-rw-   0        0        0    14115 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-rw-rw-   0        0        0     9531 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-rw-rw-   0        0        0   264961 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-rw-rw-   0        0        0    13157 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-rw-rw-   0        0        0    24146 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-rw-rw-   0        0        0    20480 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-rw-rw-   0        0        0     3232 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-rw-rw-   0        0        0      389 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-rw-rw-   0        0        0    11682 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-rw-rw-   0        0        0     2433 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-rw-rw-   0        0        0      462 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-rw-rw-   0        0        0   141402 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-rw-rw-   0        0        0   105264 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.236396 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/
--rw-rw-rw-   0        0        0   305775 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-rw-rw-   0        0        0      250 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.245403 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/chat/
--rw-rw-rw-   0        0        0   149542 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-rw-rw-   0        0        0    91461 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-rw-rw-   0        0        0     3926 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.256402 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/css/
--rw-rw-rw-   0        0        0   108647 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.268401 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-rw-rw-   0        0        0     2308 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-rw-rw-   0        0        0       77 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-rw-rw-   0        0        0     4159 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/apple-touch-icon.png
--rw-rw-rw-   0        0        0      730 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/favicon-16x16.png
--rw-rw-rw-   0        0        0     1292 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/favicon-32x32.png
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.385398 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/
--rw-rw-rw-   0        0        0     7716 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-rw-rw-   0        0        0     7656 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-rw-rw-   0        0        0    13296 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-rw-rw-   0        0        0    13208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-rw-rw-   0        0        0    29912 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-rw-rw-   0        0        0    19412 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-rw-rw-   0        0        0    19676 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-rw-rw-   0        0        0    30772 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-rw-rw-   0        0        0    18668 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-rw-rw-   0        0        0    18748 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-rw-rw-   0        0        0    14408 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-rw-rw-   0        0        0    14112 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-rw-rw-   0        0        0    12316 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-rw-rw-   0        0        0    10588 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-rw-rw-   0        0        0     6496 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-rw-rw-   0        0        0     6188 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-rw-rw-   0        0        0     4420 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-rw-rw-   0        0        0     5980 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-rw-rw-   0        0        0    16028 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-rw-rw-   0        0        0   324208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Signifier-Regular.otf
--rw-rw-rw-   0        0        0   210840 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Sohne-Buch.otf
--rw-rw-rw-   0        0        0   230012 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-rw-rw-   0        0        0    30824 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf
--rw-rw-rw-   0        0        0    31116 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.970400 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/images/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:17.973398 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/images/2022/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.388401 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/images/2022/11/
--rw-rw-rw-   0        0        0     1714 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.395403 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/templates/
--rw-rw-rw-   0        0        0     8752 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/templates/chat.html
--rw-rw-rw-   0        0        0     7540 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/launcher.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.411400 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/__init__.py
--rw-rw-rw-   0        0        0      262 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/database.py
--rw-rw-rw-   0        0        0      640 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/migrate.py
--rw-rw-rw-   0        0        0     4293 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/models.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.415397 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/scripts/
--rw-rw-rw-   0        0        0      904 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.436401 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/__init__.py
--rw-rw-rw-   0        0        0    12076 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/api.py
--rw-rw-rw-   0        0        0     9090 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/auth.py
--rw-rw-rw-   0        0        0      439 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/token.py
--rw-rw-rw-   0        0        0     3532 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/utils.py
--rw-rw-rw-   0        0        0        0 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:18.451400 shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/base.py
--rw-rw-rw-   0        0        0    12819 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/chat.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.406514 shootpandora-ChatGPT-20230725.1.1/
+-rw-rw-rw-   0        0        0    18431 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/LICENSE
+-rw-rw-rw-   0        0        0      192 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7062 2023-07-25 06:00:48.403511 shootpandora-ChatGPT-20230725.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5472 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.1/README.md
+-rw-rw-rw-   0        0        0      288 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       77 2023-07-25 06:00:05.000000 shootpandora-ChatGPT-20230725.1.1/requirements_api.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:00:48.407511 shootpandora-ChatGPT-20230725.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2547 2023-07-25 06:00:05.000000 shootpandora-ChatGPT-20230725.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.996511 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/
+-rw-rw-rw-   0        0        0     7062 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4634 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      400 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 06:00:47.000000 shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.906511 shootpandora-ChatGPT-20230725.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.019513 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/
+-rw-rw-rw-   0        0        0       57 2023-07-25 06:00:05.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.034511 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/__init__.py
+-rw-rw-rw-   0        0        0    17946 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/legacy.py
+-rw-rw-rw-   0        0        0    10683 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/server.py
+-rw-rw-rw-   0        0        0     2232 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/cloud_launcher.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.060512 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/__init__.py
+-rw-rw-rw-   0        0        0      540 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/config.py
+-rw-rw-rw-   0        0        0      968 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/hooks.py
+-rw-rw-rw-   0        0        0      502 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/sentry.py
+-rw-rw-rw-   0        0        0     1841 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/token.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.932509 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.075510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.914510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.922510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.165516 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/
+-rw-rw-rw-   0        0        0   905465 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-rw-rw-   0        0        0    14115 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-rw-rw-   0        0        0     9531 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-rw-rw-   0        0        0   264961 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-rw-rw-   0        0        0    13157 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-rw-rw-   0        0        0    24146 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-rw-rw-   0        0        0    20480 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-rw-rw-   0        0        0     3232 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-rw-rw-   0        0        0      389 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-rw-rw-   0        0        0    11682 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-rw-rw-   0        0        0     2433 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-rw-rw-   0        0        0      462 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-rw-rw-   0        0        0   141402 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-rw-rw-   0        0        0   105264 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.175511 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/
+-rw-rw-rw-   0        0        0   305775 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-rw-rw-   0        0        0      250 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.179513 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/chat/
+-rw-rw-rw-   0        0        0   149542 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-rw-rw-   0        0        0    91461 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-rw-rw-   0        0        0     3926 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.188539 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/css/
+-rw-rw-rw-   0        0        0   108647 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.201512 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-rw-rw-   0        0        0     2308 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-rw-rw-   0        0        0       77 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-rw-rw-   0        0        0     4159 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      730 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1292 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/favicon-32x32.png
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.334510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/
+-rw-rw-rw-   0        0        0     7716 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-rw-rw-   0        0        0     7656 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-rw-rw-   0        0        0    13296 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-rw-rw-   0        0        0    13208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-rw-rw-   0        0        0    29912 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-rw-rw-   0        0        0    19412 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-rw-rw-   0        0        0    19676 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-rw-rw-   0        0        0    30772 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-rw-rw-   0        0        0    18668 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-rw-rw-   0        0        0    18748 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-rw-rw-   0        0        0    14408 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-rw-rw-   0        0        0    14112 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-rw-rw-   0        0        0    12316 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-rw-rw-   0        0        0    10588 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-rw-rw-   0        0        0     6496 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-rw-rw-   0        0        0     6188 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-rw-rw-   0        0        0     4420 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-rw-rw-   0        0        0     5980 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-rw-rw-   0        0        0    16028 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-rw-rw-   0        0        0   324208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Signifier-Regular.otf
+-rw-rw-rw-   0        0        0   210840 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Sohne-Buch.otf
+-rw-rw-rw-   0        0        0   230012 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-rw-rw-   0        0        0    30824 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-rw-rw-   0        0        0    31116 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.928513 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/images/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:47.930510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/images/2022/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.339510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/images/2022/11/
+-rw-rw-rw-   0        0        0     1714 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.345512 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/templates/
+-rw-rw-rw-   0        0        0     8752 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/templates/chat.html
+-rw-rw-rw-   0        0        0     7540 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/launcher.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.361512 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/database.py
+-rw-rw-rw-   0        0        0      640 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/migrate.py
+-rw-rw-rw-   0        0        0     4293 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/models.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.365510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/scripts/
+-rw-rw-rw-   0        0        0      904 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.385511 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/__init__.py
+-rw-rw-rw-   0        0        0    12076 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/api.py
+-rw-rw-rw-   0        0        0     9090 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/auth.py
+-rw-rw-rw-   0        0        0      439 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/token.py
+-rw-rw-rw-   0        0        0     3532 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/utils.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:48.399510 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/base.py
+-rw-rw-rw-   0        0        0    12819 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/chat.py
```

### Comparing `shootpandora-ChatGPT-1.2.9/LICENSE` & `shootpandora-ChatGPT-20230725.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/PKG-INFO` & `shootpandora-ChatGPT-20230725.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-ChatGPT
-Version: 1.2.9
+Version: 20230725.1.1
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 1.2.9 Summary: A
-command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
+Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.1 Summary:
+A command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
 shootpandora Author: XiaoZhou Huang Author-email: shoot82003@qq.com Project-
 URL: Source, https://github.com/shoot82003/shootpandora Project-URL: Tracker,
 https://github.com/shoot82003/shootpandora/issues Keywords: OpenAI ChatGPT
 ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301 Classifier: Development Status ::
 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Web Environment Classifier: Framework :: Flask Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
```

### Comparing `shootpandora-ChatGPT-1.2.9/README.md` & `shootpandora-ChatGPT-20230725.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/setup.py` & `shootpandora-ChatGPT-20230725.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/shoot82003/shootpandora',
     packages=find_packages('src'),
     package_dir={'shootpandora': 'src/shootpandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['shootpandora-cloud~=1.2.9'],
+        'cloud': ['shootpandora-cloud~=20230725.1.1'],
     },
     entry_points={
         'console_scripts': [
             'shootpandora = shootpandora.launcher:run',
             'shootpandora-cloud = shootpandora.cloud_launcher:run',
         ]
     },
```

### Comparing `shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/PKG-INFO` & `shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-ChatGPT
-Version: 1.2.9
+Version: 20230725.1.1
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 1.2.9 Summary: A
-command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
+Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.1 Summary:
+A command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
 shootpandora Author: XiaoZhou Huang Author-email: shoot82003@qq.com Project-
 URL: Source, https://github.com/shoot82003/shootpandora Project-URL: Tracker,
 https://github.com/shoot82003/shootpandora/issues Keywords: OpenAI ChatGPT
 ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301 Classifier: Development Status ::
 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Web Environment Classifier: Framework :: Flask Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
```

### Comparing `shootpandora-ChatGPT-1.2.9/shootpandora_ChatGPT.egg-info/SOURCES.txt` & `shootpandora-ChatGPT-20230725.1.1/shootpandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/legacy.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/bots/server.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/cloud_launcher.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/config.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/config.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/hooks.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/exts/token.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/apple-touch-icon.png` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/favicon-16x16.png` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/favicon-32x32.png` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Signifier-Regular.otf` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Sohne-Buch.otf` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/flask/templates/chat.html` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/launcher.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/launcher.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/migrate.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/models.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/api.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/api.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/auth.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/auth.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/openai/utils.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/base.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-1.2.9/src/shootpandora/turbo/chat.py` & `shootpandora-ChatGPT-20230725.1.1/src/shootpandora/turbo/chat.py`

 * *Files identical despite different names*

