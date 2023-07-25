# Comparing `tmp/common_version-0.0.3.tar.gz` & `tmp/common_version-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_version-0.0.3.tar", last modified: Tue Jul 25 07:07:30 2023, max compression
+gzip compressed data, was "common_version-0.0.4.tar", last modified: Tue Jul 25 07:11:06 2023, max compression
```

## Comparing `common_version-0.0.3.tar` & `common_version-0.0.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.900483 common_version-0.0.3/
--rw-rw-rw-   0        0        0     1543 2023-07-11 06:12:49.000000 common_version-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1423 2023-07-25 07:07:30.900483 common_version-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      618 2023-07-25 07:07:27.000000 common_version-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.858922 common_version-0.0.3/common_version.egg-info/
--rw-rw-rw-   0        0        0     1423 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 07:07:30.000000 common_version-0.0.3/common_version.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1246 2023-07-25 07:07:30.901482 common_version-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      191 2023-07-25 06:59:09.000000 common_version-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.870922 common_version-0.0.3/tests/
--rw-rw-rw-   0        0        0      812 2023-07-25 06:41:44.000000 common_version-0.0.3/tests/test_c_version.py
--rw-rw-rw-   0        0        0      929 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_cargo_version.py
--rw-rw-rw-   0        0        0      727 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_coco_version.py
--rw-rw-rw-   0        0        0     1122 2023-07-25 06:31:04.000000 common_version-0.0.3/tests/test_common.py
--rw-rw-rw-   0        0        0     1112 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_composer_version.py
--rw-rw-rw-   0        0        0      743 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_go_version.py
--rw-rw-rw-   0        0        0      717 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_hex_version.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 06:34:33.000000 common_version-0.0.3/tests/test_linux_version.py
--rw-rw-rw-   0        0        0      839 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_maven_version.py
--rw-rw-rw-   0        0        0      811 2023-07-25 06:31:04.000000 common_version-0.0.3/tests/test_merge_versions_expression.py
--rw-rw-rw-   0        0        0     1683 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_npm_version.py
--rw-rw-rw-   0        0        0      753 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_nuget_version.py
--rw-rw-rw-   0        0        0      915 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_nvd_version.py
--rw-rw-rw-   0        0        0     1039 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_other_version.py
--rw-rw-rw-   0        0        0     1247 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_pip_version.py
--rw-rw-rw-   0        0        0      723 2023-07-25 06:33:38.000000 common_version-0.0.3/tests/test_ruby_version.py
--rw-rw-rw-   0        0        0     1724 2023-07-25 06:45:33.000000 common_version-0.0.3/tests/test_snyk_version.py
--rw-rw-rw-   0        0        0      383 2023-07-25 06:36:58.000000 common_version-0.0.3/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.873926 common_version-0.0.3/version/
--rw-rw-rw-   0        0        0    12819 2023-07-25 07:02:04.000000 common_version-0.0.3/version/__init__.py
--rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.3/version/base.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.876922 common_version-0.0.3/version/command/
--rw-rw-rw-   0        0        0      149 2023-07-25 06:59:09.000000 common_version-0.0.3/version/command/__init__.py
--rw-rw-rw-   0        0        0      210 2023-02-07 06:12:25.000000 common_version-0.0.3/version/command/__main__.py
--rw-rw-rw-   0        0        0    11319 2023-07-25 07:00:35.000000 common_version-0.0.3/version/command/case.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.878922 common_version-0.0.3/version/core/
--rw-rw-rw-   0        0        0        0 2023-03-30 09:25:46.000000 common_version-0.0.3/version/core/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-04-04 05:58:07.000000 common_version-0.0.3/version/core/utils.py
--rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.3/version/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.891482 common_version-0.0.3/version/expression/
--rw-rw-rw-   0        0        0     2099 2023-07-25 06:52:02.000000 common_version-0.0.3/version/expression/__init__.py
--rw-rw-rw-   0        0        0      436 2023-07-25 06:52:15.000000 common_version-0.0.3/version/expression/base.py
--rw-rw-rw-   0        0        0    28047 2023-07-25 06:33:38.000000 common_version-0.0.3/version/expression/base_method.py
--rw-rw-rw-   0        0        0     2318 2023-07-25 06:26:36.000000 common_version-0.0.3/version/expression/c_version_expression.py
--rw-rw-rw-   0        0        0     2581 2023-07-25 06:27:06.000000 common_version-0.0.3/version/expression/cargo_version_expression.py
--rw-rw-rw-   0        0        0     2144 2023-07-25 06:27:06.000000 common_version-0.0.3/version/expression/cocoapods_version_expression.py
--rw-rw-rw-   0        0        0     6942 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/composer_version_expression.py
--rw-rw-rw-   0        0        0      626 2023-07-25 06:46:05.000000 common_version-0.0.3/version/expression/go_version_expression.py
--rw-rw-rw-   0        0        0     2449 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/hex_version_expression.py
--rw-rw-rw-   0        0        0     2946 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/linux_version_expression.py
--rw-rw-rw-   0        0        0     4036 2023-07-25 06:46:07.000000 common_version-0.0.3/version/expression/maven_version_expression.py
--rw-rw-rw-   0        0        0     6331 2023-07-25 06:46:08.000000 common_version-0.0.3/version/expression/npm_version_expression.py
--rw-rw-rw-   0        0        0     4329 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/nuget_version_expression.py
--rw-rw-rw-   0        0        0     1529 2023-07-25 06:46:11.000000 common_version-0.0.3/version/expression/nvd_version_expression.py
--rw-rw-rw-   0        0        0     4465 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/other_version_expression.py
--rw-rw-rw-   0        0        0     6270 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/pip_version_expression.py
--rw-rw-rw-   0        0        0     3353 2023-07-25 06:29:26.000000 common_version-0.0.3/version/expression/ruby_version_expression.py
--rw-rw-rw-   0        0        0     3970 2023-07-25 06:46:12.000000 common_version-0.0.3/version/expression/snyk_version_expression.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:07:30.899482 common_version-0.0.3/version/version_base/
--rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.3/version/version_base/__init__.py
--rw-rw-rw-   0        0        0    33829 2023-07-25 06:33:38.000000 common_version-0.0.3/version/version_base/base_item.py
--rw-rw-rw-   0        0        0    19296 2023-07-25 06:29:26.000000 common_version-0.0.3/version/version_base/base_version.py
--rw-rw-rw-   0        0        0     1906 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/common_method.py
--rw-rw-rw-   0        0        0     1839 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/composer_version.py
--rw-rw-rw-   0        0        0     1605 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/go_version.py
--rw-rw-rw-   0        0        0     4200 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/linux_version.py
--rw-rw-rw-   0        0        0    11651 2023-07-25 07:00:35.000000 common_version-0.0.3/version/version_base/lj_version.py
--rw-rw-rw-   0        0        0     2397 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/maven_version.py
--rw-rw-rw-   0        0        0     1511 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/npm_version.py
--rw-rw-rw-   0        0        0     5766 2023-07-25 06:30:16.000000 common_version-0.0.3/version/version_base/snyk_version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.201582 common_version-0.0.4/
+-rw-rw-rw-   0        0        0     1544 2023-07-25 07:08:49.000000 common_version-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1423 2023-07-25 07:11:06.202582 common_version-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-07-25 07:07:27.000000 common_version-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.161422 common_version-0.0.4/common_version.egg-info/
+-rw-rw-rw-   0        0        0     1423 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 07:11:06.000000 common_version-0.0.4/common_version.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1246 2023-07-25 07:11:06.202582 common_version-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      191 2023-07-25 06:59:09.000000 common_version-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.175253 common_version-0.0.4/tests/
+-rw-rw-rw-   0        0        0      812 2023-07-25 06:41:44.000000 common_version-0.0.4/tests/test_c_version.py
+-rw-rw-rw-   0        0        0      929 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_cargo_version.py
+-rw-rw-rw-   0        0        0      727 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_coco_version.py
+-rw-rw-rw-   0        0        0     1122 2023-07-25 06:31:04.000000 common_version-0.0.4/tests/test_common.py
+-rw-rw-rw-   0        0        0     1112 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_composer_version.py
+-rw-rw-rw-   0        0        0      743 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_go_version.py
+-rw-rw-rw-   0        0        0      717 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_hex_version.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 06:34:33.000000 common_version-0.0.4/tests/test_linux_version.py
+-rw-rw-rw-   0        0        0      839 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_maven_version.py
+-rw-rw-rw-   0        0        0      811 2023-07-25 06:31:04.000000 common_version-0.0.4/tests/test_merge_versions_expression.py
+-rw-rw-rw-   0        0        0     1683 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_npm_version.py
+-rw-rw-rw-   0        0        0      753 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_nuget_version.py
+-rw-rw-rw-   0        0        0      915 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_nvd_version.py
+-rw-rw-rw-   0        0        0     1039 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_other_version.py
+-rw-rw-rw-   0        0        0     1247 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_pip_version.py
+-rw-rw-rw-   0        0        0      723 2023-07-25 06:33:38.000000 common_version-0.0.4/tests/test_ruby_version.py
+-rw-rw-rw-   0        0        0     1724 2023-07-25 06:45:33.000000 common_version-0.0.4/tests/test_snyk_version.py
+-rw-rw-rw-   0        0        0      383 2023-07-25 06:36:58.000000 common_version-0.0.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.177238 common_version-0.0.4/version/
+-rw-rw-rw-   0        0        0    12819 2023-07-25 07:09:38.000000 common_version-0.0.4/version/__init__.py
+-rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.4/version/base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.179237 common_version-0.0.4/version/command/
+-rw-rw-rw-   0        0        0      149 2023-07-25 06:59:09.000000 common_version-0.0.4/version/command/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-02-07 06:12:25.000000 common_version-0.0.4/version/command/__main__.py
+-rw-rw-rw-   0        0        0    11319 2023-07-25 07:00:35.000000 common_version-0.0.4/version/command/case.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.181237 common_version-0.0.4/version/core/
+-rw-rw-rw-   0        0        0        0 2023-03-30 09:25:46.000000 common_version-0.0.4/version/core/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-04-04 05:58:07.000000 common_version-0.0.4/version/core/utils.py
+-rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.4/version/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.194165 common_version-0.0.4/version/expression/
+-rw-rw-rw-   0        0        0     2099 2023-07-25 06:52:02.000000 common_version-0.0.4/version/expression/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 06:52:15.000000 common_version-0.0.4/version/expression/base.py
+-rw-rw-rw-   0        0        0    28047 2023-07-25 06:33:38.000000 common_version-0.0.4/version/expression/base_method.py
+-rw-rw-rw-   0        0        0     2318 2023-07-25 06:26:36.000000 common_version-0.0.4/version/expression/c_version_expression.py
+-rw-rw-rw-   0        0        0     2581 2023-07-25 06:27:06.000000 common_version-0.0.4/version/expression/cargo_version_expression.py
+-rw-rw-rw-   0        0        0     2144 2023-07-25 06:27:06.000000 common_version-0.0.4/version/expression/cocoapods_version_expression.py
+-rw-rw-rw-   0        0        0     6942 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/composer_version_expression.py
+-rw-rw-rw-   0        0        0      626 2023-07-25 06:46:05.000000 common_version-0.0.4/version/expression/go_version_expression.py
+-rw-rw-rw-   0        0        0     2449 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/hex_version_expression.py
+-rw-rw-rw-   0        0        0     2946 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/linux_version_expression.py
+-rw-rw-rw-   0        0        0     4036 2023-07-25 06:46:07.000000 common_version-0.0.4/version/expression/maven_version_expression.py
+-rw-rw-rw-   0        0        0     6331 2023-07-25 06:46:08.000000 common_version-0.0.4/version/expression/npm_version_expression.py
+-rw-rw-rw-   0        0        0     4329 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/nuget_version_expression.py
+-rw-rw-rw-   0        0        0     1529 2023-07-25 06:46:11.000000 common_version-0.0.4/version/expression/nvd_version_expression.py
+-rw-rw-rw-   0        0        0     4465 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/other_version_expression.py
+-rw-rw-rw-   0        0        0     6270 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/pip_version_expression.py
+-rw-rw-rw-   0        0        0     3353 2023-07-25 06:29:26.000000 common_version-0.0.4/version/expression/ruby_version_expression.py
+-rw-rw-rw-   0        0        0     3970 2023-07-25 06:46:12.000000 common_version-0.0.4/version/expression/snyk_version_expression.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:06.201582 common_version-0.0.4/version/version_base/
+-rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.4/version/version_base/__init__.py
+-rw-rw-rw-   0        0        0    33829 2023-07-25 06:33:38.000000 common_version-0.0.4/version/version_base/base_item.py
+-rw-rw-rw-   0        0        0    19296 2023-07-25 06:29:26.000000 common_version-0.0.4/version/version_base/base_version.py
+-rw-rw-rw-   0        0        0     1906 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/common_method.py
+-rw-rw-rw-   0        0        0     1839 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/composer_version.py
+-rw-rw-rw-   0        0        0     1605 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/go_version.py
+-rw-rw-rw-   0        0        0     4200 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/linux_version.py
+-rw-rw-rw-   0        0        0    11651 2023-07-25 07:00:35.000000 common_version-0.0.4/version/version_base/lj_version.py
+-rw-rw-rw-   0        0        0     2397 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/maven_version.py
+-rw-rw-rw-   0        0        0     1511 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/npm_version.py
+-rw-rw-rw-   0        0        0     5766 2023-07-25 06:30:16.000000 common_version-0.0.4/version/version_base/snyk_version.py
```

### Comparing `common_version-0.0.3/LICENSE` & `common_version-0.0.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, 007gzs
+Copyright (c) 2020, hsc1102
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `common_version-0.0.3/PKG-INFO` & `common_version-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_version
-Version: 0.0.3
+Version: 0.0.4
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `common_version-0.0.3/README.md` & `common_version-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/common_version.egg-info/PKG-INFO` & `common_version-0.0.4/common_version.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-version
-Version: 0.0.3
+Version: 0.0.4
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `common_version-0.0.3/common_version.egg-info/SOURCES.txt` & `common_version-0.0.4/common_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/setup.cfg` & `common_version-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_c_version.py` & `common_version-0.0.4/tests/test_c_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_cargo_version.py` & `common_version-0.0.4/tests/test_cargo_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_coco_version.py` & `common_version-0.0.4/tests/test_coco_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_common.py` & `common_version-0.0.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_composer_version.py` & `common_version-0.0.4/tests/test_composer_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_go_version.py` & `common_version-0.0.4/tests/test_go_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_hex_version.py` & `common_version-0.0.4/tests/test_hex_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_linux_version.py` & `common_version-0.0.4/tests/test_linux_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_maven_version.py` & `common_version-0.0.4/tests/test_maven_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_merge_versions_expression.py` & `common_version-0.0.4/tests/test_merge_versions_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_npm_version.py` & `common_version-0.0.4/tests/test_npm_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_nuget_version.py` & `common_version-0.0.4/tests/test_nuget_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_nvd_version.py` & `common_version-0.0.4/tests/test_nvd_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_other_version.py` & `common_version-0.0.4/tests/test_other_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_pip_version.py` & `common_version-0.0.4/tests/test_pip_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_ruby_version.py` & `common_version-0.0.4/tests/test_ruby_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/tests/test_snyk_version.py` & `common_version-0.0.4/tests/test_snyk_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/__init__.py` & `common_version-0.0.4/version/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import enum
 
 __all__ = [
     "check_version_in_expression",
     "PackageType",
     "get_base_version",
```

