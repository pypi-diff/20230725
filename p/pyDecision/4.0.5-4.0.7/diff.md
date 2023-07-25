# Comparing `tmp/pyDecision-4.0.5.tar.gz` & `tmp/pyDecision-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.0.5.tar", last modified: Tue Jul 25 21:45:19 2023, max compression
+gzip compressed data, was "dist\pyDecision-4.0.7.tar", last modified: Tue Jul 25 21:53:48 2023, max compression
```

## Comparing `pyDecision-4.0.5.tar` & `pyDecision-4.0.7.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 21:45:19.000000 pyDecision-4.0.5/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.0.5/LICENSE
--rw-rw-rw-   0        0        0    16107 2023-07-25 21:45:19.000000 pyDecision-4.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    15694 2023-07-25 21:20:13.000000 pyDecision-4.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 21:45:19.000000 pyDecision-4.0.5/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.0.5/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:45:19.000000 pyDecision-4.0.5/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2379 2023-07-23 16:35:36.000000 pyDecision-4.0.5/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.0.5/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.0.5/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.0.5/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.0.5/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.0.5/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.0.5/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.0.5/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.0.5/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.0.5/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.0.5/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.0.5/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.0.5/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.0.5/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.0.5/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.0.5/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.0.5/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.0.5/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.0.5/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.0.5/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.0.5/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.0.5/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.0.5/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.0.5/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.0.5/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.0.5/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.0.5/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.0.5/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.0.5/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.0.5/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.0.5/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.0.5/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.0.5/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.0.5/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.0.5/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.0.5/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.0.5/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.0.5/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.0.5/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.0.5/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.0.5/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.0.5/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.0.5/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.0.5/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.0.5/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.0.5/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.0.5/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.0.5/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.0.5/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.0.5/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.0.5/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:45:19.000000 pyDecision-4.0.5/pyDecision/util/
--rw-rw-rw-   0        0        0     3151 2023-07-25 21:32:57.000000 pyDecision-4.0.5/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      179 2023-07-25 21:37:55.000000 pyDecision-4.0.5/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0    15667 2023-07-25 21:44:53.000000 pyDecision-4.0.5/pyDecision/util/compare.py
--rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.0.5/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.0.5/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:45:19.000000 pyDecision-4.0.5/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    16107 2023-07-25 21:45:18.000000 pyDecision-4.0.5/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2165 2023-07-25 21:45:19.000000 pyDecision-4.0.5/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 21:45:18.000000 pyDecision-4.0.5/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-25 21:45:18.000000 pyDecision-4.0.5/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 21:45:18.000000 pyDecision-4.0.5/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 21:45:19.000000 pyDecision-4.0.5/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-07-25 21:42:26.000000 pyDecision-4.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.0.7/LICENSE
+-rw-rw-rw-   0        0        0    16107 2023-07-25 21:53:48.000000 pyDecision-4.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15694 2023-07-25 21:20:13.000000 pyDecision-4.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.0.7/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2379 2023-07-23 16:35:36.000000 pyDecision-4.0.7/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.0.7/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.0.7/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.0.7/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.0.7/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.0.7/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.0.7/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.0.7/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.0.7/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.0.7/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.0.7/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.0.7/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.0.7/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.0.7/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.0.7/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.0.7/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.0.7/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.0.7/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.0.7/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.0.7/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.0.7/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.0.7/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.0.7/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.0.7/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.0.7/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.0.7/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.0.7/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.0.7/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.0.7/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.0.7/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.0.7/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.0.7/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.0.7/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.0.7/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.0.7/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.0.7/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.0.7/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.0.7/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.0.7/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.0.7/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.0.7/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.0.7/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.0.7/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.0.7/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.0.7/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.0.7/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.0.7/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.0.7/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.0.7/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.0.7/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.0.7/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/pyDecision/compare/
+-rw-rw-rw-   0        0        0       94 2023-07-25 21:52:02.000000 pyDecision-4.0.7/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    18201 2023-07-25 21:53:22.000000 pyDecision-4.0.7/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/pyDecision/util/
+-rw-rw-rw-   0        0        0     3151 2023-07-25 21:32:57.000000 pyDecision-4.0.7/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      138 2023-07-25 21:52:24.000000 pyDecision-4.0.7/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.0.7/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.0.7/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:53:48.000000 pyDecision-4.0.7/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    16107 2023-07-25 21:53:47.000000 pyDecision-4.0.7/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2199 2023-07-25 21:53:47.000000 pyDecision-4.0.7/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:53:47.000000 pyDecision-4.0.7/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-25 21:53:47.000000 pyDecision-4.0.7/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 21:53:47.000000 pyDecision-4.0.7/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 21:53:48.000000 pyDecision-4.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-07-25 21:53:41.000000 pyDecision-4.0.7/setup.py
```

### Comparing `pyDecision-4.0.5/LICENSE` & `pyDecision-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/PKG-INFO` & `pyDecision-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.0.5
+Version: 4.0.7
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-4.0.5/README.md` & `pyDecision-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/__init__.py` & `pyDecision-4.0.7/pyDecision/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/ahp.py` & `pyDecision-4.0.7/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/aras.py` & `pyDecision-4.0.7/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/borda.py` & `pyDecision-4.0.7/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/bwm.py` & `pyDecision-4.0.7/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/cilos.py` & `pyDecision-4.0.7/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/cocoso.py` & `pyDecision-4.0.7/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/codas.py` & `pyDecision-4.0.7/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/copeland.py` & `pyDecision-4.0.7/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/copras.py` & `pyDecision-4.0.7/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/cradis.py` & `pyDecision-4.0.7/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/critic.py` & `pyDecision-4.0.7/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/dematel.py` & `pyDecision-4.0.7/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_i.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_ii.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_iii.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_iv.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.0.7/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/edas.py` & `pyDecision-4.0.7/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/entropy.py` & `pyDecision-4.0.7/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.0.7/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/gra.py` & `pyDecision-4.0.7/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/idocriw.py` & `pyDecision-4.0.7/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/mabac.py` & `pyDecision-4.0.7/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/mairca.py` & `pyDecision-4.0.7/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/marcos.py` & `pyDecision-4.0.7/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/maut.py` & `pyDecision-4.0.7/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/merec.py` & `pyDecision-4.0.7/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/moora.py` & `pyDecision-4.0.7/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/moosra.py` & `pyDecision-4.0.7/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/multimoora.py` & `pyDecision-4.0.7/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/ocra.py` & `pyDecision-4.0.7/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_i.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_ii.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_iii.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_iv.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_v.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_vi.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.0.7/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/piv.py` & `pyDecision-4.0.7/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/psi.py` & `pyDecision-4.0.7/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/rov.py` & `pyDecision-4.0.7/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/saw.py` & `pyDecision-4.0.7/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/smart.py` & `pyDecision-4.0.7/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/todim.py` & `pyDecision-4.0.7/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/topsis.py` & `pyDecision-4.0.7/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/vikor.py` & `pyDecision-4.0.7/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/waspas.py` & `pyDecision-4.0.7/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/algorithm/wings.py` & `pyDecision-4.0.7/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/util/LLM.py` & `pyDecision-4.0.7/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/util/compare.py` & `pyDecision-4.0.7/pyDecision/compare/compare.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,59 @@
 # Required Libraries
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 
 from scipy.stats import rankdata
