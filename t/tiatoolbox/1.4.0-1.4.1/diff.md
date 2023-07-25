# Comparing `tmp/tiatoolbox-1.4.0.tar.gz` & `tmp/tiatoolbox-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiatoolbox-1.4.0.tar", last modified: Fri May  5 13:47:15 2023, max compression
+gzip compressed data, was "tiatoolbox-1.4.1.tar", last modified: Tue Jul 25 15:23:43 2023, max compression
```

## Comparing `tiatoolbox-1.4.0.tar` & `tiatoolbox-1.4.1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.749420 tiatoolbox-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.761420 tiatoolbox-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_idars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_mapde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_micronet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_nuclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_sccnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_hovernetplus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_multi_task_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_nucleus_instance_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29697 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74022 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_annotation_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_annotation_tilerendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_meta_ngff_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_save_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_slide_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_slide_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_stainaugment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_stainnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tiatoolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tiffreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tileserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tissuemask.py
--rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsi_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsimeta.py
--rw-r--r--   0 runner    (1001) docker     (123)    90197 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsireader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)   124137 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.781421 tiatoolbox-1.4.0/tiatoolbox/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/nucleus_instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/read_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/save_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/semantic_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/show_wsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/slide_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/slide_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/stain_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/tissue_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.785421 tiatoolbox-1.4.0/tiatoolbox/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/pretrained_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/remote_samples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  2018995 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/target_image.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.745420 tiatoolbox-1.4.0/tiatoolbox/data/visualization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.745420 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.793421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    59306 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   125385 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol-ext.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.801421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   670414 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol-ext.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1262003 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol.js
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/polyfill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   747470 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144562 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   917989 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernetplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/idars.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/mapde.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/micronet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/nuclick.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/sccnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/dataset_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/multi_task_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/nucleus_instance_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    33563 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    64566 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/semantic_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/models_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tiatoolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.833422 tiatoolbox-1.4.0/tiatoolbox/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    27806 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/patchextraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/pyramid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.837422 tiatoolbox-1.4.0/tiatoolbox/tools/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57079 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/registration/wsi_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainaugment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/tissuemask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/env_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23901 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31597 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/visualization/tileserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/wsicore/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/ngff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/wsimeta.py
--rw-r--r--   0 runner    (1001) docker     (123)   213228 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/wsireader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.167608 tiatoolbox-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    34956 2023-07-25 15:23:43.167608 tiatoolbox-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.075608 tiatoolbox-1.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 15:23:43.171608 tiatoolbox-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.091608 tiatoolbox-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.099608 tiatoolbox-1.4.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_idars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_mapde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_micronet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_nuclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_sccnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_arch_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_hovernetplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_multi_task_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_nucleus_instance_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29697 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74022 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_annotation_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_annotation_tilerendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_meta_ngff_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_save_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_slide_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_stainaugment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_stainnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_tiatoolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_tiffreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_tileserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_tissuemask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_wsi_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_wsimeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90197 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tests/test_wsireader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.099608 tiatoolbox-1.4.1/tiatoolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.103608 tiatoolbox-1.4.1/tiatoolbox/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/annotation/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124137 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/annotation/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.111608 tiatoolbox-1.4.1/tiatoolbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/nucleus_instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/read_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/save_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/semantic_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/show_wsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/slide_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/stain_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/cli/tissue_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.111608 tiatoolbox-1.4.1/tiatoolbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/pretrained_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/remote_samples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  2018995 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/target_image.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.067608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.067608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.119608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    59306 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   125385 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/ol-ext.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/ol.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.123608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   670414 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/ol-ext.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1262003 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/ol.js
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/polyfill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.143608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   747470 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144562 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   917989 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.143608 tiatoolbox-1.4.1/tiatoolbox/data/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/data/visualization/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.143608 tiatoolbox-1.4.1/tiatoolbox/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.147608 tiatoolbox-1.4.1/tiatoolbox/models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/hovernetplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/idars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/mapde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/micronet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/nuclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/sccnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/architecture/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.151608 tiatoolbox-1.4.1/tiatoolbox/models/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/dataset/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/dataset/dataset_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/dataset/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.155608 tiatoolbox-1.4.1/tiatoolbox/models/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/engine/multi_task_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/engine/nucleus_instance_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33563 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/engine/patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64566 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/engine/semantic_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/models/models_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tiatoolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.159608 tiatoolbox-1.4.1/tiatoolbox/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27806 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/patchextraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/pyramid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.159608 tiatoolbox-1.4.1/tiatoolbox/tools/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57079 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/registration/wsi_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/stainaugment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/stainextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/stainnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/tools/tissuemask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.163608 tiatoolbox-1.4.1/tiatoolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/env_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23901 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31597 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.167608 tiatoolbox-1.4.1/tiatoolbox/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/visualization/tileserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.167608 tiatoolbox-1.4.1/tiatoolbox/wsicore/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/wsicore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.167608 tiatoolbox-1.4.1/tiatoolbox/wsicore/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/wsicore/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/wsicore/metadata/ngff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/wsicore/wsimeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213228 2023-07-25 15:19:54.000000 tiatoolbox-1.4.1/tiatoolbox/wsicore/wsireader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:23:43.103608 tiatoolbox-1.4.1/tiatoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34956 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 15:23:43.000000 tiatoolbox-1.4.1/tiatoolbox.egg-info/top_level.txt
```

### Comparing `tiatoolbox-1.4.0/AUTHORS.md` & `tiatoolbox-1.4.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/CONTRIBUTING.rst` & `tiatoolbox-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/HISTORY.md` & `tiatoolbox-1.4.1/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 1.4.1 (2023-07-25)
+
+### Bug Fixes and Other Changes
+
+- Fix dictionary changed size Error #626 (#605)
+
 ## 1.4.0 (2023-04-24)
 
 ### Major Updates and Feature Improvements
 
 - Adds Python 3.11 support \[experimental\] #500
   - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
 - Removes Python 3.7 support
