# Comparing `tmp/sdo-cli-0.0.8.tar.gz` & `tmp/sdo-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdo-cli-0.0.8.tar", last modified: Tue Apr 26 14:07:37 2022, max compression
+gzip compressed data, was "dist/sdo-cli-0.0.9.tar", last modified: Tue Apr 26 14:09:28 2022, max compression
```

## Comparing `sdo-cli-0.0.8.tar` & `sdo-cli-0.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.724768 sdo-cli-0.0.8/
--rw-r--r--   0 mariusgiger   (501) staff       (20)     3310 2022-04-26 14:07:37.724231 sdo-cli-0.0.8/PKG-INFO
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2884 2022-04-26 13:19:13.000000 sdo-cli-0.0.8/README.md
--rw-r--r--   0 mariusgiger   (501) staff       (20)       38 2022-04-26 14:07:37.724897 sdo-cli-0.0.8/setup.cfg
--rw-r--r--   0 mariusgiger   (501) staff       (20)     1517 2022-04-26 14:07:21.000000 sdo-cli-0.0.8/setup.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.692463 sdo-cli-0.0.8/src/
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.693599 sdo-cli-0.0.8/src/sdo/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2020-12-29 12:34:14.000000 sdo-cli-0.0.8/src/sdo/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2175 2022-04-26 11:23:34.000000 sdo-cli-0.0.8/src/sdo/cli.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.694966 sdo-cli-0.0.8/src/sdo/cmd/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-29 10:43:21.000000 sdo-cli-0.0.8/src/sdo/cmd/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      275 2021-01-05 11:21:23.000000 sdo-cli-0.0.8/src/sdo/cmd/cmd_data.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      334 2021-08-05 16:46:39.000000 sdo-cli-0.0.8/src/sdo/cmd/cmd_events.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      136 2021-08-08 13:04:57.000000 sdo-cli-0.0.8/src/sdo/cmd/cmd_goes.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      187 2021-08-06 13:12:31.000000 sdo-cli-0.0.8/src/sdo/cmd/cmd_sood.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.697431 sdo-cli-0.0.8/src/sdo/cmd/data/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-29 12:54:57.000000 sdo-cli-0.0.8/src/sdo/cmd/data/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     7331 2021-11-12 14:36:48.000000 sdo-cli-0.0.8/src/sdo/cmd/data/cmd_download.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     3714 2022-01-21 08:49:47.000000 sdo-cli-0.0.8/src/sdo/cmd/data/cmd_patch.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2331 2021-01-26 10:34:37.000000 sdo-cli-0.0.8/src/sdo/cmd/data/cmd_resize.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.698547 sdo-cli-0.0.8/src/sdo/cmd/events/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:44.000000 sdo-cli-0.0.8/src/sdo/cmd/events/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     1248 2022-04-26 08:50:54.000000 sdo-cli-0.0.8/src/sdo/cmd/events/cmd_analyze_events.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      818 2021-08-06 14:26:40.000000 sdo-cli-0.0.8/src/sdo/cmd/events/cmd_list_events.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      896 2021-08-06 14:26:47.000000 sdo-cli-0.0.8/src/sdo/cmd/events/cmd_load_events.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.699197 sdo-cli-0.0.8/src/sdo/cmd/goes/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:40.000000 sdo-cli-0.0.8/src/sdo/cmd/goes/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2138 2022-04-26 11:50:43.000000 sdo-cli-0.0.8/src/sdo/cmd/goes/cmd_download.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.700065 sdo-cli-0.0.8/src/sdo/cmd/sood/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:24.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/__init__.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.701816 sdo-cli-0.0.8/src/sdo/cmd/sood/ae/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2021-08-06 13:12:49.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ae/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2130 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ae/cmd_predict.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     1526 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ae/cmd_train.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.702916 sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2021-08-06 12:37:04.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2737 2022-04-26 11:22:38.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_generate.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2714 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_predict.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2375 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_train.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      178 2021-08-06 13:29:58.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/cmd_ae.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      239 2021-08-06 13:29:17.000000 sdo-cli-0.0.8/src/sdo/cmd/sood/cmd_ce_vae.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.703224 sdo-cli-0.0.8/src/sdo/data_loader/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2020-12-29 13:07:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/__init__.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.703655 sdo-cli-0.0.8/src/sdo/data_loader/image_param/
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.706545 sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2076 2021-02-16 14:56:56.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/CONSTANTS.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     1605 2021-02-16 14:57:02.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/URL_STRINGS.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/__init__.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.706968 sdo-cli-0.0.8/src/sdo/data_loader/image_param/api_wrappers/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/api_wrappers/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)    18910 2021-08-07 12:40:55.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/api_wrappers/api_wrappers.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.707530 sdo-cli-0.0.8/src/sdo/data_loader/image_param/objects/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/objects/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     4896 2021-06-01 08:46:19.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/objects/spatiotemporal_event.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.708782 sdo-cli-0.0.8/src/sdo/data_loader/image_param/utils/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/utils/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     1675 2021-02-16 14:57:22.000000 sdo-cli-0.0.8/src/sdo/data_loader/image_param/utils/coord_convertor.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.709842 sdo-cli-0.0.8/src/sdo/events/
--rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2021-08-06 14:31:09.000000 sdo-cli-0.0.8/src/sdo/events/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)    17168 2021-11-12 10:07:57.000000 sdo-cli-0.0.8/src/sdo/events/bboxes.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     9416 2021-08-17 16:04:17.000000 sdo-cli-0.0.8/src/sdo/events/event_loader.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.710123 sdo-cli-0.0.8/src/sdo/sood/
--rw-rw-r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 08:54:08.000000 sdo-cli-0.0.8/src/sdo/sood/__init__.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.710806 sdo-cli-0.0.8/src/sdo/sood/algorithms/
--rw-rw-r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 08:48:38.000000 sdo-cli-0.0.8/src/sdo/sood/algorithms/__init__.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     9054 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/sood/algorithms/ae_2d.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)    17815 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/sood/algorithms/ce_vae.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.712326 sdo-cli-0.0.8/src/sdo/sood/data/
--rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.8/src/sdo/sood/data/__init__.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)     2765 2022-04-19 10:50:04.000000 sdo-cli-0.0.8/src/sdo/sood/data/image_dataset.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)      694 2021-02-02 18:44:55.000000 sdo-cli-0.0.8/src/sdo/sood/data/path_dataset.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)    11194 2022-04-22 08:58:47.000000 sdo-cli-0.0.8/src/sdo/sood/data/sdo_ml_v1_dataset.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.718193 sdo-cli-0.0.8/src/sdo/sood/models/
--rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.8/src/sdo/sood/models/__init__.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)    10660 2022-04-26 11:22:37.000000 sdo-cli-0.0.8/src/sdo/sood/models/aes.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)    11901 2021-01-31 21:58:01.000000 sdo-cli-0.0.8/src/sdo/sood/models/iwgan_nets.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)    19366 2022-04-12 12:23:41.000000 sdo-cli-0.0.8/src/sdo/sood/models/nets.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.719135 sdo-cli-0.0.8/src/sdo/sood/util/
--rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.8/src/sdo/sood/util/__init__.py
--rw-rw-r--   0 mariusgiger   (501) staff       (20)     6264 2021-01-31 21:58:23.000000 sdo-cli-0.0.8/src/sdo/sood/util/ce_noise.py
--rw-r--r--   0 mariusgiger   (501) staff       (20)     9106 2022-04-19 15:49:12.000000 sdo-cli-0.0.8/src/sdo/sood/util/utils.py
-drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:07:37.723715 sdo-cli-0.0.8/src/sdo_cli.egg-info/
--rw-r--r--   0 mariusgiger   (501) staff       (20)     3310 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/PKG-INFO
--rw-r--r--   0 mariusgiger   (501) staff       (20)     2208 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mariusgiger   (501) staff       (20)       40 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/entry_points.txt
--rw-r--r--   0 mariusgiger   (501) staff       (20)      287 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/requires.txt
--rw-r--r--   0 mariusgiger   (501) staff       (20)        4 2022-04-26 14:07:37.000000 sdo-cli-0.0.8/src/sdo_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.579053 sdo-cli-0.0.9/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     3310 2022-04-26 14:09:28.578631 sdo-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2884 2022-04-26 13:19:13.000000 sdo-cli-0.0.9/README.md
+-rw-r--r--   0 mariusgiger   (501) staff       (20)       38 2022-04-26 14:09:28.579155 sdo-cli-0.0.9/setup.cfg
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     1562 2022-04-26 14:09:26.000000 sdo-cli-0.0.9/setup.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.560821 sdo-cli-0.0.9/src/
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.562217 sdo-cli-0.0.9/src/sdo/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2020-12-29 12:34:14.000000 sdo-cli-0.0.9/src/sdo/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2175 2022-04-26 11:23:34.000000 sdo-cli-0.0.9/src/sdo/cli.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.563612 sdo-cli-0.0.9/src/sdo/cmd/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-29 10:43:21.000000 sdo-cli-0.0.9/src/sdo/cmd/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      275 2021-01-05 11:21:23.000000 sdo-cli-0.0.9/src/sdo/cmd/cmd_data.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      334 2021-08-05 16:46:39.000000 sdo-cli-0.0.9/src/sdo/cmd/cmd_events.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      136 2021-08-08 13:04:57.000000 sdo-cli-0.0.9/src/sdo/cmd/cmd_goes.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      187 2021-08-06 13:12:31.000000 sdo-cli-0.0.9/src/sdo/cmd/cmd_sood.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.564899 sdo-cli-0.0.9/src/sdo/cmd/data/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-29 12:54:57.000000 sdo-cli-0.0.9/src/sdo/cmd/data/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     7331 2021-11-12 14:36:48.000000 sdo-cli-0.0.9/src/sdo/cmd/data/cmd_download.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     3714 2022-01-21 08:49:47.000000 sdo-cli-0.0.9/src/sdo/cmd/data/cmd_patch.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2331 2021-01-26 10:34:37.000000 sdo-cli-0.0.9/src/sdo/cmd/data/cmd_resize.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.565878 sdo-cli-0.0.9/src/sdo/cmd/events/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:44.000000 sdo-cli-0.0.9/src/sdo/cmd/events/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     1248 2022-04-26 08:50:54.000000 sdo-cli-0.0.9/src/sdo/cmd/events/cmd_analyze_events.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      818 2021-08-06 14:26:40.000000 sdo-cli-0.0.9/src/sdo/cmd/events/cmd_list_events.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      896 2021-08-06 14:26:47.000000 sdo-cli-0.0.9/src/sdo/cmd/events/cmd_load_events.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.566324 sdo-cli-0.0.9/src/sdo/cmd/goes/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:40.000000 sdo-cli-0.0.9/src/sdo/cmd/goes/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2138 2022-04-26 11:50:43.000000 sdo-cli-0.0.9/src/sdo/cmd/goes/cmd_download.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.567045 sdo-cli-0.0.9/src/sdo/cmd/sood/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 11:47:24.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/__init__.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.567750 sdo-cli-0.0.9/src/sdo/cmd/sood/ae/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2021-08-06 13:12:49.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ae/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2130 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ae/cmd_predict.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     1526 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ae/cmd_train.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.568697 sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2021-08-06 12:37:04.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2737 2022-04-26 11:22:38.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_generate.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2714 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_predict.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2375 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_train.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      178 2021-08-06 13:29:58.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/cmd_ae.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      239 2021-08-06 13:29:17.000000 sdo-cli-0.0.9/src/sdo/cmd/sood/cmd_ce_vae.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.568949 sdo-cli-0.0.9/src/sdo/data_loader/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2020-12-29 13:07:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/__init__.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.569207 sdo-cli-0.0.9/src/sdo/data_loader/image_param/
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.569918 sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2076 2021-02-16 14:56:56.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/CONSTANTS.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     1605 2021-02-16 14:57:02.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/URL_STRINGS.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/__init__.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.570329 sdo-cli-0.0.9/src/sdo/data_loader/image_param/api_wrappers/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/api_wrappers/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)    18910 2021-08-07 12:40:55.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/api_wrappers/api_wrappers.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.570862 sdo-cli-0.0.9/src/sdo/data_loader/image_param/objects/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/objects/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     4896 2021-06-01 08:46:19.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/objects/spatiotemporal_event.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.571364 sdo-cli-0.0.9/src/sdo/data_loader/image_param/utils/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        0 2020-12-12 16:18:33.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/utils/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     1675 2021-02-16 14:57:22.000000 sdo-cli-0.0.9/src/sdo/data_loader/image_param/utils/coord_convertor.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.572198 sdo-cli-0.0.9/src/sdo/events/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2021-08-06 14:31:09.000000 sdo-cli-0.0.9/src/sdo/events/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)    17168 2021-11-12 10:07:57.000000 sdo-cli-0.0.9/src/sdo/events/bboxes.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     9416 2021-08-17 16:04:17.000000 sdo-cli-0.0.9/src/sdo/events/event_loader.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.572456 sdo-cli-0.0.9/src/sdo/sood/
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 08:54:08.000000 sdo-cli-0.0.9/src/sdo/sood/__init__.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.573090 sdo-cli-0.0.9/src/sdo/sood/algorithms/
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)        0 2022-04-26 08:48:38.000000 sdo-cli-0.0.9/src/sdo/sood/algorithms/__init__.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     9054 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/sood/algorithms/ae_2d.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)    17815 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/sood/algorithms/ce_vae.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.574151 sdo-cli-0.0.9/src/sdo/sood/data/
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.9/src/sdo/sood/data/__init__.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)     2765 2022-04-19 10:50:04.000000 sdo-cli-0.0.9/src/sdo/sood/data/image_dataset.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      694 2021-02-02 18:44:55.000000 sdo-cli-0.0.9/src/sdo/sood/data/path_dataset.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)    11194 2022-04-22 08:58:47.000000 sdo-cli-0.0.9/src/sdo/sood/data/sdo_ml_v1_dataset.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.575230 sdo-cli-0.0.9/src/sdo/sood/models/
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.9/src/sdo/sood/models/__init__.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)    10660 2022-04-26 11:22:37.000000 sdo-cli-0.0.9/src/sdo/sood/models/aes.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)    11901 2021-01-31 21:58:01.000000 sdo-cli-0.0.9/src/sdo/sood/models/iwgan_nets.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)    19366 2022-04-12 12:23:41.000000 sdo-cli-0.0.9/src/sdo/sood/models/nets.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.576146 sdo-cli-0.0.9/src/sdo/sood/util/
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)        1 2020-10-06 14:35:51.000000 sdo-cli-0.0.9/src/sdo/sood/util/__init__.py
+-rw-rw-r--   0 mariusgiger   (501) staff       (20)     6264 2021-01-31 21:58:23.000000 sdo-cli-0.0.9/src/sdo/sood/util/ce_noise.py
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     9106 2022-04-19 15:49:12.000000 sdo-cli-0.0.9/src/sdo/sood/util/utils.py
+drwxr-xr-x   0 mariusgiger   (501) staff       (20)        0 2022-04-26 14:09:28.578230 sdo-cli-0.0.9/src/sdo_cli.egg-info/
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     3310 2022-04-26 14:09:27.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mariusgiger   (501) staff       (20)     2208 2022-04-26 14:09:28.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        1 2022-04-26 14:09:28.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mariusgiger   (501) staff       (20)       40 2022-04-26 14:09:28.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mariusgiger   (501) staff       (20)      307 2022-04-26 14:09:28.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/requires.txt
+-rw-r--r--   0 mariusgiger   (501) staff       (20)        4 2022-04-26 14:09:28.000000 sdo-cli-0.0.9/src/sdo_cli.egg-info/top_level.txt
```

### Comparing `sdo-cli-0.0.8/PKG-INFO` & `sdo-cli-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdo-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ML practitioners utility for working with SDO data.
 Home-page: https://github.com/i4DS/sdo-cli
 Author: Marius Giger
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdo-cli-0.0.8/README.md` & `sdo-cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/setup.py` & `sdo-cli-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sdo-cli",
-    version="0.0.8",
+    version="0.0.9",
     author="Marius Giger",
     description="An ML practitioners utility for working with SDO data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where='src'),
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -23,14 +23,15 @@
                       "drms>=0.6.2",
                       "h5netcdf>=1.0.0",
                       "matplotlib>=3.5.1",
                       "opencv-python>=4.5.5.64",
                       "python-dotenv>=0.20.0",
                       "pandas>=1.4.2",
                       "pytorch-lightning>=1.6.1",