### Comparing `common_version-0.0.3/version/base.py` & `common_version-0.0.4/version/base.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/command/case.py` & `common_version-0.0.4/version/command/case.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/core/utils.py` & `common_version-0.0.4/version/core/utils.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/exceptions.py` & `common_version-0.0.4/version/exceptions.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/__init__.py` & `common_version-0.0.4/version/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/base_method.py` & `common_version-0.0.4/version/expression/base_method.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/c_version_expression.py` & `common_version-0.0.4/version/expression/c_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/cargo_version_expression.py` & `common_version-0.0.4/version/expression/cargo_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/cocoapods_version_expression.py` & `common_version-0.0.4/version/expression/cocoapods_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/composer_version_expression.py` & `common_version-0.0.4/version/expression/composer_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/go_version_expression.py` & `common_version-0.0.4/version/expression/go_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/hex_version_expression.py` & `common_version-0.0.4/version/expression/hex_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/linux_version_expression.py` & `common_version-0.0.4/version/expression/linux_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/maven_version_expression.py` & `common_version-0.0.4/version/expression/maven_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/npm_version_expression.py` & `common_version-0.0.4/version/expression/npm_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/nuget_version_expression.py` & `common_version-0.0.4/version/expression/nuget_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/nvd_version_expression.py` & `common_version-0.0.4/version/expression/nvd_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/other_version_expression.py` & `common_version-0.0.4/version/expression/other_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/pip_version_expression.py` & `common_version-0.0.4/version/expression/pip_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/ruby_version_expression.py` & `common_version-0.0.4/version/expression/ruby_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/expression/snyk_version_expression.py` & `common_version-0.0.4/version/expression/snyk_version_expression.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/__init__.py` & `common_version-0.0.4/version/version_base/__init__.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/base_item.py` & `common_version-0.0.4/version/version_base/base_item.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/base_version.py` & `common_version-0.0.4/version/version_base/base_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/common_method.py` & `common_version-0.0.4/version/version_base/common_method.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/composer_version.py` & `common_version-0.0.4/version/version_base/composer_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/go_version.py` & `common_version-0.0.4/version/version_base/go_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/linux_version.py` & `common_version-0.0.4/version/version_base/linux_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/lj_version.py` & `common_version-0.0.4/version/version_base/lj_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/maven_version.py` & `common_version-0.0.4/version/version_base/maven_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/npm_version.py` & `common_version-0.0.4/version/version_base/npm_version.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.3/version/version_base/snyk_version.py` & `common_version-0.0.4/version/version_base/snyk_version.py`

 * *Files identical despite different names*

