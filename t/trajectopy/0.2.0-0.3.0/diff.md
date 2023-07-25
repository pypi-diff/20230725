# Comparing `tmp/trajectopy-0.2.0.tar.gz` & `tmp/trajectopy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy-0.2.0.tar", last modified: Thu Jul 20 06:59:13 2023, max compression
+gzip compressed data, was "trajectopy-0.3.0.tar", last modified: Tue Jul 25 08:41:41 2023, max compression
```

## Comparing `trajectopy-0.2.0.tar` & `trajectopy-0.3.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:13.024731 trajectopy-0.2.0/
--rw-rw-rw-   0        0        0    35790 2023-07-18 19:10:13.000000 trajectopy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    19776 2023-07-20 06:59:13.022499 trajectopy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    19355 2023-07-19 23:21:45.000000 trajectopy-0.2.0/README.md
--rw-rw-rw-   0        0        0      787 2023-07-20 06:56:52.000000 trajectopy-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 06:59:13.024731 trajectopy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1628 2023-07-20 06:38:26.000000 trajectopy-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.735893 trajectopy-0.2.0/test/
--rw-rw-rw-   0        0        0     7503 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/test_alignment.py
--rw-rw-rw-   0        0        0     5569 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/test_comparison.py
--rw-rw-rw-   0        0        0     2347 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/test_settings.py
--rw-rw-rw-   0        0        0     1372 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/test_sorting.py
--rw-rw-rw-   0        0        0     6331 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/test_trajectory.py
--rw-rw-rw-   0        0        0      339 2023-07-18 19:10:13.000000 trajectopy-0.2.0/test/testdata.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.757604 trajectopy-0.2.0/trajectopy/
--rw-rw-rw-   0        0        0    35790 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/__init__.py
--rw-rw-rw-   0        0        0      630 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.825443 trajectopy-0.2.0/trajectopy/alignment/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/__init__.py
--rw-rw-rw-   0        0        0    39680 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/alignment.py
--rw-rw-rw-   0        0        0     9340 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/data.py
--rw-rw-rw-   0        0        0     2421 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/direct_helmert_transformation.py
--rw-rw-rw-   0        0        0     5354 2023-07-20 06:52:52.000000 trajectopy-0.2.0/trajectopy/alignment/direct_leverarm.py
--rw-rw-rw-   0        0        0     2181 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/direct_timeshift.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.832444 trajectopy-0.2.0/trajectopy/alignment/functional_model/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/functional_model/__init__.py
--rw-rw-rw-   0        0        0    16031 2023-07-20 06:41:07.000000 trajectopy-0.2.0/trajectopy/alignment/functional_model/equations.py
--rw-rw-rw-   0        0        0     8022 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/functional_model/interface.py
--rw-rw-rw-   0        0        0    19324 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/parameters.py
--rw-rw-rw-   0        0        0     3910 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/alignment/util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.847705 trajectopy-0.2.0/trajectopy/approximation/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/__init__.py
--rw-rw-rw-   0        0        0     8005 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/cubic_approximation.py
--rw-rw-rw-   0        0        0     5795 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/mls_approximation.py
--rw-rw-rw-   0        0        0     5303 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/rot_approximation.py
--rw-rw-rw-   0        0        0     6116 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/trajectory_approximation.py
--rw-rw-rw-   0        0        0     4272 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/util.py
--rw-rw-rw-   0        0        0     4843 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/approximation/voxelizer.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.861385 trajectopy-0.2.0/trajectopy/evaluation/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/evaluation/__init__.py
--rw-rw-rw-   0        0        0    14623 2023-07-20 06:46:40.000000 trajectopy-0.2.0/trajectopy/evaluation/comparison.py
--rw-rw-rw-   0        0        0     4872 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/evaluation/matching.py
--rw-rw-rw-   0        0        0    29217 2023-07-20 06:46:09.000000 trajectopy-0.2.0/trajectopy/evaluation/trajectory_deviations.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.869393 trajectopy-0.2.0/trajectopy/gui/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/__init__.py
--rw-rw-rw-   0        0        0    14315 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.888937 trajectopy-0.2.0/trajectopy/gui/managers/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/managers/__init__.py
--rw-rw-rw-   0        0        0     4444 2023-07-20 06:49:01.000000 trajectopy-0.2.0/trajectopy/gui/managers/file_manager.py
--rw-rw-rw-   0        0        0     1730 2023-07-20 06:48:37.000000 trajectopy-0.2.0/trajectopy/gui/managers/manager.py
--rw-rw-rw-   0        0        0     3677 2023-07-19 23:21:41.000000 trajectopy-0.2.0/trajectopy/gui/managers/plot_manager.py
--rw-rw-rw-   0        0        0     3812 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/managers/session_manager.py
--rw-rw-rw-   0        0        0    31367 2023-07-20 06:53:35.000000 trajectopy-0.2.0/trajectopy/gui/managers/trajectory_manager.py
--rw-rw-rw-   0        0        0     8040 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/managers/ui_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.905095 trajectopy-0.2.0/trajectopy/gui/models/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/models/__init__.py
--rw-rw-rw-   0        0        0    11907 2023-07-20 06:47:00.000000 trajectopy-0.2.0/trajectopy/gui/models/entry.py
--rw-rw-rw-   0        0        0     1115 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/models/property_model.py
--rw-rw-rw-   0        0        0     3904 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/models/result_model.py
--rw-rw-rw-   0        0        0      983 2023-07-20 06:47:25.000000 trajectopy-0.2.0/trajectopy/gui/models/selection.py
--rw-rw-rw-   0        0        0     4030 2023-07-20 06:49:34.000000 trajectopy-0.2.0/trajectopy/gui/models/table_model.py
--rw-rw-rw-   0        0        0     4837 2023-07-20 06:52:31.000000 trajectopy-0.2.0/trajectopy/gui/models/trajectory_model.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.932578 trajectopy-0.2.0/trajectopy/gui/requests/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/__init__.py
--rw-rw-rw-   0        0        0      666 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/file_request.py
--rw-rw-rw-   0        0        0      635 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/plot_requests.py
--rw-rw-rw-   0        0        0      424 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/plot_settings_request.py
--rw-rw-rw-   0        0        0      371 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/property_request.py
--rw-rw-rw-   0        0        0      500 2023-07-20 06:47:56.000000 trajectopy-0.2.0/trajectopy/gui/requests/request.py
--rw-rw-rw-   0        0        0      565 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/result_model_request.py
--rw-rw-rw-   0        0        0      388 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/session_request.py
--rw-rw-rw-   0        0        0     1029 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/trajectory_manager_request.py
--rw-rw-rw-   0        0        0      593 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/trajectory_model_request.py
--rw-rw-rw-   0        0        0      836 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/requests/ui_request.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.937372 trajectopy-0.2.0/trajectopy/gui/resources/
--rw-rw-rw-   0        0        0   120742 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/resources/full-icon-poppins.png
--rw-rw-rw-   0        0        0    24491 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/resources/icon.png
--rw-rw-rw-   0        0        0     1751 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.963950 trajectopy-0.2.0/trajectopy/gui/views/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/__init__.py
--rw-rw-rw-   0        0        0     3757 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/about_window.py
--rw-rw-rw-   0        0        0     9601 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/alignment_edit_window.py
--rw-rw-rw-   0        0        0    21480 2023-07-18 20:44:08.000000 trajectopy-0.2.0/trajectopy/gui/views/plot_settings_window.py
--rw-rw-rw-   0        0        0     2483 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/progress_window.py
--rw-rw-rw-   0        0        0     4013 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/properties_window.py
--rw-rw-rw-   0        0        0     6154 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/result_context_menu.py
--rw-rw-rw-   0        0        0     4717 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/result_selection_window.py
--rw-rw-rw-   0        0        0     4725 2023-07-19 23:21:41.000000 trajectopy-0.2.0/trajectopy/gui/views/result_table_view.py
--rw-rw-rw-   0        0        0    53997 2023-07-19 23:21:41.000000 trajectopy-0.2.0/trajectopy/gui/views/settings_window.py
--rw-rw-rw-   0        0        0    20852 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/trajectory_context_menu.py
--rw-rw-rw-   0        0        0     6744 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/gui/views/trajectory_table_view.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.979813 trajectopy-0.2.0/trajectopy/plotting/
--rw-rw-rw-   0        0        0       81 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/plotting/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/plotting/alignment_plot.py
--rw-rw-rw-   0        0        0      498 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/plotting/default.mplstyle
--rw-rw-rw-   0        0        0    21537 2023-07-20 06:51:33.000000 trajectopy-0.2.0/trajectopy/plotting/deviation_plot.py
--rw-rw-rw-   0        0        0     7223 2023-07-19 23:21:41.000000 trajectopy-0.2.0/trajectopy/plotting/plot_tabs.py
--rw-rw-rw-   0        0        0     3911 2023-07-20 06:52:04.000000 trajectopy-0.2.0/trajectopy/plotting/trajectory_plot.py
--rw-rw-rw-   0        0        0     7826 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/plotting/util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.998828 trajectopy-0.2.0/trajectopy/settings/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/alignment_settings.py
--rw-rw-rw-   0        0        0     1558 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/approximation_settings.py
--rw-rw-rw-   0        0        0     5669 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/comparison_settings.py
--rw-rw-rw-   0        0        0     3578 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/core.py
--rw-rw-rw-   0        0        0     1703 2023-07-18 20:45:43.000000 trajectopy-0.2.0/trajectopy/settings/plot_settings.py
--rw-rw-rw-   0        0        0     2433 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/processing_settings.py
--rw-rw-rw-   0        0        0      945 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/settings/sorting_settings.py
--rw-rw-rw-   0        0        0    35120 2023-07-20 06:45:51.000000 trajectopy-0.2.0/trajectopy/trajectory.py
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:13.019498 trajectopy-0.2.0/trajectopy/util/
--rw-rw-rw-   0        0        0        0 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/__init__.py
--rw-rw-rw-   0        0        0    18312 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/datahandling.py
--rw-rw-rw-   0        0        0     1490 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/definitions.py
--rw-rw-rw-   0        0        0      935 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/path.py
--rw-rw-rw-   0        0        0     5389 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/printing.py
--rw-rw-rw-   0        0        0    13611 2023-07-20 06:40:33.000000 trajectopy-0.2.0/trajectopy/util/reading.py
--rw-rw-rw-   0        0        0     1956 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/rotationset.py
--rw-rw-rw-   0        0        0    16143 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/spatialsorter.py
--rw-rw-rw-   0        0        0      973 2023-07-18 19:10:13.000000 trajectopy-0.2.0/trajectopy/util/trajectory_processing_state.py
--rw-rw-rw-   0        0        0        5 2023-07-20 06:56:47.000000 trajectopy-0.2.0/trajectopy/version
-drwxrwxrwx   0        0        0        0 2023-07-20 06:59:12.805978 trajectopy-0.2.0/trajectopy.egg-info/
--rw-rw-rw-   0        0        0    19776 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3943 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 20:19:00.000000 trajectopy-0.2.0/trajectopy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 06:59:12.000000 trajectopy-0.2.0/trajectopy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.752533 trajectopy-0.3.0/
+-rw-rw-rw-   0        0        0    35790 2023-07-17 09:26:39.000000 trajectopy-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    19879 2023-07-25 08:41:41.751531 trajectopy-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    19479 2023-07-25 08:40:03.000000 trajectopy-0.3.0/README.md
+-rw-rw-rw-   0        0        0      787 2023-07-25 08:40:25.000000 trajectopy-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:41:41.752533 trajectopy-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1628 2023-07-19 07:37:04.000000 trajectopy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.661479 trajectopy-0.3.0/test/
+-rw-rw-rw-   0        0        0     7503 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_alignment.py
+-rw-rw-rw-   0        0        0     5487 2023-07-25 08:37:59.000000 trajectopy-0.3.0/test/test_comparison.py
+-rw-rw-rw-   0        0        0     2347 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_settings.py
+-rw-rw-rw-   0        0        0     1372 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_sorting.py
+-rw-rw-rw-   0        0        0     6331 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_trajectory.py
+-rw-rw-rw-   0        0        0      339 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/testdata.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.671034 trajectopy-0.3.0/trajectopy/
+-rw-rw-rw-   0        0        0    35790 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/__init__.py
+-rw-rw-rw-   0        0        0      630 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.692991 trajectopy-0.3.0/trajectopy/alignment/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/__init__.py
+-rw-rw-rw-   0        0        0    39680 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/alignment/alignment.py
+-rw-rw-rw-   0        0        0     9340 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/data.py
+-rw-rw-rw-   0        0        0     2421 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/direct_helmert_transformation.py
+-rw-rw-rw-   0        0        0     5354 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/alignment/direct_leverarm.py
+-rw-rw-rw-   0        0        0     2181 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/direct_timeshift.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.694989 trajectopy-0.3.0/trajectopy/alignment/functional_model/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/__init__.py
+-rw-rw-rw-   0        0        0    16031 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/equations.py
+-rw-rw-rw-   0        0        0     8022 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/interface.py
+-rw-rw-rw-   0        0        0    19324 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/parameters.py
+-rw-rw-rw-   0        0        0     3910 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.700534 trajectopy-0.3.0/trajectopy/approximation/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/__init__.py
+-rw-rw-rw-   0        0        0     8005 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/cubic_approximation.py
+-rw-rw-rw-   0        0        0     5795 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/mls_approximation.py
+-rw-rw-rw-   0        0        0     5303 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/rot_approximation.py
+-rw-rw-rw-   0        0        0     6116 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/trajectory_approximation.py
+-rw-rw-rw-   0        0        0     4272 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/util.py
+-rw-rw-rw-   0        0        0     4843 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/voxelizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.702536 trajectopy-0.3.0/trajectopy/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/evaluation/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-07-25 08:26:56.000000 trajectopy-0.3.0/trajectopy/evaluation/comparison.py
+-rw-rw-rw-   0        0        0     4872 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/evaluation/matching.py
+-rw-rw-rw-   0        0        0    29996 2023-07-25 08:30:17.000000 trajectopy-0.3.0/trajectopy/evaluation/trajectory_deviations.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.704534 trajectopy-0.3.0/trajectopy/gui/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/__init__.py
+-rw-rw-rw-   0        0        0    14315 2023-07-25 07:49:54.000000 trajectopy-0.3.0/trajectopy/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.709533 trajectopy-0.3.0/trajectopy/gui/managers/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/gui/managers/__init__.py
+-rw-rw-rw-   0        0        0     4444 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/file_manager.py
+-rw-rw-rw-   0        0        0     1730 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/manager.py
+-rw-rw-rw-   0        0        0     3677 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/gui/managers/plot_manager.py
+-rw-rw-rw-   0        0        0     3812 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/managers/session_manager.py
+-rw-rw-rw-   0        0        0    31367 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/trajectory_manager.py
+-rw-rw-rw-   0        0        0     8040 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/managers/ui_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.714536 trajectopy-0.3.0/trajectopy/gui/models/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/models/__init__.py
+-rw-rw-rw-   0        0        0    11907 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/entry.py
+-rw-rw-rw-   0        0        0     1115 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/models/property_model.py
+-rw-rw-rw-   0        0        0     3904 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/models/result_model.py
+-rw-rw-rw-   0        0        0      983 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/selection.py
+-rw-rw-rw-   0        0        0     4030 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/table_model.py
+-rw-rw-rw-   0        0        0     4837 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/trajectory_model.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.722534 trajectopy-0.3.0/trajectopy/gui/requests/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/gui/requests/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/file_request.py
+-rw-rw-rw-   0        0        0      635 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/plot_requests.py
+-rw-rw-rw-   0        0        0      424 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/plot_settings_request.py
+-rw-rw-rw-   0        0        0      371 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/property_request.py
+-rw-rw-rw-   0        0        0      500 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/requests/request.py
+-rw-rw-rw-   0        0        0      565 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/result_model_request.py
+-rw-rw-rw-   0        0        0      388 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/session_request.py
+-rw-rw-rw-   0        0        0     1029 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/trajectory_manager_request.py
+-rw-rw-rw-   0        0        0      593 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/trajectory_model_request.py
+-rw-rw-rw-   0        0        0      836 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/ui_request.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.723536 trajectopy-0.3.0/trajectopy/gui/resources/
+-rw-rw-rw-   0        0        0   120742 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/resources/full-icon-poppins.png
+-rw-rw-rw-   0        0        0    24491 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/resources/icon.png
+-rw-rw-rw-   0        0        0     1751 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.733481 trajectopy-0.3.0/trajectopy/gui/views/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/__init__.py
+-rw-rw-rw-   0        0        0     3757 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/about_window.py
+-rw-rw-rw-   0        0        0     9601 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/alignment_edit_window.py
+-rw-rw-rw-   0        0        0    21480 2023-07-19 07:37:04.000000 trajectopy-0.3.0/trajectopy/gui/views/plot_settings_window.py
+-rw-rw-rw-   0        0        0     2483 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/progress_window.py
+-rw-rw-rw-   0        0        0     4013 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/properties_window.py
+-rw-rw-rw-   0        0        0     6154 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/result_context_menu.py
+-rw-rw-rw-   0        0        0     4717 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/result_selection_window.py
+-rw-rw-rw-   0        0        0     4725 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/gui/views/result_table_view.py
+-rw-rw-rw-   0        0        0    54090 2023-07-25 08:15:18.000000 trajectopy-0.3.0/trajectopy/gui/views/settings_window.py
+-rw-rw-rw-   0        0        0    20852 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/trajectory_context_menu.py
+-rw-rw-rw-   0        0        0     6744 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/trajectory_table_view.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.738485 trajectopy-0.3.0/trajectopy/plotting/
+-rw-rw-rw-   0        0        0       81 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/__init__.py
+-rw-rw-rw-   0        0        0     2185 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/alignment_plot.py
+-rw-rw-rw-   0        0        0      498 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/default.mplstyle
+-rw-rw-rw-   0        0        0    21537 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/plotting/deviation_plot.py
+-rw-rw-rw-   0        0        0     7223 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/plotting/plot_tabs.py
+-rw-rw-rw-   0        0        0     3911 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/plotting/trajectory_plot.py
+-rw-rw-rw-   0        0        0     7826 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.743486 trajectopy-0.3.0/trajectopy/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/__init__.py
+-rw-rw-rw-   0        0        0     8256 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/settings/alignment_settings.py
+-rw-rw-rw-   0        0        0     1558 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/approximation_settings.py
+-rw-rw-rw-   0        0        0     5669 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/comparison_settings.py
+-rw-rw-rw-   0        0        0     3578 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/core.py
+-rw-rw-rw-   0        0        0     1703 2023-07-19 07:37:04.000000 trajectopy-0.3.0/trajectopy/settings/plot_settings.py
+-rw-rw-rw-   0        0        0     2433 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/processing_settings.py
+-rw-rw-rw-   0        0        0      945 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/sorting_settings.py
+-rw-rw-rw-   0        0        0    35120 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/trajectory.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.749531 trajectopy-0.3.0/trajectopy/util/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/__init__.py
+-rw-rw-rw-   0        0        0    18312 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/datahandling.py
+-rw-rw-rw-   0        0        0     1490 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/definitions.py
+-rw-rw-rw-   0        0        0      935 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/path.py
+-rw-rw-rw-   0        0        0     5389 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/printing.py
+-rw-rw-rw-   0        0        0    13611 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/util/reading.py
+-rw-rw-rw-   0        0        0     1956 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/rotationset.py
+-rw-rw-rw-   0        0        0    16143 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/spatialsorter.py
+-rw-rw-rw-   0        0        0      973 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/trajectory_processing_state.py
+-rw-rw-rw-   0        0        0        5 2023-07-25 08:33:24.000000 trajectopy-0.3.0/trajectopy/version
+drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.686987 trajectopy-0.3.0/trajectopy.egg-info/
+-rw-rw-rw-   0        0        0    19879 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3943 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 07:43:35.000000 trajectopy-0.3.0/trajectopy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/top_level.txt
```

### Comparing `trajectopy-0.2.0/LICENSE` & `trajectopy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/PKG-INFO` & `trajectopy-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: trajectopy
-Version: 0.2.0
+Version: 0.3.0
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 License: GPLv3
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Trajectopy - Trajectory Evaluation in Python
 Welcome to Trajectopy, a Python package designed to simplify the alignment and comparison of trajectories using an intuitive graphical user interface (GUI).
 ![](.images/main_gui.png)
