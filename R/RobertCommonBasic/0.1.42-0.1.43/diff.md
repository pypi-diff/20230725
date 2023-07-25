# Comparing `tmp/RobertCommonBasic-0.1.42.tar.gz` & `tmp/RobertCommonBasic-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.42.tar", last modified: Thu Jun 15 07:13:23 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.43.tar", last modified: Tue Jul 25 09:53:04 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.42.tar` & `RobertCommonBasic-0.1.43.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.42/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.42/MANIFEST.in
--rw-rw-rw-   0        0        0      868 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-06-02 07:56:40.000000 RobertCommonBasic-0.1.42/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.363424 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0      868 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4467 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.42/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.367016 RobertCommonBasic-0.1.42/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.42/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.368119 RobertCommonBasic-0.1.42/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.370124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.372125 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.374124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12853 2023-06-09 09:28:37.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.388125 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/express.py
--rw-rw-rw-   0        0        0     8304 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0    12943 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.391127 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.396124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    12394 2023-06-13 02:45:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.402431 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.405430 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.408498 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.417847 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.425847 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6582 2023-06-09 09:52:58.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.428221 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.440098 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.442562 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.444568 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.446980 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.451549 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.454613 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.459878 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.463911 RobertCommonBasic-0.1.42/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.464914 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.467252 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.474250 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.476250 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.481577 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.484584 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.489665 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.492638 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.495381 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.499258 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.502116 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.222743 RobertCommonBasic-0.1.43/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.43/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.43/MANIFEST.in
+-rw-rw-rw-   0        0        0      868 2023-07-25 09:53:04.222743 RobertCommonBasic-0.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-06-02 07:56:40.000000 RobertCommonBasic-0.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.082768 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0      868 2023-07-25 09:53:03.000000 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4467 2023-07-25 09:53:03.000000 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:53:03.000000 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-07-25 09:53:03.000000 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-25 09:53:03.000000 RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.43/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.083778 RobertCommonBasic-0.1.43/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.43/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.084774 RobertCommonBasic-0.1.43/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.086774 RobertCommonBasic-0.1.43/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.088774 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.090773 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12839 2023-06-20 06:02:17.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.107042 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    15096 2023-07-25 09:42:23.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/express.py
+-rw-rw-rw-   0        0        0     8304 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0    12952 2023-07-25 09:14:12.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.109051 RobertCommonBasic-0.1.43/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.112978 RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    12394 2023-06-13 02:45:07.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.120187 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.124183 RobertCommonBasic-0.1.43/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.126455 RobertCommonBasic-0.1.43/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.135697 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     4978 2023-07-25 08:55:44.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.139143 RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-06-09 09:52:58.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.142577 RobertCommonBasic-0.1.43/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.148434 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.154723 RobertCommonBasic-0.1.43/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.157154 RobertCommonBasic-0.1.43/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.159583 RobertCommonBasic-0.1.43/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.164206 RobertCommonBasic-0.1.43/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.166963 RobertCommonBasic-0.1.43/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.169974 RobertCommonBasic-0.1.43/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.43/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.173107 RobertCommonBasic-0.1.43/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.176115 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.178115 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.186658 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.188656 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.197657 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.200656 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.207669 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.209920 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.214404 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.216936 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:53:04.220748 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:53:04.222743 RobertCommonBasic-0.1.43/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-07-25 09:14:12.000000 RobertCommonBasic-0.1.43/setup.py
```

### Comparing `RobertCommonBasic-0.1.42/LICENSE` & `RobertCommonBasic-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/PKG-INFO` & `RobertCommonBasic-0.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.43/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/cls/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,23 +137,23 @@
 
     def __init__(self):
         self.timer = None
 
     def is_running(self):
         return self.timer and self.timer.is_alive()
 
-    def run(self, interval: int, function: Callable, args=None, kwargs=None):
+    def run(self, interval: int, function: Callable, *args, **kwargs):
         if self.is_running():
             if kwargs.get('force', False) is False:
                 raise Exception(f"timer is running, please cancel")
             else:
                 self.cancel()
         self._run_timer(interval, function, args, kwargs)
 
-    def _run_timer(self, interval: int, function: Callable, args=None, kwargs=None):
+    def _run_timer(self, interval: int, function: Callable, *args, **kwargs):
         self.timer = Timer(interval, function, args, kwargs)
         self.timer.start()
 
     def cancel(self):
         if self.is_running():
             self.timer.cancel()
         self.timer = None
