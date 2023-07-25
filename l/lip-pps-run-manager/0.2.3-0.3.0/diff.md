# Comparing `tmp/lip-pps-run-manager-0.2.3.tar.gz` & `tmp/lip-pps-run-manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lip-pps-run-manager-0.2.3.tar", last modified: Sun Jul 23 19:20:56 2023, max compression
+gzip compressed data, was "lip-pps-run-manager-0.3.0.tar", last modified: Tue Jul 25 15:59:06 2023, max compression
```

## Comparing `lip-pps-run-manager-0.2.3.tar` & `lip-pps-run-manager-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.007891 lip-pps-run-manager-0.2.3/
--rw-r--r--   0 cristovao   (501) staff       (20)      639 2023-07-23 19:10:53.000000 lip-pps-run-manager-0.2.3/.bumpversion.cfg
--rw-r--r--   0 cristovao   (501) staff       (20)     3216 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/.cookiecutterrc
--rw-r--r--   0 cristovao   (501) staff       (20)      187 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/.coveragerc
--rw-r--r--   0 cristovao   (501) staff       (20)      353 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/.editorconfig
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.988296 lip-pps-run-manager-0.2.3/.github/
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.994869 lip-pps-run-manager-0.2.3/.github/workflows/
--rw-r--r--   0 cristovao   (501) staff       (20)     5615 2023-07-21 18:18:07.000000 lip-pps-run-manager-0.2.3/.github/workflows/github-actions.yml
--rw-r--r--   0 cristovao   (501) staff       (20)      628 2023-07-21 18:08:44.000000 lip-pps-run-manager-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 cristovao   (501) staff       (20)      231 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/.readthedocs.yml
--rw-r--r--   0 cristovao   (501) staff       (20)     1614 2023-07-21 18:16:38.000000 lip-pps-run-manager-0.2.3/.travis.yml
--rw-r--r--   0 cristovao   (501) staff       (20)       79 2023-07-23 19:13:39.000000 lip-pps-run-manager-0.2.3/AUTHORS.rst
--rw-r--r--   0 cristovao   (501) staff       (20)     1442 2023-07-23 19:17:42.000000 lip-pps-run-manager-0.2.3/CHANGELOG.rst
--rw-r--r--   0 cristovao   (501) staff       (20)     2763 2023-07-21 17:21:32.000000 lip-pps-run-manager-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 cristovao   (501) staff       (20)     1118 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/LICENSE
--rw-r--r--   0 cristovao   (501) staff       (20)      470 2022-10-19 21:18:35.000000 lip-pps-run-manager-0.2.3/MANIFEST.in
--rw-r--r--   0 cristovao   (501) staff       (20)     3719 2023-07-23 19:20:56.008036 lip-pps-run-manager-0.2.3/PKG-INFO
--rw-r--r--   0 cristovao   (501) staff       (20)     3083 2023-07-23 19:10:53.000000 lip-pps-run-manager-0.2.3/README.rst
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.995726 lip-pps-run-manager-0.2.3/ci/
--rwxr-xr-x   0 cristovao   (501) staff       (20)     3063 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/ci/bootstrap.py
--rw-r--r--   0 cristovao   (501) staff       (20)       66 2022-10-13 19:26:58.000000 lip-pps-run-manager-0.2.3/ci/requirements.txt
--rw-r--r--   0 cristovao   (501) staff       (20)       73 2022-10-13 19:27:51.000000 lip-pps-run-manager-0.2.3/ci/requirements_travis.txt
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.996055 lip-pps-run-manager-0.2.3/ci/templates/
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.988922 lip-pps-run-manager-0.2.3/ci/templates/.github/
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.996344 lip-pps-run-manager-0.2.3/ci/templates/.github/workflows/
--rw-r--r--   0 cristovao   (501) staff       (20)     2001 2022-10-13 19:03:29.000000 lip-pps-run-manager-0.2.3/ci/templates/.github/workflows/github-actions.yml
--rw-r--r--   0 cristovao   (501) staff       (20)     1363 2022-10-17 11:28:14.000000 lip-pps-run-manager-0.2.3/ci/templates/.travis.yml
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.999744 lip-pps-run-manager-0.2.3/docs/
--rw-r--r--   0 cristovao   (501) staff       (20)       28 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/authors.rst
--rw-r--r--   0 cristovao   (501) staff       (20)       30 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/changelog.rst
--rw-r--r--   0 cristovao   (501) staff       (20)     1271 2023-07-23 19:10:53.000000 lip-pps-run-manager-0.2.3/docs/conf.py
--rw-r--r--   0 cristovao   (501) staff       (20)       33 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/contributing.rst
--rw-r--r--   0 cristovao   (501) staff       (20)      244 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/index.rst
--rw-r--r--   0 cristovao   (501) staff       (20)       99 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/installation.rst
--rw-r--r--   0 cristovao   (501) staff       (20)       27 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/readme.rst
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.000303 lip-pps-run-manager-0.2.3/docs/reference/
--rw-r--r--   0 cristovao   (501) staff       (20)       71 2022-09-29 18:41:00.000000 lip-pps-run-manager-0.2.3/docs/reference/index.rst
--rw-r--r--   0 cristovao   (501) staff       (20)     1663 2022-10-24 20:46:28.000000 lip-pps-run-manager-0.2.3/docs/reference/lip_pps_run_manager.rst
--rw-r--r--   0 cristovao   (501) staff       (20)       29 2022-10-24 16:13:41.000000 lip-pps-run-manager-0.2.3/docs/requirements.txt
--rw-r--r--   0 cristovao   (501) staff       (20)      109 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/spelling_wordlist.txt
--rw-r--r--   0 cristovao   (501) staff       (20)       90 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/docs/usage.rst
--rw-r--r--   0 cristovao   (501) staff       (20)      160 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/pyproject.toml
--rw-r--r--   0 cristovao   (501) staff       (20)      784 2022-09-27 14:13:20.000000 lip-pps-run-manager-0.2.3/pytest.ini
--rw-r--r--   0 cristovao   (501) staff       (20)      326 2023-07-23 19:20:56.008633 lip-pps-run-manager-0.2.3/setup.cfg
--rwxr-xr-x   0 cristovao   (501) staff       (20)     3152 2023-07-23 19:10:53.000000 lip-pps-run-manager-0.2.3/setup.py
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:55.989506 lip-pps-run-manager-0.2.3/src/
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.002451 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/
--rw-r--r--   0 cristovao   (501) staff       (20)      261 2023-07-23 19:10:53.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/__init__.py
--rw-r--r--   0 cristovao   (501) staff       (20)      385 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/__main__.py
--rw-r--r--   0 cristovao   (501) staff       (20)      950 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/cli.py
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.005270 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/instruments/
--rw-r--r--   0 cristovao   (501) staff       (20)      883 2022-10-24 20:26:54.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/instruments/Keithley6487.py
--rw-r--r--   0 cristovao   (501) staff       (20)      143 2022-10-24 19:59:38.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/instruments/__init__.py
--rw-r--r--   0 cristovao   (501) staff       (20)      166 2022-10-24 20:00:18.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/instruments/functions.py
--rw-r--r--   0 cristovao   (501) staff       (20)    59999 2023-07-23 19:01:29.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/run_manager.py
--rw-r--r--   0 cristovao   (501) staff       (20)     1328 2023-07-23 19:03:26.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/setup_manager.py
--rw-r--r--   0 cristovao   (501) staff       (20)     8202 2022-10-17 14:07:06.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/telegram_reporter.py
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.004434 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/
--rw-r--r--   0 cristovao   (501) staff       (20)     3719 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/PKG-INFO
--rw-r--r--   0 cristovao   (501) staff       (20)     1618 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/SOURCES.txt
--rw-r--r--   0 cristovao   (501) staff       (20)        1 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/dependency_links.txt
--rw-r--r--   0 cristovao   (501) staff       (20)       70 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/entry_points.txt
--rw-r--r--   0 cristovao   (501) staff       (20)        1 2023-07-23 19:19:04.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/not-zip-safe
--rw-r--r--   0 cristovao   (501) staff       (20)       25 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/requires.txt
--rw-r--r--   0 cristovao   (501) staff       (20)       20 2023-07-23 19:20:55.000000 lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/top_level.txt
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.007066 lip-pps-run-manager-0.2.3/tests/
-drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-23 19:20:56.007646 lip-pps-run-manager-0.2.3/tests/intruments/
--rw-r--r--   0 cristovao   (501) staff       (20)     1421 2022-11-02 22:04:37.000000 lip-pps-run-manager-0.2.3/tests/intruments/test_Keithley6487.py
--rw-r--r--   0 cristovao   (501) staff       (20)     1034 2022-11-02 18:32:03.000000 lip-pps-run-manager-0.2.3/tests/intruments/test_functions.py
--rw-r--r--   0 cristovao   (501) staff       (20)       73 2022-09-28 09:54:24.000000 lip-pps-run-manager-0.2.3/tests/test_lip_pps_run_manager.py
--rw-r--r--   0 cristovao   (501) staff       (20)    58081 2023-07-23 18:41:12.000000 lip-pps-run-manager-0.2.3/tests/test_run_manager_class.py
--rw-r--r--   0 cristovao   (501) staff       (20)     3418 2022-10-24 13:35:25.000000 lip-pps-run-manager-0.2.3/tests/test_run_manager_functions.py
--rw-r--r--   0 cristovao   (501) staff       (20)    75575 2023-07-23 19:00:24.000000 lip-pps-run-manager-0.2.3/tests/test_task_manager_class.py
--rw-r--r--   0 cristovao   (501) staff       (20)     7306 2022-10-21 17:00:56.000000 lip-pps-run-manager-0.2.3/tests/test_telegram_reporter_class.py
--rw-r--r--   0 cristovao   (501) staff       (20)     1809 2023-07-21 18:10:42.000000 lip-pps-run-manager-0.2.3/tox.ini
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.957678 lip-pps-run-manager-0.3.0/
+-rw-r--r--   0 cristovao   (501) staff       (20)      639 2023-07-25 15:56:24.000000 lip-pps-run-manager-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 cristovao   (501) staff       (20)     3216 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/.cookiecutterrc
+-rw-r--r--   0 cristovao   (501) staff       (20)      187 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/.coveragerc
+-rw-r--r--   0 cristovao   (501) staff       (20)      353 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/.editorconfig
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.923019 lip-pps-run-manager-0.3.0/.github/
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.932760 lip-pps-run-manager-0.3.0/.github/workflows/
+-rw-r--r--   0 cristovao   (501) staff       (20)     5615 2023-07-21 18:18:07.000000 lip-pps-run-manager-0.3.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 cristovao   (501) staff       (20)      628 2023-07-21 18:08:44.000000 lip-pps-run-manager-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 cristovao   (501) staff       (20)      231 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/.readthedocs.yml
+-rw-r--r--   0 cristovao   (501) staff       (20)     1614 2023-07-21 18:16:38.000000 lip-pps-run-manager-0.3.0/.travis.yml
+-rw-r--r--   0 cristovao   (501) staff       (20)       79 2023-07-23 19:13:39.000000 lip-pps-run-manager-0.3.0/AUTHORS.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)     1645 2023-07-25 15:57:12.000000 lip-pps-run-manager-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)     2763 2023-07-21 17:21:32.000000 lip-pps-run-manager-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)     1118 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/LICENSE
+-rw-r--r--   0 cristovao   (501) staff       (20)      470 2022-10-19 21:18:35.000000 lip-pps-run-manager-0.3.0/MANIFEST.in
+-rw-r--r--   0 cristovao   (501) staff       (20)     3922 2023-07-25 15:59:06.957902 lip-pps-run-manager-0.3.0/PKG-INFO
+-rw-r--r--   0 cristovao   (501) staff       (20)     3083 2023-07-25 15:56:24.000000 lip-pps-run-manager-0.3.0/README.rst
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.934451 lip-pps-run-manager-0.3.0/ci/
+-rwxr-xr-x   0 cristovao   (501) staff       (20)     3063 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/ci/bootstrap.py
+-rw-r--r--   0 cristovao   (501) staff       (20)       66 2022-10-13 19:26:58.000000 lip-pps-run-manager-0.3.0/ci/requirements.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)       73 2022-10-13 19:27:51.000000 lip-pps-run-manager-0.3.0/ci/requirements_travis.txt
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.935215 lip-pps-run-manager-0.3.0/ci/templates/
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.923559 lip-pps-run-manager-0.3.0/ci/templates/.github/
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.935749 lip-pps-run-manager-0.3.0/ci/templates/.github/workflows/
+-rw-r--r--   0 cristovao   (501) staff       (20)     2001 2022-10-13 19:03:29.000000 lip-pps-run-manager-0.3.0/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 cristovao   (501) staff       (20)     1363 2022-10-17 11:28:14.000000 lip-pps-run-manager-0.3.0/ci/templates/.travis.yml
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.940927 lip-pps-run-manager-0.3.0/docs/
+-rw-r--r--   0 cristovao   (501) staff       (20)       28 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/authors.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)       30 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/changelog.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)     1271 2023-07-25 15:56:24.000000 lip-pps-run-manager-0.3.0/docs/conf.py
+-rw-r--r--   0 cristovao   (501) staff       (20)       33 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/contributing.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)      244 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/index.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)       99 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/installation.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)       27 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/readme.rst
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.941871 lip-pps-run-manager-0.3.0/docs/reference/
+-rw-r--r--   0 cristovao   (501) staff       (20)       71 2022-09-29 18:41:00.000000 lip-pps-run-manager-0.3.0/docs/reference/index.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)     1663 2022-10-24 20:46:28.000000 lip-pps-run-manager-0.3.0/docs/reference/lip_pps_run_manager.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)       29 2022-10-24 16:13:41.000000 lip-pps-run-manager-0.3.0/docs/requirements.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)      109 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)       90 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/docs/usage.rst
+-rw-r--r--   0 cristovao   (501) staff       (20)      160 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/pyproject.toml
+-rw-r--r--   0 cristovao   (501) staff       (20)      784 2022-09-27 14:13:20.000000 lip-pps-run-manager-0.3.0/pytest.ini
+-rw-r--r--   0 cristovao   (501) staff       (20)      326 2023-07-25 15:59:06.958351 lip-pps-run-manager-0.3.0/setup.cfg
+-rwxr-xr-x   0 cristovao   (501) staff       (20)     3152 2023-07-25 15:56:24.000000 lip-pps-run-manager-0.3.0/setup.py
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.924158 lip-pps-run-manager-0.3.0/src/
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.945931 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/
+-rw-r--r--   0 cristovao   (501) staff       (20)      261 2023-07-25 15:56:24.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/__init__.py
+-rw-r--r--   0 cristovao   (501) staff       (20)      385 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/__main__.py
+-rw-r--r--   0 cristovao   (501) staff       (20)      950 2022-09-27 09:19:54.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/cli.py
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.949382 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/instruments/
+-rw-r--r--   0 cristovao   (501) staff       (20)      883 2022-10-24 20:26:54.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/instruments/Keithley6487.py
+-rw-r--r--   0 cristovao   (501) staff       (20)      143 2022-10-24 19:59:38.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/instruments/__init__.py
+-rw-r--r--   0 cristovao   (501) staff       (20)      166 2022-10-24 20:00:18.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/instruments/functions.py
+-rw-r--r--   0 cristovao   (501) staff       (20)    60771 2023-07-25 15:42:16.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/run_manager.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     1328 2023-07-23 19:03:26.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/setup_manager.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     8202 2022-10-17 14:07:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/telegram_reporter.py
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.947885 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/
+-rw-r--r--   0 cristovao   (501) staff       (20)     3922 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/PKG-INFO
+-rw-r--r--   0 cristovao   (501) staff       (20)     1618 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)        1 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)       70 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/entry_points.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)        1 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/not-zip-safe
+-rw-r--r--   0 cristovao   (501) staff       (20)       25 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/requires.txt
+-rw-r--r--   0 cristovao   (501) staff       (20)       20 2023-07-25 15:59:06.000000 lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/top_level.txt
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.953575 lip-pps-run-manager-0.3.0/tests/
+drwxr-xr-x   0 cristovao   (501) staff       (20)        0 2023-07-25 15:59:06.956541 lip-pps-run-manager-0.3.0/tests/intruments/
+-rw-r--r--   0 cristovao   (501) staff       (20)     1421 2022-11-02 22:04:37.000000 lip-pps-run-manager-0.3.0/tests/intruments/test_Keithley6487.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     1034 2022-11-02 18:32:03.000000 lip-pps-run-manager-0.3.0/tests/intruments/test_functions.py
+-rw-r--r--   0 cristovao   (501) staff       (20)       73 2022-09-28 09:54:24.000000 lip-pps-run-manager-0.3.0/tests/test_lip_pps_run_manager.py
+-rw-r--r--   0 cristovao   (501) staff       (20)    58054 2023-07-25 09:09:07.000000 lip-pps-run-manager-0.3.0/tests/test_run_manager_class.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     3418 2022-10-24 13:35:25.000000 lip-pps-run-manager-0.3.0/tests/test_run_manager_functions.py
+-rw-r--r--   0 cristovao   (501) staff       (20)    75575 2023-07-23 19:00:24.000000 lip-pps-run-manager-0.3.0/tests/test_task_manager_class.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     7306 2022-10-21 17:00:56.000000 lip-pps-run-manager-0.3.0/tests/test_telegram_reporter_class.py
+-rw-r--r--   0 cristovao   (501) staff       (20)     1809 2023-07-21 18:10:42.000000 lip-pps-run-manager-0.3.0/tox.ini
```

### Comparing `lip-pps-run-manager-0.2.3/.bumpversion.cfg` & `lip-pps-run-manager-0.3.0/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.3
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `lip-pps-run-manager-0.2.3/.cookiecutterrc` & `lip-pps-run-manager-0.3.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/.github/workflows/github-actions.yml` & `lip-pps-run-manager-0.3.0/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/.pre-commit-config.yaml` & `lip-pps-run-manager-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/.travis.yml` & `lip-pps-run-manager-0.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/CHANGELOG.rst` & `lip-pps-run-manager-0.3.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 
 Changelog
 =========
 
-Current (2023-07-23)
+Current (2023-07-25)
 --------------------
 
+
+0.3.0 (2023-07-25)
+------------------
+
+* Fixed the name of the loop_iterations parameter in the handle_task method. **this is a breaking change**
+* Added status information when a looped task progresses
+
 0.2.3 (2023-07-23)
---------------------
+------------------
 
 * Added a backup_directory property to the RunManager
 * Added the copy_file_to method to the RunManager
 * Added the backup_file method to the RunManager
 
 Not numbered (2022-10-24)
 -------------------------
```