@@ -24,34 +23,37 @@
 - Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
 - Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
 - Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
 - Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
 - Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
 
 ## Installation
-Trajectopy currently requires Python >=3.10
-Using pip:
+#### Using pip:
 ```console
 pip install trajectopy
 ```
 
-Or using the repository:
+#### Or using the repository:
 ```console
 $ git clone https://github.com/gereon-t/trajectopy.git
 ```
 ```console
 cd trajectopy
 ```
 
-
-Install
+Using pip
 ```
 python3 -m pip install -e .
 ```
 
+Using poetry:
+```console
+poetry install
+```
+
 Run
 ```
 trajectopy
 ```
 
 ## Exemplary Evaluation
 The primary function of this program is to align and compare trajectories, which represent the position and orientation of a vehicle over time. To empirically evaluate a trajectory, it can be compared to a ground truth. However, since the two trajectories may not be in the same coordinate system, may differ by a lever arm, or may not be exactly synchronized, they need to be aligned first before the actual comparison. After that, both absolute and relative comparison metrics can be calculated.
@@ -130,15 +132,15 @@
 - Lever arm y
 - Lever arm z
 
 Both trajectories should be roughly synchronized to improve trajectory matching before alignment.
 
 
 ## Comparing Trajectories
-This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
+This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed. If both trajectory are defined in different coordinate systems, it is recommended to align them accordingly.
 
 ### Matching
 There are three different types of trajectory matching implemented in trajectopy:
 * Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
 * Matching via Nearest Temporal Neighbor: Poses are matched using their timestamps while considering some pre-defined tolerance.
 * Matching via Nearest Spatial Neighbor: Poses are matched using their nearest neighbors while considering some pre-defined distance tolerance.
 
