# Comparing `tmp/etils-1.3.0.tar.gz` & `tmp/etils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etils-1.3.0.tar", last modified: Fri May 12 12:49:54 2023, max compression
+gzip compressed data, was "etils-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `etils-1.3.0.tar` & `etils-1.4.0.tar`

### file list

```diff
@@ -1,80 +1,85 @@
--rw-r--r--   0        0        0    11357 2023-05-12 12:49:33.017113 etils-1.3.0/LICENSE
--rw-r--r--   0        0        0     2063 2023-05-12 12:49:33.017113 etils-1.3.0/README.md
--rw-r--r--   0        0        0      859 2023-05-12 12:49:33.017113 etils-1.3.0/etils/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-12 12:49:33.017113 etils-1.3.0/etils/array_types/__init__.py
--rw-r--r--   0        0        0      720 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/__init__.py
--rw-r--r--   0        0        0     2740 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/dataclass_flags.py
--rw-r--r--   0        0        0     3770 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/logging_utils.py
--rw-r--r--   0        0        0     1229 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/__init__.py
--rw-r--r--   0        0        0     6379 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/array_as_img.py
--rw-r--r--   0        0        0     6156 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/colab_utils.py
--rw-r--r--   0        0        0     1511 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/highlight_util.py
--rw-r--r--   0        0        0      583 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/inspects/__init__.py
--rw-r--r--   0        0        0     1500 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/inspects/attrs.py
--rw-r--r--   0        0        0     2630 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/auto_utils.py
--rw-r--r--   0        0        0     2050 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/core.py
--rw-r--r--   0        0        0     2047 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/html_helper.py
--rw-r--r--   0        0        0    14441 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/nodes.py
--rw-r--r--   0        0        0     1540 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/resource_utils.py
--rw-r--r--   0        0        0      191 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/auto_activate.css
--rw-r--r--   0        0        0     1500 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/auto_activate.js
--rw-r--r--   0        0        0     2487 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/main.js
--rw-r--r--   0        0        0     2557 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/theme.css
--rw-r--r--   0        0        0    16290 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/lazy_imports.py
--rw-r--r--   0        0        0     4563 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/module_utils.py
--rw-r--r--   0        0        0     2441 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/patch_utils.py
--rw-r--r--   0        0        0      756 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/__init__.py
--rw-r--r--   0        0        0     3031 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.js
--rw-r--r--   0        0        0     4460 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.py
--rw-r--r--   0        0        0     1074 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/static/highlight.css
--rw-r--r--   0        0        0     1282 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/test_utils.py
--rw-r--r--   0        0        0      872 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/__init__.py
--rw-r--r--   0        0        0     1678 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/cast_utils.py
--rw-r--r--   0        0        0     2621 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/context.py
--rw-r--r--   0        0        0     8594 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/dataclass_utils.py
--rw-r--r--   0        0        0     5405 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/field_utils.py
--rw-r--r--   0        0        0     8161 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/frozen_utils.py
--rw-r--r--   0        0        0     5001 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/helpers.py
--rw-r--r--   0        0        0     1919 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/__init__.py
--rw-r--r--   0        0        0     3680 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_spec.py
--rw-r--r--   0        0        0      603 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/__init__.py
--rw-r--r--   0        0        0     7867 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/dtypes.py
--rw-r--r--   0        0        0     3677 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/typing.py
--rw-r--r--   0        0        0     9794 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/checking.py
--rw-r--r--   0        0        0     4233 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/compat.py
--rw-r--r--   0        0        0     2726 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/geo_utils.py
--rw-r--r--   0        0        0     4128 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/interp_utils.py
--rw-r--r--   0        0        0     1034 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/linalg.py
--rw-r--r--   0        0        0    10814 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/numpy_utils.py
--rw-r--r--   0        0        0     2804 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/testing.py
--rw-r--r--   0        0        0     2086 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/type_parsing.py
--rw-r--r--   0        0        0     2192 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/typing.py
--rw-r--r--   0        0        0      995 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/__init__.py
--rw-r--r--   0        0        0     6239 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/abstract_path.py
--rw-r--r--   0        0        0     9084 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/backend.py
--rw-r--r--   0        0        0     3159 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/flags.py
--rw-r--r--   0        0        0     9026 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/gpath.py
--rw-r--r--   0        0        0     3410 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/register.py
--rw-r--r--   0        0        0     4937 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/resource_utils.py
--rw-r--r--   0        0        0      922 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/stat_utils.py
--rw-r--r--   0        0        0     4927 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/testing.py
--rw-r--r--   0        0        0      940 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/typing.py
--rw-r--r--   0        0        0     1467 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/_internal.py
--rw-r--r--   0        0        0     1629 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/backports.py
--rw-r--r--   0        0        0     2173 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/contextlib.py
--rw-r--r--   0        0        0     1097 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/env_utils.py
--rw-r--r--   0        0        0     3777 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/itertools.py
--rw-r--r--   0        0        0     4060 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/py_utils.py
--rw-r--r--   0        0        0     4859 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/reraise_utils.py
--rw-r--r--   0        0        0     2843 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/testing.py
--rw-r--r--   0        0        0     6165 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/text_utils.py
--rw-r--r--   0        0        0      642 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etqdm/__init__.py
--rw-r--r--   0        0        0     1454 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etqdm/tqdm_utils.py
--rw-r--r--   0        0        0     1195 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/__init__.py
--rw-r--r--   0        0        0     7798 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/backend.py
--rw-r--r--   0        0        0     4998 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/tree_utils.py
--rw-r--r--   0        0        0      906 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/typing.py
--rw-r--r--   0        0        0     1049 2023-05-12 12:49:33.033113 etils-1.3.0/etils/lazy_imports/__init__.py
--rw-r--r--   0        0        0     2893 2023-05-12 12:49:33.033113 etils-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 etils-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 14:31:41.665450 etils-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2167 2023-07-25 14:31:41.665450 etils-1.4.0/README.md
+-rw-r--r--   0        0        0      859 2023-07-25 14:31:41.665450 etils-1.4.0/etils/__init__.py
+-rw-r--r--   0        0        0     1412 2023-07-25 14:31:41.665450 etils-1.4.0/etils/array_types/__init__.py
+-rw-r--r--   0        0        0      720 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/__init__.py
+-rw-r--r--   0        0        0     2740 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/dataclass_flags.py
+-rw-r--r--   0        0        0     3770 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/logging_utils.py
+-rw-r--r--   0        0        0     1318 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/__init__.py
+-rw-r--r--   0        0        0     6379 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/array_as_img.py
+-rw-r--r--   0        0        0     6099 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/cell_autoreload.py
+-rw-r--r--   0        0        0     5442 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/colab_utils.py
+-rw-r--r--   0        0        0     1511 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/highlight_util.py
+-rw-r--r--   0        0        0     8136 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inplace_reload.py
+-rw-r--r--   0        0        0      583 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/__init__.py
+-rw-r--r--   0        0        0     1500 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/attrs.py
+-rw-r--r--   0        0        0     2354 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/auto_utils.py
+-rw-r--r--   0        0        0     2050 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/core.py
+-rw-r--r--   0        0        0     2047 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/html_helper.py
+-rw-r--r--   0        0        0    14441 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/nodes.py
+-rw-r--r--   0        0        0     1540 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/resource_utils.py
+-rw-r--r--   0        0        0      191 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/auto_activate.css
+-rw-r--r--   0        0        0     1500 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/auto_activate.js
+-rw-r--r--   0        0        0     2487 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/main.js
+-rw-r--r--   0        0        0     2557 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/theme.css
+-rw-r--r--   0        0        0     1713 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/ip_utils.py
+-rw-r--r--   0        0        0     5529 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/lazy_imports.py
+-rw-r--r--   0        0        0    11303 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/lazy_utils.py
+-rw-r--r--   0        0        0     4436 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/module_utils.py
+-rw-r--r--   0        0        0     2441 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/patch_utils.py
+-rw-r--r--   0        0        0      756 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/__init__.py
+-rw-r--r--   0        0        0     3031 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.js
+-rw-r--r--   0        0        0     4460 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.py
+-rw-r--r--   0        0        0     1074 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/static/highlight.css
+-rw-r--r--   0        0        0     1282 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/test_utils.py
+-rw-r--r--   0        0        0      872 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/__init__.py
+-rw-r--r--   0        0        0     1678 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/cast_utils.py
+-rw-r--r--   0        0        0     2621 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/context.py
+-rw-r--r--   0        0        0     8532 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/dataclass_utils.py
+-rw-r--r--   0        0        0     5405 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/field_utils.py
+-rw-r--r--   0        0        0     8161 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/frozen_utils.py
+-rw-r--r--   0        0        0     5001 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/helpers.py
+-rw-r--r--   0        0        0     1919 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/__init__.py
+-rw-r--r--   0        0        0     3752 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_spec.py
+-rw-r--r--   0        0        0      603 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/__init__.py
+-rw-r--r--   0        0        0     7867 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/dtypes.py
+-rw-r--r--   0        0        0     3725 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/typing.py
+-rw-r--r--   0        0        0     9794 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/checking.py
+-rw-r--r--   0        0        0     4233 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/compat.py
+-rw-r--r--   0        0        0     2726 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/geo_utils.py
+-rw-r--r--   0        0        0     4128 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/interp_utils.py
+-rw-r--r--   0        0        0     1034 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/linalg.py
+-rw-r--r--   0        0        0    10836 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/numpy_utils.py
+-rw-r--r--   0        0        0     2804 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/testing.py
+-rw-r--r--   0        0        0     2086 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/type_parsing.py
+-rw-r--r--   0        0        0     2063 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/typing.py
+-rw-r--r--   0        0        0      995 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/__init__.py
+-rw-r--r--   0        0        0     6237 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/abstract_path.py
+-rw-r--r--   0        0        0     9479 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/backend.py
+-rw-r--r--   0        0        0     3159 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/flags.py
+-rw-r--r--   0        0        0     9026 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/gpath.py
+-rw-r--r--   0        0        0     3410 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/register.py
+-rw-r--r--   0        0        0     4937 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/resource_utils.py
+-rw-r--r--   0        0        0     1078 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/stat_utils.py
+-rw-r--r--   0        0        0     4927 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/testing.py
+-rw-r--r--   0        0        0      940 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/typing.py
+-rw-r--r--   0        0        0     1559 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/__init__.py
+-rw-r--r--   0        0        0     1622 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/_internal.py
+-rw-r--r--   0        0        0     1629 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/backports.py
+-rw-r--r--   0        0        0     2173 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/contextlib.py
+-rw-r--r--   0        0        0     1097 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/env_utils.py
+-rw-r--r--   0        0        0     3777 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/itertools.py
+-rw-r--r--   0        0        0     3361 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/lazy_imports_utils.py
+-rw-r--r--   0        0        0     4135 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/py_utils.py
+-rw-r--r--   0        0        0     4859 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/reraise_utils.py
+-rw-r--r--   0        0        0     2843 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/testing.py
+-rw-r--r--   0        0        0     6205 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/text_utils.py
+-rw-r--r--   0        0        0      642 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etqdm/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etqdm/tqdm_utils.py
+-rw-r--r--   0        0        0     1195 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/__init__.py
+-rw-r--r--   0        0        0     8009 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/backend.py
+-rw-r--r--   0        0        0     4998 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/tree_utils.py
+-rw-r--r--   0        0        0      906 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/typing.py
+-rw-r--r--   0        0        0      965 2023-07-25 14:31:41.677450 etils-1.4.0/etils/lazy_imports/__init__.py
+-rw-r--r--   0        0        0     3099 2023-07-25 14:31:41.677450 etils-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 etils-1.4.0/PKG-INFO
```

