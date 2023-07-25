# Comparing `tmp/shootpandora-Cloud-1.2.9.tar.gz` & `tmp/shootpandora-Cloud-20230725.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootpandora-Cloud-1.2.9.tar", last modified: Tue Jul 25 04:09:10 2023, max compression
+gzip compressed data, was "shootpandora-Cloud-20230725.1.1.tar", last modified: Tue Jul 25 06:00:42 2023, max compression
```

## Comparing `shootpandora-Cloud-1.2.9.tar` & `shootpandora-Cloud-20230725.1.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.768220 shootpandora-Cloud-1.2.9/
--rw-rw-rw-   0        0        0    18092 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/LICENSE
--rw-rw-rw-   0        0        0       89 2023-07-25 02:29:01.000000 shootpandora-Cloud-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2306 2023-07-25 04:09:10.769235 shootpandora-Cloud-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-07-25 02:30:59.000000 shootpandora-Cloud-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 04:09:10.770222 shootpandora-Cloud-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1837 2023-07-25 02:30:59.000000 shootpandora-Cloud-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.202218 shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/
--rw-rw-rw-   0        0        0     2306 2023-07-25 04:09:09.000000 shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7643 2023-07-25 04:09:09.000000 shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:09:09.000000 shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-25 04:09:09.000000 shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.111217 shootpandora-Cloud-1.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.213216 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/
--rw-rw-rw-   0        0        0       47 2023-07-25 04:08:13.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.165217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.232215 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.119217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.147215 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.322219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/
--rw-rw-rw-   0        0        0    69737 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-rw-rw-   0        0        0   262802 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-rw-rw-   0        0        0    74170 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
--rw-rw-rw-   0        0        0    29389 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
--rw-rw-rw-   0        0        0      657 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
--rw-rw-rw-   0        0        0    23052 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
--rw-rw-rw-   0        0        0   417248 2023-07-25 02:30:59.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
--rw-rw-rw-   0        0        0   248252 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
--rw-rw-rw-   0        0        0    16805 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
--rw-rw-rw-   0        0        0     3092 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
--rw-rw-rw-   0        0        0  1085662 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
--rw-rw-rw-   0        0        0     8750 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
--rw-rw-rw-   0        0        0    26962 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
--rw-rw-rw-   0        0        0     1044 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
--rw-rw-rw-   0        0        0   141071 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-rw-rw-   0        0        0   121704 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.348219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.362232 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
--rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
--rw-rw-rw-   0        0        0     2755 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
--rw-rw-rw-   0        0        0    21936 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.130219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.135217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.365214 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
--rw-rw-rw-   0        0        0     1344 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
--rw-rw-rw-   0        0        0   987027 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.391217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-rw-rw-   0        0        0     3189 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
--rw-rw-rw-   0        0        0      661 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
--rw-rw-rw-   0        0        0      611 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
--rw-rw-rw-   0        0        0     5527 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
--rw-rw-rw-   0        0        0     1069 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
--rw-rw-rw-   0        0        0      596 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
--rw-rw-rw-   0        0        0      488 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.396218 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-rw-rw-   0        0        0     5629 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
--rw-rw-rw-   0        0        0      250 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
--rw-rw-rw-   0        0        0     5414 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.399219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-rw-rw-   0        0        0    20064 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.404219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-rw-rw-   0        0        0     7543 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
--rw-rw-rw-   0        0        0      399 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
--rw-rw-rw-   0        0        0    91460 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-rw-rw-   0        0        0     4976 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.406214 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/css/
--rw-rw-rw-   0        0        0   138266 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.417219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
--rw-rw-rw-   0        0        0     2375 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
--rw-rw-rw-   0        0        0       77 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
--rw-rw-rw-   0        0        0     4159 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/apple-touch-icon.png
--rw-rw-rw-   0        0        0      730 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/favicon-16x16.png
--rw-rw-rw-   0        0        0     1292 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/favicon-32x32.png
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.155226 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.449220 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/
--rw-rw-rw-   0        0        0    34336 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-rw-rw-   0        0        0    27412 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-rw-rw-   0        0        0    35956 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-rw-rw-   0        0        0    28532 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-rw-rw-   0        0        0    35268 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-rw-rw-   0        0        0    28060 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-rw-rw-   0        0        0    37480 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-rw-rw-   0        0        0    29824 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.641221 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/
--rw-rw-rw-   0        0        0    28076 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-rw-rw-   0        0        0     6912 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-rw-rw-   0        0        0     6908 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-rw-rw-   0        0        0    11348 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-rw-rw-   0        0        0    11316 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-rw-rw-   0        0        0    25324 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-rw-rw-   0        0        0    16780 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-rw-rw-   0        0        0    16988 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-rw-rw-   0        0        0    26272 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-rw-rw-   0        0        0    16400 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-rw-rw-   0        0        0    16440 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-rw-rw-   0        0        0    12216 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-rw-rw-   0        0        0    12028 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-rw-rw-   0        0        0    10344 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-rw-rw-   0        0        0     9644 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-rw-rw-   0        0        0     5468 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-rw-rw-   0        0        0     5208 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-rw-rw-   0        0        0     3624 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-rw-rw-   0        0        0     4928 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-rw-rw-   0        0        0    13568 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.675216 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/
--rw-rw-rw-   0        0        0    56682 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-rw-rw-   0        0        0    56021 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-rw-rw-   0        0        0    56456 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-rw-rw-   0        0        0    53009 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.729217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/
--rw-rw-rw-   0        0        0    34084 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-rw-rw-   0        0        0    33350 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-rw-rw-   0        0        0    40456 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-rw-rw-   0        0        0    37996 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-rw-rw-   0        0        0    38746 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-rw-rw-   0        0        0    35690 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-rw-rw-   0        0        0    28148 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-rw-rw-   0        0        0    27437 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-rw-rw-   0        0        0    28285 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
--rw-rw-rw-   0        0        0      336 2023-07-25 02:29:01.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/manifest.json
--rw-rw-rw-   0        0        0     6133 2023-07-25 02:29:01.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.738218 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/sweetalert2/
--rw-rw-rw-   0        0        0    19844 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css
--rw-rw-rw-   0        0        0    68840 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.160218 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.162219 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/react-components/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.163220 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.742217 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-rw-rw-   0        0        0   233073 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxrwxrwx   0        0        0        0 2023-07-25 04:09:10.764216 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/
--rw-rw-rw-   0        0        0     4586 2023-07-25 04:03:54.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/404.html
--rw-rw-rw-   0        0        0     7119 2023-07-25 04:05:11.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/chat.html
--rw-rw-rw-   0        0        0     4465 2023-07-25 03:51:23.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/detail.html
--rw-rw-rw-   0        0        0    40079 2023-07-25 03:57:25.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/login.html
--rw-rw-rw-   0        0        0     5733 2023-07-25 03:51:58.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/share.html
--rw-rw-rw-   0        0        0        0 2023-07-21 02:59:44.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/py.typed
--rw-rw-rw-   0        0        0    19767 2023-07-25 02:29:01.000000 shootpandora-Cloud-1.2.9/src/shootpandora_cloud/server.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:42.002435 shootpandora-Cloud-20230725.1.1/
+-rw-rw-rw-   0        0        0    18092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2313 2023-07-25 06:00:42.002435 shootpandora-Cloud-20230725.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:00:42.005441 shootpandora-Cloud-20230725.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1837 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.402436 shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/
+-rw-rw-rw-   0        0        0     2313 2023-07-25 06:00:40.000000 shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7643 2023-07-25 06:00:41.000000 shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:00:40.000000 shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 06:00:40.000000 shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.271431 shootpandora-Cloud-20230725.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.416433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/
+-rw-rw-rw-   0        0        0       54 2023-07-25 06:00:18.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.353433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.438434 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.302436 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.338434 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.543434 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/
+-rw-rw-rw-   0        0        0    69737 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-rw-rw-   0        0        0   262802 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-rw-rw-   0        0        0    74170 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
+-rw-rw-rw-   0        0        0    29389 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
+-rw-rw-rw-   0        0        0      657 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
+-rw-rw-rw-   0        0        0    23052 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
+-rw-rw-rw-   0        0        0   417248 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
+-rw-rw-rw-   0        0        0   248252 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
+-rw-rw-rw-   0        0        0    16805 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
+-rw-rw-rw-   0        0        0     3092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
+-rw-rw-rw-   0        0        0  1085662 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
+-rw-rw-rw-   0        0        0     8750 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
+-rw-rw-rw-   0        0        0    26962 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
+-rw-rw-rw-   0        0        0     1044 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
+-rw-rw-rw-   0        0        0   141071 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-rw-rw-   0        0        0   121704 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.574432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.597439 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
+-rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
+-rw-rw-rw-   0        0        0     2755 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
+-rw-rw-rw-   0        0        0    21936 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.328433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.329431 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.601435 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
+-rw-rw-rw-   0        0        0     1344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
+-rw-rw-rw-   0        0        0   987027 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.630432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-rw-rw-   0        0        0     3189 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
+-rw-rw-rw-   0        0        0      661 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
+-rw-rw-rw-   0        0        0      611 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
+-rw-rw-rw-   0        0        0     5527 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
+-rw-rw-rw-   0        0        0     1069 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
+-rw-rw-rw-   0        0        0      596 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
+-rw-rw-rw-   0        0        0      488 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.636431 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-rw-rw-   0        0        0     5629 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
+-rw-rw-rw-   0        0        0      250 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
+-rw-rw-rw-   0        0        0     5414 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.641433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-rw-rw-   0        0        0    20064 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.649439 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-rw-rw-   0        0        0     7543 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
+-rw-rw-rw-   0        0        0      399 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
+-rw-rw-rw-   0        0        0    91460 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-rw-rw-   0        0        0     4976 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.653433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/css/
+-rw-rw-rw-   0        0        0   138266 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.666432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
+-rw-rw-rw-   0        0        0     2375 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
+-rw-rw-rw-   0        0        0       77 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
+-rw-rw-rw-   0        0        0     4159 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      730 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1292 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/favicon-32x32.png
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.346433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.718434 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/
+-rw-rw-rw-   0        0        0    34336 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-rw-rw-   0        0        0    27412 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-rw-rw-   0        0        0    35956 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-rw-rw-   0        0        0    28532 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-rw-rw-   0        0        0    35268 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-rw-rw-   0        0        0    28060 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-rw-rw-   0        0        0    37480 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-rw-rw-   0        0        0    29824 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.837432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/
+-rw-rw-rw-   0        0        0    28076 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-rw-rw-   0        0        0     6912 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-rw-rw-   0        0        0     6908 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-rw-rw-   0        0        0    11348 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-rw-rw-   0        0        0    11316 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-rw-rw-   0        0        0    25324 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-rw-rw-   0        0        0    16780 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-rw-rw-   0        0        0    16988 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-rw-rw-   0        0        0    26272 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-rw-rw-   0        0        0    16400 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-rw-rw-   0        0        0    16440 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-rw-rw-   0        0        0    12216 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-rw-rw-   0        0        0    12028 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-rw-rw-   0        0        0    10344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-rw-rw-   0        0        0     9644 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-rw-rw-   0        0        0     5468 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-rw-rw-   0        0        0     5208 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-rw-rw-   0        0        0     3624 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-rw-rw-   0        0        0     4928 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-rw-rw-   0        0        0    13568 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.855432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/
+-rw-rw-rw-   0        0        0    56682 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-rw-rw-   0        0        0    56021 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-rw-rw-   0        0        0    56456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-rw-rw-   0        0        0    53009 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.924432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/
+-rw-rw-rw-   0        0        0    34084 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-rw-rw-   0        0        0    33350 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-rw-rw-   0        0        0    40456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-rw-rw-   0        0        0    37996 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-rw-rw-   0        0        0    38746 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-rw-rw-   0        0        0    35690 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-rw-rw-   0        0        0    28148 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-rw-rw-   0        0        0    27437 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-rw-rw-   0        0        0    28285 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/manifest.json
+-rw-rw-rw-   0        0        0     6133 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.967432 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/sweetalert2/
+-rw-rw-rw-   0        0        0    19844 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css
+-rw-rw-rw-   0        0        0    68840 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.350433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.351431 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/react-components/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.352437 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.972433 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-rw-rw-   0        0        0   233073 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxrwxrwx   0        0        0        0 2023-07-25 06:00:41.999436 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/
+-rw-rw-rw-   0        0        0     4586 2023-07-25 04:03:54.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/404.html
+-rw-rw-rw-   0        0        0     7119 2023-07-25 04:05:11.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/chat.html
+-rw-rw-rw-   0        0        0     4465 2023-07-25 03:51:23.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/detail.html
+-rw-rw-rw-   0        0        0    40079 2023-07-25 03:57:25.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/login.html
+-rw-rw-rw-   0        0        0     5733 2023-07-25 03:51:58.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/share.html
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/py.typed
+-rw-rw-rw-   0        0        0    19767 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/server.py
```

### Comparing `shootpandora-Cloud-1.2.9/LICENSE` & `shootpandora-Cloud-20230725.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/PKG-INFO` & `shootpandora-Cloud-20230725.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-Cloud
-Version: 1.2.9
+Version: 20230725.1.1
 Summary: A package for shootpandora-ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora-cloud
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora-cloud
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `shootpandora-Cloud-1.2.9/README.md` & `shootpandora-Cloud-20230725.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/setup.py` & `shootpandora-Cloud-20230725.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/PKG-INFO` & `shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-Cloud
-Version: 1.2.9
+Version: 20230725.1.1
 Summary: A package for shootpandora-ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora-cloud
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora-cloud
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `shootpandora-Cloud-1.2.9/shootpandora_Cloud.egg-info/SOURCES.txt` & `shootpandora-Cloud-20230725.1.1/shootpandora_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/apple-touch-icon.png` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/favicon-16x16.png` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/favicon-32x32.png` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/service-worker.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/404.html` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/404.html`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/chat.html` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/detail.html` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/login.html` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/flask/templates/share.html` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/flask/templates/share.html`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-1.2.9/src/shootpandora_cloud/server.py` & `shootpandora-Cloud-20230725.1.1/src/shootpandora_cloud/server.py`

 * *Files identical despite different names*