@@ -242,8 +244,7 @@
 | Show Directed Deviations (Along / Cross / Vertical)| Absolute position deviations can be separated into along-track, horizontal cross-track and vertical cross-track direction. For this, either the trajectory orientations or positions are used. If turned off, the deviations will be separated into x,y,z which depend on the definition of the world coordinate frame.|
 | Grid Megapixels | For every scatter plot, the trajectory data is divided into a grid with a certain number of pixels that can be set with this setting. This prevents slow plotting with large trajectories. |
 | RMS Window Width | Similar to the Smoothing Window Width, this parameter sets the width of a sliding window used to smooth the RMS values that are mapped onto the trajectory in scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
 | Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a colorbar, which can be toggled to show the zero-crossing explicitly. |
 | Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are determined by either the minimum or maximum values, or by the X-sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on which limit is more restrictive. Starting at the lower bound, the colorbar ticks are placed at positions each separated by the total colorbar range divided by the colorbar step divisor. |
 | Do Not Plot Axis | Toggles the visibility of axes in scatter plots |
 | Rotate Scatter Plots to Main Axis | When set to true, the scatter plot trajectories will be rotated to align their main axis of extension (determined through principal component analysis) with the x-axis. This can be beneficial for elongated trajectories. |
-
```

### Comparing `trajectopy-0.2.0/README.md` & `trajectopy-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 - Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
 - Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
 - Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
 - Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
 - Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
 
 ## Installation
