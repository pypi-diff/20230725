# Comparing `tmp/common_version-0.0.2.tar.gz` & `tmp/common_version-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_version-0.0.2.tar", last modified: Tue Jul 25 06:56:05 2023, max compression
+gzip compressed data, was "common_version-0.0.3.tar", last modified: Tue Jul 25 07:07:30 2023, max compression
```

## Comparing `common_version-0.0.2.tar` & `common_version-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.321009 common_version-0.0.2/
--rw-rw-rw-   0        0        0     1543 2023-07-11 06:12:49.000000 common_version-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1326 2023-07-25 06:56:05.322009 common_version-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-07-25 06:55:59.000000 common_version-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.277789 common_version-0.0.2/common_version.egg-info/
--rw-rw-rw-   0        0        0     1326 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2054 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 06:54:17.000000 common_version-0.0.2/common_version.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1246 2023-07-25 06:56:05.322009 common_version-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       62 2023-07-11 06:12:49.000000 common_version-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.291923 common_version-0.0.2/tests/
--rw-rw-rw-   0        0        0      812 2023-07-25 06:41:44.000000 common_version-0.0.2/tests/test_c_version.py
--rw-rw-rw-   0        0        0      929 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_cargo_version.py
--rw-rw-rw-   0        0        0      727 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_coco_version.py
--rw-rw-rw-   0        0        0     1122 2023-07-25 06:31:04.000000 common_version-0.0.2/tests/test_common.py
--rw-rw-rw-   0        0        0     1112 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_composer_version.py
--rw-rw-rw-   0        0        0      743 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_go_version.py
--rw-rw-rw-   0        0        0      717 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_hex_version.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 06:34:33.000000 common_version-0.0.2/tests/test_linux_version.py
--rw-rw-rw-   0        0        0      839 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_maven_version.py
--rw-rw-rw-   0        0        0      811 2023-07-25 06:31:04.000000 common_version-0.0.2/tests/test_merge_versions_expression.py
--rw-rw-rw-   0        0        0     1683 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_npm_version.py
--rw-rw-rw-   0        0        0      753 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_nuget_version.py
--rw-rw-rw-   0        0        0      915 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_nvd_version.py
--rw-rw-rw-   0        0        0     1039 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_other_version.py
--rw-rw-rw-   0        0        0     1247 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_pip_version.py
--rw-rw-rw-   0        0        0      723 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_ruby_version.py
--rw-rw-rw-   0        0        0     1724 2023-07-25 06:45:33.000000 common_version-0.0.2/tests/test_snyk_version.py
--rw-rw-rw-   0        0        0      383 2023-07-25 06:36:58.000000 common_version-0.0.2/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.294460 common_version-0.0.2/version/
--rw-rw-rw-   0        0        0    12831 2023-07-25 06:54:00.000000 common_version-0.0.2/version/__init__.py
--rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.2/version/base.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.295461 common_version-0.0.2/version/core/
--rw-rw-rw-   0        0        0        0 2023-03-30 09:25:46.000000 common_version-0.0.2/version/core/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-04-04 05:58:07.000000 common_version-0.0.2/version/core/utils.py
--rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.2/version/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.310009 common_version-0.0.2/version/expression/
--rw-rw-rw-   0        0        0     2099 2023-07-25 06:52:02.000000 common_version-0.0.2/version/expression/__init__.py
--rw-rw-rw-   0        0        0      436 2023-07-25 06:52:15.000000 common_version-0.0.2/version/expression/base.py
--rw-rw-rw-   0        0        0    28047 2023-07-25 06:33:38.000000 common_version-0.0.2/version/expression/base_method.py
--rw-rw-rw-   0        0        0     2318 2023-07-25 06:26:36.000000 common_version-0.0.2/version/expression/c_version_expression.py
--rw-rw-rw-   0        0        0     2581 2023-07-25 06:27:06.000000 common_version-0.0.2/version/expression/cargo_version_expression.py
--rw-rw-rw-   0        0        0     2144 2023-07-25 06:27:06.000000 common_version-0.0.2/version/expression/cocoapods_version_expression.py
--rw-rw-rw-   0        0        0     6942 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/composer_version_expression.py
--rw-rw-rw-   0        0        0      626 2023-07-25 06:46:05.000000 common_version-0.0.2/version/expression/go_version_expression.py
--rw-rw-rw-   0        0        0     2449 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/hex_version_expression.py
--rw-rw-rw-   0        0        0     2946 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/linux_version_expression.py
--rw-rw-rw-   0        0        0     4036 2023-07-25 06:46:07.000000 common_version-0.0.2/version/expression/maven_version_expression.py
--rw-rw-rw-   0        0        0     6331 2023-07-25 06:46:08.000000 common_version-0.0.2/version/expression/npm_version_expression.py
--rw-rw-rw-   0        0        0     4329 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/nuget_version_expression.py
--rw-rw-rw-   0        0        0     1529 2023-07-25 06:46:11.000000 common_version-0.0.2/version/expression/nvd_version_expression.py
--rw-rw-rw-   0        0        0     4465 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/other_version_expression.py
--rw-rw-rw-   0        0        0     6270 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/pip_version_expression.py
--rw-rw-rw-   0        0        0     3353 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/ruby_version_expression.py
--rw-rw-rw-   0        0        0     3970 2023-07-25 06:46:12.000000 common_version-0.0.2/version/expression/snyk_version_expression.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.321009 common_version-0.0.2/version/version_base/
--rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.2/version/version_base/__init__.py
--rw-rw-rw-   0        0        0    33829 2023-07-25 06:33:38.000000 common_version-0.0.2/version/version_base/base_item.py
--rw-rw-rw-   0        0        0    19296 2023-07-25 06:29:26.000000 common_version-0.0.2/version/version_base/base_version.py
--rw-rw-rw-   0        0        0     1906 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/common_method.py
--rw-rw-rw-   0        0        0     1839 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/composer_version.py
--rw-rw-rw-   0        0        0     1605 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/go_version.py
--rw-rw-rw-   0        0        0     4200 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/linux_version.py
--rw-rw-rw-   0        0        0    11663 2023-07-25 06:33:38.000000 common_version-0.0.2/version/version_base/lj_version.py
--rw-rw-rw-   0        0        0     2397 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/maven_version.py
--rw-rw-rw-   0        0        0     1511 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/npm_version.py
--rw-rw-rw-   0        0        0     5766 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/snyk_version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.900483 common_version-0.0.3/
+-rw-rw-rw-   0        0        0     1543 2023-07-11 06:12:49.000000 common_version-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1423 2023-07-25 07:07:30.900483 common_version-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-07-25 07:07:27.000000 common_version-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.858922 common_version-0.0.3/common_version.egg-info/
+-rw-rw-rw-   0        0        0     1423 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1246 2023-07-25 07:07:30.901482 common_version-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      191 2023-07-25 06:59:09.000000 common_version-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.870922 common_version-0.0.3/tests/
+-rw-rw-rw-   0        0        0      812 2023-07-25 06:41:44.000000 common_version-0.0.3/tests/test_c_version.py
+-rw-rw-rw-   0        0        0      929 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_cargo_version.py
+-rw-rw-rw-   0        0        0      727 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_coco_version.py
+-rw-rw-rw-   0        0        0     1122 2023-07-25 06:31:04.000000 common_version-0.0.3/tests/test_common.py
+-rw-rw-rw-   0        0        0     1112 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_composer_version.py
+-rw-rw-rw-   0        0        0      743 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_go_version.py
+-rw-rw-rw-   0        0        0      717 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_hex_version.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 06:34:33.000000 common_version-0.0.3/tests/test_linux_version.py
+-rw-rw-rw-   0        0        0      839 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_maven_version.py
+-rw-rw-rw-   0        0        0      811 2023-07-25 06:31:04.000000 common_version-0.0.3/tests/test_merge_versions_expression.py
+-rw-rw-rw-   0        0        0     1683 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_npm_version.py
+-rw-rw-rw-   0        0        0      753 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_nuget_version.py
+-rw-rw-rw-   0        0        0      915 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_nvd_version.py
+-rw-rw-rw-   0        0        0     1039 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_other_version.py
+-rw-rw-rw-   0        0        0     1247 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_pip_version.py
+-rw-rw-rw-   0        0        0      723 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_ruby_version.py
+-rw-rw-rw-   0        0        0     1724 2023-07-25 06:45:33.000000 common_version-0.0.3/tests/test_snyk_version.py
+-rw-rw-rw-   0        0        0      383 2023-07-25 06:36:58.000000 common_version-0.0.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.873926 common_version-0.0.3/version/
+-rw-rw-rw-   0        0        0    12819 2023-07-25 07:02:04.000000 common_version-0.0.3/version/__init__.py
+-rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.3/version/base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.876922 common_version-0.0.3/version/command/
+-rw-rw-rw-   0        0        0      149 2023-07-25 06:59:09.000000 common_version-0.0.3/version/command/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-02-07 06:12:25.000000 common_version-0.0.3/version/command/__main__.py
+-rw-rw-rw-   0        0        0    11319 2023-07-25 07:00:35.000000 common_version-0.0.3/version/command/case.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.878922 common_version-0.0.3/version/core/
+-rw-rw-rw-   0        0        0        0 2023-03-30 09:25:46.000000 common_version-0.0.3/version/core/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-04-04 05:58:07.000000 common_version-0.0.3/version/core/utils.py
+-rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.3/version/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.891482 common_version-0.0.3/version/expression/
+-rw-rw-rw-   0        0        0     2099 2023-07-25 06:52:02.000000 common_version-0.0.3/version/expression/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 06:52:15.000000 common_version-0.0.3/version/expression/base.py
+-rw-rw-rw-   0        0        0    28047 2023-07-25 06:33:38.000000 common_version-0.0.3/version/expression/base_method.py
+-rw-rw-rw-   0        0        0     2318 2023-07-25 06:26:36.000000 common_version-0.0.3/version/expression/c_version_expression.py
+-rw-rw-rw-   0        0        0     2581 2023-07-25 06:27:06.000000 common_version-0.0.3/version/expression/cargo_version_expression.py
+-rw-rw-rw-   0        0        0     2144 2023-07-25 06:27:06.000000 common_version-0.0.3/version/expression/cocoapods_version_expression.py
+-rw-rw-rw-   0        0        0     6942 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/composer_version_expression.py
+-rw-rw-rw-   0        0        0      626 2023-07-25 06:46:05.000000 common_version-0.0.3/version/expression/go_version_expression.py
+-rw-rw-rw-   0        0        0     2449 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/hex_version_expression.py
+-rw-rw-rw-   0        0        0     2946 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/linux_version_expression.py
+-rw-rw-rw-   0        0        0     4036 2023-07-25 06:46:07.000000 common_version-0.0.3/version/expression/maven_version_expression.py
+-rw-rw-rw-   0        0        0     6331 2023-07-25 06:46:08.000000 common_version-0.0.3/version/expression/npm_version_expression.py
+-rw-rw-rw-   0        0        0     4329 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/nuget_version_expression.py
+-rw-rw-rw-   0        0        0     1529 2023-07-25 06:46:11.000000 common_version-0.0.3/version/expression/nvd_version_expression.py
+-rw-rw-rw-   0        0        0     4465 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/other_version_expression.py
+-rw-rw-rw-   0        0        0     6270 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/pip_version_expression.py
+-rw-rw-rw-   0        0        0     3353 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/ruby_version_expression.py
+-rw-rw-rw-   0        0        0     3970 2023-07-25 06:46:12.000000 common_version-0.0.3/version/expression/snyk_version_expression.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.899482 common_version-0.0.3/version/version_base/
+-rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.3/version/version_base/__init__.py
+-rw-rw-rw-   0        0        0    33829 2023-07-25 06:33:38.000000 common_version-0.0.3/version/version_base/base_item.py
+-rw-rw-rw-   0        0        0    19296 2023-07-25 06:29:26.000000 common_version-0.0.3/version/version_base/base_version.py
+-rw-rw-rw-   0        0        0     1906 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/common_method.py
+-rw-rw-rw-   0        0        0     1839 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/composer_version.py
+-rw-rw-rw-   0        0        0     1605 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/go_version.py
+-rw-rw-rw-   0        0        0     4200 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/linux_version.py
+-rw-rw-rw-   0        0        0    11651 2023-07-25 07:00:35.000000 common_version-0.0.3/version/version_base/lj_version.py
+-rw-rw-rw-   0        0        0     2397 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/maven_version.py
+-rw-rw-rw-   0        0        0     1511 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/npm_version.py
+-rw-rw-rw-   0        0        0     5766 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/snyk_version.py
```

### Comparing `common_version-0.0.2/LICENSE` & `common_version-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/PKG-INFO` & `common_version-0.0.3/common_version.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common_version
-Version: 0.0.2
+Name: common-version
+Version: 0.0.3
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,27 +18,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # common_version
 