### Comparing `etils-1.3.0/LICENSE` & `etils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/__init__.py` & `etils-1.4.0/etils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Etils API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 
 # Do NOT add anything to this file. This is left empty on purpose.
 # Users should import subprojects directly.
```

### Comparing `etils-1.3.0/etils/array_types/__init__.py` & `etils-1.4.0/etils/array_types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,9 @@
 complex64 = enp.typing.complex64
 complex128 = enp.typing.complex128
 bool_ = enp.typing.bool_
 
 # Random number generator jax key
 PRNGKey = enp.typing.PRNGKey
 
-# TODO(epot): Those aliases should be deprecated. Should remame usage
-dtypes = enp.dtypes
-typing = enp.array_types.typing
-
-__all__ = enp.typing.__all__
-
 # Keep API clean
 del enp
```

### Comparing `etils-1.3.0/etils/eapp/__init__.py` & `etils-1.4.0/etils/eapp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/eapp/dataclass_flags.py` & `etils-1.4.0/etils/eapp/dataclass_flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/eapp/logging_utils.py` & `etils-1.4.0/etils/eapp/logging_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/__init__.py` & `etils-1.4.0/etils/ecolab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Colab public API."""
 
+# pylint: disable=g-importing-member
+
 from etils.ecolab.array_as_img import auto_plot_array
 from etils.ecolab.colab_utils import collapse
 from etils.ecolab.colab_utils import interruptible
 from etils.ecolab.colab_utils import json
 from etils.ecolab.highlight_util import highlight_html
+from etils.ecolab.inplace_reload import ReloadMode
 from etils.ecolab.inspects.auto_utils import auto_inspect
 from etils.ecolab.inspects.core import inspect
 from etils.ecolab.module_utils import clear_cached_modules
 from etils.ecolab.patch_utils import patch_graphviz
 from etils.ecolab.patch_utils import set_verbose
 from etils.ecolab.pyjs_com import js_import as pyjs_import
 from etils.ecolab.pyjs_com import register_js_fn
```

### Comparing `etils-1.3.0/etils/ecolab/array_as_img.py` & `etils-1.4.0/etils/ecolab/array_as_img.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/colab_utils.py` & `etils-1.4.0/etils/ecolab/colab_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """Colab utils."""
 
 from __future__ import annotations
 
 import contextlib
 import html
-import io
 import json as json_std
 import signal
 import threading
 import typing
 from typing import Iterator, Iterable, TypeVar
 import uuid
 
@@ -32,98 +31,63 @@
   JsonValue = str | float | int | bool | None
   Json = JsonValue | dict[JsonValue, 'Json'] | list['Json']
 
 _T = TypeVar('_T')
 
 
 @contextlib.contextmanager
-def _collapse_std(
-    *,
-    name: str,
-    redirect_fn,
-) -> Iterator[None]:
-  """Base colapsible implementation."""
-  name = html.escape(name)
-  f = io.StringIO()
-  with redirect_fn(f):
-    yield
-  content = f.getvalue()
-  content = html.escape(content)
-  content = f'<pre><code>{content}</code></pre>'
-  content = IPython.display.HTML(
-      f'<details><summary>{name}</summary>{content}</details>'
-  )
-  IPython.display.display(content)
-
-
-@contextlib.contextmanager
-def _redirect_stdall(new_target: io.StringIO) -> Iterator[None]:
-  with contextlib.redirect_stderr(new_target):
-    with contextlib.redirect_stdout(new_target):
-      yield
-
-
-@contextlib.contextmanager
-def collapse(name: str = '', *, widget: bool = False) -> Iterator[None]:
-  """Capture stderr/stdout and display it in a collapsible block.
+def collapse(name: str = '', *, expanded: bool = False) -> Iterator[None]:
+  """Capture all outputs and display it in a collapsible block.
 
   Args:
     name: Name of the collapsible section.
-    widget: If True, use `ipywidgets` backend. Will become the default in the
-      future (output appear in real time, support HTML,...)
+    expanded: If `True`, the section is expanded by default.
 
   Yields:
     None
   """