```

### Comparing `tiatoolbox-1.4.0/LICENSE` & `tiatoolbox-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/Makefile` & `tiatoolbox-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/PKG-INFO` & `tiatoolbox-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiatoolbox
-Version: 1.4.0
+Version: 1.4.1
 Summary: Computational pathology toolbox developed by TIA Centre.
 Home-page: https://github.com/TissueImageAnalytics/tiatoolbox
 Author: TIA Centre
 Author-email: tia@dcs.warwick.ac.uk
 Keywords: tiatoolbox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -173,14 +173,20 @@
     year = {2022}
 }
 ```
 
 
 # History
 
+## 1.4.1 (2023-07-25)
+
+### Bug Fixes and Other Changes
+
+- Fix dictionary changed size Error #626 (#605)
+
 ## 1.4.0 (2023-04-24)
 
 ### Major Updates and Feature Improvements
 
 - Adds Python 3.11 support \[experimental\] #500
   - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
 - Removes Python 3.7 support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.0 Summary: Computational
+Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.1 Summary: Computational
 pathology toolbox developed by TIA Centre. Home-page: https://github.com/
 TissueImageAnalytics/tiatoolbox Author: TIA Centre Author-email:
 tia@dcs.warwick.ac.uk Keywords: tiatoolbox Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -94,40 +94,42 @@
 Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and Shephard, Adam
 and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi and Epstein,
 David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E Ahmed}, doi =
 {10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal = {Communications
 Medicine}, month = {sep}, number = {1}, pages = {120}, publisher = {Springer
 US}, title = {{TIAToolbox as an end-to-end library for advanced tissue image
 analytics}}, url = {https://www.nature.com/articles/s43856-022-00186-5}, volume
-= {2}, year = {2022} } ``` # History ## 1.4.0 (2023-04-24) ### Major Updates
-and Feature Improvements - Adds Python 3.11 support \[experimental\] #500 -
-Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/
-pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-
-python/pull/188 - Removes Python 3.7 support - This allows upgrading all the
-dependencies which were dependent on an older version of Python. - Adds
-Neighbourhood Querying Support To AnnotationStore #540 - This enables easy and
-efficient querying of annotations within a neighbourhood of other annotations.
-- Adds `MultiTaskSegmentor` engine #424 - Fixes an issue with stain
-augmentation to apply augmentation to only tissue regions. - #546 contributed
-by @navidstuv - Filters logger output to stdout instead of stderr. - Fixes #255
-- Allows import of some modules at higher level for improved usability -
-`WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader` -
-`WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta` -
-`HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN`
-can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus,
-IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves `PatchExtractor` performance.
-Updates `WSIPatchDataset` to be consistent. #571 - Updates documentation for
-`License` for clarity on source code and model weights license. ### Changes to
-API - Updates SCCNN architecture to make it consistent with other models. #544
-### Bug Fixes and Other Changes - Fixes Parsing Missing Omero Version NGFF
-Metadata #568 - Fixes #535 raised by @benkamphaus - Fixes reading of DICOM WSIs
-at the correct level #564 - Fixes #529 - Fixes `scipy`, `matplotlib`, `scikit-
-image` deprecated code - Fixes breaking changes in `DICOMWSIReader` to make it
-compatible with latest `wsidicom` version. #539, #580 - Updates `shapely`
-dependency to version >=2.0.0 and fixes any breaking changes. - Fixes bug with
+= {2}, year = {2022} } ``` # History ## 1.4.1 (2023-07-25) ### Bug Fixes and
+Other Changes - Fix dictionary changed size Error #626 (#605) ## 1.4.0 (2023-
+04-24) ### Major Updates and Feature Improvements - Adds Python 3.11 support \
+[experimental\] #500 - Python 3.11 is not fully supported by `pytorch` https://
+github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/
+openslide/openslide-python/pull/188 - Removes Python 3.7 support - This allows
+upgrading all the dependencies which were dependent on an older version of
+Python. - Adds Neighbourhood Querying Support To AnnotationStore #540 - This
+enables easy and efficient querying of annotations within a neighbourhood of
+other annotations. - Adds `MultiTaskSegmentor` engine #424 - Fixes an issue
+with stain augmentation to apply augmentation to only tissue regions. - #546
+contributed by @navidstuv - Filters logger output to stdout instead of stderr.
+- Fixes #255 - Allows import of some modules at higher level for improved
+usability - `WSIReader` can now be imported as `from tiatoolbox.wsicore import
+WSIReader` - `WSIMeta` can now be imported as `from tiatoolbox.wsicore import
+WSIMeta` - `HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`,
+`SCCNN` can now be imported as \`from tiatoolbox.models import HoVerNet,
+HoVerNetPlus, IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves
+`PatchExtractor` performance. Updates `WSIPatchDataset` to be consistent. #571
+- Updates documentation for `License` for clarity on source code and model
+weights license. ### Changes to API - Updates SCCNN architecture to make it
+consistent with other models. #544 ### Bug Fixes and Other Changes - Fixes
+Parsing Missing Omero Version NGFF Metadata #568 - Fixes #535 raised by
+@benkamphaus - Fixes reading of DICOM WSIs at the correct level #564 - Fixes
+#529 - Fixes `scipy`, `matplotlib`, `scikit-image` deprecated code - Fixes
+breaking changes in `DICOMWSIReader` to make it compatible with latest
+`wsidicom` version. #539, #580 - Updates `shapely` dependency to version
+>=2.0.0 and fixes any breaking changes. - Fixes bug with
 `DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate
 given. - Partly Fixes #532 raised by @blaginin - Fixes local tests for Windows/
 Linux - Fixes `flake8`, `deepsource` errors. - Uses `logger` instead of
 `warnings` and `print` statements to properly log runs. ### Development related
 changes - Upgrades dependencies which are dependent on Python 3.7 - Moves
 `requirements*.txt` files to `requirements` folder - Removes `tox` - Uses
 `pyproject.toml` for `bdist_wheel`, `pytest` and `isort` - Adds `joblib` and