-基于包管理器以及漏洞网站的版本表达式统一化 初始化
+基于包管理器以及漏洞网站的版本表达式统一化
 
--------
-
-.. code-block:: bash
+. code-block:: bash
 
     git clone https://github.com/hsc1102/common_version.git
     cd common_version
     pip install "flake8<3.8" bumpversion pep8-naming
     flake8 --install-hook git
     git config --bool flake8.strict true
 
 版本发布
 --------
 
-.. code-block:: bash
+. code-block:: bash
 
     bumpversion patch
     git push origin master --tags
     git pull && bumpversion patch && git push origin master --tags
+
+
+. code-block:: bash
+
+    pip install twine whell
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
```

### Comparing `common_version-0.0.2/README.md` & `common_version-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # common_version
 
-基于包管理器以及漏洞网站的版本表达式统一化 初始化
+基于包管理器以及漏洞网站的版本表达式统一化
 
--------
-
-.. code-block:: bash
+. code-block:: bash
 
     git clone https://github.com/hsc1102/common_version.git
     cd common_version
     pip install "flake8<3.8" bumpversion pep8-naming
     flake8 --install-hook git
     git config --bool flake8.strict true
 
 版本发布
 --------
 
-.. code-block:: bash
+. code-block:: bash
 
     bumpversion patch
     git push origin master --tags
     git pull && bumpversion patch && git push origin master --tags
