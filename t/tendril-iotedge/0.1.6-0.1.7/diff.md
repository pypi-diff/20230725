# Comparing `tmp/tendril-iotedge-0.1.6.tar.gz` & `tmp/tendril-iotedge-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-iotedge-0.1.6.tar", last modified: Wed Apr 12 18:22:05 2023, max compression
+gzip compressed data, was "tendril-iotedge-0.1.7.tar", last modified: Tue Jul 25 05:59:40 2023, max compression
```

## Comparing `tendril-iotedge-0.1.6.tar` & `tendril-iotedge-0.1.7.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.299721 tendril-iotedge-0.1.6/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-12 18:22:05.299721 tendril-iotedge-0.1.6/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.231723 tendril-iotedge-0.1.6/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.247723 tendril-iotedge-0.1.6/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-12 18:22:05.303721 tendril-iotedge-0.1.6/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.1.6/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.215724 tendril-iotedge-0.1.6/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.247723 tendril-iotedge-0.1.6/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.251723 tendril-iotedge-0.1.6/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.255723 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1855 2023-04-05 18:31:23.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2266 2023-04-05 09:34:19.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.255723 tendril-iotedge-0.1.6/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.259723 tendril-iotedge-0.1.6/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 15:45:45.000000 tendril-iotedge-0.1.6/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.1.6/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.263723 tendril-iotedge-0.1.6/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      733 2023-04-12 18:16:23.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.267722 tendril-iotedge-0.1.6/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.1.6/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.267722 tendril-iotedge-0.1.6/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.271722 tendril-iotedge-0.1.6/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4351 2023-04-05 17:19:08.000000 tendril-iotedge-0.1.6/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.275722 tendril-iotedge-0.1.6/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.1.6/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.1.6/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.279722 tendril-iotedge-0.1.6/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2636 2023-04-12 18:17:22.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/heartbeat.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.287721 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      963 2023-04-05 18:20:26.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-04-08 07:11:19.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.291721 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1534 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.295721 tendril-iotedge-0.1.6/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.1.7/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.943522 tendril-iotedge-0.1.7/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.947522 tendril-iotedge-0.1.7/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2023-07-25 05:05:32.000000 tendril-iotedge-0.1.7/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2267 2023-07-23 18:59:09.000000 tendril-iotedge-0.1.7/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril-iotedge-0.1.7/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril-iotedge-0.1.7/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.1.7/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      733 2023-04-12 18:16:23.000000 tendril-iotedge-0.1.7/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.1.7/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4654 2023-07-25 05:17:43.000000 tendril-iotedge-0.1.7/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.1.7/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.1.7/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2664 2023-04-12 18:53:32.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/heartbeat.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      963 2023-04-05 18:20:26.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-04-08 07:11:19.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.7/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-25 05:59:40.000000 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1575 2023-07-25 05:59:40.000000 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-25 05:59:40.000000 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-07-25 05:59:40.000000 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-25 05:59:40.000000 tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 05:59:40.951522 tendril-iotedge-0.1.7/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.7/tox.ini
```

### Comparing `tendril-iotedge-0.1.6/.gitignore` & `tendril-iotedge-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/.readthedocs.yml` & `tendril-iotedge-0.1.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/.travis.yml` & `tendril-iotedge-0.1.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/LICENSE` & `tendril-iotedge-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/PKG-INFO` & `tendril-iotedge-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.6/README.rst` & `tendril-iotedge-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/Makefile` & `tendril-iotedge-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/_static/custom.css` & `tendril-iotedge-0.1.7/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/_static/favicon.ico` & `tendril-iotedge-0.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/_static/logo.png` & `tendril-iotedge-0.1.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/_static/logo_packed.png` & `tendril-iotedge-0.1.7/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/_templates/about.html` & `tendril-iotedge-0.1.7/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/conf.py` & `tendril-iotedge-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/index.rst` & `tendril-iotedge-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/docs/installation.rst` & `tendril-iotedge-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/setup.py` & `tendril-iotedge-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotcore.py` & `tendril-iotedge-0.1.7/src/tendril/apiserver/routers/iotcore.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 
 @device_management_router.get("/{id}/settings",
                               response_model=device_config_unified_model)
 async def read_device_settings(id: int,
                                user: AuthUserModel = auth_spec(scopes=['device:read'])):
     with get_session() as session:
         return get_device_settings(id=id, auth_user=user,
-                                   session=session).export()
+                                   session=session).export(expand=False)
 
 
 @device_management_router.post("/{id}/settings",
                                response_model=device_config_unified_model)
 async def write_device_settings(id: int, settings: device_config_unified_model,
                                 user: AuthUserModel = auth_spec(scopes=['device:write'])):
     with get_session() as session:
         result = set_device_settings(id=id, settings=settings,
                                      auth_user=user, session=session)
         return get_device_settings(id=id, auth_user=user,
-                                   session=session).export()
+                                   session=session).export(expand=False)
 
 if INTERESTS_API_ENABLED:
     routers = [
         device_management_router
     ]
 else:
     logger.info("Not creating Device Management API routers.")