```

### Comparing `tiatoolbox-1.4.0/README.md` & `tiatoolbox-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/pyproject.toml` & `tiatoolbox-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/requirements/requirements.txt` & `tiatoolbox-1.4.1/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/setup.cfg` & `tiatoolbox-1.4.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.0
+current_version = 1.4.1
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `tiatoolbox-1.4.0/setup.py` & `tiatoolbox-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,10 +59,10 @@
     keywords="tiatoolbox",
     name="tiatoolbox",
     packages=find_packages(include=["tiatoolbox", "tiatoolbox.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/TissueImageAnalytics/tiatoolbox",
-    version="1.4.0",
+    version="1.4.1",
     zip_safe=False,
 )
```

### Comparing `tiatoolbox-1.4.0/tests/conftest.py` & `tiatoolbox-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_abc.py` & `tiatoolbox-1.4.1/tests/models/test_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_idars.py` & `tiatoolbox-1.4.1/tests/models/test_arch_idars.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_mapde.py` & `tiatoolbox-1.4.1/tests/models/test_arch_mapde.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_micronet.py` & `tiatoolbox-1.4.1/tests/models/test_arch_micronet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_nuclick.py` & `tiatoolbox-1.4.1/tests/models/test_arch_nuclick.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_sccnn.py` & `tiatoolbox-1.4.1/tests/models/test_arch_sccnn.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_unet.py` & `tiatoolbox-1.4.1/tests/models/test_arch_unet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_utils.py` & `tiatoolbox-1.4.1/tests/models/test_arch_utils.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_arch_vanilla.py` & `tiatoolbox-1.4.1/tests/models/test_arch_vanilla.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_dataset.py` & `tiatoolbox-1.4.1/tests/models/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_feature_extractor.py` & `tiatoolbox-1.4.1/tests/models/test_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_hovernet.py` & `tiatoolbox-1.4.1/tests/models/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_hovernetplus.py` & `tiatoolbox-1.4.1/tests/models/test_hovernetplus.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_multi_task_segmentor.py` & `tiatoolbox-1.4.1/tests/models/test_multi_task_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_nucleus_instance_segmentor.py` & `tiatoolbox-1.4.1/tests/models/test_nucleus_instance_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_patch_predictor.py` & `tiatoolbox-1.4.1/tests/models/test_patch_predictor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/models/test_semantic_segmentation.py` & `tiatoolbox-1.4.1/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_annotation_stores.py` & `tiatoolbox-1.4.1/tests/test_annotation_stores.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_annotation_tilerendering.py` & `tiatoolbox-1.4.1/tests/test_annotation_tilerendering.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_data.py` & `tiatoolbox-1.4.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_docs.py` & `tiatoolbox-1.4.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_dsl.py` & `tiatoolbox-1.4.1/tests/test_dsl.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_exceptions.py` & `tiatoolbox-1.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_graph.py` & `tiatoolbox-1.4.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_init.py` & `tiatoolbox-1.4.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_meta_ngff_dataclasses.py` & `tiatoolbox-1.4.1/tests/test_meta_ngff_dataclasses.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_metrics.py` & `tiatoolbox-1.4.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_patch_extraction.py` & `tiatoolbox-1.4.1/tests/test_patch_extraction.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_pyramid.py` & `tiatoolbox-1.4.1/tests/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_save_tiles.py` & `tiatoolbox-1.4.1/tests/test_save_tiles.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_scale.py` & `tiatoolbox-1.4.1/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_slide_info.py` & `tiatoolbox-1.4.1/tests/test_slide_info.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_slide_thumbnail.py` & `tiatoolbox-1.4.1/tests/test_slide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_stainaugment.py` & `tiatoolbox-1.4.1/tests/test_stainaugment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_stainnorm.py` & `tiatoolbox-1.4.1/tests/test_stainnorm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_tiatoolbox.py` & `tiatoolbox-1.4.1/tests/test_tiatoolbox.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_tiffreader.py` & `tiatoolbox-1.4.1/tests/test_tiffreader.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_tileserver.py` & `tiatoolbox-1.4.1/tests/test_tileserver.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_tissuemask.py` & `tiatoolbox-1.4.1/tests/test_tissuemask.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_utils.py` & `tiatoolbox-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_visualization.py` & `tiatoolbox-1.4.1/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_wsi_registration.py` & `tiatoolbox-1.4.1/tests/test_wsi_registration.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_wsimeta.py` & `tiatoolbox-1.4.1/tests/test_wsimeta.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tests/test_wsireader.py` & `tiatoolbox-1.4.1/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/__init__.py` & `tiatoolbox-1.4.1/tiatoolbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 import pkg_resources
 import yaml
 
 __author__ = """TIA Lab"""
 __email__ = "tialab@dcs.warwick.ac.uk"
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 # This will set the tiatoolbox external data
 # default to be the user home folder, should work on both Window and Unix/Linux
 # C:\Users\USER\.tiatoolbox
 # /home/USER/.tiatoolbox
 
 # Initialize internal logging facilities, such that models etc.