-  if widget:
-    with _collapse_widget(name):
-      yield
-  else:
-    with _collapse_std(name=name, redirect_fn=_redirect_stdall):
-      yield
-
-
-@contextlib.contextmanager
-def _collapse_widget(name: str = '') -> Iterator[None]:
-  """Widget implementation of Collapsible widget."""
   import ipywidgets  # pylint: disable=g-import-not-at-top
 
   out = ipywidgets.Output()
   accordion = ipywidgets.Accordion(children=[out])
   accordion.set_title(0, name)
-  accordion.selected_index = None
+  if expanded:
+    accordion.selected_index = 0
+  else:
+    accordion.selected_index = None
   IPython.display.display(accordion)
   with out:
     try:
       yield
     except Exception as e:
       # ipywidgets.Output erase exceptions, so we save it and reraise it after
       # the scope.
-      exc = e
+      exc = e  # pylint: disable=unused-variable
       raise
     else:
       exc = None
   if exc is not None:
-    raise exc
+    raise exc  # pylint: disable=g-doc-exception
 
 
-def json(value: Json) -> None:
+def json(value: Json, expanded: bool = False) -> None:
   """Display the Json `dict` / `list` interactivelly (with collapsible elems).
 
   Examples:
 
   ```python
   ecolab.json({'a': [1, 2, 3], 'b': {'x': True, 'y': False}})
   ```
 
   The dict keys and list indices can be filtered from the display field using
   regex (e.g. `a.[0-9]` in the above example).
 
   Args:
     value: Json `dict` or `list` to inspect.
+    expanded: Whether the elements start as expanded or as collapsed.
   """
   # Unique id to make sure multiple Json display do not interact with each other
   id_ = uuid.uuid1().hex
 
   # There are a lot of alternative to `alenaksu/json-viewer`.
   # Likely the most popular one is `react-json-view`. However, this one
   # display preview for collapsible elements, which is nice (and not present
@@ -160,19 +124,21 @@
   }
   .ecolab-json input {
       border-color: var(--colab-highlighted-surface-color);
   }
   """
 
   html_content = html.escape(json_std.dumps(value))
+  # if expanded is True, call viewer.expandAll()
+  expand_line = f'viewer{id_}.expandAll();\n' if expanded else ''
   html_content = f"""
   <script src="https://unpkg.com/@alenaksu/json-viewer@2.0.0/dist/json-viewer.bundle.js"></script>
   <script>
     const viewer{id_} = document.querySelector('#json{id_}');
-    viewer{id_}.expandAll();
+    {expand_line}
   </script>
   <style>
   {css_content}
   </style>
   <div class="ecolab-json">
     <button onclick="viewer{id_}.expandAll();">Expand All</button>
     <button onclick="viewer{id_}.collapseAll();">Collapse All</button>
@@ -188,14 +154,15 @@
 
   While this iterator is running, the first SIGINT (e.g. from interrupting
   the colab runtime, or pressing Ctrl+C ) will not raise an exception but
   instead end the loop after the current iteration.
   A second SIGINT will raise a KeyboardInterrupt Exception as usual.
 
   Examples:
+
   ```python
   for i in interruptible(range(10)):
     print(i)
     time.sleep(3)
   ```
 
   Args:
```

### Comparing `etils-1.3.0/etils/ecolab/highlight_util.py` & `etils-1.4.0/etils/ecolab/highlight_util.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/__init__.py` & `etils-1.4.0/etils/ecolab/inspects/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/attrs.py` & `etils-1.4.0/etils/ecolab/inspects/attrs.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/auto_utils.py` & `etils-1.4.0/etils/ecolab/inspects/auto_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,37 +12,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utils to auto-apply `ecolab.inspect`."""
 
 import functools
 
+from etils.ecolab import ip_utils
 from etils.ecolab import pyjs_com
 from etils.ecolab.inspects import core
 from etils.ecolab.inspects import nodes
 from etils.ecolab.inspects import resource_utils
 import IPython
 import IPython.display
 
 
 @functools.lru_cache(None)
 def auto_inspect() -> None:
   """Add a button on each cell outputs to switch output to `ecolab.inspect`."""
-  ip = IPython.get_ipython()
-
-  # Remove the previous callback (if any)
-  for callback in ip.events.callbacks['post_run_cell']:
-    if hasattr(callback, '__is_auto_inspect__'):
-      ip.events.unregister('post_run_cell', callback)
-      break
-
-  # Mark the function (so it can be cleared when reloaded)
-  _post_run_cell_add_inspect.__is_auto_inspect__ = True
-
-  ip.events.register('post_run_cell', _post_run_cell_add_inspect)
+  ip_utils.register_once(
+      'post_run_cell',
+      _post_run_cell_add_inspect,
+      '__is_auto_inspect__',
+  )
 
 
 def _post_run_cell_add_inspect(*args) -> None:
   """Callback after cell execution to add the `inspect` button."""
   del args  # Future version of IPython will have a `result` arg
 
   # TODO(epot): Detect if IPython has output
```

#### html2text {}

```diff
@@ -2,29 +2,25 @@
 Version 2.0 (the "License"); # you may not use this file except in compliance
 with the License. # You may obtain a copy of the License at # # http://
 www.apache.org/licenses/LICENSE-2.0 # # Unless required by applicable law or
 agreed to in writing, software # distributed under the License is distributed
 on an "AS IS" BASIS, # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. # See the License for the specific language governing
 permissions and # limitations under the License. """Utils to auto-apply
