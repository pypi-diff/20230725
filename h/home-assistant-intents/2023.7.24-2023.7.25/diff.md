# Comparing `tmp/home-assistant-intents-2023.7.24.tar.gz` & `tmp/home-assistant-intents-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.7.24.tar", last modified: Mon Jul 24 20:16:32 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.7.25.tar", last modified: Tue Jul 25 19:39:29 2023, max compression
```

## Comparing `home-assistant-intents-2023.7.24.tar` & `home-assistant-intents-2023.7.25.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.7.24/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.7.24/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2023.7.24/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.7.24/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.239743 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54168 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36159 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    57384 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      975 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/et.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6147 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/eu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17116 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15293 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    59543 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    60255 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    75862 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1760 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2318 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-07-24 20:16:27.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/eu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3252 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3222 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1914 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:28.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1642 2023-07-24 20:16:29.000000 home-assistant-intents-2023.7.24/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 20:16:32.235743 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-24 20:16:31.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5395 2023-07-24 20:16:32.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 20:16:31.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-24 20:16:32.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1036 2023-07-24 20:14:44.000000 home-assistant-intents-2023.7.24/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-24 20:16:32.243744 home-assistant-intents-2023.7.24/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.489218 home-assistant-intents-2023.7.25/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.7.25/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.7.25/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-25 19:39:29.489218 home-assistant-intents-2023.7.25/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2023.7.25/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.481218 home-assistant-intents-2023.7.25/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.7.25/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.481218 home-assistant-intents-2023.7.25/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.485218 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54106 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36159 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    57442 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      975 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/et.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6147 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/eu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17116 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15293 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    59543 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    60255 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    75862 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1760 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11970 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.489218 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-07-25 19:39:24.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2318 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/eu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3252 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3222 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1914 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.489218 home-assistant-intents-2023.7.25/home_assistant_intents/data/shopping_list/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      557 2023-07-25 19:39:25.000000 home-assistant-intents-2023.7.25/home_assistant_intents/data/shopping_list/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1671 2023-07-25 19:39:26.000000 home-assistant-intents-2023.7.25/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 19:39:29.485218 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1287 2023-07-25 19:39:29.000000 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5445 2023-07-25 19:39:29.000000 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-25 19:39:29.000000 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-25 19:39:29.000000 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1036 2023-07-25 19:38:19.000000 home-assistant-intents-2023.7.25/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-25 19:39:29.489218 home-assistant-intents-2023.7.25/setup.cfg
```

### Comparing `home-assistant-intents-2023.7.24/LICENSE.md` & `home-assistant-intents-2023.7.25/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/PKG-INFO` & `home-assistant-intents-2023.7.25/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.7.24
+Version: 2023.7.25
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.7.24/README.md` & `home-assistant-intents-2023.7.25/README.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.7.25/home_assistant_intents/__init__.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/bg.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999903549382716%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {7: {'slots': {delete: ['area']}}}}, 'HassTurnOn': "*

 * *              "{'data': {3: {'slots': {delete: ['area']}}}}}"}*

```diff
@@ -773,15 +773,14 @@
                 {
                     "response": "cover_area",
                     "sentences": [
                         "<close> [<all>] <covers> <area>",
                         "<close>  <area> [<all>] <covers>"
                     ],
                     "slots": {
-                        "area": "bedroom",
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
@@ -823,15 +822,14 @@
                 {
                     "response": "cover_area",
                     "sentences": [
                         "<open> [<all>] <covers> <area>",
                         "<open> <area> [<all>] <covers>"
                     ],
                     "slots": {
-                        "area": "bedroom",
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978070175438596%*

 * *Differences: {"'lists'": "{'shopping_list_item': OrderedDict([('wildcard', True)])}"}*

```diff
@@ -2101,14 +2101,17 @@
                 },
                 {
                     "in": "off",
                     "out": "off"
                 }
             ]
         },
+        "shopping_list_item": {
+            "wildcard": true
+        },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/et.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/et.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/eu.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/eu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ko.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ko.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/vi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997519841269842%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {0: {'slots': {delete: ['name']}}}}, 'HassTurnOn': "*

 * *              "{'data': {3: {'slots': {delete: ['name']}}}}}"}*

```diff
@@ -112,16 +112,15 @@
                 {
                     "sentences": [
                         "t\u1eaft <name> <area>",
                         "t\u1eaft <name> [trong]  <area>",
                         "t\u1eaft [t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] <name> [trong] <area>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "fan"
                     }
                 },
                 {
                     "sentences": [
                         "t\u1eaft <name>"
                     ]
                 },
@@ -204,16 +203,15 @@
                 },
                 {
                     "sentences": [
                         "b\u1eadt <name> <area>",
                         "b\u1eadt [h\u1ebft | t\u1ea5t c\u1ea3 | to\u00e0n b\u1ed9] <name> <area>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "fan"
                     }
                 },
                 {
                     "sentences": [
                         "b\u1eadt <name>"
                     ]
                 },
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/he.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555555%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {1: {delete: ['slots']}}}}"}*

```diff
@@ -12,18 +12,15 @@
                 },
                 {
                     "response": "brightness_area",
                     "sentences": [
                         "\u05e7\u05d1\u05e2 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
                         "\u05e9\u05e0\u05d4 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
                         "\u05d4\u05d2\u05d3\u05e8 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>"
-                    ],
-                    "slots": {
-                        "name": "all"
-                    }
+                    ]
                 }
             ]
         }
     },
     "language": "he",
     "responses": {
         "intents": {
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/is.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ko.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ko.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.7.25/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents/domains.py` & `home-assistant-intents-2023.7.25/home_assistant_intents/domains.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,8 +108,9 @@
         "uk",
         "ur",
         "vi",
         "zh-cn",
         "zh-hk",
         "zh-tw",
     ],
+    "shopping_list": ["en"],
 }
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.7.24
+Version: 2023.7.25
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.7.24/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.7.25/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,9 @@
 home_assistant_intents/data/light/te.json
 home_assistant_intents/data/light/tr.json
 home_assistant_intents/data/light/uk.json
 home_assistant_intents/data/light/ur.json
 home_assistant_intents/data/light/vi.json
 home_assistant_intents/data/light/zh-cn.json
 home_assistant_intents/data/light/zh-hk.json
-home_assistant_intents/data/light/zh-tw.json
+home_assistant_intents/data/light/zh-tw.json
+home_assistant_intents/data/shopping_list/en.json
```

### Comparing `home-assistant-intents-2023.7.24/pyproject.toml` & `home-assistant-intents-2023.7.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.7.24"
+version     = "2023.7.25"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