-Trajectopy currently requires Python >=3.10
-Using pip:
+#### Using pip:
 ```console
 pip install trajectopy
 ```
 
-Or using the repository:
+#### Or using the repository:
 ```console
 $ git clone https://github.com/gereon-t/trajectopy.git
 ```
 ```console
 cd trajectopy
 ```
 
-
-Install
+Using pip
 ```
 python3 -m pip install -e .
 ```
 
+Using poetry:
+```console
+poetry install
+```
+
 Run
 ```
 trajectopy
 ```
 
 ## Exemplary Evaluation
 The primary function of this program is to align and compare trajectories, which represent the position and orientation of a vehicle over time. To empirically evaluate a trajectory, it can be compared to a ground truth. However, since the two trajectories may not be in the same coordinate system, may differ by a lever arm, or may not be exactly synchronized, they need to be aligned first before the actual comparison. After that, both absolute and relative comparison metrics can be calculated.
@@ -116,15 +119,15 @@
 - Lever arm y
 - Lever arm z
 
 Both trajectories should be roughly synchronized to improve trajectory matching before alignment.
 
 
 ## Comparing Trajectories
-This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
+This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed. If both trajectory are defined in different coordinate systems, it is recommended to align them accordingly.
 
 ### Matching
 There are three different types of trajectory matching implemented in trajectopy:
 * Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
 * Matching via Nearest Temporal Neighbor: Poses are matched using their timestamps while considering some pre-defined tolerance.
 * Matching via Nearest Spatial Neighbor: Poses are matched using their nearest neighbors while considering some pre-defined distance tolerance.
```

### Comparing `trajectopy-0.2.0/pyproject.toml` & `trajectopy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy"
-version = "0.2.0"
+version = "0.3.0"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "GPLv3"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy"
 repository = "https://github.com/gereon-t/trajectopy.git"
```

### Comparing `trajectopy-0.2.0/setup.py` & `trajectopy-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/test/test_alignment.py` & `trajectopy-0.3.0/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/test/test_comparison.py` & `trajectopy-0.3.0/test/test_comparison.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,50 +68,48 @@
         transformed = generated_trajectory.copy()
 
         x_random = np.random.randn(len(transformed)) * 0.1
         y_random = np.random.randn(len(transformed)) * 0.1
         z_random = np.random.randn(len(transformed)) * 0.1
         transformed.pos.xyz += np.c_[x_random, y_random, z_random]
 
+        x_diff = np.abs(np.diff(x_random))
+        y_diff = np.abs(np.diff(y_random))
+        z_diff = np.abs(np.diff(z_random))
+
         settings = ComparisonSettings(
             type=ComparisonType(
                 comparison_method=ComparisonMethod.RELATIVE,
                 matching_settings=MatchingSettings(method=MatchingMethod.NEAREST_TEMPORAL),
                 relative_mode=RelativeMode.TIME,
             ),
             use_all_pose_pairs=True,
             relative_pair_time_difference=1.0,
         )
 
         deviations_time = compare_trajectories(traj_ref=trajectory, traj_test=transformed, settings=settings)
 
-        np.testing.assert_almost_equal(-deviations_time.x_drift_per_second, np.diff(x_random)[:-1])
-        np.testing.assert_almost_equal(-deviations_time.y_drift_per_second, np.diff(y_random)[:-1])
-        np.testing.assert_almost_equal(-deviations_time.z_drift_per_second, np.diff(z_random)[:-1])
+        np.testing.assert_almost_equal(deviations_time.x_drift_per_second, x_diff[:-1])
+        np.testing.assert_almost_equal(deviations_time.y_drift_per_second, y_diff[:-1])
+        np.testing.assert_almost_equal(deviations_time.z_drift_per_second, z_diff[:-1])
 
         np.testing.assert_almost_equal(
-            -deviations_time.x_drift_per_meter, (np.diff(x_random) / np.diff(trajectory.arc_lengths))[:-1]
+            deviations_time.x_drift_per_meter, (x_diff / np.diff(trajectory.arc_lengths))[:-1]
         )
         np.testing.assert_almost_equal(
-            -deviations_time.y_drift_per_meter, (np.diff(y_random) / np.diff(trajectory.arc_lengths))[:-1]
+            deviations_time.y_drift_per_meter, (y_diff / np.diff(trajectory.arc_lengths))[:-1]
         )
         np.testing.assert_almost_equal(
-            -deviations_time.z_drift_per_meter, (np.diff(z_random) / np.diff(trajectory.arc_lengths))[:-1]
+            deviations_time.z_drift_per_meter, (z_diff / np.diff(trajectory.arc_lengths))[:-1]
         )
 
         settings.type.relative_mode = RelativeMode.DISTANCE
         settings.relative_pair_distance = 1.0
 
         deviations_dist = compare_trajectories(traj_ref=trajectory, traj_test=transformed, settings=settings)