```

### Comparing `tiatoolbox-1.4.0/tiatoolbox/annotation/dsl.py` & `tiatoolbox-1.4.1/tiatoolbox/annotation/dsl.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/annotation/storage.py` & `tiatoolbox-1.4.1/tiatoolbox/annotation/storage.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/__init__.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/common.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/common.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/nucleus_instance_segment.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/nucleus_instance_segment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/patch_predictor.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/patch_predictor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/read_bounds.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/read_bounds.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/save_tiles.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/save_tiles.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/semantic_segment.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/semantic_segment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/show_wsi.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/show_wsi.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/slide_info.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/slide_info.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/slide_thumbnail.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/slide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/stain_norm.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/stain_norm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/cli/tissue_mask.py` & `tiatoolbox-1.4.1/tiatoolbox/cli/tissue_mask.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/__init__.py` & `tiatoolbox-1.4.1/tiatoolbox/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/pretrained_model.yaml` & `tiatoolbox-1.4.1/tiatoolbox/data/pretrained_model.yaml`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/remote_samples.yaml` & `tiatoolbox-1.4.1/tiatoolbox/data/remote_samples.yaml`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/target_image.png` & `tiatoolbox-1.4.1/tiatoolbox/data/target_image.png`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol-ext.min.css` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/ol-ext.min.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol.css` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/css/ol.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol-ext.min.js` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/ol-ext.min.js`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol.js` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/js/ol.js`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/index.html` & `tiatoolbox-1.4.1/tiatoolbox/data/visualization/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/__init__.py` & `tiatoolbox-1.4.1/tiatoolbox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/__init__.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernet.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/hovernet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernetplus.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/hovernetplus.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/idars.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/idars.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/mapde.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/mapde.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/micronet.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/micronet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/nuclick.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/nuclick.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/sccnn.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/sccnn.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/unet.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/unet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/utils.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/utils.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/architecture/vanilla.py` & `tiatoolbox-1.4.1/tiatoolbox/models/architecture/vanilla.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/dataset/classification.py` & `tiatoolbox-1.4.1/tiatoolbox/models/dataset/classification.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/dataset/dataset_abc.py` & `tiatoolbox-1.4.1/tiatoolbox/models/dataset/dataset_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/dataset/info.py` & `tiatoolbox-1.4.1/tiatoolbox/models/dataset/info.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/engine/multi_task_segmentor.py` & `tiatoolbox-1.4.1/tiatoolbox/models/engine/multi_task_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/engine/nucleus_instance_segmentor.py` & `tiatoolbox-1.4.1/tiatoolbox/models/engine/nucleus_instance_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/engine/patch_predictor.py` & `tiatoolbox-1.4.1/tiatoolbox/models/engine/patch_predictor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/engine/semantic_segmentor.py` & `tiatoolbox-1.4.1/tiatoolbox/models/engine/semantic_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/models/models_abc.py` & `tiatoolbox-1.4.1/tiatoolbox/models/models_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/graph.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/graph.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/patchextraction.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/patchextraction.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/pyramid.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/pyramid.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/registration/wsi_registration.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/registration/wsi_registration.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/stainaugment.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/stainaugment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/stainextract.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/stainextract.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/stainnorm.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/stainnorm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/tools/tissuemask.py` & `tiatoolbox-1.4.1/tiatoolbox/tools/tissuemask.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/env_detection.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/env_detection.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/image.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/image.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/metrics.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/misc.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/transforms.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/utils/visualization.py` & `tiatoolbox-1.4.1/tiatoolbox/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/visualization/tileserver.py` & `tiatoolbox-1.4.1/tiatoolbox/visualization/tileserver.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/ngff.py` & `tiatoolbox-1.4.1/tiatoolbox/wsicore/metadata/ngff.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/wsicore/wsimeta.py` & `tiatoolbox-1.4.1/tiatoolbox/wsicore/wsimeta.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox/wsicore/wsireader.py` & `tiatoolbox-1.4.1/tiatoolbox/wsicore/wsireader.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox.egg-info/PKG-INFO` & `tiatoolbox-1.4.1/tiatoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiatoolbox
-Version: 1.4.0
+Version: 1.4.1
 Summary: Computational pathology toolbox developed by TIA Centre.
 Home-page: https://github.com/TissueImageAnalytics/tiatoolbox
 Author: TIA Centre
 Author-email: tia@dcs.warwick.ac.uk
 Keywords: tiatoolbox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -173,14 +173,20 @@
     year = {2022}
 }
 ```
 
 
 # History
 
