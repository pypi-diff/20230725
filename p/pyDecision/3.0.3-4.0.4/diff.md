# Comparing `tmp/pyDecision-3.0.3.tar.gz` & `tmp/pyDecision-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-3.0.3.tar", last modified: Tue Jul 18 01:05:03 2023, max compression
+gzip compressed data, was "dist\pyDecision-4.0.4.tar", last modified: Tue Jul 25 21:39:41 2023, max compression
```

## Comparing `pyDecision-3.0.3.tar` & `pyDecision-4.0.4.tar`

### file list

```diff
@@ -1,70 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-3.0.3/LICENSE
--rw-rw-rw-   0        0        0    13774 2023-07-18 01:05:03.000000 pyDecision-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13376 2023-07-18 01:03:18.000000 pyDecision-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-3.0.3/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2035 2023-07-18 00:56:12.000000 pyDecision-3.0.3/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-3.0.3/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-3.0.3/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-3.0.3/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-3.0.3/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-3.0.3/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-3.0.3/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-3.0.3/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-3.0.3/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2302 2023-07-18 00:55:14.000000 pyDecision-3.0.3/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-3.0.3/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-3.0.3/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-3.0.3/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-3.0.3/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-3.0.3/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-3.0.3/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-3.0.3/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-3.0.3/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-3.0.3/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-3.0.3/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2551 2023-07-16 13:00:46.000000 pyDecision-3.0.3/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-3.0.3/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-3.0.3/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0      967 2023-07-15 20:29:25.000000 pyDecision-3.0.3/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-3.0.3/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-3.0.3/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-3.0.3/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-3.0.3/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-3.0.3/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-3.0.3/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-3.0.3/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-3.0.3/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-3.0.3/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-3.0.3/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-3.0.3/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2115 2023-07-16 16:14:56.000000 pyDecision-3.0.3/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-3.0.3/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-3.0.3/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-3.0.3/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-3.0.3/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-3.0.3/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-3.0.3/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-3.0.3/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/util/
--rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-3.0.3/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-3.0.3/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-3.0.3/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    13774 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1851 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 01:05:03.000000 pyDecision-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-18 01:04:43.000000 pyDecision-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:39:41.000000 pyDecision-4.0.4/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.0.4/LICENSE
+-rw-rw-rw-   0        0        0    16107 2023-07-25 21:39:41.000000 pyDecision-4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15694 2023-07-25 21:20:13.000000 pyDecision-4.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 21:39:41.000000 pyDecision-4.0.4/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.0.4/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:39:41.000000 pyDecision-4.0.4/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2379 2023-07-23 16:35:36.000000 pyDecision-4.0.4/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.0.4/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.0.4/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.0.4/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.0.4/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.0.4/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.0.4/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.0.4/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.0.4/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.0.4/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.0.4/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.0.4/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.0.4/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.0.4/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.0.4/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.0.4/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.0.4/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.0.4/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.0.4/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.0.4/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.0.4/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.0.4/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.0.4/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.0.4/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.0.4/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.0.4/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.0.4/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.0.4/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.0.4/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.0.4/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.0.4/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.0.4/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.0.4/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.0.4/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.0.4/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.0.4/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.0.4/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.0.4/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.0.4/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.0.4/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.0.4/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.0.4/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.0.4/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.0.4/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.0.4/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.0.4/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.0.4/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.0.4/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.0.4/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.0.4/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.0.4/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:39:41.000000 pyDecision-4.0.4/pyDecision/util/
+-rw-rw-rw-   0        0        0     3151 2023-07-25 21:32:57.000000 pyDecision-4.0.4/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      179 2023-07-25 21:37:55.000000 pyDecision-4.0.4/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0    18201 2023-07-25 21:19:42.000000 pyDecision-4.0.4/pyDecision/util/compare.py
+-rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.0.4/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.0.4/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:39:41.000000 pyDecision-4.0.4/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    16107 2023-07-25 21:39:40.000000 pyDecision-4.0.4/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2165 2023-07-25 21:39:40.000000 pyDecision-4.0.4/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:39:40.000000 pyDecision-4.0.4/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-25 21:39:40.000000 pyDecision-4.0.4/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 21:39:40.000000 pyDecision-4.0.4/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 21:39:41.000000 pyDecision-4.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-07-25 21:39:33.000000 pyDecision-4.0.4/setup.py
```

### Comparing `pyDecision-3.0.3/LICENSE` & `pyDecision-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/PKG-INFO` & `pyDecision-4.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,128 +1,132 @@
-Metadata-Version: 2.1
-Name: pyDecision
-Version: 3.0.3
-Summary: A MCDA Library
-Home-page: https://github.com/Valdecy/pyDecisions
-Author: Valdecy Pereira
-Author-email: valdecy.pereira@gmail.com
-License: GNU
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyDecision
-
-## Introduction
-
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
-
-## Usage
-
-1. Install
-```bash
-pip install pyDecision
-```
-
-2. Import
-
-```py3
-
-# Import AHP
-from pyDecision.algorithm import ahp_method
-
-# Parameters
-weight_derivation = 'geometric' # 'mean' or 'geometric'
-
-# Dataset
-dataset = np.array([
-  #g1     g2     g3     g4     g5     g6     g7                  
-  [1  ,   1/3,   1/5,   1  ,   1/4,   1/2,   3  ],   #g1
-  [3  ,   1  ,   1/2,   2  ,   1/3,   3  ,   3  ],   #g2
-  [5  ,   2  ,   1  ,   4  ,   5  ,   6  ,   5  ],   #g3
-  [1  ,   1/2,   1/4,   1  ,   1/4,   1  ,   2  ],   #g4
-  [4  ,   3  ,   1/5,   4  ,   1  ,   3  ,   2  ],   #g5
-  [2  ,   1/3,   1/6,   1  ,   1/3,   1  ,   1/3],   #g6
-  [1/3,   1/3,   1/5,   1/2,   1/2,   3  ,   1  ]    #g7
-])
-
-# Call AHP Function
-weights, rc = ahp_method(dataset, wd = weight_derivation)
-
-# Weigths
-for i in range(0, weights.shape[0]):
-  print('w(g'+str(i+1)+'): ', round(weights[i], 3))
-  
-# Consistency Ratio
-print('RC: ' + str(round(rc, 2)))
-if (rc > 0.10):
-  print('The solution is inconsistent, the pairwise comparisons must be reviewed')
-else:
-  print('The solution is consistent')
-
-```
-
-3. Try it in **Colab**:
-
-- AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
-- Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
-- ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
-- Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
-- BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
-- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
-- CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
-- CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
-- COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
-- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
-- CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
-- DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
-- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
-- EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
-- Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
-- ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
-- ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
-- ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
-- GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
-- IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
-- MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
-- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
-- MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
-- MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
-- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
-- MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
-- MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
-- MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
-- OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
-- PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
-))
-- PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
-- PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
-- SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
-- SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
-- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
-- TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
-- Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
-- VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
-- Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
-- WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
-- WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
-
-4. Advanced MCDA Methods:
-
-- [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
-- [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
-- [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
-- [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
-
-# Acknowledgement 
-
-This section is dedicated to all the people that helped to improve or correct the code. Thank you very much!
-
-* Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - UniversitÃ© Abdelhamid Ibn Badis Mostaganem (Algeria)
+# pyDecision
+
+## Introduction
+
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+
+pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
+
+## Usage
+
+1. Install
+```bash
+pip install pyDecision
+```
+
+2. Import
+
+```py3
+
+# Import AHP
+from pyDecision.algorithm import ahp_method
+
+# Parameters
+weight_derivation = 'geometric' # 'mean' or 'geometric'
+
+# Dataset
+dataset = np.array([
+  #g1     g2     g3     g4     g5     g6     g7                  
+  [1  ,   1/3,   1/5,   1  ,   1/4,   1/2,   3  ],   #g1
+  [3  ,   1  ,   1/2,   2  ,   1/3,   3  ,   3  ],   #g2
+  [5  ,   2  ,   1  ,   4  ,   5  ,   6  ,   5  ],   #g3
+  [1  ,   1/2,   1/4,   1  ,   1/4,   1  ,   2  ],   #g4
+  [4  ,   3  ,   1/5,   4  ,   1  ,   3  ,   2  ],   #g5
+  [2  ,   1/3,   1/6,   1  ,   1/3,   1  ,   1/3],   #g6
+  [1/3,   1/3,   1/5,   1/2,   1/2,   3  ,   1  ]    #g7
+])
+
+# Call AHP Function
+weights, rc = ahp_method(dataset, wd = weight_derivation)
+
+# Weigths
+for i in range(0, weights.shape[0]):
+  print('w(g'+str(i+1)+'): ', round(weights[i], 3))
+  
+# Consistency Ratio
+print('RC: ' + str(round(rc, 2)))
+if (rc > 0.10):
+  print('The solution is inconsistent, the pairwise comparisons must be reviewed')
+else:
+  print('The solution is consistent')
+
+```
+
+3. Try it in **Colab**:
+
+- AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
+- Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
+- ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
+- Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2021/8545379))
+- Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
+- BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
+- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
+- CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
+- CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
+- Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
+- COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
+- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
+- CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
+- DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
+- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
+- EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
+- Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
+- Entropy ([ Colab Demo ](Entropy)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
+- ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
+- ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
+- ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
+- GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
+- IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
+- MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
+- MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
+- MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
+- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
+- MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
+- Fuzzy MOORA ([ Colab Demo ]()) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
+- MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
+- MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
+- OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
+- Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
+))
+- PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
+- PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
+- PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
+- SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
+- SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
+- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
+- TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
+- Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
+- VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
+- Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
+- WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
+- WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
+
+4. Compare Methods:
+- Compare Ranks & Ask chatGPT([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
+- Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
+- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+
+5. Advanced MCDA Methods:
+
+- [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
+- [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
+- [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
+- [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
+
+# Acknowledgement 
+
+This section is dedicated to all the people that helped to improve or correct the code. Thank you very much!
+
+* Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - Université Abdelhamid Ibn Badis Mostaganem (Algeria)
```

### Comparing `pyDecision-3.0.3/README.md` & `pyDecision-4.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,143 @@
-# pyDecision
-
-## Introduction
-
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
-
-## Usage
-
-1. Install
-```bash
-pip install pyDecision
-```
-
-2. Import
-
-```py3
-
-# Import AHP
-from pyDecision.algorithm import ahp_method
-
-# Parameters
-weight_derivation = 'geometric' # 'mean' or 'geometric'
-
-# Dataset
-dataset = np.array([
-  #g1     g2     g3     g4     g5     g6     g7                  
-  [1  ,   1/3,   1/5,   1  ,   1/4,   1/2,   3  ],   #g1
-  [3  ,   1  ,   1/2,   2  ,   1/3,   3  ,   3  ],   #g2
-  [5  ,   2  ,   1  ,   4  ,   5  ,   6  ,   5  ],   #g3
-  [1  ,   1/2,   1/4,   1  ,   1/4,   1  ,   2  ],   #g4
-  [4  ,   3  ,   1/5,   4  ,   1  ,   3  ,   2  ],   #g5
-  [2  ,   1/3,   1/6,   1  ,   1/3,   1  ,   1/3],   #g6
-  [1/3,   1/3,   1/5,   1/2,   1/2,   3  ,   1  ]    #g7
-])
-
-# Call AHP Function
-weights, rc = ahp_method(dataset, wd = weight_derivation)
-
-# Weigths
-for i in range(0, weights.shape[0]):
-  print('w(g'+str(i+1)+'): ', round(weights[i], 3))
-  
-# Consistency Ratio
-print('RC: ' + str(round(rc, 2)))
-if (rc > 0.10):
-  print('The solution is inconsistent, the pairwise comparisons must be reviewed')
-else:
-  print('The solution is consistent')
-
-```
-
-3. Try it in **Colab**:
-
-- AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
-- Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
-- ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
-- Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
-- BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
-- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
-- CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
-- CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
-- COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
-- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
-- CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
-- DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
-- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
-- EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
-- Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
-- ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
-- ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
-- ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
-- ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
-- GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
-- IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
-- MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
-- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
-- MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
-- MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
-- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
-- MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
-- MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
-- MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
-- OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
-- PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
-))
-- PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
-- PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
-- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
-- SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
-- SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
-- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
-- TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
-- Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
-- VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
-- Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
-- WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
-- WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
-
-4. Advanced MCDA Methods:
-
-- [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
-- [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
-- [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
-- [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
-
-# Acknowledgement 
-
-This section is dedicated to all the people that helped to improve or correct the code. Thank you very much!
-
-* Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - Université Abdelhamid Ibn Badis Mostaganem (Algeria)
+Metadata-Version: 2.1
+Name: pyDecision
+Version: 4.0.4
+Summary: A MCDA Library
+Home-page: https://github.com/Valdecy/pyDecisions
+Author: Valdecy Pereira
+Author-email: valdecy.pereira@gmail.com
+License: GNU
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyDecision
+
+## Introduction
+
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+
+pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
+
+## Usage
+
+1. Install
+```bash
+pip install pyDecision
+```
+
+2. Import
+
+```py3
+
+# Import AHP
+from pyDecision.algorithm import ahp_method
+
+# Parameters
+weight_derivation = 'geometric' # 'mean' or 'geometric'
+
+# Dataset
+dataset = np.array([
+  #g1     g2     g3     g4     g5     g6     g7                  
+  [1  ,   1/3,   1/5,   1  ,   1/4,   1/2,   3  ],   #g1
+  [3  ,   1  ,   1/2,   2  ,   1/3,   3  ,   3  ],   #g2
+  [5  ,   2  ,   1  ,   4  ,   5  ,   6  ,   5  ],   #g3
+  [1  ,   1/2,   1/4,   1  ,   1/4,   1  ,   2  ],   #g4
+  [4  ,   3  ,   1/5,   4  ,   1  ,   3  ,   2  ],   #g5
+  [2  ,   1/3,   1/6,   1  ,   1/3,   1  ,   1/3],   #g6
+  [1/3,   1/3,   1/5,   1/2,   1/2,   3  ,   1  ]    #g7
+])
+
+# Call AHP Function
+weights, rc = ahp_method(dataset, wd = weight_derivation)
+
+# Weigths
+for i in range(0, weights.shape[0]):
+  print('w(g'+str(i+1)+'): ', round(weights[i], 3))
+  
+# Consistency Ratio
+print('RC: ' + str(round(rc, 2)))
+if (rc > 0.10):
+  print('The solution is inconsistent, the pairwise comparisons must be reviewed')
+else:
+  print('The solution is consistent')
+
+```
+
+3. Try it in **Colab**:
+
+- AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
+- Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
+- ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
+- Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2021/8545379))
+- Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
+- BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
+- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
+- CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
+- CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
+- Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
+- COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
+- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
+- CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
+- DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
+- Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
+- EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
+- Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
+- Entropy ([ Colab Demo ](Entropy)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
+- ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
+- ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
+- ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
+- ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
+- GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
+- IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
+- MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
+- MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
+- MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
+- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
+- MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
+- Fuzzy MOORA ([ Colab Demo ]()) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
+- MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
+- MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
+- OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
+- Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
+))
+- PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
+- PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
+- PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
+- SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
+- SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
+- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
+- TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
+- Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
+- VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
+- Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
+- WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
+- WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
+
+4. Compare Methods:
+- Compare Ranks & Ask chatGPT([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
+- Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
+- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+
+5. Advanced MCDA Methods:
+
+- [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
+- [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
+- [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
+- [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
+
+# Acknowledgement 
+
+This section is dedicated to all the people that helped to improve or correct the code. Thank you very much!
+
+* Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - UniversitÃ© Abdelhamid Ibn Badis Mostaganem (Algeria)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/__init__.py` & `pyDecision-4.0.4/pyDecision/algorithm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from .ahp           import ahp_method
 from .aras          import aras_method
 from .borda         import borda_method
 from .bwm           import bw_method
 from .cilos         import cilos_method
 from .cocoso        import cocoso_method
 from .codas         import codas_method
+from .copeland      import copeland_method
 from .copras        import copras_method
 from .cradis        import cradis_method
 from .critic        import critic_method
 from .dematel       import dematel_method
 from .e_i           import electre_i
 from .e_i_s         import electre_i_s
 from .e_i_v         import electre_i_v
 from .e_ii          import electre_ii
 from .e_iii         import electre_iii
 from .e_iv          import electre_iv
 from .e_tri_b       import electre_tri_b
 from .edas          import edas_method
+from .entropy       import entropy_method
 from .fuzzy_ahp     import fuzzy_ahp_method
+from .fuzzy_aras    import fuzzy_aras_method
+from .fuzzy_copras  import fuzzy_copras_method
 from .fuzzy_dematel import fuzzy_dematel_method
 from .fuzzy_edas    import fuzzy_edas_method
+from .fuzzy_moora   import fuzzy_moora_method
+from .fuzzy_ocra    import fuzzy_ocra_method
 from .fuzzy_topsis  import fuzzy_topsis_method
 from .fuzzy_vikor   import fuzzy_vikor_method
 from .gra           import gra_method
 from .idocriw       import idocriw_method
 from .mabac         import mabac_method
 from .mairca        import mairca_method
 from .marcos        import marcos_method
@@ -37,14 +43,16 @@
 from .p_ii          import promethee_ii
 from .p_iii         import promethee_iii
 from .p_iv          import promethee_iv
 from .p_v           import promethee_v
 from .p_vi          import promethee_vi
 from .p_xgaia       import promethee_gaia
 from .piv           import piv_method
+from .psi           import psi_method
+from .rov           import rov_method
 from .saw           import saw_method
 from .smart         import smart_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
 from .wings         import wings_method
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/ahp.py` & `pyDecision-4.0.4/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/aras.py` & `pyDecision-4.0.4/pyDecision/algorithm/aras.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,40 +25,41 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: ARAS (Additive Ratio Assessment)
-def aras_method(dataset, weights, criterion_type, graph = True):
+def aras_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X   = np.copy(dataset)/1.0
     bst = np.zeros(X.shape[1])
     bsm = np.zeros(X.shape[1])
     for j in range(0, X.shape[1]):
         if ( criterion_type[j] == 'max'):
             bst[j] = np.max(X[:, j])
             bsm[j] = bst[j] + np.sum(X[:, j])
         elif ( criterion_type[j] == 'min'):
             bst[j]  = 1/np.min(X[:, j])
-            X[:, j] = 1/X[:, j]
+            X[:,j]  = 1/X[:, j]
             bsm[j]  = bst[j] + np.sum(X[:, j])
     for j in range(0, X.shape[1]):
         bst[j] = bst[j]/ bsm[j]
         for i in range(0, X.shape[0]):
             X[i, j] = X[i, j]/ bsm[j]
-    X    = X*weights
-    bst  = bst*weights
+    X    = X * weights
+    bst  = bst * weights
     n_0  = np.sum(bst)
     n_i  = np.sum(X, axis = 1)
     k_i  = n_i/n_0
     flow = np.copy(k_i)
     flow = np.reshape(flow, (k_i.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, k_i.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/borda.py` & `pyDecision-4.0.4/pyDecision/algorithm/borda.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,25 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: Borda
-def borda_method(dataset, criterion_type, graph = True):
+def borda_method(dataset, criterion_type, graph = True, verbose = True):
     X = np.zeros((dataset.shape[0], dataset.shape[1]))
     for j in range(0, dataset.shape[1]):
         if (criterion_type[j] == 'max'):
             X[:,j] = np.argsort(np.argsort(-dataset[:,j]))+1
         else:
             X[:,j] = np.argsort(np.argsort(dataset[:,j]))+1
     total = np.sum(X, axis = 1)
-    for i in range(0, total.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(total[i], 2)))
+    if (verbose == True):
+        for i in range(0, total.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(total[i], 2)))
     if ( graph == True):
         flow = np.copy(total)
         flow = np.reshape(flow, (total.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, total.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         ranking(flow)
     return total
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/bwm.py` & `pyDecision-4.0.4/pyDecision/algorithm/bwm.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 
 from pyDecision.util.gwo import grey_wolf_optimizer
 
 ###############################################################################
 
 # Function: BWM
-def bw_method(dataset, mic, lic, size = 50, iterations = 150):
+def bw_method(dataset, mic, lic, size = 50, iterations = 150, verbose = True):
     X         = np.copy(dataset)/1.0
     best      = np.where(mic == 1)[0][0]
     worst     = np.where(lic == 1)[0][0]
     pairs_b   = [(best, i)  for i in range(0, mic.shape[0])]
     pairs_w   = [(i, worst) for i in range(0, mic.shape[0]) if (i, worst) not in pairs_b]
     def target_function(variables):
         eps       = [float('+inf')]
@@ -27,12 +27,12 @@
             if ( i != j):
                 eps.append(diff)
         if ( np.sum(variables) == 0):
             eps = float('+inf')
         else:
             eps = max(eps[1:])
         return eps
-    weights = grey_wolf_optimizer(pack_size = size, min_values = [0.01]*X.shape[1], max_values = [1]*X.shape[1], iterations = iterations, target_function = target_function)
+    weights = grey_wolf_optimizer(pack_size = size, min_values = [0.01]*X.shape[1], max_values = [1]*X.shape[1], iterations = iterations, target_function = target_function, verbose = verbose)
     weights = weights[0][:-1]/sum(weights[0][:-1])
     return weights
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/cilos.py` & `pyDecision-4.0.4/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/cocoso.py` & `pyDecision-4.0.4/pyDecision/algorithm/cocoso.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,35 +25,40 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: COCOSO (COmbined COmpromise SOlution)
-def cocoso_method(dataset, criterion_type, weights, L = 0.5, graph = True):
+def cocoso_method(dataset, criterion_type, weights, L = 0.5, graph = True, verbose = True):
     X     = np.copy(dataset)/1.0
     best  = np.zeros(X.shape[1])
     worst = np.zeros(X.shape[1])
     for i in range(0, dataset.shape[1]):
         if (criterion_type[i] == 'max'):
             best[i]  = np.max(X[:, i])
             worst[i] = np.min(X[:, i])
         else:
             best[i]  = np.min(X[:, i])
             worst[i] = np.max(X[:, i])        
     for j in range(0, X.shape[1]):
-        X[:,j] = ( X[:,j] - worst[j] ) / ( best[j] - worst[j] ) 
+        X[:,j] = ( X[:,j] - worst[j] ) / ( best[j] - worst[j] + 0.0000000000000001) 
     S      = np.sum(X  * weights, axis = 1)
     P      = np.sum(X ** weights, axis = 1)
+    if (np.min(S) == 0):
+        S = S + 1
+    if (np.min(P) == 0):
+        P = P + 1
     ksi_a  = (P + S) / np.sum(P + S, axis = 0)
     ksi_b  = (S / np.min(S)) + (P / np.min(P))
     ksi_c  = (L * S + (1 - L) * P) / (L * np.max(S) + (1 - L) * np.max(P))
     ksi    = np.power(ksi_a * ksi_b * ksi_c, 1/3) + 1/3 * (ksi_a + ksi_b + ksi_c)
-    for i in range(0, ksi.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(ksi[i], 2)))
+    if (verbose == True):
+        for i in range(0, ksi.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(ksi[i], 2)))
     if ( graph == True):
         flow = np.copy(ksi)
         flow = np.reshape(flow, (ksi.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, ksi.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/codas.py` & `pyDecision-4.0.4/pyDecision/algorithm/codas.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,40 +25,41 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: CODAS (Combinative Distance-based Assessment)
-def codas_method(dataset, weights, criterion_type, lmbd = 0.02, graph = True):
+def codas_method(dataset, weights, criterion_type, lmbd = 0.02, graph = True, verbose = True):
     X   = np.copy(dataset)/1.0
     bst = np.zeros(X.shape[1])
     r_m = np.zeros((X.shape[0], X.shape[0]))
     for j in range(0, X.shape[1]):
         if ( criterion_type[j] == 'max'):
             bst[j] = np.max(X[:, j])
         elif ( criterion_type[j] == 'min'):
             bst[j] = np.min(X[:, j])
     for j in range(0, X.shape[1]):
         for i in range(0, X.shape[0]):
             if ( criterion_type[j] == 'max'):
                 X[i, j] = X[i, j]/bst[j]
             elif ( criterion_type[j] == 'min'):
                 X[i, j] = bst[j]/X[i, j]
-    X   = X*weights
+    X   = X * weights
     n_i = np.min(X, axis = 0)
     e_i = np.sum( (X - n_i)**2, axis = 1)**(1/2)
     t_i = np.sum( abs(X - n_i), axis = 1)
     for j in range(0, r_m.shape[1]):
         for i in range(0, r_m.shape[0]):
             r_m[i, j] = (e_i[i] - e_i[j]) + lmbd*( (e_i[i] - e_i[j]) *  (t_i[i] - t_i[j]) )
     h_i  = np.sum(r_m, axis = 1)
     flow = np.copy(h_i)
     flow = np.reshape(flow, (h_i.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, h_i.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/copras.py` & `pyDecision-4.0.4/pyDecision/algorithm/copras.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: COPRAS (Complex Proportional Assessment)
-def copras_method(dataset, weights, criterion_type, graph = True):
+def copras_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X   = np.copy(dataset)/1.0
     X   = X/np.sum(X, axis = 0)
     X   = X*weights
     s_p = np.zeros(X.shape[0])
     s_m = np.zeros(X.shape[0])
     s_d = np.zeros(X.shape[0])
     q_i = np.zeros(X.shape[0])
@@ -47,14 +47,15 @@
         s_m = np.sum(X[:,id2], axis = 1)
         s_d = np.min(s_m)/s_m
         q_i = s_p + (np.min(s_m)*np.sum(s_m))/(s_m*np.sum(s_d))
     u_i = q_i/np.max(q_i)
     flow = np.copy(u_i)
     flow = np.reshape(flow, (u_i.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, u_i.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/cradis.py` & `pyDecision-4.0.4/pyDecision/algorithm/cradis.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,34 +25,34 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: CRADIS (Compromise Ranking of Alternatives from Distance to Ideal Solution)
-def cradis_method(dataset, criterion_type, weights, graph = True):
+def cradis_method(dataset, criterion_type, weights, graph = True, verbose = True):
     X = np.copy(dataset)/1.0
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
             X[:,j] = np.min(X[:,j]) / X[:,j]
         else:
             X[:,j] = X[:,j] / np.max(X[:,j])
     X   = X * weights
-    Sp  = np.sum(np.max(X) - X, axis = 1)
+    Sp  = np.sum(np.max(X) - X, axis = 1) + 0.0000000000000001
     Sm  = np.sum(X - np.min(X), axis = 1)
     Sop = np.sum(np.max(X) - np.max(X, axis = 0))
     Som = np.sum(np.max(X, axis = 0) - np.min(X))
     Kp  = Sop / Sp
     Km  = Sm / Som
     Q   = (Kp + Km) / 2
-    for i in range(0, Q.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(Q[i], 2)))
+    if (verbose == True):
+        for i in range(0, Q.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(Q[i], 2)))
     if ( graph == True):
         flow = np.copy(Q)
         flow = np.reshape(flow, (Q.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, Q.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
-        flow = flow[::-1]
         ranking(flow)
     return Q
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/critic.py` & `pyDecision-4.0.4/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/dematel.py` & `pyDecision-4.0.4/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_i.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_ii.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_ii.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             graph[alts[i][ :2]] = i   
             graph[alts[i][-2:]] = i 
     po_matrix = np.zeros((po_string.shape[0], po_string.shape[1]))
     for i in range (0, po_string.shape[0]):
         for j in range (0, po_string.shape[1]):
             if (po_string[i,j] == 'P+'):
                 po_matrix[i,j] = 1
-    col_sum = np.sum(po_matrix, axis = 1)
+    col_sum   = np.sum(po_matrix, axis = 1)
     alts_rank = [x for _, x in sorted(zip(col_sum, alts))]
     if (np.sum(col_sum) != 0):
         alts_rank.reverse()      
     graph_rank = {}
     for i in range(po_string.shape[0]):
         if (len(alts_rank[i]) == 0):
             graph_rank[alts_rank[i]] = i
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_iii.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_iv.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.0.4/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/edas.py` & `pyDecision-4.0.4/pyDecision/algorithm/edas.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: EDAS
-def edas_method(dataset, criterion_type, weights, graph = True):
+def edas_method(dataset, criterion_type, weights, graph = True, verbose = True):
     col_mean = np.mean(dataset, axis = 0)
     pda      = np.zeros((dataset.shape[0], dataset.shape[1]))
     nda      = np.zeros((dataset.shape[0], dataset.shape[1]))
     for i in range(0, dataset.shape[0]):
         for j in range(0, dataset.shape[1]):
             if (criterion_type[j] == 'max'):
                 pda[i,j] = max(0,  dataset[i,j] - col_mean[j]) / col_mean[j]
@@ -45,14 +45,17 @@
     w_pda = pda*weights
     w_nda = nda*weights
     s_p   = np.sum(w_pda , axis = 1)
     s_n   = np.sum(w_nda , axis = 1)
     n_s_p = s_p/max(s_p)
     n_s_n = 1 - s_n/max(s_n)
     a_s   = (1/2)*(n_s_p + n_s_n)
+    if (verbose == True):
+        for i in range(0, a_s.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(a_s[i], 4)))
     if ( graph == True):
         flow = np.copy(a_s)
         flow = np.reshape(flow, (a_s.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, a_s.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_edas.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: Fuzzy EDAS
-def fuzzy_edas_method(dataset, criterion_type, weights, graph = True):
+def fuzzy_edas_method(dataset, criterion_type, weights, graph = True, verbose = True):
     pda_A      = np.zeros((len(dataset), len(dataset[0]) ))
     nda_A      = np.zeros((len(dataset), len(dataset[0]) ))
     pda_B      = np.zeros((len(dataset), len(dataset[0]) ))
     nda_B      = np.zeros((len(dataset), len(dataset[0]) ))
     pda_C      = np.zeros((len(dataset), len(dataset[0]) ))
     nda_C      = np.zeros((len(dataset), len(dataset[0]) ))
     dataset_A  = np.zeros((len(dataset), len(dataset[0]) ))
@@ -89,14 +89,17 @@
     n_s_n_A = 1 - s_n_A/max(s_n_A)
     n_s_n_B = 1 - s_n_B/max(s_n_B)
     n_s_n_C = 1 - s_n_C/max(s_n_C)
     a_s_A   = (1/2)*(n_s_p_A + n_s_n_A)
     a_s_B   = (1/2)*(n_s_p_B + n_s_n_B)
     a_s_C   = (1/2)*(n_s_p_C + n_s_n_C)
     a_s     = (1/3)*(a_s_A + a_s_B + a_s_C)
+    if (verbose == True):
+        for i in range(0, a_s.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(a_s[i], 4)))
     if ( graph == True):
         flow = np.copy(a_s)
         flow = np.reshape(flow, (a_s.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, a_s.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: Fuzzy TOPSIS
-def fuzzy_topsis_method(dataset, weights, criterion_type, graph = True):
+def fuzzy_topsis_method(dataset, weights, criterion_type, graph = True, verbose = True):
     r_ij      = copy.deepcopy(dataset)
     v_ij      = copy.deepcopy(dataset)
     p_ideal_A = copy.deepcopy(weights)
     n_ideal_A = copy.deepcopy(weights)
     dist_p    = np.zeros( (len(dataset), len(dataset[0])) )
     dist_n    = np.zeros( (len(dataset), len(dataset[0])) )
     for j in range(0, len(dataset[0])):
@@ -82,14 +82,17 @@
             x, y, z = p_ideal_A[0][j]
             d, e, f = n_ideal_A[0][j]
             dist_p[i][j] = ( (1/dist_p.shape[1])* ( (a-x)**2 + (b-y)**2 + (c-z)**2 ) )**(1/2)
             dist_n[i][j] = ( (1/dist_n.shape[1])* ( (a-d)**2 + (b-e)**2 + (c-f)**2 ) )**(1/2)        
     d_plus  = np.sum(dist_p, axis = 1)
     d_minus = np.sum(dist_n, axis = 1) 
     c_i     = d_minus / (d_minus + d_plus)
+    if (verbose == True):
+        for i in range(0, c_i.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(c_i[i], 4)))
     if ( graph == True):
         flow = np.copy(c_i)
         flow = np.reshape(flow, (c_i.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, c_i.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: VIKOR
-def fuzzy_vikor_method(dataset, weights, criterion_type, strategy_coefficient = 0.5, graph = True):
+def fuzzy_vikor_method(dataset, weights, criterion_type, strategy_coefficient = 0.5, graph = True, verbose = True):
     dataset_A  = np.zeros((len(dataset), len(dataset[0]) ))
     dataset_B  = np.zeros((len(dataset), len(dataset[0]) ))
     dataset_C  = np.zeros((len(dataset), len(dataset[0]) ))  
     weights_A  = np.zeros(len(weights[0]))
     weights_B  = np.zeros(len(weights[0]))
     weights_C  = np.zeros(len(weights[0]))
     best_A  = np.zeros(dataset_A.shape[1])
@@ -115,14 +115,15 @@
     solution = np.copy(flow_q)
     if (condition_1 == True and condition_2 == False):
         solution = np.copy(flow_q[0:2,:])
     elif (condition_1 == False and condition_2 == True):
         for i in range(solution.shape[0] -1, -1, -1):
             if(solution[i, 1] - solution[0, 1] >= dq):
               solution = np.delete(solution, i, axis = 0)  
-    for i in range(0, solution.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(solution[i, 0], 2)))
+    if (verbose == True):
+        for i in range(0, solution.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(solution[i, 0], 2)))
     if ( graph == True):
         ranking(solution) 
     return flow_s, flow_r, flow_q, solution
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/gra.py` & `pyDecision-4.0.4/pyDecision/algorithm/gra.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,28 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: GRA Method
-def gra_method(dataset, criterion_type, weights, epsilon = 0.5, graph = True):
+# Function: GRA (Grey Relational Analysis)
+def gra_method(dataset, criterion_type, weights, epsilon = 0.5, graph = True, verbose = True):
     x = np.zeros((dataset.shape[0], dataset.shape[1]), dtype = float)
     for j in range(0, dataset.shape[1]):
         if (criterion_type[j] == 'max'):
-            x[:,j] = ( dataset[:,j] - np.min(dataset[:,j]) ) / ( np.max(dataset[:,j]) - np.min(dataset[:,j]) )
+            x[:,j] = ( dataset[:,j] - np.min(dataset[:,j]) ) / ( np.max(dataset[:,j]) - np.min(dataset[:,j]) + 0.0000000000000001)
         else:
-            x[:,j] = ( np.max(dataset[:,j]) - dataset[:,j] ) / ( np.max(dataset[:,j]) - np.min(dataset[:,j]) )
+            x[:,j] = ( np.max(dataset[:,j]) - dataset[:,j] ) / ( np.max(dataset[:,j]) - np.min(dataset[:,j]) + 0.0000000000000001)
     deviation_sequence = 1 - x
     gra_coefficient    = epsilon/(deviation_sequence + epsilon)
     gra_grade          = np.sum(gra_coefficient*weights, axis = 1) / dataset.shape[0]
+    if (verbose == True):
+        for i in range(0, gra_grade.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(gra_grade[i], 4)))
     if ( graph == True):
         flow = np.copy(gra_grade)
         flow = np.reshape(flow, (gra_grade.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, gra_grade.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/idocriw.py` & `pyDecision-4.0.4/pyDecision/algorithm/moora.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ###############################################################################
 
 # Required Libraries
-import math
 import matplotlib.pyplot as plt
 import numpy as np
 
-from pyDecision.util.ga import genetic_algorithm
-
 ###############################################################################
 
 # Function: Rank 
 def ranking(flow):    
     rank_xy = np.zeros((flow.shape[0], 2))
     for i in range(0, rank_xy.shape[0]):
         rank_xy[i, 0] = 0
@@ -27,74 +24,40 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: IDOCRIW (Integrated Determination of Objective CRIteria Weights)
-def idocriw_method(dataset, criterion_type, size = 20, gen = 12000, graph = True):
-    X    = np.copy(dataset)
-    X    = X/X.sum(axis = 0)
-    X_ln = np.copy(dataset)
-    X_r  = np.copy(dataset)
-    for i in range(0, X.shape[0]):
-        for j in range(0, X.shape[1]):
-            X_ln[i,j] = X[i,j]*math.log(X[i,j])
-    d    = np.zeros((1, X.shape[1]))
-    w    = np.zeros((1, X.shape[1]))
-    for i in range(0, d.shape[1]):
-        d[0,i] = 1-( -1/(math.log(d.shape[1]))*sum(X_ln[:,i])) 
-    for i in range(0, w.shape[1]):
-        w[0,i] = d[0,i]/d.sum(axis = 1)
-    for i in range(0, len(criterion_type)):
-        if (criterion_type[i] == 'min'):
-           X_r[:,i] = dataset[:,i].min() / X_r[:,i]
-    X_r   = X_r/X_r.sum(axis = 0)
-    #a_min = X_r.min(axis = 0)       
-    a_max = X_r.max(axis = 0) 
-    A     = np.zeros(dataset.shape)
-    np.fill_diagonal(A, a_max)
-    for k in range(0, A.shape[0]):
-        i, _ = np.where(X_r == a_max[k])
-        i    = i[0]
-        for j in range(0, A.shape[1]):
-            A[k, j] = X_r[i, j]
-    #a_min_ = A.min(axis = 0)       
-    a_max_ = A.max(axis = 0) 
-    P      = np.copy(A)    
-    for i in range(0, P.shape[1]):
-        P[:,i] = (-P[:,i] + a_max_[i])/a_max[i]
-    WP     = np.copy(P)
-    np.fill_diagonal(WP, -P.sum(axis = 0))
-    
-    ################################################
-    def target_function(variable = [0]*WP.shape[1]):
-        variable = [variable[i]/sum(variable) for i in range(0, len(variable))]
-        WP_s     = np.copy(WP)
-        for i in range(0, WP.shape[0]):
-            for j in range(0, WP.shape[1]):
-                WP_s[i, j] = WP_s[i, j]*variable[j]
-        total = abs(WP_s.sum(axis = 1)) 
-        total = sum(total) 
-        return total
-    ################################################
-    
-    solution = genetic_algorithm(population_size = size, mutation_rate = 0.1, elite = 1, min_values = [0]*WP.shape[1], max_values = [1]*WP.shape[1], eta = 1, mu = 1, generations = gen, target_function = target_function)
-    solution = solution[:-1]
-    solution = solution/sum(solution)
-    w_       = np.copy(w)
-    w_       = w_*solution
-    w_       = w_/w_.sum()
-    w_       = w_.T
-    for i in range(0, w_.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(w_[i][0], 4)))
-    if ( graph == True):
-        flow = np.copy(w_)
-        flow = np.reshape(flow, (w_.shape[0], 1))
-        flow = np.insert(flow, 0, list(range(1, w_.shape[0]+1)), axis = 1)
+# Function: MOORA (Multi-objective Optimization on the basis of Ratio Analysis)
+def moora_method(dataset, weights, criterion_type, graph = True, verbose = True):
+    X    = np.copy(dataset)/1.0
+    best = np.zeros(X.shape[1])
+    for i in range(0, X.shape[1]):
+        if ( criterion_type[i] == 'max'):
+            best[i] = np.max(X[:,i])
+        else:
+            best[i] = np.min(X[:,i])
+    root = (np.sum(X**2, axis = 0))**(1/2)
+    X    = X/root
+    X    = X*weights
+    id1 = [i for i, j in enumerate(criterion_type) if j == 'max']
+    id2 = [i for i, j in enumerate(criterion_type) if j == 'min']
+    s_p = np.zeros(X.shape[0])
+    s_m = np.zeros(X.shape[0])
+    Y   = np.zeros(X.shape[0])
+    if (len(id1) > 0):
+        s_p = np.sum(X[:,id1], axis = 1)
+    if (len(id2) > 0):
+        s_m = np.sum(X[:,id2], axis = 1)
+    Y   = s_p - s_m
+    flow = np.copy(Y)
+    flow = np.reshape(flow, (Y.shape[0], 1))
+    flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
-    return w_
-
-###############################################################################
+    return flow
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/mabac.py` & `pyDecision-4.0.4/pyDecision/algorithm/mabac.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: MABAC (Multi-Attributive Border Approximation area Comparison)
-def mabac_method(dataset, criterion_type, graph = True):
+def mabac_method(dataset, criterion_type, graph = True, verbose = True):
     X   = np.copy(dataset)/1.0
     X_r = np.copy(dataset)/1.0
     X_q = np.copy(dataset)/1.0
     for i in range(0, X.shape[0]):
         for j in range(0, X.shape[1]):
             fct = 0
             if (criterion_type[j] == 'max'):
@@ -43,16 +43,17 @@
                 if ((min(X[:,j]) - max(X[:,j])) != 0):
                     fct = (X[i,j] - max(X[:,j]))/(min(X[:,j]) - max(X[:,j]))
             X_r[i,j] = (1/X.shape[0])*(1 + fct)
     for i in range(0, X.shape[0]):
         for j in range(0, X.shape[1]):
             X_q[i,j] = X_r[i,j] - np.prod(X_r[:,j]**(1/X.shape[0]))
     rank = np.sum(X_q, axis = 1)
-    for i in range(0, rank.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(rank[i], 4)))
+    if (verbose == True):
+        for i in range(0, rank.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(rank[i], 4)))
     if ( graph == True):
         flow = np.copy(rank)
         flow = np.reshape(flow, (rank.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, rank.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/mairca.py` & `pyDecision-4.0.4/pyDecision/algorithm/mairca.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: MAIRCA (Multi-Attributive Ideal-Real Comparative Analysis)
-def mairca_method(dataset, weights, criterion_type, graph = True):
+def mairca_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X  = np.copy(dataset)/1.0
     p  = (1 / X.shape[0])
     Tp = np.ones((X.shape))
     Tr = np.ones((X.shape))
     for j in range(X.shape[1]):
         Tp[:, j] = p * weights[j]
     D  = 0
@@ -48,19 +48,19 @@
             if (np.max(X[:,j]) == np.min(X[:,j])):
                 D = 1
             else: 
                 D = np.min(X[:,j]) - np.max(X[:,j])
             Tr[:,j] = Tp[:, j] * ( X[:,j] - np.max(X[:,j]) ) / D
     G  = Tp - Tr
     G  = np.sum(G, axis = 1)
-    for i in range(0, G.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(G[i], 2)))
+    if (verbose == True):
+        for i in range(0, G.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(G[i], 2)))
     if ( graph == True):
         flow = np.copy(G)
         flow = np.reshape(flow, (G.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, G.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
-        flow = flow[::-1]
         ranking(flow)
     return G
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/marcos.py` & `pyDecision-4.0.4/pyDecision/algorithm/marcos.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: MARCOS (Measurement of Alternatives and Ranking according to COmpromise Solution)
-def marcos_method(dataset, weights, criterion_type, graph = True):
+def marcos_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X       = np.copy(dataset)/1.0
     best    = np.zeros(X.shape[1])
     worst   = np.zeros(X.shape[1])
     weights = np.array(weights)
     for i in range(0, dataset.shape[1]):
         if (criterion_type[i] == 'max'):
             best[i]  = np.max(X[:, i])
@@ -58,16 +58,17 @@
     V     = X * weights
     S     = V.sum(axis = 1)
     k_n   = S / np.sum(worst)
     k_p   = S / np.sum(best)
     f_k_n = k_p / (k_p + k_n)
     f_k_p = k_n / (k_p + k_n)
     f_k   = (k_p + k_n) / (1 + ((1 - f_k_p) / f_k_p) + ((1 - f_k_n) / f_k_n))
-    for i in range(0, f_k.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(f_k[i], 2)))
+    if (verbose == True):
+        for i in range(0, f_k.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(f_k[i], 2)))
     if ( graph == True):
         flow = np.copy(f_k)
         flow = np.reshape(flow, (f_k.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, f_k.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/maut.py` & `pyDecision-4.0.4/pyDecision/algorithm/maut.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,23 +56,21 @@
 def u_quad(x):
     y = (2*x-1)**2
     return y
 
 ###############################################################################
 
 # Function: MAUT
-def maut_method(dataset, weights, criterion_type, utility_functions, step_size = 1, graph = True):
-    X = np.copy(dataset)
-    # Normalization
-    for i in range(0, X.shape[1]):
-        if (criterion_type[i] == 'max'):
-            X[:, i] = (X[:,i] - np.min(X[:, i]))/(np.max(X[:, i]) - np.min(X[:, i]))
+def maut_method(dataset, weights, criterion_type, utility_functions, step_size = 1, graph = True, verbose = True):
+    X = np.copy(dataset)/1.0
+    for j in range(0, X.shape[1]):
+        if (criterion_type[j] == 'max'):
+            X[:, j] = (X[:,j] - np.min(X[:, j]))/(np.max(X[:, j]) - np.min(X[:, j]) + 0.0000000000000001)
         else:
-            X[:, i] = 1 + (np.min(X[:, i])- X[:, i])/(np.max(X[:, i]) - np.min(X[: ,i]))
-    # Apply Maginal Utility Function
+            X[:, j] = 1 + (np.min(X[:, j])- X[:, j])/(np.max(X[:, j]) - np.min(X[: ,j])+ 0.0000000000000001)
     for i in range(0, X.shape[1]):
         if (utility_functions[i] == 'exp'):
             ArrExp  = np.vectorize(u_exp)
             X[:, i] = ArrExp(X[:, i])
         elif (utility_functions[i] == 'step'):
             ArrStep = np.vectorize(u_step)
             X[:, i] = ArrStep(X[:, i], step_size)
@@ -83,21 +81,21 @@
             ArrLog  = np.vectorize(u_log)
             X[:, i] = ArrLog(X[:, i])
         elif (utility_functions[i] == 'ln'):
             ArrLn   = np.vectorize(u_ln)
             X[:, i] = ArrLn(X[:, i])
     for i in range(0, X.shape[1]):
         X[:, i] = X[:, i]*weights[i]
-    # Additive Utility Score
     Y    = np.sum(X, axis = 1)
     flow = np.copy(Y)
     flow = np.reshape(flow, (Y.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3)))
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3)))
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/merec.py` & `pyDecision-4.0.4/pyDecision/algorithm/merec.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     for j in range(0, X.shape[1]):
         Z       = np.delete(X, j, axis = 1)
         R[:, j] = np.log(1 + (1/X.shape[1] * np.sum(np.abs(np.log(Z)), axis = 1)))
     E = np.sum(np.abs(R.T - S), axis = 1)
     E = E / np.sum(E)
     return E
 
-
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/moora.py` & `pyDecision-4.0.4/pyDecision/algorithm/moosra.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: MOORA (Multi-objective Optimization on the basis of Ratio Analysis)
-def moora_method(dataset, weights, criterion_type, graph = True):
+# Function: MOOSRA (Multi-objective Optimisation on the Basis of Simple Ratio Analysis)
+def moosra_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X    = np.copy(dataset)/1.0
     best = np.zeros(X.shape[1])
     for i in range(0, X.shape[1]):
         if ( criterion_type[i] == 'max'):
             best[i] = np.max(X[:,i])
         else:
             best[i] = np.min(X[:,i])
@@ -45,18 +45,19 @@
     s_p = np.zeros(X.shape[0])
     s_m = np.zeros(X.shape[0])
     Y   = np.zeros(X.shape[0])
     if (len(id1) > 0):
         s_p = np.sum(X[:,id1], axis = 1)
     if (len(id2) > 0):
         s_m = np.sum(X[:,id2], axis = 1)
-    Y   = s_p - s_m
+    Y    = s_p/s_m
     flow = np.copy(Y)
     flow = np.reshape(flow, (Y.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/moosra.py` & `pyDecision-4.0.4/pyDecision/algorithm/topsis.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,39 +24,42 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: MOOSRA (Multi-objective Optimisation on the Basis of Simple Ratio Analysis)
-def moosra_method(dataset, weights, criterion_type, graph = True):
-    X    = np.copy(dataset)/1.0
-    best = np.zeros(X.shape[1])
-    for i in range(0, X.shape[1]):
-        if ( criterion_type[i] == 'max'):
-            best[i] = np.max(X[:,i])
+# Function: TOPSIS
+def topsis_method(dataset, weights, criterion_type, graph = True, verbose = True):
+    X = np.copy(dataset)
+    w = np.copy(weights)
+    sum_cols = np.sum(X*X, axis = 0)
+    sum_cols = sum_cols**(1/2)
+    r_ij = X/sum_cols
+    v_ij = r_ij*w
+    p_ideal_A = np.zeros(X.shape[1])
+    n_ideal_A = np.zeros(X.shape[1])
+    for i in range(0, dataset.shape[1]):
+        if (criterion_type[i] == 'max'):
+            p_ideal_A[i] = np.max(v_ij[:, i])
+            n_ideal_A[i] = np.min(v_ij[:, i])
         else:
-            best[i] = np.min(X[:,i])
-    root = (np.sum(X**2, axis = 0))**(1/2)
-    X    = X/root
-    X    = X*weights
-    id1 = [i for i, j in enumerate(criterion_type) if j == 'max']
-    id2 = [i for i, j in enumerate(criterion_type) if j == 'min']
-    s_p = np.zeros(X.shape[0])
-    s_m = np.zeros(X.shape[0])
-    Y   = np.zeros(X.shape[0])
-    if (len(id1) > 0):
-        s_p = np.sum(X[:,id1], axis = 1)
-    if (len(id2) > 0):
-        s_m = np.sum(X[:,id2], axis = 1)
-    Y   = s_p/s_m
-    flow = np.copy(Y)
-    flow = np.reshape(flow, (Y.shape[0], 1))
-    flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
-    if (graph == True):
+            p_ideal_A[i] = np.min(v_ij[:, i])
+            n_ideal_A[i] = np.max(v_ij[:, i]) 
+    p_s_ij = (v_ij - p_ideal_A)**2
+    p_s_ij = np.sum(p_s_ij, axis = 1)**(1/2)
+    n_s_ij = (v_ij - n_ideal_A)**2
+    n_s_ij = np.sum(n_s_ij, axis = 1)**(1/2)
+    c_i    = n_s_ij / ( p_s_ij  + n_s_ij )
+    if (verbose == True):
+        for i in range(0, c_i.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(c_i[i], 2)))
+    if ( graph == True):
+        flow = np.copy(c_i)
+        flow = np.reshape(flow, (c_i.shape[0], 1))
+        flow = np.insert(flow, 0, list(range(1, c_i.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
-    return flow
+    return c_i
+
+###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/multimoora.py` & `pyDecision-4.0.4/pyDecision/algorithm/multimoora.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 # Required Libraries
 import matplotlib.pyplot as plt
 import numpy as np
 
 ###############################################################################
 
 # Function: Rank 
-def ranking(flow_1, flow_2, flow_3):    
+def ranking_m(flow_1, flow_2, flow_3):    
     rank_xy = np.zeros((flow_1.shape[0] + 1, 6)) 
     for i in range(0, rank_xy.shape[0]):
         rank_xy[i, 0] = -1
         rank_xy[i, 1] = flow_1.shape[0]-i+1     
         rank_xy[i, 2] = 0
         rank_xy[i, 3] = flow_2.shape[0]-i+1  
         rank_xy[i, 4] = 1
         rank_xy[i, 5] = flow_3.shape[0]-i+1    
     plt.text(rank_xy[0, 0],  rank_xy[0, 1], 'MOORA', size = 12, ha = 'center', va = 'center', color = 'white', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0, 0, 0),))
     plt.text(rank_xy[0, 2],  rank_xy[0, 3], 'MOORA RP', size = 12, ha = 'center', va = 'center', color = 'white', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0, 0, 0),))
     plt.text(rank_xy[0, 4],  rank_xy[0, 5], 'MULTIMOORA', size = 12, ha = 'center', va = 'center', color = 'white', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0, 0, 0),))
+    for i in range(1, rank_xy.shape[0]):
+        plt.text(rank_xy[i, 0],  rank_xy[i, 1], 'a' + str(int(flow_1[i-1,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = "round", ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),))
+        plt.text(rank_xy[i, 2],  rank_xy[i, 3], 'a' + str(int(flow_2[i-1,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),))
+        plt.text(rank_xy[i, 4],  rank_xy[i, 5], 'a' + str(int(flow_3[i-1,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),)) 
     for i in range(1, rank_xy.shape[0]-1):
-        plt.text(rank_xy[i, 0],  rank_xy[i, 1], 'a' + str(int(flow_1[i,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = "round", ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),))
-        plt.text(rank_xy[i, 2],  rank_xy[i, 3], 'a' + str(int(flow_2[i,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),))
-        plt.text(rank_xy[i, 4],  rank_xy[i, 5], 'a' + str(int(flow_3[i,0])), size = 12, ha = 'center', va = 'center', bbox = dict(boxstyle = 'round', ec = (0.0, 0.0, 0.0), fc = (0.8, 1.0, 0.8),)) 
-    for i in range(1, rank_xy.shape[0]-2):
         plt.arrow(rank_xy[i, 0], rank_xy[i, 1], rank_xy[i+1, 0] - rank_xy[i, 0], rank_xy[i+1, 1] - rank_xy[i, 1], head_width = 0.01, head_length = 0.2, overhang = 0.0, color = 'black', linewidth = 0.9, length_includes_head = True)
         plt.arrow(rank_xy[i, 2], rank_xy[i, 3], rank_xy[i+1, 2] - rank_xy[i, 2], rank_xy[i+1, 3] - rank_xy[i, 3], head_width = 0.01, head_length = 0.2, overhang = 0.0, color = 'black', linewidth = 0.9, length_includes_head = True)
         plt.arrow(rank_xy[i, 4], rank_xy[i, 5], rank_xy[i+1, 4] - rank_xy[i, 4], rank_xy[i+1, 5] - rank_xy[i, 5], head_width = 0.01, head_length = 0.2, overhang = 0.0, color = 'black', linewidth = 0.9, length_includes_head = True)
     axes = plt.gca()
     axes.set_xlim([-2, +2])
     ymin = np.amin(rank_xy[:,1])
     ymax = np.amax(rank_xy[:,1])
@@ -58,30 +58,33 @@
         s_m = np.sum(X[:,id2], axis = 1)
     Y1 = s_p - s_m
     for i in range(0, X.shape[1]):
         if ( criterion_type[i] == 'max'):
             best[i] = np.max(X[:,i])
         else:
             best[i] = np.min(X[:,i])
-    Y2   = np.max(np.absolute(X - best), axis = 1)
+    Y2 = np.max(np.absolute(X - best), axis = 1)
     if ( criterion_type[0] == 'max'):
-        Y3 = dataset[:,0]
+        Y3 = np.copy(dataset[:,0])
     else:
-        Y3 = 1/dataset[:,0]
+        Y3 = 1/np.copy(dataset[:,0])
     for i in range(0, dataset.shape[0]):
         for j in range(1, dataset.shape[1]):
             if ( criterion_type[j] == 'max'):
                 Y3[i] = Y3[i]*dataset[i,j] 
             else:
                 Y3[i] = Y3[i]/dataset[i,j] 
+    Y1     = Y1/np.max(Y1)
+    Y2     = Y2/np.max(Y2)
+    Y3     = Y3/np.max(Y3)
     flow_1 = np.copy(Y1)
     flow_1 = np.reshape(flow_1, (Y1.shape[0], 1))
     flow_1 = np.insert(flow_1, 0, list(range(1, Y1.shape[0]+1)), axis = 1)
     flow_2 = np.copy(Y2)
     flow_2 = np.reshape(flow_2, (Y2.shape[0], 1))
     flow_2 = np.insert(flow_2, 0, list(range(1, Y2.shape[0]+1)), axis = 1)
     flow_3 = np.copy(Y3)
     flow_3 = np.reshape(flow_3, (Y3.shape[0], 1))
     flow_3 = np.insert(flow_3, 0, list(range(1, Y3.shape[0]+1)), axis = 1)
     if (graph == True):
-        ranking(flow_1[np.argsort(flow_1[:, 1])], flow_2[np.argsort(flow_2[:, 1])], flow_3[np.argsort(flow_3[:, 1])])
+        ranking_m(flow_1[np.argsort(flow_1[:, 1])[::-1]], flow_2[np.argsort(flow_2[:, 1])], flow_3[np.argsort(flow_3[:, 1])[::-1]])
     return flow_1, flow_2, flow_3
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/ocra.py` & `pyDecision-4.0.4/pyDecision/algorithm/ocra.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function:  OCRA (Operational Competitiveness RAting)
-def ocra_method(dataset, weights, criterion_type, graph = True):
+def ocra_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X       = np.copy(dataset)/1.0
     I       = np.zeros(X.shape[0])
     O       = np.zeros(X.shape[0])    
     weights = np.array(weights)
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
             A = (X[:,j] - np.min(X[:,j])) / np.min(X[:,j])
@@ -44,16 +44,17 @@
             B = (np.max(X[:,j]) - X[:,j]) / np.min(X[:,j])
             for k in range(0, B.shape[0]):
                 B[k] = B[k] * weights[j]
             I = I + B
     O = O - np.min(O)
     I = I - np.min(I)
     r = (I + O) - np.min(I + O)
-    for i in range(0, r.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(r[i], 2)))
+    if (verbose == True):
+        for i in range(0, r.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(r[i], 2)))
     if ( graph == True):
         flow = np.copy(r)
         flow = np.reshape(flow, (r.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, r.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_i.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_ii.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_ii.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,27 +94,28 @@
     plt.axis('off')
     plt.show() 
     return
 
 ###############################################################################
 
 # Function: Promethee II
-def promethee_ii(dataset, W, Q, S, P, F, sort = True, topn = 0, graph = False):
+def promethee_ii(dataset, W, Q, S, P, F, sort = True, topn = 0, graph = False, verbose = True):
     pd_matrix  = preference_degree(dataset, W, Q, S, P, F)
     flow_plus  = np.sum(pd_matrix, axis = 1)/(pd_matrix.shape[0] - 1)
     flow_minus = np.sum(pd_matrix, axis = 0)/(pd_matrix.shape[0] - 1)
     flow       = flow_plus - flow_minus 
     flow       = np.reshape(flow, (pd_matrix.shape[0], 1))
     flow       = np.insert(flow, 0, list(range(1, pd_matrix.shape[0]+1)), axis = 1)
     if (sort == True or graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
     if (topn > 0):
         if (topn > pd_matrix.shape[0]):
             topn = pd_matrix.shape[0]
-        for i in range(0, topn):
-            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+        if (verbose == True):
+            for i in range(0, topn):
+                print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_iii.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_iv.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_iv.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,27 +151,28 @@
     plt.axis('off')
     plt.show() 
     return
 
 ###############################################################################
 
 # Function: Promethee IV
-def promethee_iv(dataset, W, Q, S, P, F, sort = True, steps = 0.001, topn = 0, graph = False):
+def promethee_iv(dataset, W, Q, S, P, F, sort = True, steps = 0.001, topn = 0, graph = False, verbose = True):
     pd_matrix  = integration_prefence_degree(dataset, W, Q, S, P, F, steps)
     flow_plus  = np.sum(pd_matrix, axis = 1)/(pd_matrix.shape[0] - 1)
     flow_minus = np.sum(pd_matrix, axis = 0)/(pd_matrix.shape[0] - 1)
     flow       = flow_plus - flow_minus 
     flow       = np.reshape(flow, (pd_matrix.shape[0], 1))
     flow       = np.insert(flow, 0, list(range(1, pd_matrix.shape[0]+1)), axis = 1)
     if (sort == True or graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
     if (topn > 0):
         if (topn > pd_matrix.shape[0]):
             topn = pd_matrix.shape[0]
-        for i in range(0, topn):
-            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3)))  
+        if (verbose == True):
+            for i in range(0, topn):
+                print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3)))  
     if (graph == True):
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_v.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_v.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         for i in range(0, topn):
             print("a" + str(int(flow[i,0])) + ": " + str(round(flow[i,1], 3)))         
     return flow
 
 ###############################################################################
     
 # Function: Promethee V
-def promethee_v(dataset, W, Q, S, P, F, sort = True, criteria = 1, cost = [], budget = 0, forbidden = [], iterations = 500):
+def promethee_v(dataset, W, Q, S, P, F, sort = True, criteria = 1, cost = [], budget = 0, forbidden = [], iterations = 500, verbose = True):
     flow = promethee_ii(dataset, W, Q, S, P, F, sort = sort, topn = 0)
     def flow_set(variables):
         flow_sum = 0
         cost_sum = 0
         actions  = []
         obj_function_1 = 0
         obj_function_2 = 0
@@ -119,15 +119,15 @@
             obj_function_2 = 0
         for i in range(0, len(forbidden)):
             if ( set(forbidden[i]).issubset( set(actions) ) ):
                 obj_function_3 = 1
             else:
                 obj_function_3 = 0                
         return (1/flow_sum) + obj_function_1 + obj_function_2 + obj_function_3
-    ga = genetic_algorithm(population_size = 100, mutation_rate = 0.1, elite = 0, min_values = [0]*flow.shape[0], max_values = [1]*flow.shape[0], eta = 1, mu = 1, generations = iterations, target_function = flow_set)
+    ga = genetic_algorithm(population_size = 100, mutation_rate = 0.1, elite = 0, min_values = [0]*flow.shape[0], max_values = [1]*flow.shape[0], eta = 1, mu = 1, generations = iterations, target_function = flow_set, verbose = verbose)
     for i in range(0, len(ga)-1):
         if (ga[i] > 0.5):
             ga[i] = 1
         else:
             ga[i] = 0
     ga      = np.reshape(ga[:-1], (flow.shape[0], 1))
     flow    = np.hstack((flow, ga))
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_vi.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_vi.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     plt.axis('off')
     plt.show() 
     return
 
 ###############################################################################
 
 # Function: Promethee VI
-def promethee_vi(dataset, W_lower, W_upper, Q, S, P, F, sort = True, topn = 0, iterations = 1000, graph = False):
+def promethee_vi(dataset, W_lower, W_upper, Q, S, P, F, sort = True, topn = 0, iterations = 1000, graph = False, verbose = True):
     pd_matrix_1  = preference_degree(dataset, W_lower, Q, S, P, F)
     flow_plus_1  = np.sum(pd_matrix_1, axis = 1)/(pd_matrix_1.shape[0] - 1)
     flow_minus_1 = np.sum(pd_matrix_1, axis = 0)/(pd_matrix_1.shape[0] - 1)
     flow_1       = flow_plus_1 - flow_minus_1 
     pd_matrix_2  = preference_degree(dataset, W_upper, Q, S, P, F)
     flow_plus_2  = np.sum(pd_matrix_2, axis = 1)/(pd_matrix_2.shape[0] - 1)
     flow_minus_2 = np.sum(pd_matrix_2, axis = 0)/(pd_matrix_2.shape[0] - 1)
@@ -146,14 +146,15 @@
         flow_2 = flow_2[np.argsort(flow_2[:, 1])]
         flow_2 = flow_2[::-1]
         flow_3 = flow_3[np.argsort(flow_3[:, 1])]
         flow_3 = flow_3[::-1]
     if (topn > 0):
         if (topn > pd_matrix.shape[0]):
             topn = pd_matrix.shape[0]
-        for i in range(0, topn):
-            print('a' + str(int(flow_3[i,0])) + ': ' + str(round(flow_3[i,1], 3))) 
+        if (verbose == True):
+            for i in range(0, topn):
+                print('a' + str(int(flow_3[i,0])) + ': ' + str(round(flow_3[i,1], 3))) 
     if (graph == True):
         ranking(flow_1, flow_2, flow_3)
     return flow_1, flow_3, flow_2
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.0.4/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/piv.py` & `pyDecision-4.0.4/pyDecision/algorithm/piv.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: PIV (Proximity Indexed Value)
-def piv_method(dataset, weights, criterion_type, graph = True):
+def piv_method(dataset, weights, criterion_type, graph = True, verbose = True):
     X  = np.copy(dataset)/1.0
     for j in range(0, X.shape[1]):
         X[:,j] = (X[:,j] / (np.sum(X[:,j]**2))**(1/2))*weights[j]
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
             X[:,j] = np.max(X[:,j]) - X[:,j]
         else:
             X[:,j] = X[:,j] - np.min(X[:,j])
     D = np.sum(X, axis = 1)
-    for i in range(0, D.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(D[i], 2)))
+    if (verbose == True):
+        for i in range(0, D.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(D[i], 2)))
     if ( graph == True):
         flow = np.copy(D)
         flow = np.reshape(flow, (D.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, D.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
-        flow = flow[::-1]
         ranking(flow)
     return D
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/saw.py` & `pyDecision-4.0.4/pyDecision/algorithm/saw.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,28 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: SAW
-def saw_method(dataset, criterion_type, weights, graph = True):
+def saw_method(dataset, criterion_type, weights, graph = True, verbose = True):
     X = np.copy(dataset)/1.0
     for i in range(0, X.shape[1]):
         if ( criterion_type[i] == 'max'):
             X[:,i] = (X[:,i] / np.max(X[:,i]))*weights[i]
         else:
             X[:,i] = (np.min(X[:,i]) / X[:,i])*weights[i]
     Y    = np.sum(X, axis = 1)
     flow = np.copy(Y)
     flow = np.reshape(flow, (Y.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/smart.py` & `pyDecision-4.0.4/pyDecision/algorithm/smart.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,31 +26,32 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: SMART
-def smart_method(dataset, grades, lower, upper, criterion_type, graph = True):
+def smart_method(dataset, grades, lower, upper, criterion_type, graph = True, verbose = True):
     w = np.copy(grades)/1.0
     for i in range(0, w.shape[0]):
         w[i] = (2**(1/2))**w[i]
     w = w/np.sum(w)
     X = np.copy(dataset)/1.0
     for i in range(0, X.shape[1]):
         if ( criterion_type[i] == 'max'):
             X[:,i] =  4 + np.log2( ((dataset[:,i] - lower[i] ) / (upper[i] - lower[i]))*(64) ) 
         else:
             X[:,i] = 10 - np.log2( ((dataset[:,i] - lower[i] ) / (upper[i] - lower[i]))*(64) ) 
     Y    = np.sum(X*w, axis = 1)
     flow = np.copy(Y)
     flow = np.reshape(flow, (Y.shape[0], 1))
     flow = np.insert(flow, 0, list(range(1, Y.shape[0]+1)), axis = 1)
-    for i in range(0, flow.shape[0]):
-        print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
+    if (verbose == True):
+        for i in range(0, flow.shape[0]):
+            print('a' + str(int(flow[i,0])) + ': ' + str(round(flow[i,1], 3))) 
     if (graph == True):
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
     return flow
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/todim.py` & `pyDecision-4.0.4/pyDecision/algorithm/todim.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
 # Function: TODIM (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making)
-def todim_method(dataset, criterion_type, weights, teta = 1, graph = True):
+def todim_method(dataset, criterion_type, weights, teta = 1, graph = True, verbose = True):
     X = np.copy(dataset)/1.0
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
             X[:,j] = X[:,j]  / np.sum(X[:,j]) 
         else:
             X[:,j] = (1/X[:,j])  / np.sum(1/X[:,j])       
     weights = weights/np.max(weights)
@@ -48,16 +48,17 @@
                         D[i, j] = D[i, j] + (weights[k]*(p_i - p_j) / np.sum(weights))**(1/2)
                     elif (p_i - p_j == 0):
                         D[i, j] = D[i, j] + 0
                     else:
                         D[i, j] = D[i, j] + (-1/teta)*(np.sum(weights)*(p_j - p_i)/weights[k])**(1/2)
     r  = np.sum(D, axis = 1) 
     r  = (r - np.min(r)) / (np.max(r) - np.min(r))
-    for i in range(0, r.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(r[i], 2)))
+    if (verbose == True):
+        for i in range(0, r.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(r[i], 2)))
     if ( graph == True):
         flow = np.copy(r)
         flow = np.reshape(flow, (r.shape[0], 1))
         flow = np.insert(flow, 0, list(range(1, r.shape[0]+1)), axis = 1)
         flow = flow[np.argsort(flow[:, 1])]
         flow = flow[::-1]
         ranking(flow)
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/topsis.py` & `pyDecision-4.0.4/pyDecision/algorithm/vikor.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,41 +24,62 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: TOPSIS
-def topsis_method(dataset, weights, criterion_type, graph = True):
-    X = np.copy(dataset)
-    w = np.copy(weights)
-    sum_cols = np.sum(X*X, axis = 0)
-    sum_cols = sum_cols**(1/2)
-    r_ij = X/sum_cols
-    v_ij = r_ij*w
-    p_ideal_A = np.zeros(X.shape[1])
-    n_ideal_A = np.zeros(X.shape[1])
+# Function: VIKOR
+def vikor_method(dataset, weights, criterion_type, strategy_coefficient = 0.5, graph = True, verbose = True):
+    X     = np.copy(dataset)
+    w     = np.copy(weights)
+    best  = np.zeros(X.shape[1])
+    worst = np.zeros(X.shape[1])
     for i in range(0, dataset.shape[1]):
         if (criterion_type[i] == 'max'):
-            p_ideal_A[i] = np.max(v_ij[:, i])
-            n_ideal_A[i] = np.min(v_ij[:, i])
+            best[i]  = np.max(X[:, i])
+            worst[i] = np.min(X[:, i])
         else:
-            p_ideal_A[i] = np.min(v_ij[:, i])
-            n_ideal_A[i] = np.max(v_ij[:, i]) 
-    p_s_ij = (v_ij - p_ideal_A)**2
-    p_s_ij = np.sum(p_s_ij, axis = 1)**(1/2)
-    n_s_ij = (v_ij - n_ideal_A)**2
-    n_s_ij = np.sum(n_s_ij, axis = 1)**(1/2)
-    c_i    = n_s_ij / ( p_s_ij  + n_s_ij )
-    for i in range(0, c_i.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(c_i[i], 2)))
+            best[i]  = np.min(X[:, i])
+            worst[i] = np.max(X[:, i]) 
+    s_i = w * ( abs(best - X) / (abs(best - worst) + 0.0000000000000001) )
+    r_i = np.max(s_i, axis = 1)
+    s_i = np.sum(s_i, axis = 1)
+    s_best = np.min(s_i)
+    s_worst = np.max(s_i)
+    r_best = np.min(r_i)
+    r_worst = np.max(r_i)
+    q_i = strategy_coefficient*( (s_i - s_best) / (s_worst - s_best) ) + (1 - strategy_coefficient)*( (r_i - r_best) / (r_worst - r_best) )
+    dq = 1 /(X.shape[0] - 1)
+    flow_s = np.copy(s_i)
+    flow_s = np.reshape(flow_s, (s_i.shape[0], 1))
+    flow_s = np.insert(flow_s, 0, list(range(1, s_i.shape[0]+1)), axis = 1)
+    flow_s = flow_s[np.argsort(flow_s[:, 1])]
+    flow_r = np.copy(r_i)
+    flow_r = np.reshape(flow_r, (r_i.shape[0], 1))
+    flow_r = np.insert(flow_r, 0, list(range(1, r_i.shape[0]+1)), axis = 1)
+    flow_r = flow_r[np.argsort(flow_r[:, 1])]
+    flow_q = np.copy(q_i)
+    flow_q = np.reshape(flow_q, (q_i.shape[0], 1))
+    flow_q = np.insert(flow_q, 0, list(range(1, q_i.shape[0]+1)), axis = 1)
+    flow_q = flow_q[np.argsort(flow_q[:, 1])]
+    condition_1 = False
+    condition_2 = False
+    if (flow_q[1, 1] - flow_q[0, 1] >= dq):
+        condition_1 = True
+    if (flow_q[0,0] == flow_s[0,0] or flow_q[0,0] == flow_r[0,0]):
+        condition_2 = True
+    solution = np.copy(flow_q)
+    if (condition_1 == True and condition_2 == False):
+        solution = np.copy(flow_q[0:2,:])
+    elif (condition_1 == False and condition_2 == True):
+        for i in range(solution.shape[0] -1, -1, -1):
+            if(solution[i, 1] - solution[0, 1] >= dq):
+              solution = np.delete(solution, i, axis = 0)  
+    if (verbose == True):
+        for i in range(0, solution.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(solution[i, 0], 2)))
     if ( graph == True):
-        flow = np.copy(c_i)
-        flow = np.reshape(flow, (c_i.shape[0], 1))
-        flow = np.insert(flow, 0, list(range(1, c_i.shape[0]+1)), axis = 1)
-        flow = flow[np.argsort(flow[:, 1])]
-        flow = flow[::-1]
-        ranking(flow)
-    return c_i
+        ranking(solution) 
+    return flow_s, flow_r, flow_q, solution
 
 ###############################################################################
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/vikor.py` & `pyDecision-4.0.4/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,61 +24,70 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: VIKOR
-def vikor_method(dataset, weights, criterion_type, strategy_coefficient = 0.5, graph = True):
-    X = np.copy(dataset)
-    w = np.copy(weights)
-    best  = np.zeros(X.shape[1])
-    worst = np.zeros(X.shape[1])
-    for i in range(0, dataset.shape[1]):
-        if (criterion_type[i] == 'max'):
-            best[i]  = np.max(X[:, i])
-            worst[i] = np.min(X[:, i])
-        else:
-            best[i]  = np.min(X[:, i])
-            worst[i] = np.max(X[:, i]) 
-    s_i = w*( abs(best - X) / abs(best - worst) )
-    r_i = np.max(s_i, axis = 1)
-    s_i = np.sum(s_i, axis = 1)
-    s_best = np.min(s_i)
-    s_worst = np.max(s_i)
-    r_best = np.min(r_i)
-    r_worst = np.max(r_i)
-    q_i = strategy_coefficient*( (s_i - s_best) / (s_worst - s_best) ) + (1 - strategy_coefficient)*( (r_i - r_best) / (r_worst - r_best) )
-    dq = 1 /(X.shape[0] - 1)
-    flow_s = np.copy(s_i)
-    flow_s = np.reshape(flow_s, (s_i.shape[0], 1))
-    flow_s = np.insert(flow_s, 0, list(range(1, s_i.shape[0]+1)), axis = 1)
-    flow_s = flow_s[np.argsort(flow_s[:, 1])]
-    flow_r = np.copy(r_i)
-    flow_r = np.reshape(flow_r, (r_i.shape[0], 1))
-    flow_r = np.insert(flow_r, 0, list(range(1, r_i.shape[0]+1)), axis = 1)
-    flow_r = flow_r[np.argsort(flow_r[:, 1])]
-    flow_q = np.copy(q_i)
-    flow_q = np.reshape(flow_q, (q_i.shape[0], 1))
-    flow_q = np.insert(flow_q, 0, list(range(1, q_i.shape[0]+1)), axis = 1)
-    flow_q = flow_q[np.argsort(flow_q[:, 1])]
-    condition_1 = False
-    condition_2 = False
-    if (flow_q[1, 1] - flow_q[0, 1] >= dq):
-        condition_1 = True
-    if (flow_q[0,0] == flow_s[0,0] or flow_q[0,0] == flow_r[0,0]):
-        condition_2 = True
-    solution = np.copy(flow_q)
-    if (condition_1 == True and condition_2 == False):
-        solution = np.copy(flow_q[0:2,:])
-    elif (condition_1 == False and condition_2 == True):
-        for i in range(solution.shape[0] -1, -1, -1):
-            if(solution[i, 1] - solution[0, 1] >= dq):
-              solution = np.delete(solution, i, axis = 0)  
-    for i in range(0, solution.shape[0]):
-        print('a' + str(i+1) + ': ' + str(round(solution[i, 0], 2)))
-    if ( graph == True):
-        ranking(solution) 
-    return flow_s, flow_r, flow_q, solution
-
-###############################################################################
+# Function: Fuzzy OCRA (Operational Competitiveness RAting)
+def fuzzy_ocra_method(dataset, weights, criterion_type, graph = True, verbose = True):
+    X_a        = np.zeros((len(dataset), len(dataset[0])))
+    X_b        = np.zeros((len(dataset), len(dataset[0])))
+    X_c        = np.zeros((len(dataset), len(dataset[0])))
+    I_a        = np.zeros((len(dataset)))
+    I_b        = np.zeros((len(dataset)))
+    I_c        = np.zeros((len(dataset)))
+    O_a        = np.zeros((len(dataset)))
+    O_b        = np.zeros((len(dataset)))
+    O_c        = np.zeros((len(dataset)))
+    P_a        = np.zeros((len(dataset)))
+    P_b        = np.zeros((len(dataset)))
+    P_c        = np.zeros((len(dataset)))
+    weights_a  = np.zeros(len(weights[0]))
+    weights_b  = np.zeros(len(weights[0]))
+    weights_c  = np.zeros(len(weights[0]))
+    for j in range(0, X_a.shape[1]):
+        weights_a[j] = weights[0][j][0]
+        weights_b[j] = weights[0][j][1]
+        weights_c[j] = weights[0][j][2]
+        for i in range(0, X_a.shape[0]):
+            a, b, c  = dataset[i][j]
+            X_a[i,j] = a
+            X_b[i,j] = b
+            X_c[i,j] = c
+    for i in range(0, X_a.shape[0]):
+        for j in range(0, X_a.shape[1]):
+            if (criterion_type[j] == 'max'):
+                O_a[i] = O_a[i] + weights_a[j] * (X_a[i, j] -  np.min(X_a[:, j])) / np.min(X_a[:, j])
+                O_b[i] = O_b[i] + weights_b[j] * (X_b[i, j] -  np.min(X_b[:, j])) / np.min(X_b[:, j])
+                O_c[i] = O_c[i] + weights_c[j] * (X_c[i, j] -  np.min(X_c[:, j])) / np.min(X_c[:, j])
+            else:
+                I_a[i] = I_a[i] + weights_a[j] * (np.max(X_a[:, j]) - X_a[i, j]) / np.min(X_a[:, j])
+                I_b[i] = I_b[i] + weights_b[j] * (np.max(X_b[:, j]) - X_b[i, j]) / np.min(X_b[:, j])
+                I_c[i] = I_c[i] + weights_c[j] * (np.max(X_c[:, j]) - X_c[i, j]) / np.min(X_c[:, j])
+    min_i_a = np.min(I_a)
+    min_i_b = np.min(I_b)
+    min_i_c = np.min(I_c)
+    min_o_a = np.min(O_a)
+    min_o_b = np.min(O_b)
+    min_o_c = np.min(O_c)
+    I_a     = I_a - min_i_a
+    I_b     = I_b - min_i_b
+    I_c     = I_c - min_i_c
+    O_a     = O_a - min_o_a
+    O_b     = O_b - min_o_b
+    O_c     = O_c - min_o_c
+    P_a     = I_a + O_a - np.min(I_a + O_a)
+    P_b     = I_b + O_b - np.min(I_b + O_b)
+    P_c     = I_c + O_c - np.min(I_c + O_c)
+    P       = (P_a + P_b + P_c) / 3
+    if (verbose == True):
+        for i in range(0, P.shape[0]):
+            print('a' + str(i+1) + ': ' + str(round(P[i], 3))) 
+    if (graph == True):
+        flow = np.copy(P)
+        flow = np.reshape(flow, (P.shape[0], 1))
+        flow = np.insert(flow, 0, list(range(1, P.shape[0]+1)), axis = 1)
+        flow = flow[np.argsort(flow[:, 1])]
+        flow = flow[::-1]
+        ranking(flow)
+    return P
```

### Comparing `pyDecision-3.0.3/pyDecision/algorithm/wings.py` & `pyDecision-4.0.4/pyDecision/algorithm/wings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Required Libraries
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 ###############################################################################
 
-# Function: DEMATEL
+# Function: WINGS (Weighted Influence Non-linear Gauge System)
 def wings_method(dataset, size_x = 10, size_y = 10): 
     D = dataset
     C = D/np.sum(D)
     I = np.eye(dataset.shape[0])
     T = np.dot(C, np.linalg.inv( I - C ))
     c_i = np.sum(T, axis = 0)
     r_i = np.sum(T, axis = 1)
```

### Comparing `pyDecision-3.0.3/pyDecision/util/ga.py` & `pyDecision-4.0.4/pyDecision/util/ga.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 # PEREIRA, V. (2022). GitHub repository: https://github.com/Valdecy/pyMetaheuristic
 
 ############################################################################
 
 # Required Libraries
 import numpy  as np
-import math
 import random
 import os
 
 ############################################################################
 
 # Function
 def target_function():
```

### Comparing `pyDecision-3.0.3/pyDecision/util/gwo.py` & `pyDecision-4.0.4/pyDecision/util/gwo.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 # PEREIRA, V. (2022). GitHub repository: https://github.com/Valdecy/pyMetaheuristic
 
 ############################################################################
 
 # Required Libraries
 import numpy  as np
-import math
 import random
 import os
 
 ############################################################################
 
 # Function
 def target_function():
```

### Comparing `pyDecision-3.0.3/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.0.4/pyDecision.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 3.0.3
+Version: 4.0.4
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+
+pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -61,26 +63,30 @@
 ```
 
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
+- Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2021/8545379))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
+- Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://link.springer.com/article/10.1007/bf01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
+- Entropy ([ Colab Demo ](Entropy)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
@@ -88,37 +94,46 @@
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
+- Fuzzy MOORA ([ Colab Demo ]()) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
+- Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
+- PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
+- ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
 
-4. Advanced MCDA Methods:
+4. Compare Methods:
+- Compare Ranks & Ask chatGPT([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
+- Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
+- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+
+5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
 
 # Acknowledgement
```

### Comparing `pyDecision-3.0.3/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.0.4/pyDecision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 pyDecision/algorithm/ahp.py
 pyDecision/algorithm/aras.py
 pyDecision/algorithm/borda.py
 pyDecision/algorithm/bwm.py
 pyDecision/algorithm/cilos.py
 pyDecision/algorithm/cocoso.py
 pyDecision/algorithm/codas.py
+pyDecision/algorithm/copeland.py
 pyDecision/algorithm/copras.py
 pyDecision/algorithm/cradis.py
 pyDecision/algorithm/critic.py
 pyDecision/algorithm/dematel.py
 pyDecision/algorithm/e_i.py
 pyDecision/algorithm/e_i_s.py
 pyDecision/algorithm/e_i_v.py
 pyDecision/algorithm/e_ii.py
 pyDecision/algorithm/e_iii.py
 pyDecision/algorithm/e_iv.py
 pyDecision/algorithm/e_tri_b.py
 pyDecision/algorithm/edas.py
+pyDecision/algorithm/entropy.py
 pyDecision/algorithm/fuzzy_ahp.py
+pyDecision/algorithm/fuzzy_aras.py
+pyDecision/algorithm/fuzzy_copras.py
 pyDecision/algorithm/fuzzy_dematel.py
 pyDecision/algorithm/fuzzy_edas.py
+pyDecision/algorithm/fuzzy_moora.py
+pyDecision/algorithm/fuzzy_ocra.py
 pyDecision/algorithm/fuzzy_topsis.py
 pyDecision/algorithm/fuzzy_vikor.py
 pyDecision/algorithm/gra.py
 pyDecision/algorithm/idocriw.py
 pyDecision/algorithm/mabac.py
 pyDecision/algorithm/mairca.py
 pyDecision/algorithm/marcos.py
@@ -47,17 +53,21 @@
 pyDecision/algorithm/p_ii.py
 pyDecision/algorithm/p_iii.py
 pyDecision/algorithm/p_iv.py
 pyDecision/algorithm/p_v.py
 pyDecision/algorithm/p_vi.py
 pyDecision/algorithm/p_xgaia.py
 pyDecision/algorithm/piv.py
+pyDecision/algorithm/psi.py
+pyDecision/algorithm/rov.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
 pyDecision/algorithm/wings.py
+pyDecision/util/LLM.py
 pyDecision/util/__init__.py
+pyDecision/util/compare.py
 pyDecision/util/ga.py
 pyDecision/util/gwo.py
```

### Comparing `pyDecision-3.0.3/setup.py` & `pyDecision-4.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='3.0.3',
+    version='4.0.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
+        'openai',
+		'pandas',
         'scikit-learn',
         'scipy'
     ],
     description='A MCDA Library',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