+
+
+. code-block:: bash
+
+    pip install twine whell
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
```

### Comparing `common_version-0.0.2/common_version.egg-info/PKG-INFO` & `common_version-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common-version
-Version: 0.0.2
+Name: common_version
+Version: 0.0.3
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,27 +18,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # common_version
 
-基于包管理器以及漏洞网站的版本表达式统一化 初始化
+基于包管理器以及漏洞网站的版本表达式统一化
 
--------
-
-.. code-block:: bash
+. code-block:: bash
 
     git clone https://github.com/hsc1102/common_version.git
     cd common_version
     pip install "flake8<3.8" bumpversion pep8-naming
     flake8 --install-hook git
     git config --bool flake8.strict true
 
 版本发布
 --------
 
-.. code-block:: bash
+. code-block:: bash
 
     bumpversion patch
     git push origin master --tags
     git pull && bumpversion patch && git push origin master --tags
+
+
+. code-block:: bash
+
+    pip install twine whell
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
```

### Comparing `common_version-0.0.2/common_version.egg-info/SOURCES.txt` & `common_version-0.0.3/common_version.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 common_version.egg-info/PKG-INFO
 common_version.egg-info/SOURCES.txt
 common_version.egg-info/dependency_links.txt
+common_version.egg-info/entry_points.txt
 common_version.egg-info/not-zip-safe
 common_version.egg-info/requires.txt
 common_version.egg-info/top_level.txt
 tests/test_c_version.py
 tests/test_cargo_version.py
 tests/test_coco_version.py
 tests/test_common.py