-`ecolab.inspect`.""" import functools from etils.ecolab import pyjs_com from
-etils.ecolab.inspects import core from etils.ecolab.inspects import nodes from
-etils.ecolab.inspects import resource_utils import IPython import
-IPython.display @functools.lru_cache(None) def auto_inspect() -> None: """Add a
-button on each cell outputs to switch output to `ecolab.inspect`.""" ip =
-IPython.get_ipython() # Remove the previous callback (if any) for callback in
-ip.events.callbacks['post_run_cell']: if hasattr(callback,
-'__is_auto_inspect__'): ip.events.unregister('post_run_cell', callback) break #
-Mark the function (so it can be cleared when reloaded)
-_post_run_cell_add_inspect.__is_auto_inspect__ = True ip.events.register
-('post_run_cell', _post_run_cell_add_inspect) def _post_run_cell_add_inspect
-(*args) -> None: """Callback after cell execution to add the `inspect`
-button.""" del args # Future version of IPython will have a `result` arg # TODO
-(epot): Detect if IPython has output # Currently, this add an output because
-`_` is set to the previous # value if no output is set. ip =
+`ecolab.inspect`.""" import functools from etils.ecolab import ip_utils from
+etils.ecolab import pyjs_com from etils.ecolab.inspects import core from
+etils.ecolab.inspects import nodes from etils.ecolab.inspects import
+resource_utils import IPython import IPython.display @functools.lru_cache(None)
+def auto_inspect() -> None: """Add a button on each cell outputs to switch
+output to `ecolab.inspect`.""" ip_utils.register_once( 'post_run_cell',
+_post_run_cell_add_inspect, '__is_auto_inspect__', ) def
+_post_run_cell_add_inspect(*args) -> None: """Callback after cell execution to
+add the `inspect` button.""" del args # Future version of IPython will have a
+`result` arg # TODO(epot): Detect if IPython has output # Currently, this add
+an output because `_` is set to the previous # value if no output is set. ip =
 IPython.get_ipython() # TODO(epot): Store the `last_result` in a weakref to
 avoid memory leaks. last_result = ip.ev('_') root = nodes.Node.from_obj
 (last_result) # TODO(epot): Should not load all `css`/`js` everytime ? #
 Especially the main inspect one which is used only after activation.
 html_content = IPython.display.HTML(f""" {pyjs_com.js_import()}
 {resource_utils.resource_import('auto_activate.css')}
 {resource_utils.resource_import('auto_activate.js')}
```

### Comparing `etils-1.3.0/etils/ecolab/inspects/core.py` & `etils-1.4.0/etils/ecolab/inspects/core.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/html_helper.py` & `etils-1.4.0/etils/ecolab/inspects/html_helper.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/nodes.py` & `etils-1.4.0/etils/ecolab/inspects/nodes.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/resource_utils.py` & `etils-1.4.0/etils/ecolab/inspects/resource_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/static/auto_activate.js` & `etils-1.4.0/etils/ecolab/inspects/static/auto_activate.js`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/static/main.js` & `etils-1.4.0/etils/ecolab/inspects/static/main.js`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/inspects/static/theme.css` & `etils-1.4.0/etils/ecolab/inspects/static/theme.css`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/lazy_imports.py` & `etils-1.4.0/etils/ecolab/lazy_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,61 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Common lazy imports.
-
-Usage:
-
-```python
-from etils.ecolab.lazy_imports import *
-```
-
-To get the list of available modules:
-
-```python
-lazy_imports.__all__  # List of modules aliases
-lazy_imports.LAZY_MODULES  # Mapping <module_alias>: <lazy_module info>
-```
-"""
+"""lazy imports implementation."""
 
 from __future__ import annotations
 
-# Import as alias to avoid closure issues when updating the global()
-import builtins as builtins_
-import contextlib as contextlib_
-import dataclasses as dataclasses_
-import importlib as importlib_
-import traceback as traceback_
-import types as types_
+import builtins
+import contextlib
+import dataclasses
+import importlib
+import traceback
+import types
 from typing import Any, Iterator, Optional
 
-from etils import epy as epy_
-
-
-def __dir__() -> list[str]:  # pylint: disable=invalid-name
-  """`lazy_imports` public API.
-
-  Because `globals()` contains hundreds of symbols, we overwrite `dir(module)`
-  to avoid poluting the namespace during auto-completion.
-
-  Returns:
-    public symbols
-  """
-  # If modifying this, also update the `lazy_imports/__init__.py``
-  return [
-      '__all__',
-      'LAZY_MODULES',
-      'print_current_imports',
-      'LazyModule',
-      'LazyModuleState',
-  ]
+from etils import epy
 
 
 # Attributes which will be updated after the module is loaded.
 _MODULE_ATTR_NAMES = [
     '__builtins__',
     '__cached__',
     '__doc__',
@@ -71,15 +37,15 @@
     '__name__',
     '__package__',
     '__path__',
     '__spec__',
 ]
 
 
-@dataclasses_.dataclass(eq=False)
+@dataclasses.dataclass(eq=False)
 class LazyModuleState:
   """State of the lazy module.
 
   We store the state in a separate object to:
 
   1) Reduce the risk of collision
   2) Avoid infinite recursion error when typo on a attribute
@@ -96,33 +62,33 @@
     _module: Cached original imported module
     trace_repr: Track the trace which trigger the import (Helpful to debug) E.g.
       `Colab` call '.getdoc' on the background, which trigger import.
   """
 
   module_name: str
   alias: str
-  is_std: bool = dataclasses_.field(repr=False, default=False)
-  host: LazyModule = dataclasses_.field(repr=False, default=None)
-  extra_imports: list[str] = dataclasses_.field(default_factory=list)
-  _module: Optional[types_.ModuleType] = None
+  is_std: bool = dataclasses.field(repr=False, default=False)
+  host: LazyModule = dataclasses.field(repr=False, default=None)
+  extra_imports: list[str] = dataclasses.field(default_factory=list)
+  _module: Optional[types.ModuleType] = None
   # Track the trace which trigger the import
   # Helpful to debug.
   # E.g. `Colab` call '.getdoc' on the background, which trigger import.
-  trace_repr: Optional[str] = dataclasses_.field(default=None, repr=False)
+  trace_repr: Optional[str] = dataclasses.field(default=None, repr=False)
 
   @property
-  def module(self) -> types_.ModuleType:
+  def module(self) -> types.ModuleType:
     """Returns the module."""
     if not self.module_loaded:  # Load on first call
       # Keep track of attributes which triggered import
       # Used to track ipython internals (e.g. `<module>.get_traits` gets called
       # internally when ipython inspect the object)
       # So writing `<module>.` trigger module loading & auto-completion even if
       # the module was never used before.
-      self.trace_repr = ''.join(traceback_.format_stack())
+      self.trace_repr = ''.join(traceback.format_stack())
 
       self._module = _load_module(
           self.module_name,
           extra_imports=self.extra_imports,
       )
       # Update the module.__doc__, module.__file__,...
       self._mutate_host()
@@ -160,15 +126,15 @@
       attr_value = getattr(self.module, attr_name, missing)
       if attr_value is not missing:
         object.__setattr__(self.host, attr_name, attr_value)
 
 
 # Class name has to be `module` for Colab compatibility (colab hardcodes class
 # name instead of checking the instance)
-class module(types_.ModuleType):  # pylint: disable=invalid-name
+class module(types.ModuleType):  # pylint: disable=invalid-name
   """Lazy module which auto-loads on first attribute call."""
 
   _etils_state: LazyModuleState
 
   def __init__(self, state: LazyModuleState):
     # We set `__file__` to None, to avoid `colab_import_.reload_package(etils)`
     # to trigger a full reload of all modules here.
@@ -229,48 +195,48 @@
 
 # TODO(epot): Rather than hardcoding which modules are adhoc-imported, this
 # could be a argument.
 def _load_module(
     module_name: str,
     *,
     extra_imports: list[str],
-) -> types_.ModuleType:
+) -> types.ModuleType:
   """Load the module, eventually using adhoc-import."""
-  adhoc_cm = contextlib_.suppress()
+  adhoc_cm = contextlib.suppress()
 
   # First time, load the module
   with adhoc_cm:
     for extra_import in extra_imports:
       # Hardcoded hack to not import tqdm.notebook on non-Colab env
-      if extra_import == 'tqdm.notebook' and not epy_.is_notebook():
+      if extra_import == 'tqdm.notebook' and not epy.is_notebook():
         continue
-      importlib_.import_module(extra_import)
-    return importlib_.import_module(module_name)
+      importlib.import_module(extra_import)
+    return importlib.import_module(module_name)
 
 
-class _LazyImportsBuilder:
+class LazyImportsBuilder:
   """Capture import statements and replace them by lazy-import equivalement."""
 
   def __init__(self, globals_):
     self._globals = globals_
     self.lazy_modules: dict[str, LazyModule] = {}
 
-  @contextlib_.contextmanager
+  @contextlib.contextmanager
   def replace_imports(self, *, is_std: bool) -> Iterator[None]:
     """Replace import statement by their lazy equivalent."""
     # Step 1: Capture all imports by `_ModuleImportProxy`.
 
     # Need to mock `__import__` (instead of `sys.meta_path`, as we do not want
     # to modify the `sys.modules` cache in any way)
-    original_import = builtins_.__import__
+    original_import = builtins.__import__
     try:
-      builtins_.__import__ = _lazy_import
+      builtins.__import__ = _lazy_import
       yield
     finally:
