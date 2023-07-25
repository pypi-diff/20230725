# Comparing `tmp/Orange3-Explain-0.6.5.tar.gz` & `tmp/Orange3-Explain-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Explain-0.6.5.tar", last modified: Sun Jul  9 20:03:41 2023, max compression
+gzip compressed data, was "Orange3-Explain-0.6.6.tar", last modified: Tue Jul 25 13:50:55 2023, max compression
```

## Comparing `Orange3-Explain-0.6.5.tar` & `Orange3-Explain-0.6.6.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.299705 Orange3-Explain-0.6.5/
--rw-r--r--   0 primoz     (501) staff       (20)    35147 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/LICENSE.txt
--rw-r--r--   0 primoz     (501) staff       (20)      127 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/MANIFEST.in
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.264097 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/
--rw-r--r--   0 primoz     (501) staff       (20)     1085 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)     5109 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/SOURCES.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/dependency_links.txt
--rw-r--r--   0 primoz     (501) staff       (20)      196 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/entry_points.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/namespace_packages.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2022-07-28 09:49:17.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/not-zip-safe
--rw-r--r--   0 primoz     (501) staff       (20)      164 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/requires.txt
--rw-r--r--   0 primoz     (501) staff       (20)       14 2023-07-09 20:03:41.000000 Orange3-Explain-0.6.5/Orange3_Explain.egg-info/top_level.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1085 2023-07-09 20:03:41.299565 Orange3-Explain-0.6.5/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)      735 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/README.md
--rw-r--r--   0 primoz     (501) staff       (20)      545 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/README.pypi
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.264702 Orange3-Explain-0.6.5/doc/
--rw-r--r--   0 primoz     (501) staff       (20)     7465 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/Makefile
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.260653 Orange3-Explain-0.6.5/doc/_build/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.265789 Orange3-Explain-0.6.5/doc/_build/html/
--rw-r--r--   0 primoz     (501) staff       (20)      230 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/.buildinfo
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.268847 Orange3-Explain-0.6.5/doc/_build/html/_images/
--rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Model-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Model.png
--rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Prediction-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Prediction.png
--rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/ICE-example.png
--rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/ICE.png
--rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Permutation-Importance-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_images/Permutation-Importance.png
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.269023 Orange3-Explain-0.6.5/doc/_build/html/_sources/
--rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.269989 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-model.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-prediction.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-predictions.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/ice.md.txt
--rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/permutation-importance.md.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.274331 Orange3-Explain-0.6.5/doc/_build/html/_static/
--rw-r--r--   0 primoz     (501) staff       (20)     4418 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 primoz     (501) staff       (20)    14813 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/basic.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.274916 Orange3-Explain-0.6.5/doc/_build/html/_static/css/
--rw-r--r--   0 primoz     (501) staff       (20)     3229 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.286535 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/
--rw-r--r--   0 primoz     (501) staff       (20)    87624 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)    67312 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)    86288 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 primoz     (501) staff       (20)    66444 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   165742 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 primoz     (501) staff       (20)   444379 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 primoz     (501) staff       (20)   165548 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 primoz     (501) staff       (20)    98024 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 primoz     (501) staff       (20)    77160 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   323344 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   193308 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309728 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 primoz     (501) staff       (20)   184912 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   328412 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 primoz     (501) staff       (20)   195704 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   309192 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 primoz     (501) staff       (20)   182708 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 primoz     (501) staff       (20)   135235 2023-04-26 07:48:52.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/css/theme.css
--rw-r--r--   0 primoz     (501) staff       (20)      458 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/custom.css
--rw-r--r--   0 primoz     (501) staff       (20)     4472 2023-04-06 13:17:06.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/doctools.js
--rw-r--r--   0 primoz     (501) staff       (20)      415 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 primoz     (501) staff       (20)      286 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/file.png
--rw-r--r--   0 primoz     (501) staff       (20)   288580 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 primoz     (501) staff       (20)    89501 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/jquery.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.287598 Orange3-Explain-0.6.5/doc/_build/html/_static/js/
--rw-r--r--   0 primoz     (501) staff       (20)      934 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/js/badge_only.js
--rw-r--r--   0 primoz     (501) staff       (20)     4370 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     2734 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 primoz     (501) staff       (20)     5023 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/js/theme.js
--rw-r--r--   0 primoz     (501) staff       (20)     4758 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/language_data.js
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/minus.png
--rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/plus.png
--rw-r--r--   0 primoz     (501) staff       (20)     4846 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/pygments.css
--rw-r--r--   0 primoz     (501) staff       (20)    18215 2023-04-06 13:17:06.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 primoz     (501) staff       (20)     4712 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 primoz     (501) staff       (20)    68420 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 primoz     (501) staff       (20)    19530 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.5/doc/_build/html/_static/underscore.js
--rw-r--r--   0 primoz     (501) staff       (20)     3729 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/genindex.html
--rw-r--r--   0 primoz     (501) staff       (20)     5794 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/index.html
--rw-r--r--   0 primoz     (501) staff       (20)      351 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/objects.inv
--rw-r--r--   0 primoz     (501) staff       (20)     4128 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/search.html
--rw-r--r--   0 primoz     (501) staff       (20)     5924 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/searchindex.js
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.288607 Orange3-Explain-0.6.5/doc/_build/html/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     8689 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-model.html
--rw-r--r--   0 primoz     (501) staff       (20)    10398 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-prediction.html
--rw-r--r--   0 primoz     (501) staff       (20)     5597 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-predictions.html
--rw-r--r--   0 primoz     (501) staff       (20)     7031 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/widgets/ice.html
--rw-r--r--   0 primoz     (501) staff       (20)     7362 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.5/doc/_build/html/widgets/permutation-importance.html
--rw-r--r--   0 primoz     (501) staff       (20)     9531 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/conf.py
--rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/index.rst
--rw-r--r--   0 primoz     (501) staff       (20)     7009 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/make.bat
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.289614 Orange3-Explain-0.6.5/doc/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/explain-model.md
--rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/explain-prediction.md
--rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/explain-predictions.md
--rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.5/doc/widgets/ice.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.292828 Orange3-Explain-0.6.5/doc/widgets/images/
--rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Explain-Model-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Explain-Model.png
--rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Explain-Prediction-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Explain-Prediction.png
--rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/widgets/images/ICE-example.png
--rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/doc/widgets/images/ICE.png
--rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Permutation-Importance-Example.png
--rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/images/Permutation-Importance.png
--rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/doc/widgets/permutation-importance.md
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.293012 Orange3-Explain-0.6.5/orangecontrib/
--rw-r--r--   0 primoz     (501) staff       (20)      164 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.294119 Orange3-Explain-0.6.5/orangecontrib/explain/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.5/orangecontrib/explain/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    24970 2023-07-09 19:37:12.000000 Orange3-Explain-0.6.5/orangecontrib/explain/explainer.py
--rw-r--r--   0 primoz     (501) staff       (20)     7285 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.5/orangecontrib/explain/inspection.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.294649 Orange3-Explain-0.6.5/orangecontrib/explain/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    29073 2023-07-09 19:37:12.000000 Orange3-Explain-0.6.5/orangecontrib/explain/tests/test_explainer.py
--rw-r--r--   0 primoz     (501) staff       (20)    15039 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.5/orangecontrib/explain/tests/test_inspection.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.296961 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/
--rw-r--r--   0 primoz     (501) staff       (20)     1059 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.298045 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/
--rw-r--r--   0 primoz     (501) staff       (20)      738 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainModel.svg
--rw-r--r--   0 primoz     (501) staff       (20)      517 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainPred.svg
--rw-r--r--   0 primoz     (501) staff       (20)      842 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainPredictions.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1199 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ICE.svg
--rw-r--r--   0 primoz     (501) staff       (20)      595 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/PermutationImportance.svg
--rw-r--r--   0 primoz     (501) staff       (20)    24815 2022-10-27 09:59:01.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainfeaturebase.py
--rw-r--r--   0 primoz     (501) staff       (20)    19507 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainmodel.py
--rw-r--r--   0 primoz     (501) staff       (20)    27206 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainprediction.py
--rw-r--r--   0 primoz     (501) staff       (20)    32622 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainpredictions.py
--rw-r--r--   0 primoz     (501) staff       (20)    32238 2022-12-15 11:16:07.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owice.py
--rw-r--r--   0 primoz     (501) staff       (20)    14417 2023-06-14 09:22:48.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owpermutationimportance.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-09 20:03:41.299113 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    17230 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainmodel.py
--rw-r--r--   0 primoz     (501) staff       (20)     9615 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainprediction.py
--rw-r--r--   0 primoz     (501) staff       (20)    21495 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py
--rw-r--r--   0 primoz     (501) staff       (20)     7859 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owice.py
--rw-r--r--   0 primoz     (501) staff       (20)    18373 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py
--rw-r--r--   0 primoz     (501) staff       (20)       97 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.5/pyproject.toml
--rw-r--r--   0 primoz     (501) staff       (20)       38 2023-07-09 20:03:41.299739 Orange3-Explain-0.6.5/setup.cfg
--rw-r--r--   0 primoz     (501) staff       (20)     3024 2023-07-09 20:03:22.000000 Orange3-Explain-0.6.5/setup.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.934205 Orange3-Explain-0.6.6/
+-rw-r--r--   0 primoz     (501) staff       (20)    35147 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/LICENSE.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      127 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/MANIFEST.in
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.895416 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/
+-rw-r--r--   0 primoz     (501) staff       (20)     1090 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)     5109 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/SOURCES.txt
+-rw-r--r--   0 primoz     (501) staff       (20)        1 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/dependency_links.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      196 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/entry_points.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       14 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/namespace_packages.txt
+-rw-r--r--   0 primoz     (501) staff       (20)        1 2022-07-28 09:49:17.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/not-zip-safe
+-rw-r--r--   0 primoz     (501) staff       (20)      164 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/requires.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       14 2023-07-25 13:50:55.000000 Orange3-Explain-0.6.6/Orange3_Explain.egg-info/top_level.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1090 2023-07-25 13:50:55.934046 Orange3-Explain-0.6.6/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)      735 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/README.md
+-rw-r--r--   0 primoz     (501) staff       (20)      545 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/README.pypi
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.896146 Orange3-Explain-0.6.6/doc/
+-rw-r--r--   0 primoz     (501) staff       (20)     7465 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/Makefile
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.891502 Orange3-Explain-0.6.6/doc/_build/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.897566 Orange3-Explain-0.6.6/doc/_build/html/
+-rw-r--r--   0 primoz     (501) staff       (20)      230 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/.buildinfo
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.900754 Orange3-Explain-0.6.6/doc/_build/html/_images/
+-rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Model-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Model.png
+-rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Prediction-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Prediction.png
+-rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/ICE-example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/ICE.png
+-rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Permutation-Importance-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_images/Permutation-Importance.png
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.900959 Orange3-Explain-0.6.6/doc/_build/html/_sources/
+-rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.902171 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-model.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-prediction.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-predictions.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/ice.md.txt
+-rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/permutation-importance.md.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.906270 Orange3-Explain-0.6.6/doc/_build/html/_static/
+-rw-r--r--   0 primoz     (501) staff       (20)     4418 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 primoz     (501) staff       (20)    14813 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/basic.css
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.906839 Orange3-Explain-0.6.6/doc/_build/html/_static/css/
+-rw-r--r--   0 primoz     (501) staff       (20)     3229 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.918183 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/
+-rw-r--r--   0 primoz     (501) staff       (20)    87624 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    67312 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)    86288 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    66444 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   165742 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 primoz     (501) staff       (20)   444379 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 primoz     (501) staff       (20)   165548 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 primoz     (501) staff       (20)    98024 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 primoz     (501) staff       (20)    77160 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   323344 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   193308 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   309728 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   184912 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   328412 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   195704 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   309192 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 primoz     (501) staff       (20)   182708 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 primoz     (501) staff       (20)   135235 2023-04-26 07:48:52.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/css/theme.css
+-rw-r--r--   0 primoz     (501) staff       (20)      458 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/custom.css
+-rw-r--r--   0 primoz     (501) staff       (20)     4472 2023-04-06 13:17:06.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 primoz     (501) staff       (20)      415 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 primoz     (501) staff       (20)      286 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/file.png
+-rw-r--r--   0 primoz     (501) staff       (20)   288580 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 primoz     (501) staff       (20)    89501 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/jquery.js
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.919379 Orange3-Explain-0.6.6/doc/_build/html/_static/js/
+-rw-r--r--   0 primoz     (501) staff       (20)      934 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4370 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 primoz     (501) staff       (20)     2734 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 primoz     (501) staff       (20)     5023 2022-12-06 12:49:34.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/js/theme.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4758 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/minus.png
+-rw-r--r--   0 primoz     (501) staff       (20)       90 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/plus.png
+-rw-r--r--   0 primoz     (501) staff       (20)     4846 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 primoz     (501) staff       (20)    18215 2023-04-06 13:17:06.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4712 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 primoz     (501) staff       (20)    68420 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 primoz     (501) staff       (20)    19530 2022-10-24 08:31:27.000000 Orange3-Explain-0.6.6/doc/_build/html/_static/underscore.js
+-rw-r--r--   0 primoz     (501) staff       (20)     3729 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/genindex.html
+-rw-r--r--   0 primoz     (501) staff       (20)     5794 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/index.html
+-rw-r--r--   0 primoz     (501) staff       (20)      351 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/objects.inv
+-rw-r--r--   0 primoz     (501) staff       (20)     4128 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/search.html
+-rw-r--r--   0 primoz     (501) staff       (20)     5924 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/searchindex.js
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.920626 Orange3-Explain-0.6.6/doc/_build/html/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     8689 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-model.html
+-rw-r--r--   0 primoz     (501) staff       (20)    10398 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-prediction.html
+-rw-r--r--   0 primoz     (501) staff       (20)     5597 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-predictions.html
+-rw-r--r--   0 primoz     (501) staff       (20)     7031 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/widgets/ice.html
+-rw-r--r--   0 primoz     (501) staff       (20)     7362 2023-07-09 20:02:58.000000 Orange3-Explain-0.6.6/doc/_build/html/widgets/permutation-importance.html
+-rw-r--r--   0 primoz     (501) staff       (20)     9531 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/conf.py
+-rw-r--r--   0 primoz     (501) staff       (20)      360 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/index.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     7009 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/make.bat
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.921799 Orange3-Explain-0.6.6/doc/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     3396 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/explain-model.md
+-rw-r--r--   0 primoz     (501) staff       (20)     4778 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/explain-prediction.md
+-rw-r--r--   0 primoz     (501) staff       (20)      770 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/explain-predictions.md
+-rw-r--r--   0 primoz     (501) staff       (20)     1901 2022-10-10 13:45:58.000000 Orange3-Explain-0.6.6/doc/widgets/ice.md
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.926629 Orange3-Explain-0.6.6/doc/widgets/images/
+-rw-r--r--   0 primoz     (501) staff       (20)   148240 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Explain-Model-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)   184281 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Explain-Model.png
+-rw-r--r--   0 primoz     (501) staff       (20)   162676 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Explain-Prediction-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)   186086 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Explain-Prediction.png
+-rw-r--r--   0 primoz     (501) staff       (20)    91768 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/widgets/images/ICE-example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    70136 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/doc/widgets/images/ICE.png
+-rw-r--r--   0 primoz     (501) staff       (20)    84574 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Permutation-Importance-Example.png
+-rw-r--r--   0 primoz     (501) staff       (20)    28226 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/images/Permutation-Importance.png
+-rw-r--r--   0 primoz     (501) staff       (20)     2016 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/doc/widgets/permutation-importance.md
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.926836 Orange3-Explain-0.6.6/orangecontrib/
+-rw-r--r--   0 primoz     (501) staff       (20)      164 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.927542 Orange3-Explain-0.6.6/orangecontrib/explain/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.6/orangecontrib/explain/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    24970 2023-07-25 13:17:22.000000 Orange3-Explain-0.6.6/orangecontrib/explain/explainer.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7285 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.6/orangecontrib/explain/inspection.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.928261 Orange3-Explain-0.6.6/orangecontrib/explain/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    29073 2023-07-09 19:37:12.000000 Orange3-Explain-0.6.6/orangecontrib/explain/tests/test_explainer.py
+-rw-r--r--   0 primoz     (501) staff       (20)    15039 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.6/orangecontrib/explain/tests/test_inspection.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.930561 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/
+-rw-r--r--   0 primoz     (501) staff       (20)     1059 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.932135 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/
+-rw-r--r--   0 primoz     (501) staff       (20)      738 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainModel.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      517 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainPred.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      842 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainPredictions.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     1199 2022-10-10 13:45:40.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ICE.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      595 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/PermutationImportance.svg
+-rw-r--r--   0 primoz     (501) staff       (20)    24815 2022-10-27 09:59:01.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainfeaturebase.py
+-rw-r--r--   0 primoz     (501) staff       (20)    19507 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainmodel.py
+-rw-r--r--   0 primoz     (501) staff       (20)    27206 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainprediction.py
+-rw-r--r--   0 primoz     (501) staff       (20)    32622 2023-07-25 13:22:02.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainpredictions.py
+-rw-r--r--   0 primoz     (501) staff       (20)    32238 2022-12-15 11:16:07.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owice.py
+-rw-r--r--   0 primoz     (501) staff       (20)    14417 2023-06-14 09:22:48.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owpermutationimportance.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2023-07-25 13:50:55.933580 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    17230 2022-12-01 08:56:52.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainmodel.py
+-rw-r--r--   0 primoz     (501) staff       (20)     9615 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainprediction.py
+-rw-r--r--   0 primoz     (501) staff       (20)    21495 2023-07-25 13:21:20.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7859 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owice.py
+-rw-r--r--   0 primoz     (501) staff       (20)    18373 2022-12-15 14:34:35.000000 Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py
+-rw-r--r--   0 primoz     (501) staff       (20)       97 2022-07-28 07:30:45.000000 Orange3-Explain-0.6.6/pyproject.toml
+-rw-r--r--   0 primoz     (501) staff       (20)       38 2023-07-25 13:50:55.934255 Orange3-Explain-0.6.6/setup.cfg
+-rw-r--r--   0 primoz     (501) staff       (20)     3029 2023-07-25 13:50:44.000000 Orange3-Explain-0.6.6/setup.py
```

### Comparing `Orange3-Explain-0.6.5/LICENSE.txt` & `Orange3-Explain-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/Orange3_Explain.egg-info/PKG-INFO` & `Orange3-Explain-0.6.6/Orange3_Explain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Orange3-Explain
-Version: 0.6.5
+Version: 0.6.6
 Summary: Orange3 add-on for explanatory AI
