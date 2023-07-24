# Comparing `tmp/mio-cli-1.3.3.tar.gz` & `tmp/mio-cli-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmpt8dqxwto/mio-cli-1.3.3.tar", last modified: Mon Jul 24 22:50:02 2023, max compression
+gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmpziiwsgd2/mio-cli-1.3.4.tar", last modified: Mon Jul 24 23:07:32 2023, max compression
```

## Comparing `mio-cli-1.3.3.tar` & `mio-cli-1.3.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:02.000000 mio-cli-1.3.3/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/data/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.3.3/src/data/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.3.3/src/data/doxygen-awesome-darkmode-toggle.js
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.3.3/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.3.3/src/data/doxygen-awesome-sidebar-only.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.3.3/src/data/doxygen-awesome.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.3.3/src/data/doxygen.awesome.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.3.3/src/data/doxygen.private.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.3.3/src/data/doxygen.public.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.3.3/src/data/doxygen_footer.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.3.3/src/data/doxygen_header.awesome.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.3.3/src/data/doxygen_header.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.3.3/src/data/doxygen_layout.xml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.3.3/src/data/doxygen_stylesheet.css
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.3.3/src/data/idv_doxyfilter_sv.pl
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.3.3/src/data/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.3.3/src/data/plantuml.jar
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:02.000000 mio-cli-1.3.3/src/mio/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.3.3/src/mio/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.3.3/src/mio/__main__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49803 2023-03-28 19:31:34.000000 mio-cli-1.3.3/src/mio/cache.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9051 2023-05-16 18:43:34.000000 mio-cli-1.3.3/src/mio/cfg.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.3.3/src/mio/clean.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21825 2023-06-21 19:09:11.000000 mio-cli-1.3.3/src/mio/cli.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.3.3/src/mio/common.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.3.3/src/mio/cov.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.3.3/src/mio/doctor.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.3.3/src/mio/dox.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    91261 2023-07-24 14:15:39.000000 mio-cli-1.3.3/src/mio/eal.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12586 2023-07-24 15:43:17.000000 mio-cli-1.3.3/src/mio/help_text.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.3.3/src/mio/init.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.3.3/src/mio/install.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-02-20 21:32:41.000000 mio-cli-1.3.3/src/mio/main.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2676 2023-06-20 06:56:36.000000 mio-cli-1.3.3/src/mio/new.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16358 2023-03-14 00:06:11.000000 mio-cli-1.3.3/src/mio/publish.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35707 2023-04-02 01:22:56.000000 mio-cli-1.3.3/src/mio/regr.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.3.3/src/mio/results.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27745 2023-07-24 15:42:50.000000 mio-cli-1.3.3/src/mio/sim.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.3.3/src/mio/user.py
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:02.000000 mio-cli-1.3.3/src/mio_cli.egg-info/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.3.3/src/mio_cli.egg-info/not-zip-safe
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/requires.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2023-07-24 22:50:01.000000 mio-cli-1.3.3/src/mio_cli.egg-info/top_level.txt
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 22:50:02.000000 mio-cli-1.3.3/src/templates/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.3.3/src/templates/LICENSE_solderpad_v2p1.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.3.3/src/templates/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.3.3/src/templates/dv_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.3.3/src/templates/interactive_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.3.3/src/templates/mdc.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.3.3/src/templates/mdc.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.3.3/src/templates/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.3.3/src/templates/project_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.3.3/src/templates/qst.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.3.3/src/templates/qst.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.3.3/src/templates/regression_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.3.3/src/templates/riv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.3.3/src/templates/riv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.3.3/src/templates/rtl_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.3.3/src/templates/sim_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.3.3/src/templates/ts.yml.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.3.3/src/templates/vcs.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.3.3/src/templates/vcs.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.3.3/src/templates/viv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.3.3/src/templates/viv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.3.3/src/templates/viv.prj.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.3.3/src/templates/vivado_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.3.3/src/templates/xcl.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.3.3/src/templates/xcl.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.3.3/LICENSE
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio-cli-1.3.3/README.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.3.3/pyproject.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2023-07-24 22:50:02.000000 mio-cli-1.3.3/setup.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-07-24 22:50:02.000000 mio-cli-1.3.3/PKG-INFO
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:32.000000 mio-cli-1.3.4/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/data/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.3.4/src/data/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.3.4/src/data/doxygen-awesome-darkmode-toggle.js
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.3.4/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.3.4/src/data/doxygen-awesome-sidebar-only.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.3.4/src/data/doxygen-awesome.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.3.4/src/data/doxygen.awesome.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.3.4/src/data/doxygen.private.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.3.4/src/data/doxygen.public.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.3.4/src/data/doxygen_footer.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.3.4/src/data/doxygen_header.awesome.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.3.4/src/data/doxygen_header.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.3.4/src/data/doxygen_layout.xml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.3.4/src/data/doxygen_stylesheet.css
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.3.4/src/data/idv_doxyfilter_sv.pl
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.3.4/src/data/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.3.4/src/data/plantuml.jar
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:32.000000 mio-cli-1.3.4/src/mio/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.3.4/src/mio/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.3.4/src/mio/__main__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49803 2023-03-28 19:31:34.000000 mio-cli-1.3.4/src/mio/cache.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9051 2023-05-16 18:43:34.000000 mio-cli-1.3.4/src/mio/cfg.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.3.4/src/mio/clean.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21825 2023-06-21 19:09:11.000000 mio-cli-1.3.4/src/mio/cli.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.3.4/src/mio/common.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.3.4/src/mio/cov.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.3.4/src/mio/doctor.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.3.4/src/mio/dox.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    91267 2023-07-24 23:05:08.000000 mio-cli-1.3.4/src/mio/eal.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12586 2023-07-24 23:05:55.000000 mio-cli-1.3.4/src/mio/help_text.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.3.4/src/mio/init.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.3.4/src/mio/install.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-02-20 21:32:41.000000 mio-cli-1.3.4/src/mio/main.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2676 2023-06-20 06:56:36.000000 mio-cli-1.3.4/src/mio/new.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16358 2023-03-14 00:06:11.000000 mio-cli-1.3.4/src/mio/publish.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35707 2023-04-02 01:22:56.000000 mio-cli-1.3.4/src/mio/regr.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.3.4/src/mio/results.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27745 2023-07-24 15:42:50.000000 mio-cli-1.3.4/src/mio/sim.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.3.4/src/mio/user.py
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:32.000000 mio-cli-1.3.4/src/mio_cli.egg-info/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.3.4/src/mio_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/requires.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2023-07-24 23:07:31.000000 mio-cli-1.3.4/src/mio_cli.egg-info/top_level.txt
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-07-24 23:07:32.000000 mio-cli-1.3.4/src/templates/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.3.4/src/templates/LICENSE_solderpad_v2p1.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.3.4/src/templates/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.3.4/src/templates/dv_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.3.4/src/templates/interactive_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.3.4/src/templates/mdc.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.3.4/src/templates/mdc.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.3.4/src/templates/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.3.4/src/templates/project_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.3.4/src/templates/qst.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.3.4/src/templates/qst.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.3.4/src/templates/regression_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.3.4/src/templates/riv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.3.4/src/templates/riv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.3.4/src/templates/rtl_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.3.4/src/templates/sim_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.3.4/src/templates/ts.yml.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.3.4/src/templates/vcs.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.3.4/src/templates/vcs.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.3.4/src/templates/viv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.3.4/src/templates/viv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.3.4/src/templates/viv.prj.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.3.4/src/templates/vivado_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.3.4/src/templates/xcl.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.3.4/src/templates/xcl.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.3.4/LICENSE
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio-cli-1.3.4/README.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.3.4/pyproject.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2023-07-24 23:07:32.000000 mio-cli-1.3.4/setup.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-07-24 23:07:32.000000 mio-cli-1.3.4/PKG-INFO
```

### Comparing `mio-cli-1.3.3/src/data/doxygen-awesome-darkmode-toggle.js` & `mio-cli-1.3.4/src/data/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `mio-cli-1.3.4/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen-awesome-sidebar-only.css` & `mio-cli-1.3.4/src/data/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen-awesome.css` & `mio-cli-1.3.4/src/data/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen.awesome.cfg` & `mio-cli-1.3.4/src/data/doxygen.awesome.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen.private.cfg` & `mio-cli-1.3.4/src/data/doxygen.private.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen.public.cfg` & `mio-cli-1.3.4/src/data/doxygen.public.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen_footer.html` & `mio-cli-1.3.4/src/data/doxygen_footer.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen_header.awesome.html` & `mio-cli-1.3.4/src/data/doxygen_header.awesome.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen_header.html` & `mio-cli-1.3.4/src/data/doxygen_header.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen_layout.xml` & `mio-cli-1.3.4/src/data/doxygen_layout.xml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/doxygen_stylesheet.css` & `mio-cli-1.3.4/src/data/doxygen_stylesheet.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/idv_doxyfilter_sv.pl` & `mio-cli-1.3.4/src/data/idv_doxyfilter_sv.pl`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/mio.toml` & `mio-cli-1.3.4/src/data/mio.toml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/data/plantuml.jar` & `mio-cli-1.3.4/src/data/plantuml.jar`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/cache.py` & `mio-cli-1.3.4/src/mio/cache.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/cfg.py` & `mio-cli-1.3.4/src/mio/cfg.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/clean.py` & `mio-cli-1.3.4/src/mio/clean.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/cli.py` & `mio-cli-1.3.4/src/mio/cli.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/common.py` & `mio-cli-1.3.4/src/mio/common.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/cov.py` & `mio-cli-1.3.4/src/mio/cov.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/doctor.py` & `mio-cli-1.3.4/src/mio/doctor.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/dox.py` & `mio-cli-1.3.4/src/mio/dox.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/eal.py` & `mio-cli-1.3.4/src/mio/eal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1842,15 +1842,15 @@
                     sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", f"{file}"], wd=wd, output=cfg.dbg)
                     common.move_file(path_downloaded_file, path_final_file)
 
 
 
 def download_prism_logs_mdc(sim_job, sub_dir, mdc_tests_results_path, tests_results_path):
     file_regex = r'(?:\s+((?:\w|\.)+(?:(?:.log)|(?:.json)))\\n)'
-    wd = f"{cfg.project_dir}/{mdc_tests_results_path}/.prism/tlm"
+    wd = f"{cfg.project_dir}/{mdc_tests_results_path}/.prism/{sub_dir}"
     mdc_list = get_process_output(cfg.metrics_home + "/mdc", ["list", f"{mdc_tests_results_path}/.prism/{sub_dir}"], wd=cfg.project_dir)
     mdc_list = mdc_list.split("\\n")
     # First 4 lines are not files
     if len(mdc_list) > 4:
         mdc_list.pop(0)
         mdc_list.pop(0)
         mdc_list.pop(0)
```