```

### Comparing `tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotedge.py` & `tendril-iotedge-0.1.7/src/tendril/apiserver/routers/iotedge.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 @iotedge_router.post("/ping")
 async def iot_device_ping(message: IoTDevicePingTModel):
     result = ping(device_id=message.id, status=message.status)
     return 'pong'
 
 
-@iotedge_router.get("/settings", response_model=device_config_unified_model)
+@iotedge_router.post("/settings", response_model=device_config_unified_model)
 async def iot_device_settings(req: IoTDeviceSettingRequestTModel):
     result = get_config(device_id=req.id, appname=req.appname)
     return result
 
 
 routers = []
```

### Comparing `tendril-iotedge-0.1.6/src/tendril/common/iotedge/exceptions.py` & `tendril-iotedge-0.1.7/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/common/iotedge/formats.py` & `tendril-iotedge-0.1.7/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/config/__init__.py` & `tendril-iotedge-0.1.7/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/config/iotedge.py` & `tendril-iotedge-0.1.7/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/db/models/deviceconfig.py` & `tendril-iotedge-0.1.7/src/tendril/db/models/deviceconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 #  It includes a great number of implicit dependencies on the downstream instance
 #  implementation package which need to be better resolved.
 #  These assets will be written to be generic to the extent
 #  possible, until they reach critical mass and can perhaps be moved into a
 #  distributable package of their own. Tentatively, tendril-iotcore, holding most
 #  of the separable device related bulk from sxm-core.
 
-cfg_option_spec = namedtuple('CfgOptionSpec', ['description', 'accessor', 'type', 'default', 'read_only'],
-                             defaults=[str, None, False])
+cfg_option_spec = namedtuple('CfgOptionSpec', ['description', 'accessor', 'exporter', 'validator',
+                                               'type', 'default', 'read_only'],
+                             defaults=[None, None, str, None, False])
 
 
 class DeviceConfigurationModel(DeclBase, BaseMixin, TimestampMixin):
     device_type = "device"
     appname = Column(String(50), nullable=False, default=device_type)
     hname = Column(String(100))
 
@@ -83,20 +84,23 @@
 
     @classmethod
     @lru_cache(maxsize=None)
     def tmodel(cls):
         name = cls.__name__.replace("Model", "TModel")
         return cls._build_tmodel(name, cls.configuration_spec())
 
-    def _extract_config(self, spec):
+    def _extract_config(self, spec, expand=True):
         rv = {}
         for key, lspec in spec.items():
             if isinstance(lspec, dict):
-                rv[key] = self._extract_config(lspec)
+                rv[key] = self._extract_config(lspec, expand=expand)
             elif isinstance(lspec, cfg_option_spec):
-                rv[key] = getattr(self, lspec.accessor)
+                if expand and lspec.exporter:
+                    rv[key] = getattr(self, lspec.exporter)(getattr(self, lspec.accessor))
+                else:
+                    rv[key] = getattr(self, lspec.accessor)
             else:
                 raise TypeError(f"Got an unsupported type for device option spec {lspec}")
         return rv
 
-    def export(self):
-        return self._extract_config(self.configuration_spec())
+    def export(self, expand=True):
+        return self._extract_config(self.configuration_spec(), expand=expand)
```

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotcore/settings.py` & `tendril-iotedge-0.1.7/src/tendril/iotcore/settings.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotedge/announce.py` & `tendril-iotedge-0.1.7/src/tendril/iotedge/announce.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     # manually reset password and load it up for one-time transmission.
                     # Raise manual password reset request here. Changing device status to
                     # NEW should get the job done as presently implemented.
                 else:
                     logger.info(f"Found password for {device_id} on transit cache.")
                     transit.delete(namespace="ott:dp", key=device_id)
                     rv['password'] = password
-        if device.model_instance.status == LifecycleStatus.NEW:
+        if device.model_instance.status in [LifecycleStatus.NEW, LifecycleStatus.APPROVAL]:
             # We're waiting for activation and don't need to do anything here.
             pass
     else:
         logger.info(f"Registering new device '{device_id}' "
                     f"of type '{appname}' from announce.")
         if have_credentials:
             logger.warning(f"Unregistered device {device_id} seems to already have a token")
```

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotedge/heartbeat.py` & `tendril-iotedge-0.1.7/src/tendril/iotedge/heartbeat.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/base.py` & `tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/base.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/manager.py` & `tendril-iotedge-0.1.7/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril/iotedge/registration.py` & `tendril-iotedge-0.1.7/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/tendril/__init__.py
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/iotcore.py
 src/tendril/apiserver/routers/iotedge.py
 src/tendril/common/__init__.py
 src/tendril/common/iotcore/__init__.py
+src/tendril/common/iotcore/exceptions.py
 src/tendril/common/iotcore/formats.py
 src/tendril/common/iotedge/__init__.py
 src/tendril/common/iotedge/exceptions.py
 src/tendril/common/iotedge/formats.py
 src/tendril/config/__init__.py
 src/tendril/config/iotedge.py
 src/tendril/db/__init__.py
```

### Comparing `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/requires.txt` & `tendril-iotedge-0.1.7/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/tests/coveralls.py` & `tendril-iotedge-0.1.7/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.6/tox.ini` & `tendril-iotedge-0.1.7/tox.ini`

 * *Files identical despite different names*