```

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 
 from struct import pack, unpack
 from typing import Optional, Union, Any
 from enum import Enum
 from datetime import datetime, timedelta
+from encodings import aliases as encodings_aliases
 
 
 class DataFormat(Enum):
     """应用于多字节数据的解析或是生成格式"""
     ABCD = 0
     BADC = 1
     CDAB = 2
@@ -55,21 +56,21 @@
     elif type in [TypeFormat.INT32, TypeFormat.UINT32, TypeFormat.FLOAT]:
         return 2
     elif type in [TypeFormat.INT64, TypeFormat.UINT64, TypeFormat.DOUBLE]:
         return 4
     return length
 
 
-# 将字节数组转换成十六进制的表示形式
 def bytes_to_hex_string(datas: bytearray, segment: str = ' '):
+    """将字节数组转换成十六进制的表示形式"""
     return segment.join(['{:02X}'.format(byte) for byte in datas])
 
 
-# 从字节数组中提取bool数组变量信息
 def bytes_to_bool_array(datas: bytearray, length: int = None):
+    """从字节数组中提取bool数组变量信息"""
     if datas is None:
         return None
     if length is None or length > len(datas) * 8:
         length = len(datas) * 8
 
     buffer = []
     for i in range(length):
@@ -80,37 +81,37 @@
         if (datas[index] & temp) == temp:
             buffer.append(True)
         else:
             buffer.append(False)
     return buffer
 
 
-# 将buffer中的字节转化成byte数组对象
 def trans_byte_array(datas: bytearray, index: int, length: int):
+    """将buffer中的字节转化成byte数组对象"""
     data = bytearray(length)
     for i in range(length):
         data[i] = datas[i + index]
     return data
 
 
-# 将buffer数组转化成bool数组对象，需要转入索引，长度
 def trans_byte_bool_array(datas: bytearray, index: int, length: int):
+    """将buffer数组转化成bool数组对象，需要转入索引，长度"""
     data = bytearray(length)
     for i in range(length):
         data[i] = datas[i + index]
     return bytes_to_bool_array(data)
 
 
-# 将buffer中的字节转化成byte对象
 def trans_byte(datas: bytearray, index: int):
+    """将buffer中的字节转化成byte对象"""
     return datas[index]
 
 
-# 反转多字节
 def reverse_bytes(datas: bytearray, length: int, index: int = 0, format: DataFormat = DataFormat.ABCD):
+    """反转多字节"""
     buffer = bytearray(length)
     if format == DataFormat.ABCD:
         for i in range(length):
             buffer[i] = datas[index + i]
     elif format == DataFormat.BADC:
         for i in range(int(length / 2)):
             buffer[2 * i] = datas[index + 2 * i + 1]
@@ -406,7 +407,52 @@
 
 
 def try_convert_value(value: Union[str, float, None]) -> Union[str, float, None]:
     try:
         return float(value)
     except (ValueError, TypeError):
         return value
+
+
+def safe_convert_str(content: Union[str, bytes]):
+    if isinstance(content, str):
+        return content
+    try:
+        return content.decode(encoding='gbk', errors='ignore')  # lambda x: unicode(x, 'utf-8', 'ignore')
+    except:
+        try:
+            return content.decode(encoding='utf-8', errors='ignore')
+        except:
+            encodings = set(encodings_aliases.values())
+            for encoding in encodings:
+                if encoding not in ['gbk', 'utf-8']:
+                    try:
+                        return content.decode(encoding=encoding, errors='ignore')
+                    except:
+                        pass
+    return str(content)
+
+
+def convert_type_value(value: Any, to_type: Any, default_value: Optional[Any] = None):
+    """值类型转换"""
+    default_value = value if default_value is None else default_value
+    if to_type == int:
+        try:
+            return int(float(value))
+        except:
+            pass
+    elif to_type == float:
+        try:
+            return float(value)
+        except:
+            pass
+    elif to_type == 'set':
+        try:
+            value = float(value)
+            if int(value) == value:
+                return int(value)
+            return value
+        except:
+            pass
+    elif to_type == str:
+        return str(value)
+    return default_value
```

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/express.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/express.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/data/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,8 +421,8 @@
     start = 0
     for a in args:
         start = start | a
     return start
 
 
 # 添加自定义函数
-g_s.functions.update(max=max, min=min, bit=bit, signed=signed, inverse_long=inverse_long, inverse_float=inverse_float, inverse_double=inverse_double, _and=_and, _or=_or)
+g_s.functions.update(max=max, min=min, sum=sum, bit=bit, signed=signed, inverse_long=inverse_long, inverse_float=inverse_float, inverse_double=inverse_double, _and=_and, _or=_or)
```

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/dt/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/ini.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,38 +126,38 @@
                 f'config: {k} = {v if not self.is_secret(k) else "********"}, {type(v).__name__}')
 
 
 # 读取配置
 def read_ini(file_path: str) -> dict:
     values = {}
     if check_file_exist(file_path) is True:
-        config = ConfigParser()
+        config = SensitiveConfigParser()
         config.read(file_path)
 
         for section in config.sections():
             for option in config.options(section):
                 if section not in values.keys():
                     values[section] = {}
                 values[section][option] = config.get(section, option)
     return values
 
 
 # 读取配置
 def read_init_key(file_path: str, section: str, name: str):
     if check_file_exist(file_path) is True:
-        config = ConfigParser()
+        config = SensitiveConfigParser()
         config.read(file_path)
         if config.has_section(section) is True:
             if config.has_option(section, name) is True:
                 return config.get(section, name)
     return None
 
 
 def write_init(file_path: str, values: dict, is_update: bool = False):
-    config = ConfigParser()
+    config = SensitiveConfigParser()
     if is_update:
         config.read(file_path)
     for section, params in values.items():
         if config.has_section(section) is False:
             config.add_section(section)
         for name, value in params.items():
             config.set(section, name, value)
```

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.43/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.42/setup.py` & `RobertCommonBasic-0.1.43/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.42'
-DATE = '2023-06-15'
+VERSION = '0.1.43'
+DATE = '2023-07-25'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