### Comparing `lip-pps-run-manager-0.2.3/CONTRIBUTING.rst` & `lip-pps-run-manager-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/LICENSE` & `lip-pps-run-manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/PKG-INFO` & `lip-pps-run-manager-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lip-pps-run-manager
-Version: 0.2.3
+Version: 0.3.0
 Summary: Run Manager used in the LIP PPS software stack for handling data taking and analysis
 Home-page: https://github.com/cbeiraod/LIP_PPS_Run_Manager
 Author: Cristóvão B. da Cruz e Silva
 Author-email: cbeiraod@cern.ch
 License: MIT
 Project-URL: Documentation, https://lip-pps-run-manager.readthedocs.io/
 Project-URL: Changelog, https://lip-pps-run-manager.readthedocs.io/en/latest/changelog.html
@@ -84,19 +84,26 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-Current (2023-07-23)
+Current (2023-07-25)
 --------------------
 
+
+0.3.0 (2023-07-25)
+------------------
+
+* Fixed the name of the loop_iterations parameter in the handle_task method. **this is a breaking change**
+* Added status information when a looped task progresses
+
 0.2.3 (2023-07-23)
---------------------
+------------------
 
 * Added a backup_directory property to the RunManager
 * Added the copy_file_to method to the RunManager
 * Added the backup_file method to the RunManager
 
 Not numbered (2022-10-24)
 -------------------------