+                      "scikit-learn>=1.0.2",
                       "Shapely>=1.7.1",
                       "SQLAlchemy>=1.4.17",
                       "sunpy>=3.1.6",
                       "torch>=1.11.0",
                       "tqdm>=4.64.0",
                       "torchvision>=0.12.0",
                       "wandb>=0.12.15",
```

### Comparing `sdo-cli-0.0.8/src/sdo/cli.py` & `sdo-cli-0.0.9/src/sdo/cli.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/data/cmd_download.py` & `sdo-cli-0.0.9/src/sdo/cmd/data/cmd_download.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/data/cmd_patch.py` & `sdo-cli-0.0.9/src/sdo/cmd/data/cmd_patch.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/data/cmd_resize.py` & `sdo-cli-0.0.9/src/sdo/cmd/data/cmd_resize.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/events/cmd_analyze_events.py` & `sdo-cli-0.0.9/src/sdo/cmd/events/cmd_analyze_events.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/events/cmd_list_events.py` & `sdo-cli-0.0.9/src/sdo/cmd/events/cmd_list_events.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/events/cmd_load_events.py` & `sdo-cli-0.0.9/src/sdo/cmd/events/cmd_load_events.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/goes/cmd_download.py` & `sdo-cli-0.0.9/src/sdo/cmd/goes/cmd_download.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/sood/ae/cmd_predict.py` & `sdo-cli-0.0.9/src/sdo/cmd/sood/ae/cmd_predict.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/sood/ae/cmd_train.py` & `sdo-cli-0.0.9/src/sdo/cmd/sood/ae/cmd_train.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_generate.py` & `sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_generate.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_predict.py` & `sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_predict.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/cmd/sood/ce_vae/cmd_train.py` & `sdo-cli-0.0.9/src/sdo/cmd/sood/ce_vae/cmd_train.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/CONSTANTS.py` & `sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/data_loader/image_param/IP_CONSTANTS/URL_STRINGS.py` & `sdo-cli-0.0.9/src/sdo/data_loader/image_param/IP_CONSTANTS/URL_STRINGS.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/data_loader/image_param/api_wrappers/api_wrappers.py` & `sdo-cli-0.0.9/src/sdo/data_loader/image_param/api_wrappers/api_wrappers.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/data_loader/image_param/objects/spatiotemporal_event.py` & `sdo-cli-0.0.9/src/sdo/data_loader/image_param/objects/spatiotemporal_event.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/data_loader/image_param/utils/coord_convertor.py` & `sdo-cli-0.0.9/src/sdo/data_loader/image_param/utils/coord_convertor.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/events/bboxes.py` & `sdo-cli-0.0.9/src/sdo/events/bboxes.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/events/event_loader.py` & `sdo-cli-0.0.9/src/sdo/events/event_loader.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/algorithms/ae_2d.py` & `sdo-cli-0.0.9/src/sdo/sood/algorithms/ae_2d.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/algorithms/ce_vae.py` & `sdo-cli-0.0.9/src/sdo/sood/algorithms/ce_vae.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/data/image_dataset.py` & `sdo-cli-0.0.9/src/sdo/sood/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/data/path_dataset.py` & `sdo-cli-0.0.9/src/sdo/sood/data/path_dataset.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/data/sdo_ml_v1_dataset.py` & `sdo-cli-0.0.9/src/sdo/sood/data/sdo_ml_v1_dataset.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/models/aes.py` & `sdo-cli-0.0.9/src/sdo/sood/models/aes.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/models/iwgan_nets.py` & `sdo-cli-0.0.9/src/sdo/sood/models/iwgan_nets.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/models/nets.py` & `sdo-cli-0.0.9/src/sdo/sood/models/nets.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/util/ce_noise.py` & `sdo-cli-0.0.9/src/sdo/sood/util/ce_noise.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo/sood/util/utils.py` & `sdo-cli-0.0.9/src/sdo/sood/util/utils.py`

 * *Files identical despite different names*

### Comparing `sdo-cli-0.0.8/src/sdo_cli.egg-info/PKG-INFO` & `sdo-cli-0.0.9/src/sdo_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdo-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ML practitioners utility for working with SDO data.
 Home-page: https://github.com/i4DS/sdo-cli
 Author: Marius Giger
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdo-cli-0.0.8/src/sdo_cli.egg-info/SOURCES.txt` & `sdo-cli-0.0.9/src/sdo_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