-      builtins_.__import__ = original_import
+      builtins.__import__ = original_import
 
     # Step 1: Replace all `_ModuleImportProxy` by the actual lazy `LazyModule`.
 
     # We need 2 steps otherwise we have no way of knowing the alias used,
     # for example to discriminating between:
     # `import concurrent.futures` => `LazyModule('concurent')`
     # `import concurrent.futures as xxx` => `LazyModule('concurent.future')`
@@ -313,28 +279,28 @@
     return child  # return the inner-most module (`x.y.z`)
   else:
     # import x.y.z
     # import x.y.z as z
     return root  # return the top-level module (`x`)
 
 
-@dataclasses_.dataclass(eq=False)
+@dataclasses.dataclass(eq=False)
 class _ModuleImportProxy:
   """`_ModuleImportProxy` replace all modules during import statement.
 
   ```python
-  with _LazyImportsBuilder().replace_imports():
+  with LazyImportsBuilder().replace_imports():
     import abc.def
     assert isinstance(abc.def, _ModuleImportProxy)
   ```
   """
 
   name: str
   parent: Optional[_ModuleImportProxy] = None
-  children: dict[str, _ModuleImportProxy] = dataclasses_.field(
+  children: dict[str, _ModuleImportProxy] = dataclasses.field(
       default_factory=dict
   )
 
   @property
   def qualname(self) -> str:
     if not self.parent:
       return self.name
@@ -365,31 +331,19 @@
       self.children[name] = type(self)(
           name=name,
           parent=self,
       )
     return self.children[name]
 
 
-def print_current_imports() -> None:
-  """Display the active lazy imports.
-
-  This can be used before publishing a colab. To convert lazy imports
-  into explicit imports.
-
-  For convenience, `from etils.ecolab import lazy_imports` is excluded from
-  the current imports.
-  """
-  print(_current_import_statements())
-
-
-def _current_import_statements() -> str:
+def current_import_statements(lazy_modules: dict[str, LazyModule]) -> str:
   """Returns the lazy import statement string."""
   lines = []
 
-  lazy_modules = [m._etils_state for m in LAZY_MODULES.values()]  # pylint: disable=protected-access
+  lazy_modules = [m._etils_state for m in lazy_modules.values()]  # pylint: disable=protected-access
   used_lazy_modules = [
       # For convenience, we do not add the `lazy_imports` import
       m
       for m in lazy_modules
       if m.module_loaded and m.alias != 'lazy_imports'
   ]
   std_modules = [m.import_statement for m in used_lazy_modules if m.is_std]
@@ -399,164 +353,7 @@
 
   # Import standard python module first, then other modules
   lines.extend(std_modules)
   if std_modules and non_std_modules:
     lines.append('')  # Empty line
   lines.extend(non_std_modules)  # pylint: disable=protected-access
   return '\n'.join(lines)
-
-
-_builder = _LazyImportsBuilder(globals())
-
-
-with _builder.replace_imports(is_std=True):
-  # pylint: disable=g-import-not-at-top,unused-import,reimported
-  import abc
-  import argparse
-  import ast
-  import asyncio
-  import base64
-  import builtins
-  import collections
-  import colorsys
-  import copy
-  import concurrent.futures
-  import contextlib
-  import contextvars
-  import csv
-  import dataclasses
-  import datetime
-  import difflib
-  import dis
-  import enum
-  import functools
-  import gc
-  import gzip
-  import html
-  import inspect
-  import io
-  import importlib
-  import IPython
-  import itertools
-  import json
-  import logging
-  import math
-  import multiprocessing
-  import os
-  import pathlib
-  import pdb
-  import pickle
-  import pprint
-  import queue
-  import random
-  import re
-  import shutil
-  import stat
-  import string
-  import subprocess
-  import sys
-  import tarfile
-  import textwrap
-  import threading
-  import time
-  import timeit
-  import tomllib  # pytype: disable=import-error
-  import traceback
-  import typing  # Note we do not import `Any`, `TypeVar`,...
-  import types
-  import uuid
-  from unittest import mock
-  import warnings
-  import weakref
-  import zipfile
-  # pylint: enable=g-import-not-at-top,unused-import,reimported
-
-
-with _builder.replace_imports(is_std=False):
-  # pylint: disable=g-import-not-at-top,unused-import,reimported
-  # pytype: disable=import-error
-  # ====== Etils ======
-  from etils import array_types
-  from etils import ecolab
-  from etils import edc
-  from etils import enp
-  from etils import epath
-  from etils import epy
-  from etils import etqdm
-  from etils import etree
-  from etils.ecolab import lazy_imports
-  # ====== Common third party ======
-  from absl import app
-  from absl import flags
-  import apache_beam as beam
-  import colabtools
-  from colabtools import interactive_forms
-  import chex
-  import dataclass_array as dca
-  import einops
-  import flask
-  import flax
-  from flax import linen as nn
-  import functorch
-  import gin
-  import graphviz
-  import imageio
-  # Even though `import ipywidgets as widgets` is the common alias, widgets
-  # is likely too ambiguous.
-  import ipywidgets
-  import jax
-  from jax import numpy as jnp
-  import lark
-  import matplotlib
-  import matplotlib as mpl  # Standard alias
-  from matplotlib import pyplot as plt
-  import mediapy as media
-  import ml_collections
-  import networkx as nx
-  import numpy as np
-  import optax
-  import orbax
-  import pandas as pd
-  import PIL
-  from PIL import Image  # Common alias
-  import pycolmap
-  import scipy
-  import seaborn as sns
-  import sklearn
-  import tensorflow as tf
-  import tensorflow.experimental.numpy as tnp
-  import tensorflow_datasets as tfds
-  import torch
-  # from torch import nn  # Collision with flax.linen
-  import torchtext
-  import torchvision
-  import tqdm
-  # tqdm import also trigger additional imports.
-  # TODO(epot): Currently pylance might not infer `tqdm.auto` match
-  # `import tqdm.auto`
-  # Could try to explicitly import inside a `if typing.TYPE_CHECKING:`
-  tqdm.auto  # pylint: disable=pointless-statement
-  tqdm.notebook  # pylint: disable=pointless-statement
-  import tree
-  import typing_extensions
-  import plotly
-  from plotly import express as px
-  from plotly import graph_objects as go
-  import pydantic
-  import requests
-  import sunds
-  import visu3d as v3d
-  from xmanager.contrib import flow as xmflow
-  from xmanager import xm
-  # pytype: enable=import-error
-  # pylint: enable=g-import-not-at-top,unused-import,reimported
-
-
-# Sort the lazy modules per their <module_name>
-LAZY_MODULES: dict[str, LazyModule] = dict(
-    sorted(
-        _builder.lazy_modules.items(),
-        key=lambda x: x[1]._etils_state.module_name,  # pylint: disable=protected-access
-    )
-)
-
-__all__ = sorted(LAZY_MODULES)  # Sorted per alias
```

### Comparing `etils-1.3.0/etils/ecolab/module_utils.py` & `etils-1.4.0/etils/ecolab/module_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,32 @@
 import types
 import typing
 from typing import Sequence, NoReturn, Optional, Union
 
 StrOrStrList = Union[str, Sequence[str]]
 
 
+def get_module_names(restrict: StrOrStrList) -> list[str]:
+  """Returns all `sys.modules` matching the restrict name."""
+
+  modules = normalize_str_to_list(restrict)
+  assert all('/' not in module for module in modules)
+
+  # List all the currently loaded modules matching `modules`
+
+  modules = tuple(modules)
+  modules = [m for m in sys.modules if m.startswith(modules)]
+  return modules
+
+
 def clear_cached_modules(
     modules: StrOrStrList,
     *,
     verbose: bool = False,
     invalidate: bool = True,
-    keep_proto: bool = False,
 ) -> None:
   """Clear the `sys.modules` cache.
 
   Helpful for interactive development to reload from Jupyter notebook the
   code we're currently editing (without having to restart the notebook kernel).
 
   Usage:
@@ -46,39 +58,30 @@
   ```
 
   Args:
     modules: List of modules to clear (all submodules cleared too)
     verbose: Whether to display the list of modules cleared.
     invalidate: If `True` (default), the instances of the module will raise an
       error when used (to avoid using 2 versions of a module at the same time)
-    keep_proto: If `True`, `_pb2` proto files are not removed from the cache.
-      This allow to adhoc import reload projects with protos.
   """
-  modules = normalize_str_to_list(modules)
-  assert all('/' not in module for module in modules)
-
-  # List all the currently loaded modules matching `modules`
-
-  modules = tuple(modules)
-  modules_to_clear = [m for m in sys.modules if m.startswith(modules)]
-  if keep_proto:  # Filter proto modules
-    modules_to_clear = [m for m in modules_to_clear if not _is_proto(m)]
+  modules_to_clear = get_module_names(modules)
+  if not modules_to_clear:
+    return
 
-  # TODO(epot): Make it work with ecolab.lazy_imports
   for module_name in modules_to_clear:
     if verbose:
       print(f'Clearing {module_name}')
     # Clear the parent ref to the module
     _clear_parent_module_attr(module_name)
 
     # We do not invalidate ecolab
     # Note that `reload=['etils']` will still clear `ecolab` from `sys.modules`
     # even if it is not reloaded. In practice, this is fine as `ecolab`
     # should only be imported once in the colab.
-    if invalidate and not module_name.startswith('etils.ecolab'):
+    if invalidate and not module_name.startswith('etils'):
       # Mutate the existing modules to raise an error if accessed
       _invalidate_module(sys.modules[module_name])
 
     del sys.modules[module_name]
 
   # The typing module has side effect by caching `A[B]` from the old modules
   # but thankfully they expose the cleanup method.
```

### Comparing `etils-1.3.0/etils/ecolab/patch_utils.py` & `etils-1.4.0/etils/ecolab/patch_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/pyjs_com/__init__.py` & `etils-1.4.0/etils/ecolab/pyjs_com/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.js` & `etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.js`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.py` & `etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/static/highlight.css` & `etils-1.4.0/etils/ecolab/static/highlight.css`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/ecolab/test_utils.py` & `etils-1.4.0/etils/ecolab/test_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/__init__.py` & `etils-1.4.0/etils/edc/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/cast_utils.py` & `etils-1.4.0/etils/edc/cast_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/context.py` & `etils-1.4.0/etils/edc/context.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/dataclass_utils.py` & `etils-1.4.0/etils/edc/dataclass_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,24 +276,24 @@
 def replace(self: _T, **kwargs: Any) -> _T:
   """Similar to `dataclasses.replace`."""
   return dataclasses.replace(self, **kwargs)
 
 
 def has_default_repr(cls: _Cls) -> bool:
   return (
-      # Use `cls.__dict__` and not `hasattr` to ignore parent classes
-      '__repr__' not in cls.__dict__
-      # `__repr__` exists but is the default dataclass implementation
-      or inspect.unwrap(cls.__repr__).__qualname__
+      inspect.unwrap(cls.__repr__).__qualname__
       == '__create_fn__.<locals>.__repr__'
   )
 
 
 def add_repr(cls: _ClsT) -> _ClsT:
   """Add a `.__repr__` method to the class, if not already present."""
+  # Use `cls.__dict__` and not `hasattr` to ignore parent classes
+  if '__repr__' not in cls.__dict__:
+    return cls
   if has_default_repr(cls):
     cls.__repr__ = __repr__
   return cls
 
 
 @reprlib.recursive_repr()
 def __repr__(self) -> str:  # pylint: disable=invalid-name
```

### Comparing `etils-1.3.0/etils/edc/field_utils.py` & `etils-1.4.0/etils/edc/field_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/frozen_utils.py` & `etils-1.4.0/etils/edc/frozen_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/edc/helpers.py` & `etils-1.4.0/etils/edc/helpers.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/__init__.py` & `etils-1.4.0/etils/enp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/array_spec.py` & `etils-1.4.0/etils/enp/array_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 
   def __eq__(self, other) -> bool:
     if not isinstance(other, type(self)):
       return False
     else:
       return (other.shape, other.dtype) == (self.shape, self.dtype)
 
+  def __hash__(self) -> int:
+    return hash((self.shape, self.dtype))
+
   @classmethod
   def is_array(cls, array: Any) -> bool:
     """Returns `True` if the given value can be converted to `ArraySpec`."""
     try:
       cls.from_array(array)
     except UnknownArrayError:
       return False
```

### Comparing `etils-1.3.0/etils/enp/array_types/__init__.py` & `etils-1.4.0/etils/enp/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/array_types/dtypes.py` & `etils-1.4.0/etils/enp/array_types/dtypes.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/array_types/typing.py` & `etils-1.4.0/etils/enp/array_types/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   same as `f32['... h w c']`.
 
   """
 
   shape: ShapeSpec
   dtype: dtypes.DType
 
-  def __new__(
+  def __new__(  # pylint: disable=bad-mcs-classmethod-argument
       cls,
       shape: Optional[_ShapeSpecInput],
       dtype: Optional[_DType],
   ):
     dtype = dtypes.DType.from_value(dtype)
     # Normalize to str
     if shape is None:
```

### Comparing `etils-1.3.0/etils/enp/checking.py` & `etils-1.4.0/etils/enp/checking.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/compat.py` & `etils-1.4.0/etils/enp/compat.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/geo_utils.py` & `etils-1.4.0/etils/enp/geo_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/interp_utils.py` & `etils-1.4.0/etils/enp/interp_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/linalg.py` & `etils-1.4.0/etils/enp/linalg.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/numpy_utils.py` & `etils-1.4.0/etils/enp/numpy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
   def is_torch_xnp(self, xnp: NpModule) -> bool:
     return self.has_torch and xnp is self.torch
 
   def is_np(self, x: Array) -> bool:
     return isinstance(x, (np.ndarray, np.generic))
 
   def is_tf(self, x: Array) -> bool:
-    return self.has_tf and isinstance(x, self.tnp.ndarray)
+    return self.has_tf and isinstance(x, (self.tnp.ndarray, self.tf.TensorSpec))
 
   def is_jax(self, x: Array) -> bool:
     return self.has_jax and isinstance(x, self.jnp.ndarray)
 
   def is_torch(self, x: Array) -> bool:
     return self.has_torch and isinstance(x, self.torch.Tensor)
```

### Comparing `etils-1.3.0/etils/enp/testing.py` & `etils-1.4.0/etils/enp/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/enp/type_parsing.py` & `etils-1.4.0/etils/enp/type_parsing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/__init__.py` & `etils-1.4.0/etils/epath/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/abstract_path.py` & `etils-1.4.0/etils/epath/abstract_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,20 @@
   @abstractmethod
   def iterdir(self: _T) -> Iterator[_T]:
     """Iterates over the directory."""
     raise NotImplementedError
 
   @abstractmethod
   def glob(self: _T, pattern: str) -> Iterator[_T]:
-    """Yielding all matching files (of any kind)."""
+    """Yields all matching files (of any kind)."""
     # Might be able to implement using `iterdir` (recursivelly for `rglob`).
     raise NotImplementedError
 
   def rglob(self: _T, pattern: str) -> Iterator[_T]:
-    """Yielding all matching files recursivelly (of any kind)."""
+    """Yields all matching files recursively (of any kind)."""
     return self.glob(f'**/{pattern}')
 
   def expanduser(self: _T) -> _T:
     """Returns a new path with expanded `~` and `~user` constructs."""
     if '~' not in self.parts:  # pytype: disable=attribute-error
       return self
     raise NotImplementedError
@@ -136,15 +136,15 @@
 
   def read_bytes(self) -> bytes:
     """Reads contents of self as bytes."""
     with self.open('rb') as f:
       return f.read()
 
   def read_text(self, encoding: Optional[str] = None) -> str:
-    """Reads contents of self as bytes."""
+    """Reads contents of self as a string."""
     with self.open('r', encoding=encoding) as f:
       return f.read()
 
   @abstractmethod
   def stat(self) -> stat_utils.StatResult:
     """Returns metadata for the file/directory."""
     raise NotImplementedError
```

### Comparing `etils-1.3.0/etils/epath/backend.py` & `etils-1.4.0/etils/epath/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,19 +164,30 @@
   def copy(self, path: PathLike, dst: PathLike, overwrite: bool) -> None:
     if not overwrite and self.exists(dst):
       raise FileExistsError(f'{dst} already exists. Cannot copy {path}.')
     shutil.copyfile(path, dst)
 
   def stat(self, path: PathLike) -> stat_utils.StatResult:
     st = os.stat(path)
+    if os.name == 'nt':
+      owner = None
+      group = None
+    else:
+      import grp  # pylint: disable=g-import-not-at-top
+      import pwd  # pylint: disable=g-import-not-at-top
+
+      owner = pwd.getpwuid(st.st_uid).pw_name
+      group = grp.getgrgid(st.st_gid).gr_name
 
     return stat_utils.StatResult(
         is_directory=stat_lib.S_ISDIR(st.st_mode),
         length=st.st_size,
         mtime=int(st.st_mtime),
+        owner=owner,
+        group=group,
     )
 
 
 class _TfBackend(Backend):
   """TensorFlow backend."""
 
   @property
@@ -297,11 +308,13 @@
 
   def stat(self, path: PathLike) -> stat_utils.StatResult:
     st = self.gfile.stat(path)
     return stat_utils.StatResult(
         is_directory=st.is_directory,
         length=st.length,
         mtime=st.mtime_nsec // 1_000_000_000,
+        owner=None,  # Not available.
+        group=None,  # Not available.
     )
 
 tf_backend = _TfBackend()
 os_backend = _OsPathBackend()
```

### Comparing `etils-1.3.0/etils/epath/flags.py` & `etils-1.4.0/etils/epath/flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/gpath.py` & `etils-1.4.0/etils/epath/gpath.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/register.py` & `etils-1.4.0/etils/epath/register.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/resource_utils.py` & `etils-1.4.0/etils/epath/resource_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/testing.py` & `etils-1.4.0/etils/epath/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epath/typing.py` & `etils-1.4.0/etils/epath/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/__init__.py` & `etils-1.4.0/etils/epy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python utils public API."""
 
+# pylint: disable=g-importing-member
+
 import sys
 
 from etils.epy.backports import cached_property
 from etils.epy.contextlib import ContextManager
 from etils.epy.env_utils import is_notebook
 from etils.epy.itertools import groupby
 from etils.epy.itertools import splitby
 from etils.epy.itertools import zip_dict
+from etils.epy.lazy_imports_utils import lazy_imports
 from etils.epy.py_utils import frozen
 from etils.epy.py_utils import issubclass_ as issubclass  # pylint: disable=redefined-builtin
 from etils.epy.py_utils import StrEnum
 from etils.epy.reraise_utils import maybe_reraise
 from etils.epy.reraise_utils import reraise
 from etils.epy.text_utils import dedent
 from etils.epy.text_utils import Lines
```

### Comparing `etils-1.3.0/etils/epy/_internal.py` & `etils-1.4.0/etils/epy/_internal.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """`etils` internal utils."""
 
 import contextlib
-from typing import Iterator
+from typing import Iterator, TypeVar
 
 from etils.epy import reraise_utils
 
+_FnT = TypeVar('_FnT')
+
 
 @contextlib.contextmanager
 def check_missing_deps() -> Iterator[None]:
   """Raise a better error message in case of `ImportError`.
 
   Usage:
 
@@ -44,7 +46,17 @@
     reraise_utils.reraise(
         e,
         suffix=(
             '\nEach etils sub-modules require deps to be installed separately '
             '(e.g. `from etils import ecolab` -> `pip install etils[ecolab]`)'
         ),
     )
+
+
+def unwrap_on_reload(fn: _FnT) -> _FnT:
+  """Unwrap the function to support colab module reload."""
+  if hasattr(fn, '__original_fn__'):
+    fn = fn.__original_fn__
+
+  # Save the original function (to support reload)
+  fn.__original_fn__ = fn
+  return fn
```

### Comparing `etils-1.3.0/etils/epy/backports.py` & `etils-1.4.0/etils/epy/backports.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/contextlib.py` & `etils-1.4.0/etils/epy/contextlib.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/env_utils.py` & `etils-1.4.0/etils/epy/env_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/itertools.py` & `etils-1.4.0/etils/epy/itertools.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/py_utils.py` & `etils-1.4.0/etils/epy/py_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
 
 def _wrap_init(init_fn):
   """`__init__` wrapper."""
 
   @functools.wraps(init_fn)
   def new_init(self, *args, **kwargs):
-    if hasattr(self, '_epy_is_init_done'):
+    # Do NOT use `hasattr` to support children with custom `__getattr__`
+    if '_epy_is_init_done' in self.__dict__:
       # `_epy_is_init_done` already created, so it means we're
       # a `super().__init__` call.
       return init_fn(self, *args, **kwargs)
     object.__setattr__(self, '_epy_is_init_done', False)
     init_fn(self, *args, **kwargs)
     object.__setattr__(self, '_epy_is_init_done', True)
```

### Comparing `etils-1.3.0/etils/epy/reraise_utils.py` & `etils-1.4.0/etils/epy/reraise_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/testing.py` & `etils-1.4.0/etils/epy/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/epy/text_utils.py` & `etils-1.4.0/etils/epy/text_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,15 @@
         content={repr(k): v for k, v in obj.items()},
         braces='{',
         equal=': ',
     )
   elif (
       not isinstance(obj, type)
       and dataclasses.is_dataclass(obj)
+      and obj.__dataclass_params__.repr
       and edc.dataclass_utils.has_default_repr(type(obj))
   ):
     return edc.repr(obj)
   else:
     return repr(obj)
```

### Comparing `etils-1.3.0/etils/etqdm/__init__.py` & `etils-1.4.0/etils/etqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/etqdm/tqdm_utils.py` & `etils-1.4.0/etils/etqdm/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/etree/__init__.py` & `etils-1.4.0/etils/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/etree/backend.py` & `etils-1.4.0/etils/etree/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Tree API backends."""
 
 from __future__ import annotations
 
 import abc
+import collections
 import collections.abc
 import itertools
 import types
 from typing import Any, Callable, TypeVar
 
 from etils import epy
 from etils.etree.typing import Tree
@@ -188,17 +189,21 @@
     raise RuntimeError('Python backend do not have module')
 
   def map(self, map_fn, *trees):
     tree0 = trees[0]
     if isinstance(tree0, _SEQUENCE_TYPES):
       return type(tree0)(self.map(map_fn, *v) for v in zip(*trees))
     elif isinstance(tree0, _MAPPING_TYPES):
-      return type(tree0)(
-          (k, self.map(map_fn, *v)) for k, v in epy.zip_dict(*trees)
-      )
+      new_items = ((k, self.map(map_fn, *v)) for k, v in epy.zip_dict(*trees))
+      if isinstance(tree0, collections.defaultdict):
+        new_tree = type(tree0)(tree0.default_factory)
+        new_tree.update(new_items)
+        return new_tree
+      else:
+        return type(tree0)(new_items)
     else:  # leaf
       return map_fn(*trees)
 
   def flatten(self, tree):
     return list(self._flatten(tree)), tree
 
   def _flatten(self, tree):
```

### Comparing `etils-1.3.0/etils/etree/tree_utils.py` & `etils-1.4.0/etils/etree/tree_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/etree/typing.py` & `etils-1.4.0/etils/etree/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.3.0/etils/lazy_imports/__init__.py` & `etils-1.4.0/etils/lazy_imports/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,12 +17,10 @@
 from etils.ecolab import lazy_imports
 from etils.ecolab.lazy_imports import *
 
 # `import *` only import symbols defined in `__all__`, so manually import
 # additional symbols
 LAZY_MODULES = lazy_imports.LAZY_MODULES
 print_current_imports = lazy_imports.print_current_imports
-LazyModule = lazy_imports.LazyModule
-LazyModuleState = lazy_imports.LazyModuleState
 
 __dir__ = lazy_imports.__dir__
 __all__ = lazy_imports.__all__
```

### Comparing `etils-1.3.0/pyproject.toml` & `etils-1.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "etils"
 description = "Collection of common python utils"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "Conchylicultor", email="etils@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
     # Note: Python and license automatically added by some tools
@@ -23,15 +23,16 @@
 
 # This is set automatically by flit using `etils.__version__`
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/google/etils"
 repository = "https://github.com/google/etils"
-# Other: `documentation`, `changelog`
+documentation = "https://etils.readthedocs.io"
+changelog = "https://github.com/google/etils/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 array-types = [
     # Do not add anything here. `array_types` is an alias for `enp`
     "etils[enp]",
 ]
 eapp = [
@@ -114,14 +115,19 @@
     "pyink",
     "pylint>=2.6.0",
     # Lazy deps
     "chex",
     # "grain",  # For `etree.spec_like`  # TODO(epot): Add once released
     "torch",
     "optree",  # For `etree.optree`
+    "dataclass_array",  # To test lazy_imports
+]
+docs = [
+    "sphinx-apitree[ext]",
+    "etils[dev,all]",  # Install lazy deps
 ]
 
 [tool.flit.sdist]
 # Do not release tests, doc on PyPI
 exclude = [
   "*/**/README.md",
   "**/docs/**",
```

### Comparing `etils-1.3.0/PKG-INFO` & `etils-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: etils
-Version: 1.3.0
+Version: 1.4.0
 Summary: Collection of common python utils
 Keywords: utils,jax,tensorflow,tf,machine learning,deep learning
 Author-email: Conchylicultor <etils@google.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -29,14 +29,17 @@
 Requires-Dist: pytest-subtests ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pyink ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
 Requires-Dist: chex ; extra == "dev"
 Requires-Dist: torch ; extra == "dev"
 Requires-Dist: optree ; extra == "dev"
+Requires-Dist: dataclass_array ; extra == "dev"
+Requires-Dist: sphinx-apitree[ext] ; extra == "docs"
+Requires-Dist: etils[dev,all] ; extra == "docs"
 Requires-Dist: absl-py ; extra == "eapp"
 Requires-Dist: simple_parsing ; extra == "eapp"
 Requires-Dist: etils[epy] ; extra == "eapp"
 Requires-Dist: jupyter ; extra == "ecolab"
 Requires-Dist: numpy ; extra == "ecolab"
 Requires-Dist: mediapy ; extra == "ecolab"
 Requires-Dist: etils[enp] ; extra == "ecolab"
@@ -59,19 +62,22 @@
 Requires-Dist: dm-tree ; extra == "etree-dm"
 Requires-Dist: etils[etree] ; extra == "etree-dm"
 Requires-Dist: jax[cpu] ; extra == "etree-jax"
 Requires-Dist: etils[etree] ; extra == "etree-jax"
 Requires-Dist: tensorflow ; extra == "etree-tf"
 Requires-Dist: etils[etree] ; extra == "etree-tf"
 Requires-Dist: etils[ecolab] ; extra == "lazy-imports"
+Project-URL: changelog, https://github.com/google/etils/blob/main/CHANGELOG.md
+Project-URL: documentation, https://etils.readthedocs.io
 Project-URL: homepage, https://github.com/google/etils
 Project-URL: repository, https://github.com/google/etils
 Provides-Extra: all
 Provides-Extra: array-types
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: eapp
 Provides-Extra: ecolab
 Provides-Extra: edc
 Provides-Extra: enp
 Provides-Extra: epath
 Provides-Extra: epath-no-tf
 Provides-Extra: epy
@@ -82,14 +88,15 @@
 Provides-Extra: etree-tf
 Provides-Extra: lazy-imports
 
 # Etils
 
 [![Unittests](https://github.com/google/etils/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google/etils/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/etils.svg)](https://badge.fury.io/py/etils)
+[![Documentation Status](https://readthedocs.org/projects/etils/badge/?version=latest)](https://etils.readthedocs.io/en/latest/?badge=latest)
 
 etils (eclectic utils) is an open-source collection of utils for python.
 
 Each top-level submodule is a **self-contained independent** module (with its
 own `BUILD` rule), meant to be imported individually. To avoid collisions with
 other modules/variables, module names are prefixed by `e` (arbitrary
 convention):
@@ -103,23 +110,23 @@
 
 Becauses each module is independent, only the minimal required libraries are
 imported (for example, importing `epy` won't suffer the cost of importing TF,
 jax,...)
 
 ## Documentation
 
-* [`etils.epath`](https://github.com/google/etils/tree/main/etils/epath): pathlib-like API for `gs://`, `s3://`,...
-* [`etils.etree`](https://github.com/google/etils/tree/main/etils/etree): Tree utils for `tf.nest`, `jax.tree_utils`, DeepMind `tree`.
-* [`etils.enp`](https://github.com/google/etils/tree/main/etils/enp): Numpy utils.
-* [`etils.ecolab`](https://github.com/google/etils/tree/main/etils/ecolab): Colab utils.
-* [`etils.array_types`](https://github.com/google/etils/tree/main/etils/array_types): Typing annotations for jax, numpy,... arrays
-* [`etils.edc`](https://github.com/google/etils/tree/main/etils/edc): Dataclasses utils.
-* [`etils.epy`](https://github.com/google/etils/tree/main/etils/epy): Collection of generic python utils.
-* [`etils.eapp`](https://github.com/google/etils/tree/main/etils/eapp): Absl flags/app utils.
-*  [API design guide](https://github.com/google/etils/tree/main/docs/api-design.md).
+* [`etils.epath`](https://etils.readthedocs.io/en/latest/epath.html): pathlib-like API for `gs://`, `s3://`,...
+* [`etils.etree`](https://etils.readthedocs.io/en/latest/etree.html): Tree utils for `tf.nest`, `jax.tree_utils`, DeepMind `tree`.
+* [`etils.enp`](https://etils.readthedocs.io/en/latest/enp.html): Numpy utils.
+* [`etils.ecolab`](https://etils.readthedocs.io/en/latest/ecolab.html): Colab utils.
+* [`etils.array_types`](https://etils.readthedocs.io/en/latest/array_types.html): Typing annotations for jax, numpy,... arrays
+* [`etils.edc`](https://etils.readthedocs.io/en/latest/edc.html): Dataclasses utils.
+* [`etils.epy`](https://etils.readthedocs.io/en/latest/epy.html): Collection of generic python utils.
+* [`etils.eapp`](https://etils.readthedocs.io/en/latest/eapp.html): Absl flags/app utils.
+*  [API design guide](https://etils.readthedocs.io/en/latest/api-design.html).
 
 ## Installation
 
 Because each module is independent and require different dependencies, you
 can select which modules deps to install:
 
 ```sh
```