### Comparing `mio-cli-1.3.3/src/mio/help_text.py` & `mio-cli-1.3.4/src/mio/help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021-2023 Datum Technology Corporation
 # SPDX-License-Identifier: GPL-3.0
 ########################################################################################################################
 
 
-version = "1.3.3"
+version = "1.3.4"
 version_text = f"Moore.io CLI Client v{version}"
 
 
 
 main_help_text = f"""
                                  Moore.io (`mio`) Command Line Interface (CLI) - v{version}
                                       User Manual: https://mio-cli.readthedocs.io/
```

### Comparing `mio-cli-1.3.3/src/mio/init.py` & `mio-cli-1.3.4/src/mio/init.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/install.py` & `mio-cli-1.3.4/src/mio/install.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/new.py` & `mio-cli-1.3.4/src/mio/new.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/publish.py` & `mio-cli-1.3.4/src/mio/publish.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/regr.py` & `mio-cli-1.3.4/src/mio/regr.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/results.py` & `mio-cli-1.3.4/src/mio/results.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/sim.py` & `mio-cli-1.3.4/src/mio/sim.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio/user.py` & `mio-cli-1.3.4/src/mio/user.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/mio_cli.egg-info/PKG-INFO` & `mio-cli-1.3.4/src/mio_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

### Comparing `mio-cli-1.3.3/src/mio_cli.egg-info/SOURCES.txt` & `mio-cli-1.3.4/src/mio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/LICENSE_solderpad_v2p1.md` & `mio-cli-1.3.4/src/templates/LICENSE_solderpad_v2p1.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/dv_ip.yml` & `mio-cli-1.3.4/src/templates/dv_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/interactive_results.html.j2` & `mio-cli-1.3.4/src/templates/interactive_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/regression_results.html.j2` & `mio-cli-1.3.4/src/templates/regression_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/rtl_ip.yml` & `mio-cli-1.3.4/src/templates/rtl_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/ts.yml.j2` & `mio-cli-1.3.4/src/templates/ts.yml.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/src/templates/vivado_ip.yml` & `mio-cli-1.3.4/src/templates/vivado_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/LICENSE` & `mio-cli-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/README.md` & `mio-cli-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.3/setup.cfg` & `mio-cli-1.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mio-cli
-version = 1.3.3
+version = 1.3.4
 author = Datum Technology Corporation
 author_email = mio@datumtc.ca
 description = The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = SystemVerilog, UVM, DV, verilog, VHDL, hdl, rtl, synthesis, FPGA, simulation, Xilinx, Altera
 url = https://datum-technology-corporation.github.io/mio_cli_client/
```

### Comparing `mio-cli-1.3.3/PKG-INFO` & `mio-cli-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

