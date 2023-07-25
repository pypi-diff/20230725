# Comparing `tmp/weditor-0.6.8.tar.gz` & `tmp/weditor-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weditor-0.6.8.tar", last modified: Mon Apr  3 10:01:27 2023, max compression
+gzip compressed data, was "weditor-0.7.0.tar", last modified: Tue Jul 25 09:39:12 2023, max compression
```

## Comparing `weditor-0.6.8.tar` & `weditor-0.7.0.tar`

### file list

```diff
@@ -1,139 +1,143 @@
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.082679 weditor-0.6.8/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.946498 weditor-0.6.8/.github/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.995065 weditor-0.6.8/.github/workflows/
--rw-r--r--   0 shengxiang   (501) staff       (20)      937 2023-03-30 09:12:40.000000 weditor-0.6.8/.github/workflows/publish-to-pypi.yml
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.995898 weditor-0.6.8/.vscode/
--rw-r--r--   0 shengxiang   (501) staff       (20)       98 2023-03-30 09:02:43.000000 weditor-0.6.8/.vscode/settings.json
--rw-r--r--   0 shengxiang   (501) staff       (20)       52 2021-03-23 07:56:26.000000 weditor-0.6.8/ABOUT.rst
--rw-r--r--   0 shengxiang   (501) staff       (20)     2710 2021-03-23 07:56:26.000000 weditor-0.6.8/API.md
--rw-r--r--   0 shengxiang   (501) staff       (20)   966854 2021-03-23 07:56:26.000000 weditor-0.6.8/CHANGELOG.docx
--rw-r--r--   0 shengxiang   (501) staff       (20)     1361 2021-05-18 05:52:50.000000 weditor-0.6.8/DEVELOP.md
--rw-r--r--   0 shengxiang   (501) staff       (20)     1079 2021-03-23 07:56:26.000000 weditor-0.6.8/LICENSE
--rw-r--r--   0 shengxiang   (501) staff       (20)     2715 2023-04-03 10:01:27.082928 weditor-0.6.8/PKG-INFO
--rw-r--r--   0 shengxiang   (501) staff       (20)     1711 2021-03-23 07:56:26.000000 weditor-0.6.8/README.md
--rw-r--r--   0 shengxiang   (501) staff       (20)     1699 2021-03-23 07:56:26.000000 weditor-0.6.8/README_ZH.md
--rw-r--r--   0 shengxiang   (501) staff       (20)        6 2023-03-30 09:11:27.000000 weditor-0.6.8/dev-requirements.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)     1895 2021-03-23 07:56:26.000000 weditor-0.6.8/log.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)      150 2021-03-23 07:56:26.000000 weditor-0.6.8/requirements.txt
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.000568 weditor-0.6.8/samples/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.009141 weditor-0.6.8/samples/ace/
--rw-r--r--   0 shengxiang   (501) staff       (20)   644638 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/ace/ace.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    67635 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/ace/ext-language_tools.js
--rw-r--r--   0 shengxiang   (501) staff       (20)   205106 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/ace/keybinding-vim.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     8671 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/ace/mode-python.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     2646 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/ace/theme-monokai.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    54822 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/bg.jpg
--rw-r--r--   0 shengxiang   (501) staff       (20)      319 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/bower.json
--rw-r--r--   0 shengxiang   (501) staff       (20)    23238 2021-03-23 07:56:26.000000 weditor-0.6.8/samples/index.html
--rw-r--r--   0 shengxiang   (501) staff       (20)   258966 2021-03-23 07:56:26.000000 weditor-0.6.8/screenshot.jpg
--rw-r--r--   0 shengxiang   (501) staff       (20)      488 2023-04-03 10:01:27.084051 weditor-0.6.8/setup.cfg
--rw-r--r--   0 shengxiang   (501) staff       (20)      159 2021-03-23 07:56:26.000000 weditor-0.6.8/setup.py
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.009660 weditor-0.6.8/tests/
--rw-r--r--   0 shengxiang   (501) staff       (20)      902 2023-03-30 09:19:00.000000 weditor-0.6.8/tests/test_web_utils.py
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.012187 weditor-0.6.8/weditor/
--rw-r--r--   0 shengxiang   (501) staff       (20)       65 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/__init__.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     8172 2021-05-18 05:52:50.000000 weditor-0.6.8/weditor/__main__.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     4771 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/page.xml
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.018067 weditor-0.6.8/weditor/static/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.021709 weditor-0.6.8/weditor/static/ace/
--rw-r--r--   0 shengxiang   (501) staff       (20)   644638 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/ace/ace.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    67635 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/ace/ext-language_tools.js
--rw-r--r--   0 shengxiang   (501) staff       (20)   205106 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/ace/keybinding-vim.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     8671 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/ace/mode-python.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     2646 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/ace/theme-monokai.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.974610 weditor-0.6.8/weditor/static/cdn_libraries/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.951718 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.950770 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.951470 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.024638 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/
--rw-r--r--   0 shengxiang   (501) staff       (20)   121200 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css
--rw-r--r--   0 shengxiang   (501) staff       (20)   542194 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.026905 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/
--rw-r--r--   0 shengxiang   (501) staff       (20)    18028 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.027437 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/
--rw-r--r--   0 shengxiang   (501) staff       (20)    37045 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.949769 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.950268 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.022185 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/
--rw-r--r--   0 shengxiang   (501) staff       (20)     6655 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.023133 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/
--rw-r--r--   0 shengxiang   (501) staff       (20)    39003 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map
--rw-r--r--   0 shengxiang   (501) staff       (20)    33963 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.028148 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.952127 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.032871 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/
--rw-r--r--   0 shengxiang   (501) staff       (20)   365464 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    39225 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    12001 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     8221 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     2977 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.952757 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.033308 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/
--rw-r--r--   0 shengxiang   (501) staff       (20)    86927 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.953321 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.034193 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/
--rw-r--r--   0 shengxiang   (501) staff       (20)   139314 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.974143 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.035665 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/
--rw-r--r--   0 shengxiang   (501) staff       (20)     5667 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png
--rw-r--r--   0 shengxiang   (501) staff       (20)    27281 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css
--rw-r--r--   0 shengxiang   (501) staff       (20)     1464 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif
--rw-r--r--   0 shengxiang   (501) staff       (20)    15076 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.036044 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.975158 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.036409 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/
--rw-r--r--   0 shengxiang   (501) staff       (20)   567194 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.037626 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.044229 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/
--rw-r--r--   0 shengxiang   (501) staff       (20)    28200 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff
--rw-r--r--   0 shengxiang   (501) staff       (20)   232432 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css
--rw-r--r--   0 shengxiang   (501) staff       (20)     8699 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0
--rw-r--r--   0 shengxiang   (501) staff       (20)    32138 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/favicon.ico
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.066323 weditor-0.6.8/weditor/static/js/
--rw-r--r--   0 shengxiang   (501) staff       (20)     2330 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/js/common.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    48120 2023-03-30 09:02:43.000000 weditor-0.6.8/weditor/static/js/index.js
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.977651 weditor-0.6.8/weditor/static/libs/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.066816 weditor-0.6.8/weditor/static/libs/css/
--rw-r--r--   0 shengxiang   (501) staff       (20)    80548 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/css/buttons.css
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:26.977360 weditor-0.6.8/weditor/static/libs/fontawesome/
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.068404 weditor-0.6.8/weditor/static/libs/fontawesome/css/
--rw-r--r--   0 shengxiang   (501) staff       (20)    37414 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.css
--rw-r--r--   0 shengxiang   (501) staff       (20)    21778 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.css.map
--rw-r--r--   0 shengxiang   (501) staff       (20)    31000 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.min.css
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.074056 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/
--rw-r--r--   0 shengxiang   (501) staff       (20)   134808 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/FontAwesome.otf
--rw-r--r--   0 shengxiang   (501) staff       (20)   165742 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 shengxiang   (501) staff       (20)   444379 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 shengxiang   (501) staff       (20)   165548 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 shengxiang   (501) staff       (20)    98024 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 shengxiang   (501) staff       (20)    77160 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.076399 weditor-0.6.8/weditor/static/libs/vue-2.5.16/
--rw-r--r--   0 shengxiang   (501) staff       (20)   289303 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/vue-2.5.16/vue.js
--rw-r--r--   0 shengxiang   (501) staff       (20)    86452 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/libs/vue-2.5.16/vue.min.js
--rw-r--r--   0 shengxiang   (501) staff       (20)     3062 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/loading.svg
--rw-r--r--   0 shengxiang   (501) staff       (20)     3060 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/running.svg
--rw-r--r--   0 shengxiang   (501) staff       (20)     3758 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/static/style.css
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.077902 weditor-0.6.8/weditor/templates/
--rw-r--r--   0 shengxiang   (501) staff       (20)    15105 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/templates/index.html
--rw-r--r--   0 shengxiang   (501) staff       (20)     2187 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/templates/widget_preview.html
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.080685 weditor-0.6.8/weditor/web/
--rw-r--r--   0 shengxiang   (501) staff       (20)        0 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/web/__init__.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     2782 2023-03-30 09:02:43.000000 weditor-0.6.8/weditor/web/device.py
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.082249 weditor-0.6.8/weditor/web/handlers/
--rw-r--r--   0 shengxiang   (501) staff       (20)        0 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/web/handlers/__init__.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     7075 2023-03-30 09:02:43.000000 weditor-0.6.8/weditor/web/handlers/page.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     2152 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/web/handlers/proxy.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     8174 2021-05-18 06:02:27.000000 weditor-0.6.8/weditor/web/handlers/shell.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     5136 2023-03-30 09:21:40.000000 weditor-0.6.8/weditor/web/ipyshell-console.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     7928 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/web/uidumplib.py
--rw-r--r--   0 shengxiang   (501) staff       (20)     1302 2023-03-30 09:20:49.000000 weditor-0.6.8/weditor/web/utils.py
--rw-r--r--   0 shengxiang   (501) staff       (20)      188 2021-03-23 07:56:26.000000 weditor-0.6.8/weditor/web/version.py
-drwxr-xr-x   0 shengxiang   (501) staff       (20)        0 2023-04-03 10:01:27.016058 weditor-0.6.8/weditor.egg-info/
--rw-r--r--   0 shengxiang   (501) staff       (20)     2715 2023-04-03 10:01:21.000000 weditor-0.6.8/weditor.egg-info/PKG-INFO
--rw-r--r--   0 shengxiang   (501) staff       (20)     4022 2023-04-03 10:01:26.000000 weditor-0.6.8/weditor.egg-info/SOURCES.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)        1 2023-04-03 10:01:21.000000 weditor-0.6.8/weditor.egg-info/dependency_links.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)       51 2023-04-03 10:01:21.000000 weditor-0.6.8/weditor.egg-info/entry_points.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)        1 2021-05-18 06:00:05.000000 weditor-0.6.8/weditor.egg-info/not-zip-safe
--rw-r--r--   0 shengxiang   (501) staff       (20)       47 2023-04-03 10:01:22.000000 weditor-0.6.8/weditor.egg-info/pbr.json
--rw-r--r--   0 shengxiang   (501) staff       (20)      127 2023-04-03 10:01:21.000000 weditor-0.6.8/weditor.egg-info/requires.txt
--rw-r--r--   0 shengxiang   (501) staff       (20)        8 2023-04-03 10:01:21.000000 weditor-0.6.8/weditor.egg-info/top_level.txt
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.538706 weditor-0.7.0/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.472561 weditor-0.7.0/.github/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.490811 weditor-0.7.0/.github/workflows/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      937 2023-07-23 14:15:35.000000 weditor-0.7.0/.github/workflows/publish-to-pypi.yml
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.491120 weditor-0.7.0/.vscode/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)       98 2021-09-26 02:51:25.000000 weditor-0.7.0/.vscode/settings.json
+-rw-r--r--   0 codeskyblue   (501) staff       (20)       52 2021-05-21 09:58:42.000000 weditor-0.7.0/ABOUT.rst
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2710 2021-05-21 09:58:42.000000 weditor-0.7.0/API.md
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      135 2023-07-25 09:39:12.000000 weditor-0.7.0/AUTHORS
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   966854 2021-05-21 09:58:42.000000 weditor-0.7.0/CHANGELOG.docx
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     4249 2023-07-25 09:39:11.000000 weditor-0.7.0/ChangeLog
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1361 2021-05-21 09:58:42.000000 weditor-0.7.0/DEVELOP.md
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1079 2021-05-21 09:58:42.000000 weditor-0.7.0/LICENSE
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2715 2023-07-25 09:39:12.538865 weditor-0.7.0/PKG-INFO
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1711 2021-05-21 09:58:42.000000 weditor-0.7.0/README.md
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1699 2021-05-21 09:58:42.000000 weditor-0.7.0/README_ZH.md
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        6 2023-07-23 14:15:35.000000 weditor-0.7.0/dev-requirements.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1895 2021-05-21 09:58:42.000000 weditor-0.7.0/log.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      150 2021-05-21 09:58:42.000000 weditor-0.7.0/requirements.txt
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.492379 weditor-0.7.0/samples/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.495918 weditor-0.7.0/samples/ace/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   644638 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/ace/ace.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    67635 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/ace/ext-language_tools.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   205106 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/ace/keybinding-vim.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8671 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/ace/mode-python.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2646 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/ace/theme-monokai.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    54822 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/bg.jpg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      319 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/bower.json
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    23238 2021-05-21 09:58:42.000000 weditor-0.7.0/samples/index.html
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   258966 2021-05-21 09:58:42.000000 weditor-0.7.0/screenshot.jpg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      488 2023-07-25 09:39:12.539296 weditor-0.7.0/setup.cfg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      159 2021-05-21 09:58:42.000000 weditor-0.7.0/setup.py
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.496895 weditor-0.7.0/tests/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      134 2023-07-23 14:31:50.000000 weditor-0.7.0/tests/test_proto.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      902 2023-07-23 14:15:35.000000 weditor-0.7.0/tests/test_web_utils.py
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.497672 weditor-0.7.0/weditor/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)       65 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/__init__.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8172 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/__main__.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     4771 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/page.xml
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.502318 weditor-0.7.0/weditor/static/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.507284 weditor-0.7.0/weditor/static/ace/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   644638 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/ace/ace.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    67635 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/ace/ext-language_tools.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   205106 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/ace/keybinding-vim.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8671 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/ace/mode-python.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2646 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/ace/theme-monokai.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.482827 weditor-0.7.0/weditor/static/cdn_libraries/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.479528 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.474148 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.475806 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.508702 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   121200 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   542194 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.509769 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    18028 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.510302 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    37045 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.473716 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.473949 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.507512 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     6655 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.508018 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    39003 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    33963 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.510553 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.480153 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.512840 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   365464 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    39225 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    12001 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8221 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2977 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.480520 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.513035 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    86927 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.481970 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.513360 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   139314 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.482644 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.514430 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     5667 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    27281 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1464 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    15076 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.514653 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.483060 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.514961 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   567194 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.515952 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.516439 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    28200 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   232432 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8699 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    32138 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/favicon.ico
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.516915 weditor-0.7.0/weditor/static/js/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2330 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/js/common.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    48120 2021-09-26 02:51:25.000000 weditor-0.7.0/weditor/static/js/index.js
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.484164 weditor-0.7.0/weditor/static/libs/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.517669 weditor-0.7.0/weditor/static/libs/css/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    80548 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/css/buttons.css
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.484039 weditor-0.7.0/weditor/static/libs/fontawesome/
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.519648 weditor-0.7.0/weditor/static/libs/fontawesome/css/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    37414 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.css
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    21778 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.css.map
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    31000 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.min.css
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.525142 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   134808 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/FontAwesome.otf
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   165742 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   444379 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   165548 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    98024 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    77160 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.534413 weditor-0.7.0/weditor/static/libs/vue-2.5.16/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)   289303 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/vue-2.5.16/vue.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    86452 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/libs/vue-2.5.16/vue.min.js
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     3062 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/loading.svg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     3060 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/running.svg
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     3758 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/static/style.css
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.535750 weditor-0.7.0/weditor/templates/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)    15204 2023-07-23 14:22:06.000000 weditor-0.7.0/weditor/templates/index.html
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2187 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/templates/widget_preview.html
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.537612 weditor-0.7.0/weditor/web/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        0 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/__init__.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     3927 2023-07-23 14:41:48.000000 weditor-0.7.0/weditor/web/device.py
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.538503 weditor-0.7.0/weditor/web/handlers/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        0 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/handlers/__init__.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     7212 2023-07-23 14:37:47.000000 weditor-0.7.0/weditor/web/handlers/page.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2152 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/handlers/proxy.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     8174 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/handlers/shell.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     5136 2023-07-23 14:15:35.000000 weditor-0.7.0/weditor/web/ipyshell-console.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      150 2023-07-23 14:29:26.000000 weditor-0.7.0/weditor/web/proto.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     7928 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/uidumplib.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     1302 2023-07-23 14:15:35.000000 weditor-0.7.0/weditor/web/utils.py
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      188 2021-05-21 09:58:42.000000 weditor-0.7.0/weditor/web/version.py
+drwxr-xr-x   0 codeskyblue   (501) staff       (20)        0 2023-07-25 09:39:12.500879 weditor-0.7.0/weditor.egg-info/
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     2715 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/PKG-INFO
+-rw-r--r--   0 codeskyblue   (501) staff       (20)     4081 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/SOURCES.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        1 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/dependency_links.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)       51 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/entry_points.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        1 2021-05-27 11:20:01.000000 weditor-0.7.0/weditor.egg-info/not-zip-safe
+-rw-r--r--   0 codeskyblue   (501) staff       (20)       47 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/pbr.json
+-rw-r--r--   0 codeskyblue   (501) staff       (20)      127 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/requires.txt
+-rw-r--r--   0 codeskyblue   (501) staff       (20)        8 2023-07-25 09:39:12.000000 weditor-0.7.0/weditor.egg-info/top_level.txt
```

### Comparing `weditor-0.6.8/.github/workflows/publish-to-pypi.yml` & `weditor-0.7.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/API.md` & `weditor-0.7.0/API.md`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/CHANGELOG.docx` & `weditor-0.7.0/CHANGELOG.docx`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/DEVELOP.md` & `weditor-0.7.0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/LICENSE` & `weditor-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/PKG-INFO` & `weditor-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: weditor
-Version: 0.6.8
+Version: 0.7.0
 Summary: tool for writing atx script
 Home-page: https://github.com/openatx/weditor
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: # WEditor
         [![image](https://img.shields.io/pypi/v/weditor.svg?style=flat-square)](https://pypi.python.org/pypi/weditor)
```

### Comparing `weditor-0.6.8/README.md` & `weditor-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/README_ZH.md` & `weditor-0.7.0/README_ZH.md`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/log.txt` & `weditor-0.7.0/log.txt`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/ace/ace.js` & `weditor-0.7.0/samples/ace/ace.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/ace/ext-language_tools.js` & `weditor-0.7.0/samples/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/ace/keybinding-vim.js` & `weditor-0.7.0/samples/ace/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/ace/mode-python.js` & `weditor-0.7.0/samples/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/ace/theme-monokai.js` & `weditor-0.7.0/samples/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/bg.jpg` & `weditor-0.7.0/samples/bg.jpg`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/samples/index.html` & `weditor-0.7.0/samples/index.html`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/screenshot.jpg` & `weditor-0.7.0/screenshot.jpg`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/tests/test_web_utils.py` & `weditor-0.7.0/tests/test_web_utils.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/__main__.py` & `weditor-0.7.0/weditor/__main__.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/page.xml` & `weditor-0.7.0/weditor/page.xml`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/ace/ace.js` & `weditor-0.7.0/weditor/static/ace/ace.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/ace/ext-language_tools.js` & `weditor-0.7.0/weditor/static/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/ace/keybinding-vim.js` & `weditor-0.7.0/weditor/static/ace/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/ace/mode-python.js` & `weditor-0.7.0/weditor/static/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/ace/theme-monokai.js` & `weditor-0.7.0/weditor/static/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1` & `weditor-0.7.0/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js` & `weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff` & `weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css` & `weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0` & `weditor-0.7.0/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/favicon.ico` & `weditor-0.7.0/weditor/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/js/common.js` & `weditor-0.7.0/weditor/static/js/common.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/js/index.js` & `weditor-0.7.0/weditor/static/js/index.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/css/buttons.css` & `weditor-0.7.0/weditor/static/libs/css/buttons.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.css` & `weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.css.map` & `weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/css/font-awesome.min.css` & `weditor-0.7.0/weditor/static/libs/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/FontAwesome.otf` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2` & `weditor-0.7.0/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/vue-2.5.16/vue.js` & `weditor-0.7.0/weditor/static/libs/vue-2.5.16/vue.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/libs/vue-2.5.16/vue.min.js` & `weditor-0.7.0/weditor/static/libs/vue-2.5.16/vue.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/loading.svg` & `weditor-0.7.0/weditor/static/loading.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/running.svg` & `weditor-0.7.0/weditor/static/running.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/static/style.css` & `weditor-0.7.0/weditor/static/style.css`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/templates/index.html` & `weditor-0.7.0/weditor/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
       <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
         <!--         <ul class="nav navbar-nav">
           <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
         </ul> -->
         <form class="navbar-form navbar-left" onsubmit="return false">
           <div class="form-group">
             <select v-model="platform" class="selectpicker" value="Android" title="Platform" data-width="fit">
-              <option data-icon="fa fa-android" value="Android">Android</option>
+              <option data-icon="fa fa-android" value="Android">Android UIAutomator2</option>
+              <option data-icon="fa fa-apple" value="AndroidADB">Android ADB</option>
               <option data-icon="fa fa-apple" value="iOS">iOS</option>
               <!-- <option data-icon="glyphicon-apple" value="Neco">Neco(beta)</option> -->
             </select>
             <!-- <el-select v-model="serial" allow-create filterable placeholder="选择或输入">
               <el-option
                 v-for="item in deviceList" :key="item.value" :label="item.label + ':' + item.value" :value="item.value">
               </el-option>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
  Toggle navigation
 ATX_WEditor
-[One of: Android/iOS]  [                    ]
+[One of: Android UIAutomator2/Android ADB/iOS]  [                    ]
 disabled="connecting"> Connect
 disabled="loading || connecting" class="btn btn-default" v-on:
 click="dumpHierarchyWithScreen()">
 class='{"fa-spin": dumping}'>
  Dump Hierarchy
     * ç¸å³ææ¡£
           o openatx/weditor
```

### Comparing `weditor-0.6.8/weditor/templates/widget_preview.html` & `weditor-0.7.0/weditor/templates/widget_preview.html`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/web/device.py` & `weditor-0.7.0/weditor/web/device.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # coding: utf-8
 #
 
 import abc
 
+import adbutils
 import uiautomator2 as u2
 import wda
 from logzero import logger
 from PIL import Image
 
 from . import uidumplib
+from .proto import PlatformEnum
 
 
 class DeviceMeta(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def screenshot(self) -> Image.Image:
         pass
 
@@ -20,15 +22,45 @@
         pass
 
     @abc.abstractproperty
     def device(self):
         pass
 
 
-class _AndroidDevice(DeviceMeta):
+class _AndroidADB(DeviceMeta):
+    def __init__(self, device_url: str):
+        if not device_url:
+            self._d = adbutils.device()
+        else:
+            self._d = adbutils.device(device_url)
+    
+    def screenshot(self) -> Image:
+        return self._d.screenshot()
+    
+    def dump_hierarchy(self) -> str:
+        return self._d.dump_hierarchy()
+    
+    def dump_hierarchy2(self):
+        current = self._d.app_current()
+        page_xml = self._d.dump_hierarchy()
+        page_json = uidumplib.android_hierarchy_to_json(
+            page_xml.encode('utf-8'))
+        return {
+            "xmlHierarchy": page_xml,
+            "jsonHierarchy": page_json,
+            "activity": current.activity,
+            "packageName": current.package,
+            "windowSize": self._d.window_size(),
+        }
+
+    @property
+    def device(self):
+        return self._d
+        
+class _AndroidUiautomatorDevice(DeviceMeta):
     def __init__(self, device_url):
         d = u2.connect(device_url)
         # 登陆界面无法截图，就先返回空图片
         d.settings["fallback_to_blank_screenshot"] = True
         self._d = d
 
     def screenshot(self):
@@ -36,14 +68,16 @@
 
     def dump_hierarchy(self):
         return uidumplib.get_android_hierarchy(self._d)
 
     def dump_hierarchy2(self):
         current = self._d.app_current()
         page_xml = self._d.dump_hierarchy(pretty=True)
+        # 临时增加测试
+        # import adbutils
         page_json = uidumplib.android_hierarchy_to_json(
             page_xml.encode('utf-8'))
         return {
             "xmlHierarchy": page_xml,
             "jsonHierarchy": page_json,
             "activity": current['activity'],
             "packageName": current['package'],
@@ -87,23 +121,25 @@
     def device(self):
         return self._client
 
 
 cached_devices = {}
 
 
-def connect_device(platform, device_url):
+def connect_device(platform: PlatformEnum, device_url: str):
     """
     Returns:
         deviceId (string)
     """
     device_id = platform + ":" + device_url
-    if platform == 'android':
-        d = _AndroidDevice(device_url)
-    elif platform == 'ios':
+    if platform == PlatformEnum.AndroidUIAutomator2:
+        d = _AndroidUiautomatorDevice(device_url)
+    elif platform == PlatformEnum.AndroidADB:
+        d = _AndroidADB(device_url)
+    elif platform == PlatformEnum.IOS:
         d = _AppleDevice(device_url)
     else:
         raise ValueError("Unknown platform", platform)
 
     cached_devices[device_id] = d
     return device_id
```

### Comparing `weditor-0.6.8/weditor/web/handlers/page.py` & `weditor-0.7.0/weditor/web/handlers/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import tornado
 from logzero import logger
 from PIL import Image
 from tornado.escape import json_decode
 
 from ..device import connect_device, get_device
 from ..version import __version__
-
+from ..proto import PlatformEnum
 
 pathjoin = os.path.join
 
 
 class BaseHandler(tornado.web.RequestHandler):
     def set_default_headers(self):
         self.set_header("Access-Control-Allow-Origin", "*")
@@ -49,20 +49,23 @@
 class MainHandler(BaseHandler):
     def get(self):
         self.render("index.html")
 
 
 class DeviceConnectHandler(BaseHandler):
     def post(self):
-        platform = self.get_argument("platform").lower()
+        _platform = self.get_argument("platform")
         device_url = self.get_argument("deviceUrl")
 
+        platform = PlatformEnum(_platform)
+        del _platform
         try:
             id = connect_device(platform, device_url)
         except RuntimeError as e:
+            logger.exception("connect failed")
             self.set_status(500)
             self.write({
                 "success": False,
                 "description": str(e),
             })
         except Exception as e:
             logger.warning("device connect error: %s", e)
```

### Comparing `weditor-0.6.8/weditor/web/handlers/proxy.py` & `weditor-0.7.0/weditor/web/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/web/handlers/shell.py` & `weditor-0.7.0/weditor/web/handlers/shell.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/web/ipyshell-console.py` & `weditor-0.7.0/weditor/web/ipyshell-console.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/web/uidumplib.py` & `weditor-0.7.0/weditor/web/uidumplib.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor/web/utils.py` & `weditor-0.7.0/weditor/web/utils.py`

 * *Files identical despite different names*

### Comparing `weditor-0.6.8/weditor.egg-info/PKG-INFO` & `weditor-0.7.0/weditor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: weditor
-Version: 0.6.8
+Version: 0.7.0
 Summary: tool for writing atx script
 Home-page: https://github.com/openatx/weditor
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: # WEditor
         [![image](https://img.shields.io/pypi/v/weditor.svg?style=flat-square)](https://pypi.python.org/pypi/weditor)
```

### Comparing `weditor-0.6.8/weditor.egg-info/SOURCES.txt` & `weditor-0.7.0/weditor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ABOUT.rst
 API.md
+AUTHORS
 CHANGELOG.docx
+ChangeLog
 DEVELOP.md
 LICENSE
 README.md
 README_ZH.md
 dev-requirements.txt
 log.txt
 requirements.txt
@@ -17,14 +19,15 @@
 samples/bower.json
 samples/index.html
 samples/ace/ace.js
 samples/ace/ext-language_tools.js
 samples/ace/keybinding-vim.js
 samples/ace/mode-python.js
 samples/ace/theme-monokai.js
+tests/test_proto.py
 tests/test_web_utils.py
 weditor/__init__.py
 weditor/__main__.py
 weditor/page.xml
 weditor.egg-info/PKG-INFO
 weditor.egg-info/SOURCES.txt
 weditor.egg-info/dependency_links.txt
@@ -79,14 +82,15 @@
 weditor/static/libs/vue-2.5.16/vue.js
 weditor/static/libs/vue-2.5.16/vue.min.js
 weditor/templates/index.html
 weditor/templates/widget_preview.html
 weditor/web/__init__.py
 weditor/web/device.py
 weditor/web/ipyshell-console.py
+weditor/web/proto.py
 weditor/web/uidumplib.py
 weditor/web/utils.py
 weditor/web/version.py
 weditor/web/handlers/__init__.py
 weditor/web/handlers/page.py
 weditor/web/handlers/proxy.py
 weditor/web/handlers/shell.py
```