```

### Comparing `lip-pps-run-manager-0.2.3/README.rst` & `lip-pps-run-manager-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/lip-pps-run-manager
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/lip-pps-run-manager.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/lip-pps-run-manager
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/cbeiraod/LIP_PPS_Run_Manager/v0.2.3.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/cbeiraod/LIP_PPS_Run_Manager/v0.3.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/cbeiraod/LIP_PPS_Run_Manager/compare/v0.2.3...main
+    :target: https://github.com/cbeiraod/LIP_PPS_Run_Manager/compare/v0.3.0...main
 
 
 
 .. end-badges
 
 Run Manager used in the LIP PPS software stack for handling data taking and analysis
```

### Comparing `lip-pps-run-manager-0.2.3/ci/bootstrap.py` & `lip-pps-run-manager-0.3.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/ci/templates/.github/workflows/github-actions.yml` & `lip-pps-run-manager-0.3.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/ci/templates/.travis.yml` & `lip-pps-run-manager-0.3.0/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/docs/conf.py` & `lip-pps-run-manager-0.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'LIP_PPS_Run_Manager'
 year = '2022'
 author = 'Cristóvão B. da Cruz e Silva'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '0.2.3'
+version = release = '0.3.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/cbeiraod/LIP_PPS_Run_Manager/issues/%s', '#'),
     'pr': ('https://github.com/cbeiraod/LIP_PPS_Run_Manager/pull/%s', 'PR #'),
 }