@@ -26,14 +27,17 @@
 tests/test_pip_version.py
 tests/test_ruby_version.py
 tests/test_snyk_version.py
 tests/test_utils.py
 version/__init__.py
 version/base.py
 version/exceptions.py
+version/command/__init__.py
+version/command/__main__.py
+version/command/case.py
 version/core/__init__.py
 version/core/utils.py
 version/expression/__init__.py
 version/expression/base.py
 version/expression/base_method.py
 version/expression/c_version_expression.py
 version/expression/cargo_version_expression.py
```

### Comparing `common_version-0.0.2/setup.cfg` & `common_version-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_c_version.py` & `common_version-0.0.3/tests/test_c_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_cargo_version.py` & `common_version-0.0.3/tests/test_cargo_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_coco_version.py` & `common_version-0.0.3/tests/test_coco_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_common.py` & `common_version-0.0.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_composer_version.py` & `common_version-0.0.3/tests/test_composer_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_go_version.py` & `common_version-0.0.3/tests/test_go_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_hex_version.py` & `common_version-0.0.3/tests/test_hex_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_linux_version.py` & `common_version-0.0.3/tests/test_linux_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_maven_version.py` & `common_version-0.0.3/tests/test_maven_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_merge_versions_expression.py` & `common_version-0.0.3/tests/test_merge_versions_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_npm_version.py` & `common_version-0.0.3/tests/test_npm_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_nuget_version.py` & `common_version-0.0.3/tests/test_nuget_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_nvd_version.py` & `common_version-0.0.3/tests/test_nvd_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_other_version.py` & `common_version-0.0.3/tests/test_other_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_pip_version.py` & `common_version-0.0.3/tests/test_pip_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_ruby_version.py` & `common_version-0.0.3/tests/test_ruby_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/tests/test_snyk_version.py` & `common_version-0.0.3/tests/test_snyk_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/__init__.py` & `common_version-0.0.3/version/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import enum
 
 __all__ = [
     "check_version_in_expression",
     "PackageType",
     "get_base_version",
@@ -232,18 +232,18 @@
         return version.is_canonical(version)
     else:
         return Package_CLASSES[class_package_type](version, package_type.lower()).is_canonical(version)
 
 
 def change_to_expression(package_type: str, version_expression):
     """
-    组件版本表达式转换为棱镜版本表达式
+    组件版本表达式转换为版本表达式
     :param package_type: 包管理器类型
     :param version_expression: 组件版本表达式
-    :return: 棱镜版本表达式
+    :return: 版本表达式
     """
     expression_type = None
     if isinstance(package_type, str):
         package_type = MapPackageType.get_value_by_key(package_type)
         if package_type.lower() in PackageType.values():
             expression_type = PackageType(package_type.lower())
         else:
```

### Comparing `common_version-0.0.2/version/base.py` & `common_version-0.0.3/version/base.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/core/utils.py` & `common_version-0.0.3/version/core/utils.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/exceptions.py` & `common_version-0.0.3/version/exceptions.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/__init__.py` & `common_version-0.0.3/version/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/base_method.py` & `common_version-0.0.3/version/expression/base_method.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/c_version_expression.py` & `common_version-0.0.3/version/expression/c_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/cargo_version_expression.py` & `common_version-0.0.3/version/expression/cargo_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/cocoapods_version_expression.py` & `common_version-0.0.3/version/expression/cocoapods_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/composer_version_expression.py` & `common_version-0.0.3/version/expression/composer_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/go_version_expression.py` & `common_version-0.0.3/version/expression/go_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/hex_version_expression.py` & `common_version-0.0.3/version/expression/hex_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/linux_version_expression.py` & `common_version-0.0.3/version/expression/linux_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/maven_version_expression.py` & `common_version-0.0.3/version/expression/maven_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/npm_version_expression.py` & `common_version-0.0.3/version/expression/npm_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/nuget_version_expression.py` & `common_version-0.0.3/version/expression/nuget_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/nvd_version_expression.py` & `common_version-0.0.3/version/expression/nvd_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/other_version_expression.py` & `common_version-0.0.3/version/expression/other_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/pip_version_expression.py` & `common_version-0.0.3/version/expression/pip_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/ruby_version_expression.py` & `common_version-0.0.3/version/expression/ruby_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/expression/snyk_version_expression.py` & `common_version-0.0.3/version/expression/snyk_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/__init__.py` & `common_version-0.0.3/version/version_base/__init__.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/base_item.py` & `common_version-0.0.3/version/version_base/base_item.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/base_version.py` & `common_version-0.0.3/version/version_base/base_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/common_method.py` & `common_version-0.0.3/version/version_base/common_method.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/composer_version.py` & `common_version-0.0.3/version/version_base/composer_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/go_version.py` & `common_version-0.0.3/version/version_base/go_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/linux_version.py` & `common_version-0.0.3/version/version_base/linux_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/lj_version.py` & `common_version-0.0.3/version/version_base/lj_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         )
         version1_obj = get_base_version(self.package_type, version1)
         version2_obj = get_base_version(self.package_type, version2)
         return version1_obj.__cmp__(version2_obj)
 
     def format_version_lj_list(self, lj_expression):
         """
-        格式化棱镜表达式
+        格式化表达式
         :param lj_expression:
         :param version_str:
         :return:
         """
         if "||" in lj_expression:
             self.format_version_list = lj_expression.split("||")
         else:
@@ -153,15 +153,15 @@
         ret = ret.merge()
         return ret
 
     def check_version_in_expression(self, lj_expression):
         from version import get_base_version
         from version.version_base import Equal_Or_Compare_Type
         """
-        检查版本是否属于棱镜表达式
+        检查版本是否属于表达式
         :param lj_expression:
         :return:
         """
         if isinstance(lj_expression, Item) or isinstance(lj_expression, ItemGroup):
             if lj_expression.get_value() == "*":
                 return True
             ret = lj_expression
```

### Comparing `common_version-0.0.2/version/version_base/maven_version.py` & `common_version-0.0.3/version/version_base/maven_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/npm_version.py` & `common_version-0.0.3/version/version_base/npm_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.2/version/version_base/snyk_version.py` & `common_version-0.0.3/version/version_base/snyk_version.py`

 * *Files identical despite different names*