+
+###############################################################################
+
+from pyDecision.algorithm.bwm          import bw_method
+from pyDecision.algorithm.cilos        import cilos_method
+from pyDecision.algorithm.critic       import critic_method
+from pyDecision.algorithm.entropy      import entropy_method
+from pyDecision.algorithm.idocriw      import idocriw_method
+from pyDecision.algorithm.merec        import merec_method
+
+from pyDecision.algorithm.aras         import aras_method
+from pyDecision.algorithm.borda        import borda_method
+from pyDecision.algorithm.cocoso       import cocoso_method
+from pyDecision.algorithm.codas        import codas_method
+from pyDecision.algorithm.copeland     import copeland_method
+from pyDecision.algorithm.copras       import copras_method
+from pyDecision.algorithm.cradis       import cradis_method
+from pyDecision.algorithm.edas         import edas_method
+from pyDecision.algorithm.gra          import gra_method
+from pyDecision.algorithm.mabac        import mabac_method
+from pyDecision.algorithm.mairca       import mairca_method
+from pyDecision.algorithm.marcos       import marcos_method
+from pyDecision.algorithm.maut         import maut_method
+from pyDecision.algorithm.moora        import moora_method
+from pyDecision.algorithm.moosra       import moosra_method
+from pyDecision.algorithm.multimoora   import multimoora_method
+from pyDecision.algorithm.ocra         import ocra_method
+from pyDecision.algorithm.piv          import piv_method
+from pyDecision.algorithm.p_ii         import promethee_ii
+from pyDecision.algorithm.p_iv         import promethee_iv
+from pyDecision.algorithm.psi          import psi_method
+from pyDecision.algorithm.rov          import rov_method
+from pyDecision.algorithm.saw          import saw_method
+from pyDecision.algorithm.todim        import todim_method
+from pyDecision.algorithm.topsis       import topsis_method
+from pyDecision.algorithm.vikor        import vikor_method
+from pyDecision.algorithm.waspas       import waspas_method
+
+from pyDecision.algorithm.fuzzy_aras   import fuzzy_aras_method
+from pyDecision.algorithm.fuzzy_copras import fuzzy_copras_method
+from pyDecision.algorithm.fuzzy_edas   import fuzzy_edas_method
+from pyDecision.algorithm.fuzzy_moora  import fuzzy_moora_method
+from pyDecision.algorithm.fuzzy_ocra   import fuzzy_ocra_method
+from pyDecision.algorithm.fuzzy_topsis import fuzzy_topsis_method
+from pyDecision.algorithm.fuzzy_vikor  import fuzzy_vikor_method
  
 ###############################################################################
 
 # Function: Tranpose Dictionary
 def transpose_dict(rank_count_dict):
     transposed_dict = {}
     list_length = len(next(iter(rank_count_dict.values())))
```

### Comparing `pyDecision-4.0.5/pyDecision/util/ga.py` & `pyDecision-4.0.7/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision/util/gwo.py` & `pyDecision-4.0.7/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.0.5/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.0.7/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.0.5
+Version: 4.0.7
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-4.0.5/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.0.7/pyDecision.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,12 +62,13 @@
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
 pyDecision/algorithm/wings.py
+pyDecision/compare/__init__.py
+pyDecision/compare/compare.py
 pyDecision/util/LLM.py
 pyDecision/util/__init__.py
-pyDecision/util/compare.py
 pyDecision/util/ga.py
 pyDecision/util/gwo.py
```

### Comparing `pyDecision-4.0.5/setup.py` & `pyDecision-4.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.0.5',
+    version='4.0.7',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