```

### Comparing `lip-pps-run-manager-0.2.3/docs/reference/lip_pps_run_manager.rst` & `lip-pps-run-manager-0.3.0/docs/reference/lip_pps_run_manager.rst`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/pytest.ini` & `lip-pps-run-manager-0.3.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/setup.py` & `lip-pps-run-manager-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='lip-pps-run-manager',
-    version='0.2.3',
+    version='0.3.0',
     license='MIT',
     description='Run Manager used in the LIP PPS software stack for handling data taking and analysis',
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Cristóvão B. da Cruz e Silva',
```

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/cli.py` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/cli.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/instruments/Keithley6487.py` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/instruments/Keithley6487.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/run_manager.py` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/run_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 Contains classes and functions used to manage the runs and their tasks.
 
 """
 
 import datetime
 import inspect
 import json
+import logging
 import shutil
 import traceback
 import warnings
 from pathlib import Path
 
 import humanize
 
 from lip_pps_run_manager import __version__
 from lip_pps_run_manager.telegram_reporter import TelegramReporter
 
+# TODO: Add logger options to the managers
+
 
 def clean_path(path_to_clean: Path) -> Path:
     """Clean a path from dangerous characters
 
     Some characters are not recommended/supported by a given filesystem.
     To make matters worse, the set of supported characters varies from
     operating system to operating system. In order to make sure this
@@ -272,14 +275,15 @@
     _bot_token = None
     _chat_id = None
     _telegram_reporter = None
     _run_created = False
     _status_message_id = None
     _in_run_context = False
     _rate_limit = True
+    _logger = None
 
     def __init__(
         self,
         path_to_run_directory: Path,
         telegram_bot_name: str = None,
         telegram_chat_name: str = None,
         telegram_bot_token: str = None,
@@ -332,14 +336,16 @@
 
         if self._bot_token is not None and self._chat_id is not None:
             self._rate_limit = rate_limit
         else:
             self._bot_token = None
             self._chat_id = None
 
+        self._logger = logging.getLogger(self.run_name)
+
     def __repr__(self):
         """Get the python representation of this class"""
         if self._bot_token is None or self._chat_id is None:
             return "RunManager({})".format(repr(self.path_directory))
         else:
             classRepr = "RunManager({}".format(repr(self.path_directory))
             if self._bot_name is not None:
@@ -480,15 +486,15 @@
         self._run_created = True
 
     def handle_task(
         self,
         task_name: str,
         drop_old_data: bool = True,
         backup_python_file: bool = True,
-        telegram_loop_iterations: int = None,
+        loop_iterations: int = None,
         minimum_update_time_seconds: int = 60,
         minimum_warn_time_seconds: int = 60,
     ):
         """Method that creates a handle to a manager for a specific task
 
         The `TaskManager` that is created is under the current
         `RunManager`.
@@ -502,17 +508,18 @@
             exists, this flag controls whether that data is removed or
             not. Useful when testing and rerunning multiple times, in
             order to ensure that old data from previous runs is cleaned.
         backup_python_file
             If `True` a copy of the current python file will be backed
             up in the task directory. Useful for keeping a log of
             exactly what was done.
-        telegram_loop_iterations
-            If telegram reporting is enabled, this is the number of
-            expected iterations in the processing loop. Use
+        loop_iterations
+            This is the number of expected iterations in the processing loop.
+            Used to print out progress reporting to the terminal. If telegram
+            reporting is enabled, reports will be sent to telegram as well. Use
             `loop_tick()` to keep track of progress during the loop.
         minimum_update_time_seconds
             The minimum time allowed between updates to telegram. This
             parameter is important in order to guarantee that the limits
             imposed by telegram are respected.
         minimum_warn_time_seconds
             The minimum time allowed between warnings to telegram. This
@@ -550,19 +557,17 @@
             raise TypeError("The `drop_old_data` must be a bool type object, received object of type {}".format(type(drop_old_data)))
 
         if not isinstance(backup_python_file, bool):
             raise TypeError(
                 "The `backup_python_file` must be a bool type object, received object of type {}".format(type(backup_python_file))
             )
 
-        if telegram_loop_iterations is not None and not isinstance(telegram_loop_iterations, int):
+        if loop_iterations is not None and not isinstance(loop_iterations, int):
             raise TypeError(
-                "The `telegram_loop_iterations` must be a int type object or None, received object of type {}".format(
-                    type(telegram_loop_iterations)
-                )
+                "The `loop_iterations` must be a int type object or None, received object of type {}".format(type(loop_iterations))
             )
 
         if not isinstance(minimum_update_time_seconds, int):
             raise TypeError(
                 "The `minimum_update_time_seconds` must be a int type object, received object of type {}".format(
                     type(minimum_update_time_seconds)
                 )
@@ -583,15 +588,15 @@
             script_to_backup = Path(traceback.extract_stack()[-2].filename)
 
         TM = TaskManager(
             path_to_run=self.path_directory,
             task_name=task_name,
             drop_old_data=drop_old_data,
             script_to_backup=script_to_backup,
-            loop_iterations=telegram_loop_iterations,
+            loop_iterations=loop_iterations,
             minimum_update_time_seconds=minimum_update_time_seconds,
             minimum_warn_time_seconds=minimum_warn_time_seconds,
         )
         TM._run_created = self._run_created
         TM._in_run_context = self._in_run_context
         if self._telegram_reporter is not None:
             TM._bot_name = self._bot_name
@@ -1101,14 +1106,16 @@
         self._loop_iterations = loop_iterations
         self._in_task_context = False
         self._minimum_update_time = datetime.timedelta(seconds=float(minimum_update_time_seconds))
         self._minimum_warn_time = datetime.timedelta(seconds=float(minimum_warn_time_seconds))
         if loop_iterations is not None:
             self._processed_iterations = 0
 
+        self._logger = logging.getLogger(self.run_name + ":" + self.task_name)
+
     def __repr__(self):
         """Get the python representation of this class"""
         if self._bot_token is None or self._chat_id is None:
             return (
                 "TaskManager({}, {}, drop_old_data={}, script_to_backup={}, "
                 "loop_iterations={}, minimum_update_time_seconds={}, "
                 "minimum_warn_time_seconds={})".format(
@@ -1232,14 +1239,24 @@
     def _update_status(self):
         """Internal method to update the status of the task on the telegram status message"""
         if not self._in_task_context:
             raise RuntimeError(
                 "Tried calling _update_status() while not inside a task context. Use the 'with TaskManager as handle' syntax"
             )
 
+        message = f'Processing task {self.task_name} of run {self.run_name}'
+        if self.expected_finish_time is not None:
+            message += '\n  - Progress: {} % ({}/{})\n  - Expected finish: {}'.format(
+                int(float(self.processed_iterations) / self._loop_iterations * 100),
+                int(self.processed_iterations),
+                int(self._loop_iterations),
+                self.expected_finish_time.strftime("%Y-%m-%d %H:%M"),
+            )
+        self._logger.info(message)
+
         if self._telegram_reporter is not None:
             create_status = False
             if not hasattr(self, "_task_status_message_id") or self._task_status_message_id is None:
                 create_status = True
             if not hasattr(self, '_last_update'):
                 self._last_update = datetime.datetime.now() - 2 * self._minimum_update_time
             elapsed_time = datetime.datetime.now() - self._last_update
@@ -1415,14 +1432,16 @@
         """
         if not isinstance(message, str):
             raise TypeError("The `message` must be a str type object, received object of type {}".format(type(message)))
 
         if not hasattr(self, "_accumulated_warnings"):
             self._accumulated_warnings = {}
 
+        self._logger.warning(message)
+
         if message not in self._accumulated_warnings:
             self._accumulated_warnings[message] = 1
         else:
             self._accumulated_warnings[message] += 1
 
         self._send_warnings()
```

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/setup_manager.py` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/setup_manager.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager/telegram_reporter.py` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager/telegram_reporter.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/PKG-INFO` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lip-pps-run-manager
-Version: 0.2.3
+Version: 0.3.0
 Summary: Run Manager used in the LIP PPS software stack for handling data taking and analysis
 Home-page: https://github.com/cbeiraod/LIP_PPS_Run_Manager
 Author: Cristóvão B. da Cruz e Silva
 Author-email: cbeiraod@cern.ch
 License: MIT
 Project-URL: Documentation, https://lip-pps-run-manager.readthedocs.io/
 Project-URL: Changelog, https://lip-pps-run-manager.readthedocs.io/en/latest/changelog.html
@@ -84,19 +84,26 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-Current (2023-07-23)
+Current (2023-07-25)
 --------------------
 
+
+0.3.0 (2023-07-25)
+------------------
+
+* Fixed the name of the loop_iterations parameter in the handle_task method. **this is a breaking change**
+* Added status information when a looped task progresses
+
 0.2.3 (2023-07-23)
---------------------
+------------------
 
 * Added a backup_directory property to the RunManager
 * Added the copy_file_to method to the RunManager
 * Added the backup_file method to the RunManager
 
 Not numbered (2022-10-24)
 -------------------------
```