-        np.testing.assert_almost_equal(-deviations_dist.x_drift_per_second, np.diff(x_random))
-        np.testing.assert_almost_equal(-deviations_dist.y_drift_per_second, np.diff(y_random))
-        np.testing.assert_almost_equal(-deviations_dist.z_drift_per_second, np.diff(z_random))
-
-        np.testing.assert_almost_equal(
-            -deviations_dist.x_drift_per_meter, (np.diff(x_random) / np.diff(trajectory.arc_lengths))
-        )
-        np.testing.assert_almost_equal(
-            -deviations_dist.y_drift_per_meter, (np.diff(y_random) / np.diff(trajectory.arc_lengths))
-        )
-        np.testing.assert_almost_equal(
-            -deviations_dist.z_drift_per_meter, (np.diff(z_random) / np.diff(trajectory.arc_lengths))
-        )
+        np.testing.assert_almost_equal(deviations_dist.x_drift_per_second, x_diff)
+        np.testing.assert_almost_equal(deviations_dist.y_drift_per_second, y_diff)
+        np.testing.assert_almost_equal(deviations_dist.z_drift_per_second, z_diff)
+
+        np.testing.assert_almost_equal(deviations_dist.x_drift_per_meter, (x_diff / np.diff(trajectory.arc_lengths)))
+        np.testing.assert_almost_equal(deviations_dist.y_drift_per_meter, (y_diff / np.diff(trajectory.arc_lengths)))
+        np.testing.assert_almost_equal(deviations_dist.z_drift_per_meter, (z_diff / np.diff(trajectory.arc_lengths)))
```

### Comparing `trajectopy-0.2.0/test/test_settings.py` & `trajectopy-0.3.0/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/test/test_sorting.py` & `trajectopy-0.3.0/test/test_sorting.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/test/test_trajectory.py` & `trajectopy-0.3.0/test/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/LICENSE` & `trajectopy-0.3.0/trajectopy/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/__main__.py` & `trajectopy-0.3.0/trajectopy/__main__.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/alignment.py` & `trajectopy-0.3.0/trajectopy/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/data.py` & `trajectopy-0.3.0/trajectopy/alignment/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/direct_helmert_transformation.py` & `trajectopy-0.3.0/trajectopy/alignment/direct_helmert_transformation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/direct_leverarm.py` & `trajectopy-0.3.0/trajectopy/alignment/direct_leverarm.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/direct_timeshift.py` & `trajectopy-0.3.0/trajectopy/alignment/direct_timeshift.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/functional_model/equations.py` & `trajectopy-0.3.0/trajectopy/alignment/functional_model/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/functional_model/interface.py` & `trajectopy-0.3.0/trajectopy/alignment/functional_model/interface.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/parameters.py` & `trajectopy-0.3.0/trajectopy/alignment/parameters.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/alignment/util.py` & `trajectopy-0.3.0/trajectopy/alignment/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/cubic_approximation.py` & `trajectopy-0.3.0/trajectopy/approximation/cubic_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/mls_approximation.py` & `trajectopy-0.3.0/trajectopy/approximation/mls_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/rot_approximation.py` & `trajectopy-0.3.0/trajectopy/approximation/rot_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/trajectory_approximation.py` & `trajectopy-0.3.0/trajectopy/approximation/trajectory_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/util.py` & `trajectopy-0.3.0/trajectopy/approximation/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/approximation/voxelizer.py` & `trajectopy-0.3.0/trajectopy/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/evaluation/comparison.py` & `trajectopy-0.3.0/trajectopy/evaluation/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,16 @@
         traj_test (Trajectory): Test trajectory.
         traj_ref (Trajectory): Reference trajectory.
         settings (ComparisonSettings): Comparison settings.
 
     Returns:
         RelativeTrajectoryDeviations: Relative trajectory deviations.
     """
-    arc_lengths = traj_ref.arc_lengths
-    sorted_indices = np.argsort(arc_lengths)
-    traj_ref = traj_ref.apply_index(sorted_indices, inplace=False)
-    traj_test = traj_test.apply_index(sorted_indices, inplace=False)
+    traj_ref = traj_ref.set_sorting(sorting=Sorting.CHRONO, inplace=False)
+    traj_test = traj_test.set_sorting(sorting=Sorting.CHRONO, inplace=False)
 
     pair_indices = _get_pair_indices_dist(traj_ref, settings)
 
     return pairwise_comparison(traj_test=traj_test, traj_ref=traj_ref, pair_indices=pair_indices, settings=settings)
 
 
 def compare_trajectories_relative_time(
@@ -143,15 +141,15 @@
     traj_test = traj_test.set_sorting(sorting=Sorting.CHRONO, inplace=False)
 
     pair_indices = _get_pair_indices_time(traj_ref, settings)
 
     return pairwise_comparison(traj_test=traj_test, traj_ref=traj_ref, pair_indices=pair_indices, settings=settings)
 
 
-def _get_pair_indices_time(traj_ref: Trajectory, settings: ComparisonSettings) -> np.ndarray[int]:
+def _get_pair_indices_time(traj_ref: Trajectory, settings: ComparisonSettings) -> np.ndarray:
     if settings.use_all_pose_pairs:
         time_steps = np.array(
             [
                 [i, tstamp + settings.relative_pair_time_difference]
                 for i, tstamp in enumerate(traj_ref.tstamps)
                 if (tstamp + settings.relative_pair_time_difference) < traj_ref.tstamps[-1]
             ],
@@ -166,15 +164,15 @@
         settings.relative_pair_time_difference,
     )
 
     indices = np.searchsorted(traj_ref.tstamps, time_steps)
     return np.c_[indices[:-1], indices[1:]]
 
 
-def _get_pair_indices_dist(traj_ref: Trajectory, settings: ComparisonSettings) -> np.ndarray[int]:
+def _get_pair_indices_dist(traj_ref: Trajectory, settings: ComparisonSettings) -> np.ndarray:
     if settings.use_all_pose_pairs:
         dist_steps = np.array(
             [
                 [i, arc_length + settings.relative_pair_distance]
                 for i, arc_length in enumerate(traj_ref.arc_lengths)
                 if (arc_length + settings.relative_pair_distance) < traj_ref.arc_lengths[-1]
             ],
@@ -190,42 +188,51 @@
     )
 
     indices = np.searchsorted(traj_ref.arc_lengths, dist_steps)
     return np.c_[indices[:-1], indices[1:]]
 
 
 def pairwise_comparison(
-    *, traj_test: Trajectory, traj_ref: Trajectory, pair_indices: np.ndarray[int], settings: ComparisonSettings
+    *, traj_test: Trajectory, traj_ref: Trajectory, pair_indices: np.ndarray, settings: ComparisonSettings
 ) -> RelativeTrajectoryDeviations:
+    if len(pair_indices) == 0:
+        raise ValueError("No pairs found")
+
     pos_dev = []
+    ref_dev = []
+    test_dev = []
     rot_dev = []
     pair_distance = []
     pair_time_difference = []
     both_orientations = traj_ref.rot is not None and traj_test.rot is not None
 
     for pair in pair_indices:
         ref_translation_diff = traj_ref.pos.xyz[pair[1]] - traj_ref.pos.xyz[pair[0]]
         test_translation_diff = traj_test.pos.xyz[pair[1]] - traj_test.pos.xyz[pair[0]]
-        pos_dev.append(ref_translation_diff - test_translation_diff)
+        ref_dev.append(ref_translation_diff)
+        test_dev.append(test_translation_diff)
+        pos_dev.append(np.abs(ref_translation_diff - test_translation_diff))
 
         if both_orientations:
             ref_rotation_diff = traj_ref.rot[pair[1]] - traj_ref.rot[pair[0]]
             test_rotation_diff = traj_test.rot[pair[1]] - traj_test.rot[pair[0]]
             rot_dev.append((ref_rotation_diff - test_rotation_diff).as_quat())
 
         pair_distance.append(traj_ref.arc_lengths[pair[1]] - traj_ref.arc_lengths[pair[0]])
         pair_time_difference.append(traj_ref.tstamps[pair[1]] - traj_ref.tstamps[pair[0]])
 
     pos = PointSet(xyz=traj_ref.pos.xyz[pair_indices[:, 0]], epsg=traj_ref.pos.epsg)
+    norm_pos_dev = np.abs(np.linalg.norm(np.array(ref_dev), axis=1) - np.linalg.norm(np.array(test_dev), axis=1))
     return RelativeTrajectoryDeviations(
         name=f"{traj_test.name} vs. {traj_ref.name}",
         pair_distances=np.array(pair_distance),
         pair_time_differences=np.array(pair_time_difference),
         pos=pos,
         pos_dev=np.array(pos_dev),
+        norm_pos_dev=norm_pos_dev,
         rot_dev=RotationSet.from_quat(np.array(rot_dev)) if rot_dev else None,
         comparison_type=settings.type,
     )
 
 
 def compare_trajectories_relative(
     *,
@@ -321,15 +328,15 @@
     a = line_pts[0]
     b = line_pts[1]
     p_nearest, t = datahandling.nearest_point(p=p, line_pts=line_pts)
 
     if not is_last:
         return np.sign(t) * np.linalg.norm(p_nearest - a)
 
-    return (
+    return float(
         -np.linalg.norm(p_nearest - b)
         if np.linalg.norm(b - a) > np.linalg.norm(p_nearest - a)
         else np.linalg.norm(p_nearest - b)
     )
 
 
 def _cross_track_dev(*, p: np.ndarray, line_pts: list, z_slope_dist: bool = False) -> Tuple[float, float]:
```

### Comparing `trajectopy-0.2.0/trajectopy/evaluation/matching.py` & `trajectopy-0.3.0/trajectopy/evaluation/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/evaluation/trajectory_deviations.py` & `trajectopy-0.3.0/trajectopy/evaluation/trajectory_deviations.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 class RelativeTrajectoryDeviations(Trajectory):
     def __init__(
         self,
         pair_distances: np.ndarray,
         pair_time_differences: np.ndarray,
         pos: PointSet,
         pos_dev: np.ndarray,
-        rot_dev: RotationSet = None,
+        norm_pos_dev: np.ndarray,
+        rot_dev: Union[RotationSet, None] = None,
         name: str = "",
         comparison_type: ComparisonType = ComparisonType(),
     ) -> None:
         super().__init__(
             pos=pos.copy(),
             name=name,
         )
         self.pair_distances = pair_distances
         self.pair_time_differences = pair_time_differences
         self.pos_dev = pos_dev
+        self.norm_pos_dev = norm_pos_dev
         self.rot_dev = rot_dev
         self.comparison_type = comparison_type
 
     def __len__(self) -> int:
         return len(self.pos)
 
     @property
@@ -59,26 +61,28 @@
             "Type": str(self.comparison_type),
             "Number of deviations": str(len(self)),
             "Average Metric Pose Distance": f"{np.mean(self.pair_distances):.3f} m",
             "Average Temporal Pose Difference": f"{np.mean(self.pair_time_differences):.3f} s",
             "Maximum Position Drift per Second": f"{np.max(self.pos_drift_per_second):.3f} m/s",
             "Minimum Position Drift per Second": f"{np.min(self.pos_drift_per_second):.3f} m/s",
             "Average Position Drift per Second": f"{np.mean(self.pos_drift_per_second):.3f} m/s",
+            "Median Position Drift per Second": f"{np.median(self.pos_drift_per_second):.3f} m/s",
             "Average X Drift per Second": f"{np.mean(self.x_drift_per_second):.3f} m/s",
             "Average Y Drift per Second": f"{np.mean(self.y_drift_per_second):.3f} m/s",
             "Average Z Drift per Second": f"{np.mean(self.z_drift_per_second):.3f} m/s",
         }
 
         if self.rot_dev is None:
             return metric_dict
 
         rot_dict = {
             "Maximum Rotation Drift per Second": f"{np.rad2deg(np.max(self.rot_drift_per_second)):.3f} deg/s",
             "Minimum Rotation Drift per Second": f"{np.rad2deg(np.min(self.rot_drift_per_second)):.3f} deg/s",
             "Average Rotation Drift per Second": f"{np.rad2deg(np.mean(self.rot_drift_per_second)):.3f} deg/s",
+            "Median Rotation Drift per Second": f"{np.rad2deg(np.median(self.rot_drift_per_second)):.3f} deg/s",
             "Average Roll Drift per Second": f"{np.rad2deg(np.mean(self.roll_drift_per_second)):.3f} deg/s",
             "Average Pitch Drift per Second": f"{np.rad2deg(np.mean(self.pitch_drift_per_second)):.3f} deg/s",
             "Average Yaw Drift per Second": f"{np.rad2deg(np.mean(self.yaw_drift_per_second)):.3f} deg/s",
         }
         return metric_dict | rot_dict
 
     @property
@@ -86,97 +90,108 @@
         metric_dict = {
             "Name": self.name,
             "Type": str(self.comparison_type),
             "Number of deviations": str(len(self)),
             "Average Metric Pose Distance": f"{np.mean(self.pair_distances):.3f} m",
             "Average Temporal Pose Difference": f"{np.mean(self.pair_time_differences):.3f} s",
             "Maximum Position Drift": f"{np.max(self.pos_drift_per_meter) * 100:.3f} %",
-            "Minimum Position Drift": f"{np.min(self.pos_drift_per_meter) *100:.3f} %",
-            "Average Position Drift": f"{np.mean(self.pos_drift_per_meter) *100:.3f} %",
+            "Minimum Position Drift": f"{np.min(self.pos_drift_per_meter) * 100:.3f} %",
+            "Average Position Drift": f"{np.mean(self.pos_drift_per_meter) * 100:.3f} %",
+            "Median Position Drift": f"{np.median(self.pos_drift_per_meter) * 100:.3f} %",
             "Average X Drift": f"{np.mean(self.x_drift_per_meter) * 100:.3f} %",
             "Average Y Drift": f"{np.mean(self.y_drift_per_meter) * 100:.3f} %",
             "Average Z Drift": f"{np.mean(self.z_drift_per_meter) * 100:.3f} %",
         }
 
         if self.rot_dev is None:
             return metric_dict
 
         rot_dict = {
             "Maximum Rotation Drift per Meter": f"{np.rad2deg(np.max(self.rot_drift_per_meter)):.3f} deg/m",
             "Minimum Rotation Drift per Meter": f"{np.rad2deg(np.min(self.rot_drift_per_meter)):.3f} deg/m",
             "Average Rotation Drift per Meter": f"{np.rad2deg(np.mean(self.rot_drift_per_meter)):.3f} deg/m",
+            "Median Rotation Drift per Meter": f"{np.rad2deg(np.median(self.rot_drift_per_meter)):.3f} deg/m",
             "Average Roll Drift per Meter": f"{np.rad2deg(np.mean(self.roll_drift_per_meter)):.3f} deg/m",
             "Average Pitch Drift per Meter": f"{np.rad2deg(np.mean(self.pitch_drift_per_meter)):.3f} deg/m",
             "Average Yaw Drift per Meter": f"{np.rad2deg(np.mean(self.yaw_drift_per_meter)):.3f} deg/m",
         }
         return metric_dict | rot_dict
 
     @classmethod
     def from_file(cls: "RelativeTrajectoryDeviations", filename: str) -> "RelativeTrajectoryDeviations":
         header_data, deviation_data = read_data(filename=filename)
 
         pair_distances = deviation_data[:, 0]
         pair_time_differences = deviation_data[:, 1]
         pos = PointSet(xyz=deviation_data[:, 2:5], epsg=header_data.epsg)
         pos_dev = deviation_data[:, 5:8]
+        norm_pos_dev = deviation_data[:, 8]
 
-        if deviation_data.shape[1] == 12:
-            rot_dev = RotationSet.from_quat(deviation_data[:, 8:])
+        if deviation_data.shape[1] == 13:
+            rot_dev = RotationSet.from_quat(deviation_data[:, 9:])
         else:
             rot_dev = None
 
         return RelativeTrajectoryDeviations(
             name=header_data.name,
             pos=pos,
             pos_dev=pos_dev,
+            norm_pos_dev=norm_pos_dev,
             rot_dev=rot_dev,
             comparison_type=header_data.comparison_type,
             pair_distances=pair_distances,
             pair_time_differences=pair_time_differences,
         )
 
     def to_dataframe(self) -> pd.DataFrame:
         if self.rot_dev is not None:
             return pd.DataFrame(
                 np.c_[
-                    self.pair_distances, self.pair_time_differences, self.pos.xyz, self.pos_dev, self.rot_dev.as_quat()
+                    self.pair_distances,
+                    self.pair_time_differences,
+                    self.pos.xyz,
+                    self.pos_dev,
+                    self.norm_pos_dev,
+                    self.rot_dev.as_quat(),
                 ],
                 columns=[
                     "pair_distances",
                     "pair_time_differences",
                     "pos_x",
                     "pos_y",
                     "pos_z",
                     "pos_dev_x",
                     "pos_dev_y",
                     "pos_dev_z",
+                    "norm_pos_dev",
                     "rot_dev_qx",
                     "rot_dev_qy",
                     "rot_dev_qz",
                     "rot_dev_qw",
                 ],
             )
         return pd.DataFrame(
-            np.c_[self.pair_distances, self.pair_time_differences, self.pos.xyz, self.pos_dev],
+            np.c_[self.pair_distances, self.pair_time_differences, self.pos.xyz, self.pos_dev, self.norm_pos_dev],
             columns=[
                 "pair_distances",
                 "pair_time_differences",
                 "pos_x",
                 "pos_y",
                 "pos_z",
                 "pos_dev_x",
                 "pos_dev_y",
                 "pos_dev_z",
+                "norm_pos_dev",
             ],
         )
 
     @cached_property
     def rpy(self) -> np.ndarray:
         """Returns roll, pitch and yaw"""
-        return self.rot_dev.as_euler(seq="xyz")
+        return np.abs(self.rot_dev.as_euler(seq="xyz"))
 
     @property
     def x_drift_per_meter(self) -> np.ndarray:
         return self.pos_dev[:, 0] / self.pair_distances
 
     @property
     def y_drift_per_meter(self) -> np.ndarray:
@@ -220,19 +235,19 @@
 
     @property
     def yaw_drift_per_second(self) -> np.ndarray:
         return self.rpy[:, 2] / self.pair_time_differences
 
     @property
     def pos_drift_per_meter(self) -> np.ndarray:
-        return np.linalg.norm(self.pos_dev, axis=1) / self.pair_distances
+        return self.norm_pos_dev / self.pair_distances
 
     @property
     def pos_drift_per_second(self) -> np.ndarray:
-        return np.linalg.norm(self.pos_dev, axis=1) / self.pair_time_differences
+        return self.norm_pos_dev / self.pair_time_differences
 
     @property
     def rot_drift_per_meter(self) -> np.ndarray:
         return self.rot_dev.rotangle / self.pair_distances
 
     @property
     def rot_drift_per_second(self) -> np.ndarray:
```

### Comparing `trajectopy-0.2.0/trajectopy/gui/main_window.py` & `trajectopy-0.3.0/trajectopy/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/file_manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/plot_manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/plot_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/session_manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/trajectory_manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/trajectory_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/managers/ui_manager.py` & `trajectopy-0.3.0/trajectopy/gui/managers/ui_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/entry.py` & `trajectopy-0.3.0/trajectopy/gui/models/entry.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/property_model.py` & `trajectopy-0.3.0/trajectopy/gui/models/property_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/result_model.py` & `trajectopy-0.3.0/trajectopy/gui/models/result_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/selection.py` & `trajectopy-0.3.0/trajectopy/gui/models/selection.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/table_model.py` & `trajectopy-0.3.0/trajectopy/gui/models/table_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/models/trajectory_model.py` & `trajectopy-0.3.0/trajectopy/gui/models/trajectory_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/file_request.py` & `trajectopy-0.3.0/trajectopy/gui/requests/file_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/plot_requests.py` & `trajectopy-0.3.0/trajectopy/gui/requests/plot_requests.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/result_model_request.py` & `trajectopy-0.3.0/trajectopy/gui/requests/result_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/trajectory_manager_request.py` & `trajectopy-0.3.0/trajectopy/gui/requests/trajectory_manager_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/trajectory_model_request.py` & `trajectopy-0.3.0/trajectopy/gui/requests/trajectory_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/requests/ui_request.py` & `trajectopy-0.3.0/trajectopy/gui/requests/ui_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/resources/full-icon-poppins.png` & `trajectopy-0.3.0/trajectopy/gui/resources/full-icon-poppins.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/resources/icon.png` & `trajectopy-0.3.0/trajectopy/gui/resources/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/util.py` & `trajectopy-0.3.0/trajectopy/gui/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/about_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/about_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/alignment_edit_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/alignment_edit_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/plot_settings_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/plot_settings_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/progress_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/progress_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/properties_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/properties_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/result_context_menu.py` & `trajectopy-0.3.0/trajectopy/gui/views/result_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/result_selection_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/result_selection_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/result_table_view.py` & `trajectopy-0.3.0/trajectopy/gui/views/result_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/settings_window.py` & `trajectopy-0.3.0/trajectopy/gui/views/settings_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,25 +522,27 @@
 
         self.relative_tdist_label = QtWidgets.QLabel(self.comparisonVerticalLayoutWidget)
         self.relative_tdist_label.setObjectName("relative_tdist_label")
         self.comparisonFormLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.LabelRole, self.relative_tdist_label)
         self.relativeTDist = QtWidgets.QDoubleSpinBox(self.comparisonVerticalLayoutWidget)
         self.relativeTDist.setDecimals(2)
         self.relativeTDist.setMinimum(0.01)
+        self.relativeTDist.setMaximum(999999)
         self.relativeTDist.setSingleStep(0.01)
         self.relativeTDist.setProperty("value", 100)
         self.relativeTDist.setObjectName("relativeTDist")
         self.comparisonFormLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.relativeTDist)
 
         self.relative_dist_label = QtWidgets.QLabel(self.comparisonVerticalLayoutWidget)
         self.relative_dist_label.setObjectName("relative_dist_label")
         self.comparisonFormLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.relative_dist_label)
         self.relativeDist = QtWidgets.QDoubleSpinBox(self.comparisonVerticalLayoutWidget)
         self.relativeDist.setDecimals(2)
         self.relativeDist.setMinimum(0.01)
+        self.relativeDist.setMaximum(999999)
         self.relativeDist.setSingleStep(0.01)
         self.relativeDist.setProperty("value", 100)
         self.relativeDist.setObjectName("relativeDist")
         self.comparisonFormLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.relativeDist)
 
         self.relative_all_pairs_label = QtWidgets.QLabel(self.comparisonVerticalLayoutWidget)
         self.relative_all_pairs_label.setObjectName("relative_all_pairs_label")
```

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/trajectory_context_menu.py` & `trajectopy-0.3.0/trajectopy/gui/views/trajectory_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/gui/views/trajectory_table_view.py` & `trajectopy-0.3.0/trajectopy/gui/views/trajectory_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/plotting/alignment_plot.py` & `trajectopy-0.3.0/trajectopy/plotting/alignment_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/plotting/deviation_plot.py` & `trajectopy-0.3.0/trajectopy/plotting/deviation_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/plotting/plot_tabs.py` & `trajectopy-0.3.0/trajectopy/plotting/plot_tabs.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/plotting/trajectory_plot.py` & `trajectopy-0.3.0/trajectopy/plotting/trajectory_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/plotting/util.py` & `trajectopy-0.3.0/trajectopy/plotting/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/alignment_settings.py` & `trajectopy-0.3.0/trajectopy/settings/alignment_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     helmert: bool = True
     trans_x: bool = True
     trans_y: bool = True
     trans_z: bool = True
     rot_x: bool = True
     rot_y: bool = True
     rot_z: bool = True
-    scale: bool = True
+    scale: bool = False
 
     time_shift: bool = False
     use_x_speed: bool = True
     use_y_speed: bool = True
     use_z_speed: bool = True
 
     leverarm: bool = False
```

### Comparing `trajectopy-0.2.0/trajectopy/settings/approximation_settings.py` & `trajectopy-0.3.0/trajectopy/settings/approximation_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/comparison_settings.py` & `trajectopy-0.3.0/trajectopy/settings/comparison_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/core.py` & `trajectopy-0.3.0/trajectopy/settings/core.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/plot_settings.py` & `trajectopy-0.3.0/trajectopy/settings/plot_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/processing_settings.py` & `trajectopy-0.3.0/trajectopy/settings/processing_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/settings/sorting_settings.py` & `trajectopy-0.3.0/trajectopy/settings/sorting_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/trajectory.py` & `trajectopy-0.3.0/trajectopy/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/datahandling.py` & `trajectopy-0.3.0/trajectopy/util/datahandling.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/definitions.py` & `trajectopy-0.3.0/trajectopy/util/definitions.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/path.py` & `trajectopy-0.3.0/trajectopy/util/path.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/printing.py` & `trajectopy-0.3.0/trajectopy/util/printing.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/reading.py` & `trajectopy-0.3.0/trajectopy/util/reading.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/rotationset.py` & `trajectopy-0.3.0/trajectopy/util/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/spatialsorter.py` & `trajectopy-0.3.0/trajectopy/util/spatialsorter.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy/util/trajectory_processing_state.py` & `trajectopy-0.3.0/trajectopy/util/trajectory_processing_state.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.2.0/trajectopy.egg-info/PKG-INFO` & `trajectopy-0.3.0/trajectopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: trajectopy
-Version: 0.2.0
+Version: 0.3.0
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 License: GPLv3
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Trajectopy - Trajectory Evaluation in Python
 Welcome to Trajectopy, a Python package designed to simplify the alignment and comparison of trajectories using an intuitive graphical user interface (GUI).
 ![](.images/main_gui.png)
@@ -24,34 +23,37 @@
 - Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
 - Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
 - Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
 - Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
 - Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
 
 ## Installation
-Trajectopy currently requires Python >=3.10
-Using pip:
+#### Using pip:
 ```console
 pip install trajectopy
 ```
 
-Or using the repository:
+#### Or using the repository:
 ```console
 $ git clone https://github.com/gereon-t/trajectopy.git
 ```
 ```console
 cd trajectopy
 ```
 
-
-Install
+Using pip
 ```
 python3 -m pip install -e .
 ```
 
+Using poetry:
+```console
+poetry install
+```
+
 Run
 ```
 trajectopy
 ```
 
 ## Exemplary Evaluation
 The primary function of this program is to align and compare trajectories, which represent the position and orientation of a vehicle over time. To empirically evaluate a trajectory, it can be compared to a ground truth. However, since the two trajectories may not be in the same coordinate system, may differ by a lever arm, or may not be exactly synchronized, they need to be aligned first before the actual comparison. After that, both absolute and relative comparison metrics can be calculated.
@@ -130,15 +132,15 @@
 - Lever arm y
 - Lever arm z
 
 Both trajectories should be roughly synchronized to improve trajectory matching before alignment.
 
 
 ## Comparing Trajectories
-This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
+This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed. If both trajectory are defined in different coordinate systems, it is recommended to align them accordingly.
 
 ### Matching
 There are three different types of trajectory matching implemented in trajectopy:
 * Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
 * Matching via Nearest Temporal Neighbor: Poses are matched using their timestamps while considering some pre-defined tolerance.
 * Matching via Nearest Spatial Neighbor: Poses are matched using their nearest neighbors while considering some pre-defined distance tolerance.
 
@@ -242,8 +244,7 @@
 | Show Directed Deviations (Along / Cross / Vertical)| Absolute position deviations can be separated into along-track, horizontal cross-track and vertical cross-track direction. For this, either the trajectory orientations or positions are used. If turned off, the deviations will be separated into x,y,z which depend on the definition of the world coordinate frame.|
 | Grid Megapixels | For every scatter plot, the trajectory data is divided into a grid with a certain number of pixels that can be set with this setting. This prevents slow plotting with large trajectories. |
 | RMS Window Width | Similar to the Smoothing Window Width, this parameter sets the width of a sliding window used to smooth the RMS values that are mapped onto the trajectory in scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
 | Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a colorbar, which can be toggled to show the zero-crossing explicitly. |
 | Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are determined by either the minimum or maximum values, or by the X-sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on which limit is more restrictive. Starting at the lower bound, the colorbar ticks are placed at positions each separated by the total colorbar range divided by the colorbar step divisor. |
 | Do Not Plot Axis | Toggles the visibility of axes in scatter plots |
 | Rotate Scatter Plots to Main Axis | When set to true, the scatter plot trajectories will be rotated to align their main axis of extension (determined through principal component analysis) with the x-axis. This can be beneficial for elongated trajectories. |
-
```

### Comparing `trajectopy-0.2.0/trajectopy.egg-info/SOURCES.txt` & `trajectopy-0.3.0/trajectopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