-Home-page: http://orange.biolab.si/download
+Home-page: https://orangedatamining.com/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
 Keywords: orange3 add-on,orange3-explain
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `Orange3-Explain-0.6.5/Orange3_Explain.egg-info/SOURCES.txt` & `Orange3-Explain-0.6.6/Orange3_Explain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/PKG-INFO` & `Orange3-Explain-0.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Orange3-Explain
-Version: 0.6.5
+Version: 0.6.6
 Summary: Orange3 add-on for explanatory AI
-Home-page: http://orange.biolab.si/download
+Home-page: https://orangedatamining.com/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
 Keywords: orange3 add-on,orange3-explain
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `Orange3-Explain-0.6.5/README.md` & `Orange3-Explain-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/README.pypi` & `Orange3-Explain-0.6.6/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/Makefile` & `Orange3-Explain-0.6.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Model-Example.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Model-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Model.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Model.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Prediction-Example.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Prediction-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Explain-Prediction.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Explain-Prediction.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/ICE-example.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/ICE-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/ICE.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/ICE.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Permutation-Importance-Example.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Permutation-Importance-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_images/Permutation-Importance.png` & `Orange3-Explain-0.6.6/doc/_build/html/_images/Permutation-Importance.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-model.md.txt` & `Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-model.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-prediction.md.txt` & `Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-prediction.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/explain-predictions.md.txt` & `Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/explain-predictions.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/ice.md.txt` & `Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/ice.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_sources/widgets/permutation-importance.md.txt` & `Orange3-Explain-0.6.6/doc/_build/html/_sources/widgets/permutation-importance.md.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/basic.css` & `Orange3-Explain-0.6.6/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/badge_only.css` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold-italic.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-bold.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal-italic.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal.woff` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/fonts/lato-normal.woff2` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/css/theme.css` & `Orange3-Explain-0.6.6/doc/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/doctools.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/jquery-3.6.0.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/jquery.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/js/badge_only.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/js/html5shiv-printshiv.min.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/js/html5shiv.min.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/js/theme.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/language_data.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/pygments.css` & `Orange3-Explain-0.6.6/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/searchtools.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/sphinx_highlight.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/underscore-1.13.1.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/_static/underscore.js` & `Orange3-Explain-0.6.6/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/genindex.html` & `Orange3-Explain-0.6.6/doc/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/index.html` & `Orange3-Explain-0.6.6/doc/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/search.html` & `Orange3-Explain-0.6.6/doc/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/searchindex.js` & `Orange3-Explain-0.6.6/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-model.html` & `Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-model.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-prediction.html` & `Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-prediction.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/widgets/explain-predictions.html` & `Orange3-Explain-0.6.6/doc/_build/html/widgets/explain-predictions.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/widgets/ice.html` & `Orange3-Explain-0.6.6/doc/_build/html/widgets/ice.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/_build/html/widgets/permutation-importance.html` & `Orange3-Explain-0.6.6/doc/_build/html/widgets/permutation-importance.html`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/conf.py` & `Orange3-Explain-0.6.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/make.bat` & `Orange3-Explain-0.6.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/explain-model.md` & `Orange3-Explain-0.6.6/doc/widgets/explain-model.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/explain-prediction.md` & `Orange3-Explain-0.6.6/doc/widgets/explain-prediction.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/explain-predictions.md` & `Orange3-Explain-0.6.6/doc/widgets/explain-predictions.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/ice.md` & `Orange3-Explain-0.6.6/doc/widgets/ice.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Explain-Model-Example.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Explain-Model-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Explain-Model.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Explain-Model.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Explain-Prediction-Example.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Explain-Prediction-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Explain-Prediction.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Explain-Prediction.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/ICE-example.png` & `Orange3-Explain-0.6.6/doc/widgets/images/ICE-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/ICE.png` & `Orange3-Explain-0.6.6/doc/widgets/images/ICE.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Permutation-Importance-Example.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Permutation-Importance-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/images/Permutation-Importance.png` & `Orange3-Explain-0.6.6/doc/widgets/images/Permutation-Importance.png`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/doc/widgets/permutation-importance.md` & `Orange3-Explain-0.6.6/doc/widgets/permutation-importance.md`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/explainer.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/inspection.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/inspection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/tests/test_explainer.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/tests/test_explainer.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/tests/test_inspection.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/__init__.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainModel.svg` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainModel.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainPred.svg` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainPred.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ExplainPredictions.svg` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ExplainPredictions.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/ICE.svg` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/ICE.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/icons/PermutationImportance.svg` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/icons/PermutationImportance.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainfeaturebase.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainfeaturebase.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainmodel.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainmodel.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainprediction.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainprediction.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owexplainpredictions.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owexplainpredictions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owice.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owice.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/owpermutationimportance.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/owpermutationimportance.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainmodel.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainmodel.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainprediction.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainprediction.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owexplainpredictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         self.widget.graph.set_axis = Mock()
         simulate.combobox_activate_index(self.widget._annot_combo, 3)
         args = ([[(0, "0"), (1, "0"), (2, "0"), (3, "1"), (4, "1")]],)
         self.widget.graph.set_axis.assert_called_once_with(*args)
 
         self.widget.graph.set_axis.reset_mock()
         simulate.combobox_activate_index(self.widget._annot_combo, 1)
-        args = ([[(0, "4"), (1, "5"), (2, "1"), (3, "3"), (4, "2")]],)
+        args = ([[(0, "1"), (1, "5"), (2, "4"), (3, "3"), (4, "2")]],)
         self.widget.graph.set_axis.assert_called_once_with(*args)
 
         self.send_signal(self.widget.Inputs.data, None)
         self.assertEqual(self.widget._annot_combo.currentText(), "None")
         self.assertEqual(self.widget._annot_combo.count(), 2)
 
     def test_setup_plot(self):
```

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owice.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owice.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py` & `Orange3-Explain-0.6.6/orangecontrib/explain/widgets/tests/test_owpermutationimportance.py`

 * *Files identical despite different names*

### Comparing `Orange3-Explain-0.6.5/setup.py` & `Orange3-Explain-0.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from os import path, walk
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "Orange3-Explain"
 
-VERSION = "0.6.5"
+VERSION = "0.6.6"
 
 AUTHOR = "Bioinformatics Laboratory, FRI UL"
 AUTHOR_EMAIL = "contact@orange.biolab.si"
 
-URL = "http://orange.biolab.si/download"
+URL = "https://orangedatamining.com/download"
 DESCRIPTION = "Orange3 add-on for explanatory AI"
 LONG_DESCRIPTION = open(
     path.join(path.dirname(__file__), "README.pypi"), "r", encoding="utf-8"
 ).read()
 
 LICENSE = "GPL3+"
 
@@ -40,15 +40,15 @@
 INSTALL_REQUIRES = [
     "Orange3 >= 3.33.0",
     "orange-widget-base",
     "AnyQt",
     "numpy",
     "pyqtgraph",
     "scipy",
-    "shap >=0.42.0",
+    "shap >=0.42.1",
     "scikit-learn>=1.0.1",
 ]
 
 EXTRAS_REQUIRE = {
     'test': ['pytest', 'coverage'],
     'doc': ['sphinx', 'recommonmark', 'sphinx_rtd_theme'],
 }
```