### Comparing `lip-pps-run-manager-0.2.3/src/lip_pps_run_manager.egg-info/SOURCES.txt` & `lip-pps-run-manager-0.3.0/src/lip_pps_run_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tests/intruments/test_Keithley6487.py` & `lip-pps-run-manager-0.3.0/tests/intruments/test_Keithley6487.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tests/intruments/test_functions.py` & `lip-pps-run-manager-0.3.0/tests/intruments/test_functions.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tests/test_run_manager_class.py` & `lip-pps-run-manager-0.3.0/tests/test_run_manager_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,29 +1132,29 @@
             John.handle_task("myTask", backup_python_file=2)
             raise Exception("Passed through a fail condition without failing")  # pragma: no cover
         except TypeError as e:
             assert str(e) == "The `backup_python_file` must be a bool type object, received object of type <class 'int'>"
 
 
 @patch('requests.Session', new=SessionReplacement)  # To avoid sending actual http requests
-def test_handle_task_bad_type_telegram_loop_iterations():
+def test_handle_task_bad_type_loop_iterations():
     tmpdir = tempfile.gettempdir()
     run_name = "Run0001"
     bot_token = "bot_token"
     chat_id = "chat_id"
     rate_limit = False
     runPath = Path(tmpdir) / run_name
     ensure_clean(runPath)
 
     with RM.RunManager(runPath, telegram_bot_token=bot_token, telegram_chat_id=chat_id, rate_limit=rate_limit) as John:
         try:
-            John.handle_task("myTask", telegram_loop_iterations="2")
+            John.handle_task("myTask", loop_iterations="2")
             raise Exception("Passed through a fail condition without failing")  # pragma: no cover
         except TypeError as e:
-            assert str(e) == "The `telegram_loop_iterations` must be a int type object or None, received object of type <class 'str'>"
+            assert str(e) == "The `loop_iterations` must be a int type object or None, received object of type <class 'str'>"
 
 
 @patch('requests.Session', new=SessionReplacement)  # To avoid sending actual http requests
 def test_handle_task_bad_type_minimum_update_time_seconds():
     tmpdir = tempfile.gettempdir()
     run_name = "Run0001"
     bot_token = "bot_token"
```

### Comparing `lip-pps-run-manager-0.2.3/tests/test_run_manager_functions.py` & `lip-pps-run-manager-0.3.0/tests/test_run_manager_functions.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tests/test_task_manager_class.py` & `lip-pps-run-manager-0.3.0/tests/test_task_manager_class.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tests/test_telegram_reporter_class.py` & `lip-pps-run-manager-0.3.0/tests/test_telegram_reporter_class.py`

 * *Files identical despite different names*

### Comparing `lip-pps-run-manager-0.2.3/tox.ini` & `lip-pps-run-manager-0.3.0/tox.ini`

 * *Files identical despite different names*