+## 1.4.1 (2023-07-25)
+
+### Bug Fixes and Other Changes
+
+- Fix dictionary changed size Error #626 (#605)
+
 ## 1.4.0 (2023-04-24)
 
 ### Major Updates and Feature Improvements
 
 - Adds Python 3.11 support \[experimental\] #500
   - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
 - Removes Python 3.7 support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.0 Summary: Computational
+Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.1 Summary: Computational
 pathology toolbox developed by TIA Centre. Home-page: https://github.com/
 TissueImageAnalytics/tiatoolbox Author: TIA Centre Author-email:
 tia@dcs.warwick.ac.uk Keywords: tiatoolbox Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -94,40 +94,42 @@
 Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and Shephard, Adam
 and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi and Epstein,
 David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E Ahmed}, doi =
 {10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal = {Communications
 Medicine}, month = {sep}, number = {1}, pages = {120}, publisher = {Springer
 US}, title = {{TIAToolbox as an end-to-end library for advanced tissue image
 analytics}}, url = {https://www.nature.com/articles/s43856-022-00186-5}, volume
-= {2}, year = {2022} } ``` # History ## 1.4.0 (2023-04-24) ### Major Updates
-and Feature Improvements - Adds Python 3.11 support \[experimental\] #500 -
-Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/
-pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-
-python/pull/188 - Removes Python 3.7 support - This allows upgrading all the
-dependencies which were dependent on an older version of Python. - Adds
-Neighbourhood Querying Support To AnnotationStore #540 - This enables easy and
-efficient querying of annotations within a neighbourhood of other annotations.
-- Adds `MultiTaskSegmentor` engine #424 - Fixes an issue with stain
-augmentation to apply augmentation to only tissue regions. - #546 contributed
-by @navidstuv - Filters logger output to stdout instead of stderr. - Fixes #255
-- Allows import of some modules at higher level for improved usability -
-`WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader` -
-`WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta` -
-`HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN`
-can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus,
-IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves `PatchExtractor` performance.
-Updates `WSIPatchDataset` to be consistent. #571 - Updates documentation for
-`License` for clarity on source code and model weights license. ### Changes to
-API - Updates SCCNN architecture to make it consistent with other models. #544
-### Bug Fixes and Other Changes - Fixes Parsing Missing Omero Version NGFF
-Metadata #568 - Fixes #535 raised by @benkamphaus - Fixes reading of DICOM WSIs
-at the correct level #564 - Fixes #529 - Fixes `scipy`, `matplotlib`, `scikit-
-image` deprecated code - Fixes breaking changes in `DICOMWSIReader` to make it
-compatible with latest `wsidicom` version. #539, #580 - Updates `shapely`
-dependency to version >=2.0.0 and fixes any breaking changes. - Fixes bug with
+= {2}, year = {2022} } ``` # History ## 1.4.1 (2023-07-25) ### Bug Fixes and
+Other Changes - Fix dictionary changed size Error #626 (#605) ## 1.4.0 (2023-
+04-24) ### Major Updates and Feature Improvements - Adds Python 3.11 support \
+[experimental\] #500 - Python 3.11 is not fully supported by `pytorch` https://
+github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/
+openslide/openslide-python/pull/188 - Removes Python 3.7 support - This allows
+upgrading all the dependencies which were dependent on an older version of
+Python. - Adds Neighbourhood Querying Support To AnnotationStore #540 - This
+enables easy and efficient querying of annotations within a neighbourhood of
+other annotations. - Adds `MultiTaskSegmentor` engine #424 - Fixes an issue
+with stain augmentation to apply augmentation to only tissue regions. - #546
+contributed by @navidstuv - Filters logger output to stdout instead of stderr.
+- Fixes #255 - Allows import of some modules at higher level for improved
+usability - `WSIReader` can now be imported as `from tiatoolbox.wsicore import
+WSIReader` - `WSIMeta` can now be imported as `from tiatoolbox.wsicore import
+WSIMeta` - `HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`,
+`SCCNN` can now be imported as \`from tiatoolbox.models import HoVerNet,
+HoVerNetPlus, IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves
+`PatchExtractor` performance. Updates `WSIPatchDataset` to be consistent. #571
+- Updates documentation for `License` for clarity on source code and model
+weights license. ### Changes to API - Updates SCCNN architecture to make it
+consistent with other models. #544 ### Bug Fixes and Other Changes - Fixes
+Parsing Missing Omero Version NGFF Metadata #568 - Fixes #535 raised by
+@benkamphaus - Fixes reading of DICOM WSIs at the correct level #564 - Fixes
+#529 - Fixes `scipy`, `matplotlib`, `scikit-image` deprecated code - Fixes
+breaking changes in `DICOMWSIReader` to make it compatible with latest
+`wsidicom` version. #539, #580 - Updates `shapely` dependency to version
+>=2.0.0 and fixes any breaking changes. - Fixes bug with
 `DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate
 given. - Partly Fixes #532 raised by @blaginin - Fixes local tests for Windows/
 Linux - Fixes `flake8`, `deepsource` errors. - Uses `logger` instead of
 `warnings` and `print` statements to properly log runs. ### Development related
 changes - Upgrades dependencies which are dependent on Python 3.7 - Moves
 `requirements*.txt` files to `requirements` folder - Removes `tox` - Uses
 `pyproject.toml` for `bdist_wheel`, `pytest` and `isort` - Adds `joblib` and
```

### Comparing `tiatoolbox-1.4.0/tiatoolbox.egg-info/SOURCES.txt` & `tiatoolbox-1.4.1/tiatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.4.0/tiatoolbox.egg-info/requires.txt` & `tiatoolbox-1.4.1/tiatoolbox.egg-info/requires.txt`

 * *Files identical despite different names*

