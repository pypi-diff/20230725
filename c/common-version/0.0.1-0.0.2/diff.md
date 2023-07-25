# Comparing `tmp/common_version-0.0.1.tar.gz` & `tmp/common_version-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_version-0.0.1.tar", last modified: Tue Jul 25 06:19:19 2023, max compression
+gzip compressed data, was "common_version-0.0.2.tar", last modified: Tue Jul 25 06:56:05 2023, max compression
```

## Comparing `common_version-0.0.1.tar` & `common_version-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:19:19.740234 common_version-0.0.1/
--rw-rw-rw-   0        0        0     1543 2023-07-11 06:12:49.000000 common_version-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      888 2023-07-25 06:19:19.740234 common_version-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-07-25 03:24:59.000000 common_version-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:19:19.713779 common_version-0.0.1/common_version.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1521 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 06:19:19.000000 common_version-0.0.1/common_version.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1238 2023-07-25 06:19:19.741229 common_version-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       62 2023-07-11 06:12:49.000000 common_version-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:19:19.715781 common_version-0.0.1/version/
--rw-rw-rw-   0        0        0    12844 2023-06-07 05:52:02.000000 common_version-0.0.1/version/__init__.py
--rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.1/version/base.py
--rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.1/version/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:19:19.729196 common_version-0.0.1/version/expression/
--rw-rw-rw-   0        0        0     2527 2023-02-10 10:31:15.000000 common_version-0.0.1/version/expression/__init__.py
--rw-rw-rw-   0        0        0      419 2023-02-14 09:21:18.000000 common_version-0.0.1/version/expression/base.py
--rw-rw-rw-   0        0        0    28275 2023-04-24 09:15:29.000000 common_version-0.0.1/version/expression/base_method.py
--rw-rw-rw-   0        0        0     2360 2023-02-14 09:36:41.000000 common_version-0.0.1/version/expression/c_version_expression.py
--rw-rw-rw-   0        0        0     2638 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/cargo_version_expression.py
--rw-rw-rw-   0        0        0     2203 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/cocoapods_version_expression.py
--rw-rw-rw-   0        0        0     7281 2023-03-10 09:59:08.000000 common_version-0.0.1/version/expression/composer_version_expression.py
--rw-rw-rw-   0        0        0      850 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/go_version_expression.py
--rw-rw-rw-   0        0        0     2686 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/hex_version_expression.py
--rw-rw-rw-   0        0        0     3198 2023-03-15 11:02:43.000000 common_version-0.0.1/version/expression/linux_version_expression.py
--rw-rw-rw-   0        0        0     4277 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/maven_version_expression.py
--rw-rw-rw-   0        0        0     6642 2023-02-15 08:48:33.000000 common_version-0.0.1/version/expression/npm_version_expression.py
--rw-rw-rw-   0        0        0     4596 2023-02-15 09:50:08.000000 common_version-0.0.1/version/expression/nuget_version_expression.py
--rw-rw-rw-   0        0        0     1768 2023-02-07 06:12:25.000000 common_version-0.0.1/version/expression/nvd_version_expression.py
--rw-rw-rw-   0        0        0     4747 2023-02-14 09:25:22.000000 common_version-0.0.1/version/expression/other_version_expression.py
--rw-rw-rw-   0        0        0     6544 2023-03-07 06:00:52.000000 common_version-0.0.1/version/expression/pip_version_expression.py
--rw-rw-rw-   0        0        0     3622 2023-03-15 11:16:38.000000 common_version-0.0.1/version/expression/ruby_version_expression.py
--rw-rw-rw-   0        0        0     4224 2023-04-12 09:01:36.000000 common_version-0.0.1/version/expression/snyk_version_expression.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:19:19.739229 common_version-0.0.1/version/version_base/
--rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.1/version/version_base/__init__.py
--rw-rw-rw-   0        0        0    33955 2023-04-26 02:12:21.000000 common_version-0.0.1/version/version_base/base_item.py
--rw-rw-rw-   0        0        0    19356 2023-06-07 03:49:26.000000 common_version-0.0.1/version/version_base/base_version.py
--rw-rw-rw-   0        0        0     1921 2023-02-27 08:46:55.000000 common_version-0.0.1/version/version_base/common_method.py
--rw-rw-rw-   0        0        0     1869 2023-04-25 09:58:21.000000 common_version-0.0.1/version/version_base/composer_version.py
--rw-rw-rw-   0        0        0     1635 2023-04-25 09:56:45.000000 common_version-0.0.1/version/version_base/go_version.py
--rw-rw-rw-   0        0        0     4230 2023-06-07 06:01:43.000000 common_version-0.0.1/version/version_base/linux_version.py
--rw-rw-rw-   0        0        0    11861 2023-04-25 10:24:13.000000 common_version-0.0.1/version/version_base/lj_version.py
--rw-rw-rw-   0        0        0     2427 2023-04-25 12:25:01.000000 common_version-0.0.1/version/version_base/maven_version.py
--rw-rw-rw-   0        0        0     1541 2023-04-25 09:56:10.000000 common_version-0.0.1/version/version_base/npm_version.py
--rw-rw-rw-   0        0        0     5811 2023-06-07 06:01:45.000000 common_version-0.0.1/version/version_base/snyk_version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.321009 common_version-0.0.2/
+-rw-rw-rw-   0        0        0     1543 2023-07-11 06:12:49.000000 common_version-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-07-11 06:12:49.000000 common_version-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1326 2023-07-25 06:56:05.322009 common_version-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-07-25 06:55:59.000000 common_version-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.277789 common_version-0.0.2/common_version.egg-info/
+-rw-rw-rw-   0        0        0     1326 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2054 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 06:54:17.000000 common_version-0.0.2/common_version.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 06:56:05.000000 common_version-0.0.2/common_version.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1246 2023-07-25 06:56:05.322009 common_version-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       62 2023-07-11 06:12:49.000000 common_version-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.291923 common_version-0.0.2/tests/
+-rw-rw-rw-   0        0        0      812 2023-07-25 06:41:44.000000 common_version-0.0.2/tests/test_c_version.py
+-rw-rw-rw-   0        0        0      929 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_cargo_version.py
+-rw-rw-rw-   0        0        0      727 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_coco_version.py
+-rw-rw-rw-   0        0        0     1122 2023-07-25 06:31:04.000000 common_version-0.0.2/tests/test_common.py
+-rw-rw-rw-   0        0        0     1112 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_composer_version.py
+-rw-rw-rw-   0        0        0      743 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_go_version.py
+-rw-rw-rw-   0        0        0      717 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_hex_version.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 06:34:33.000000 common_version-0.0.2/tests/test_linux_version.py
+-rw-rw-rw-   0        0        0      839 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_maven_version.py
+-rw-rw-rw-   0        0        0      811 2023-07-25 06:31:04.000000 common_version-0.0.2/tests/test_merge_versions_expression.py
+-rw-rw-rw-   0        0        0     1683 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_npm_version.py
+-rw-rw-rw-   0        0        0      753 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_nuget_version.py
+-rw-rw-rw-   0        0        0      915 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_nvd_version.py
+-rw-rw-rw-   0        0        0     1039 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_other_version.py
+-rw-rw-rw-   0        0        0     1247 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_pip_version.py
+-rw-rw-rw-   0        0        0      723 2023-07-25 06:33:38.000000 common_version-0.0.2/tests/test_ruby_version.py
+-rw-rw-rw-   0        0        0     1724 2023-07-25 06:45:33.000000 common_version-0.0.2/tests/test_snyk_version.py
+-rw-rw-rw-   0        0        0      383 2023-07-25 06:36:58.000000 common_version-0.0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.294460 common_version-0.0.2/version/
+-rw-rw-rw-   0        0        0    12831 2023-07-25 06:54:00.000000 common_version-0.0.2/version/__init__.py
+-rw-rw-rw-   0        0        0      593 2023-02-07 06:12:25.000000 common_version-0.0.2/version/base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.295461 common_version-0.0.2/version/core/
+-rw-rw-rw-   0        0        0        0 2023-03-30 09:25:46.000000 common_version-0.0.2/version/core/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-04-04 05:58:07.000000 common_version-0.0.2/version/core/utils.py
+-rw-rw-rw-   0        0        0      827 2023-02-07 06:12:25.000000 common_version-0.0.2/version/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.310009 common_version-0.0.2/version/expression/
+-rw-rw-rw-   0        0        0     2099 2023-07-25 06:52:02.000000 common_version-0.0.2/version/expression/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 06:52:15.000000 common_version-0.0.2/version/expression/base.py
+-rw-rw-rw-   0        0        0    28047 2023-07-25 06:33:38.000000 common_version-0.0.2/version/expression/base_method.py
+-rw-rw-rw-   0        0        0     2318 2023-07-25 06:26:36.000000 common_version-0.0.2/version/expression/c_version_expression.py
+-rw-rw-rw-   0        0        0     2581 2023-07-25 06:27:06.000000 common_version-0.0.2/version/expression/cargo_version_expression.py
+-rw-rw-rw-   0        0        0     2144 2023-07-25 06:27:06.000000 common_version-0.0.2/version/expression/cocoapods_version_expression.py
+-rw-rw-rw-   0        0        0     6942 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/composer_version_expression.py
+-rw-rw-rw-   0        0        0      626 2023-07-25 06:46:05.000000 common_version-0.0.2/version/expression/go_version_expression.py
+-rw-rw-rw-   0        0        0     2449 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/hex_version_expression.py
+-rw-rw-rw-   0        0        0     2946 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/linux_version_expression.py
+-rw-rw-rw-   0        0        0     4036 2023-07-25 06:46:07.000000 common_version-0.0.2/version/expression/maven_version_expression.py
+-rw-rw-rw-   0        0        0     6331 2023-07-25 06:46:08.000000 common_version-0.0.2/version/expression/npm_version_expression.py
+-rw-rw-rw-   0        0        0     4329 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/nuget_version_expression.py
+-rw-rw-rw-   0        0        0     1529 2023-07-25 06:46:11.000000 common_version-0.0.2/version/expression/nvd_version_expression.py
+-rw-rw-rw-   0        0        0     4465 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/other_version_expression.py
+-rw-rw-rw-   0        0        0     6270 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/pip_version_expression.py
+-rw-rw-rw-   0        0        0     3353 2023-07-25 06:29:26.000000 common_version-0.0.2/version/expression/ruby_version_expression.py
+-rw-rw-rw-   0        0        0     3970 2023-07-25 06:46:12.000000 common_version-0.0.2/version/expression/snyk_version_expression.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:56:05.321009 common_version-0.0.2/version/version_base/
+-rw-rw-rw-   0        0        0      633 2023-04-26 02:08:34.000000 common_version-0.0.2/version/version_base/__init__.py
+-rw-rw-rw-   0        0        0    33829 2023-07-25 06:33:38.000000 common_version-0.0.2/version/version_base/base_item.py
+-rw-rw-rw-   0        0        0    19296 2023-07-25 06:29:26.000000 common_version-0.0.2/version/version_base/base_version.py
+-rw-rw-rw-   0        0        0     1906 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/common_method.py
+-rw-rw-rw-   0        0        0     1839 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/composer_version.py
+-rw-rw-rw-   0        0        0     1605 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/go_version.py
+-rw-rw-rw-   0        0        0     4200 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/linux_version.py
+-rw-rw-rw-   0        0        0    11663 2023-07-25 06:33:38.000000 common_version-0.0.2/version/version_base/lj_version.py
+-rw-rw-rw-   0        0        0     2397 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/maven_version.py
+-rw-rw-rw-   0        0        0     1511 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/npm_version.py
+-rw-rw-rw-   0        0        0     5766 2023-07-25 06:30:16.000000 common_version-0.0.2/version/version_base/snyk_version.py
```

### Comparing `common_version-0.0.1/LICENSE` & `common_version-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `common_version-0.0.1/PKG-INFO` & `common_version-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_version
-Version: 0.0.1
+Version: 0.0.2
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,8 +17,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # common_version
-基于包管理器以及漏洞网站的版本表达式统一化
+
+基于包管理器以及漏洞网站的版本表达式统一化 初始化
+
+-------
+
+.. code-block:: bash
+
+    git clone https://github.com/hsc1102/common_version.git
+    cd common_version
+    pip install "flake8<3.8" bumpversion pep8-naming
+    flake8 --install-hook git
+    git config --bool flake8.strict true
+
+版本发布
+--------
+
+.. code-block:: bash
+
+    bumpversion patch
+    git push origin master --tags
+    git pull && bumpversion patch && git push origin master --tags
```

### Comparing `common_version-0.0.1/common_version.egg-info/PKG-INFO` & `common_version-0.0.2/common_version.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-version
-Version: 0.0.1
+Version: 0.0.2
 Summary: common_version
 Home-page: https://github.com/hsc1102/common_version.git
 Author: hsc
 Author-email: 1608531788@qq.com
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,8 +17,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # common_version
-基于包管理器以及漏洞网站的版本表达式统一化
+
+基于包管理器以及漏洞网站的版本表达式统一化 初始化
+
+-------
+
+.. code-block:: bash
+
+    git clone https://github.com/hsc1102/common_version.git
+    cd common_version
+    pip install "flake8<3.8" bumpversion pep8-naming
+    flake8 --install-hook git
+    git config --bool flake8.strict true
+
+版本发布
+--------
+
+.. code-block:: bash
+
+    bumpversion patch
+    git push origin master --tags
+    git pull && bumpversion patch && git push origin master --tags
```

### Comparing `common_version-0.0.1/setup.cfg` & `common_version-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6d 6d6f 6e5f 7665 7273 696f   = common_versio
 00000020: 6e0d 0a76 6572 7369 6f6e 203d 2061 7474  n..version = att
-00000030: 723a 205f 5f76 6572 7369 6f6e 5f5f 0d0a  r: __version__..
-00000040: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000050: 7468 7562 2e63 6f6d 2f68 7363 3131 3032  thub.com/hsc1102
-00000060: 2f63 6f6d 6d6f 6e5f 7665 7273 696f 6e2e  /common_version.
-00000070: 6769 740d 0a61 7574 686f 7220 3d20 6873  git..author = hs
-00000080: 630d 0a61 7574 686f 725f 656d 6169 6c20  c..author_email 
-00000090: 3d20 3136 3038 3533 3137 3838 4071 712e  = 1608531788@qq.
-000000a0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
-000000b0: 203d 2063 6f6d 6d6f 6e5f 7665 7273 696f   = common_versio
-000000c0: 6e0d 0a6c 6f6e 675f 6465 7363 7269 7074  n..long_descript
-000000d0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-00000100: 7479 7065 203d 2074 6578 742f 782d 7273  type = text/x-rs
-00000110: 740d 0a6c 6963 656e 7365 203d 2042 5344  t..license = BSD
-00000120: 2d33 2d43 6c61 7573 650d 0a63 6c61 7373  -3-Clause..class
-00000130: 6966 6965 7273 203d 200d 0a09 4465 7665  ifiers = ...Deve
-00000140: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000150: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
-00000160: 2f53 7461 626c 650d 0a09 496e 7465 6e64  /Stable...Intend
-00000170: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000180: 6576 656c 6f70 6572 730d 0a09 4c69 6365  evelopers...Lice
-00000190: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001a0: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
-000001b0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-000001c0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001d0: 7065 6e64 656e 740d 0a09 5072 6f67 7261  pendent...Progra
-000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001f0: 3a20 5079 7468 6f6e 0d0a 0950 726f 6772  : Python...Progr
-00000200: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000210: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-00000220: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000240: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 0950  :: 3 :: Only...P
-00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000270: 2033 2e36 0d0a 0950 726f 6772 616d 6d69   3.6...Programmi
-00000280: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000290: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
-000002a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002c0: 2033 2e38 0d0a 0d0a 5b6f 7074 696f 6e73   3.8....[options
-000002d0: 5d0d 0a70 7974 686f 6e5f 7265 7175 6972  ]..python_requir
-000002e0: 6573 203d 203e 3d33 2e36 0d0a 7061 636b  es = >=3.6..pack
-000002f0: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000300: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000310: 7461 203d 2074 7275 650d 0a7a 6970 5f73  ta = true..zip_s
-00000320: 6166 6520 3d20 6661 6c73 650d 0a69 6e73  afe = false..ins
-00000330: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000340: 0d0a 0972 6571 7565 7374 730d 0a0d 0a5b  ...requests....[
-00000350: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000360: 2e66 696e 645d 0d0a 6578 636c 7564 6520  .find]..exclude 
-00000370: 3d20 7465 7374 732c 7465 7374 732e 2a2c  = tests,tests.*,
-00000380: 646f 6373 2c64 6f63 732e 2a0d 0a0d 0a5b  docs,docs.*....[
-00000390: 666c 616b 6538 5d0d 0a65 7863 6c75 6465  flake8]..exclude
-000003a0: 203d 202e 7376 6e2c 4356 532c 2e62 7a72   = .svn,CVS,.bzr
-000003b0: 2c2e 6867 2c2e 6769 742c 5f5f 7079 6361  ,.hg,.git,__pyca
-000003c0: 6368 652c 2e72 6f70 6570 726f 6a65 6374  che,.ropeproject
-000003d0: 2c76 656e 762c 6d69 6772 6174 696f 6e73  ,venv,migrations
-000003e0: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
-000003f0: 6820 3d20 3131 390d 0a0d 0a5b 6973 6f72  h = 119....[isor
-00000400: 745d 0d0a 636f 6d62 696e 655f 6173 5f69  t]..combine_as_i
-00000410: 6d70 6f72 7473 203d 2074 7275 650d 0a64  mports = true..d
-00000420: 6566 6175 6c74 5f73 6563 7469 6f6e 203d  efault_section =
-00000430: 2054 4849 5244 5041 5254 590d 0a69 6e63   THIRDPARTY..inc
-00000440: 6c75 6465 5f74 7261 696c 696e 675f 636f  lude_trailing_co
-00000450: 6d6d 6120 3d20 7472 7565 0d0a 6b6e 6f77  mma = true..know
-00000460: 6e5f 6669 7273 745f 7061 7274 7920 3d20  n_first_party = 
-00000470: 636f 6d6d 6f6e 5f76 6572 7369 6f6e 0d0a  common_version..
-00000480: 6c69 6e65 5f6c 656e 6774 6820 3d20 3131  line_length = 11
-00000490: 390d 0a6d 756c 7469 5f6c 696e 655f 6f75  9..multi_line_ou
-000004a0: 7470 7574 203d 2035 0d0a 0d0a 5b65 6767  tput = 5....[egg
-000004b0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004c0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004d0: 2030 0d0a 0d0a                            0....
+00000030: 723a 2076 6572 7369 6f6e 2e5f 5f76 6572  r: version.__ver
+00000040: 7369 6f6e 5f5f 0d0a 7572 6c20 3d20 6874  sion__..url = ht
+00000050: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000060: 2f68 7363 3131 3032 2f63 6f6d 6d6f 6e5f  /hsc1102/common_
+00000070: 7665 7273 696f 6e2e 6769 740d 0a61 7574  version.git..aut
+00000080: 686f 7220 3d20 6873 630d 0a61 7574 686f  hor = hsc..autho
+00000090: 725f 656d 6169 6c20 3d20 3136 3038 3533  r_email = 160853
+000000a0: 3137 3838 4071 712e 636f 6d0d 0a64 6573  1788@qq.com..des
+000000b0: 6372 6970 7469 6f6e 203d 2063 6f6d 6d6f  cription = commo
+000000c0: 6e5f 7665 7273 696f 6e0d 0a6c 6f6e 675f  n_version..long_
+000000d0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000e0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000100: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000110: 6578 742f 782d 7273 740d 0a6c 6963 656e  ext/x-rst..licen
+00000120: 7365 203d 2042 5344 2d33 2d43 6c61 7573  se = BSD-3-Claus
+00000130: 650d 0a63 6c61 7373 6966 6965 7273 203d  e..classifiers =
+00000140: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
+00000150: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+00000160: 6f64 7563 7469 6f6e 2f53 7461 626c 650d  oduction/Stable.
+00000170: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000180: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000190: 730d 0a09 4c69 6365 6e73 6520 3a3a 204f  s...License :: O
+000001a0: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+000001b0: 5344 204c 6963 656e 7365 0d0a 094f 7065  SD License...Ope
+000001c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001d0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+000001e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000200: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000210: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000220: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000240: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+00000250: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e36 0d0a 0950  ython :: 3.6...P
+00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002a0: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
+000002b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002c0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0d0a  ython :: 3.8....
+000002d0: 5b6f 7074 696f 6e73 5d0d 0a70 7974 686f  [options]..pytho
+000002e0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+000002f0: 2e36 0d0a 7061 636b 6167 6573 203d 2066  .6..packages = f
+00000300: 696e 643a 0d0a 696e 636c 7564 655f 7061  ind:..include_pa
+00000310: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
+00000320: 650d 0a7a 6970 5f73 6166 6520 3d20 6661  e..zip_safe = fa
+00000330: 6c73 650d 0a69 6e73 7461 6c6c 5f72 6571  lse..install_req
+00000340: 7569 7265 7320 3d20 0d0a 0972 6571 7565  uires = ...reque
+00000350: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
+00000360: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000370: 6578 636c 7564 6520 3d20 7465 7374 732c  exclude = tests,
+00000380: 7465 7374 732e 2a2c 646f 6373 2c64 6f63  tests.*,docs,doc
+00000390: 732e 2a0d 0a0d 0a5b 666c 616b 6538 5d0d  s.*....[flake8].
+000003a0: 0a65 7863 6c75 6465 203d 202e 7376 6e2c  .exclude = .svn,
+000003b0: 4356 532c 2e62 7a72 2c2e 6867 2c2e 6769  CVS,.bzr,.hg,.gi
+000003c0: 742c 5f5f 7079 6361 6368 652c 2e72 6f70  t,__pycache,.rop
+000003d0: 6570 726f 6a65 6374 2c76 656e 762c 6d69  eproject,venv,mi
+000003e0: 6772 6174 696f 6e73 0d0a 6d61 782d 6c69  grations..max-li
+000003f0: 6e65 2d6c 656e 6774 6820 3d20 3131 390d  ne-length = 119.
+00000400: 0a0d 0a5b 6973 6f72 745d 0d0a 636f 6d62  ...[isort]..comb
+00000410: 696e 655f 6173 5f69 6d70 6f72 7473 203d  ine_as_imports =
+00000420: 2074 7275 650d 0a64 6566 6175 6c74 5f73   true..default_s
+00000430: 6563 7469 6f6e 203d 2054 4849 5244 5041  ection = THIRDPA
+00000440: 5254 590d 0a69 6e63 6c75 6465 5f74 7261  RTY..include_tra
+00000450: 696c 696e 675f 636f 6d6d 6120 3d20 7472  iling_comma = tr
+00000460: 7565 0d0a 6b6e 6f77 6e5f 6669 7273 745f  ue..known_first_
+00000470: 7061 7274 7920 3d20 636f 6d6d 6f6e 5f76  party = common_v
+00000480: 6572 7369 6f6e 0d0a 6c69 6e65 5f6c 656e  ersion..line_len
+00000490: 6774 6820 3d20 3131 390d 0a6d 756c 7469  gth = 119..multi
+000004a0: 5f6c 696e 655f 6f75 7470 7574 203d 2035  _line_output = 5
+000004b0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000004c0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000004d0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `common_version-0.0.1/version/__init__.py` & `common_version-0.0.2/version/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
+__version__ = "0.0.2"
+
 import enum
 
 __all__ = [
     "check_version_in_expression",
     "PackageType",
     "get_base_version",
     "is_canonical",
-    "change_to_lj_expression",
+    "change_to_expression",
+    "check_versions_in_expression",
 ]
 
-from lj_spider_core.version.expression import VersionPipExpression, VersionMavenExpression, VersionNpmExpression, \
+from version.expression import VersionPipExpression, VersionMavenExpression, VersionNpmExpression, \
     VersionNugetExpression, VersionCargoExpression, VersionGoExpression, VersionCocoExpression, VersionCExpression, \
     VersionRubyExpression, VersionComposerExpression, VersionHexExpression, VersionNvdExpression, \
     VersionSnykExpression, VersionLinuxExpression, VersionOtherExpression
-from lj_spider_core.version.version_base import LjVersion, Version, NpmVersion, GoVersion, ComposerVersion, SnykVersion
-from lj_spider_core.version.version_base.linux_version import LinuxVersion
-from lj_spider_core.version.version_base.maven_version import MavenVersion
+from version.version_base import LjVersion, Version, NpmVersion, GoVersion, ComposerVersion, SnykVersion
+from version.version_base.linux_version import LinuxVersion
+from version.version_base.maven_version import MavenVersion
 
 
 class PackageType(enum.Enum):
     Base = "base"
     Pip = "pip"
     Maven = "maven"
     Npm = "npm"
@@ -227,15 +230,15 @@
     assert class_package_type in Package_CLASSES
     if isinstance(version, Version):
         return version.is_canonical(version)
     else:
         return Package_CLASSES[class_package_type](version, package_type.lower()).is_canonical(version)
 
 
-def change_to_lj_expression(package_type: str, version_expression):
+def change_to_expression(package_type: str, version_expression):
     """
     组件版本表达式转换为棱镜版本表达式
     :param package_type: 包管理器类型
     :param version_expression: 组件版本表达式
     :return: 棱镜版本表达式
     """
     expression_type = None
@@ -243,15 +246,15 @@
         package_type = MapPackageType.get_value_by_key(package_type)
         if package_type.lower() in PackageType.values():
             expression_type = PackageType(package_type.lower())
         else:
             expression_type = PackageType.Other
             package_type = "other"
     assert expression_type in Expression_CLASSES
-    return Expression_CLASSES[expression_type].change_to_lj_expression(
+    return Expression_CLASSES[expression_type].change_to_expression(
         package_type.lower(), version_expression
     )
 
 
 def sort_versions(versions, remove_not_final, package_type="snyk"):
     """
     版本大小比较
@@ -309,15 +312,15 @@
         if package_type.lower() in PackageType.values():
             class_package_type = PackageType(package_type.lower())
         else:
             class_package_type = PackageType.Other
             package_type = "other"
     assert class_package_type in LJ_VERSION_CLASS
     assert isinstance(versions, list)
-    final_item = change_to_lj_expression(package_type, version_expression)
+    final_item = change_to_expression(package_type, version_expression)
     final_list = []
     not_in_list = []
     for i in versions:
         part_bool = LJ_VERSION_CLASS[class_package_type](package_type=package_type.lower(),
                                                          version_str=i).check_version_in_expression(
             final_item)
         if part_bool:
@@ -345,15 +348,15 @@
         if package_type.lower() in PackageType.values():
             class_package_type = PackageType(package_type.lower())
         else:
             class_package_type = PackageType.Other
             package_type = "other"
     assert class_package_type in LJ_VERSION_CLASS
     assert isinstance(versions, list)
-    final_item = change_to_lj_expression(package_type, version_expression)
+    final_item = change_to_expression(package_type, version_expression)
     final_list = []
     for i in versions:
         part_bool = LJ_VERSION_CLASS[class_package_type](package_type=package_type.lower(),
                                                          version_str=i).check_version_in_expression(
             final_item)
         if part_bool:
             final_list.append(i)
```

### Comparing `common_version-0.0.1/version/base.py` & `common_version-0.0.2/version/base.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.1/version/exceptions.py` & `common_version-0.0.2/version/exceptions.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.1/version/expression/__init__.py` & `common_version-0.0.2/version/expression/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,29 @@
 # -*- coding: utf-8 -*-
-from lj_spider_core.version.expression.base_method import (
-    arrangement_version,
-    dest_change_source,
-    find_str_index,
-    handle_version_change_source,
-    handle_version_comma,
-    handle_version_compatible,
-    handle_version_or,
-)
-from lj_spider_core.version.expression.c_version_expression import (
-    VersionCExpression,
-)
-from lj_spider_core.version.expression.cargo_version_expression import (
-    VersionCargoExpression,
-)
-from lj_spider_core.version.expression.cocoapods_version_expression import (
-    VersionCocoExpression,
-)
-from lj_spider_core.version.expression.composer_version_expression import (
-    VersionComposerExpression,
-)
-from lj_spider_core.version.expression.go_version_expression import (
-    VersionGoExpression,
-)
-from lj_spider_core.version.expression.hex_version_expression import (
-    VersionHexExpression,
-)
-from lj_spider_core.version.expression.linux_version_expression import VersionLinuxExpression
-from lj_spider_core.version.expression.maven_version_expression import (
-    VersionMavenExpression,
-)
-from lj_spider_core.version.expression.npm_version_expression import (
-    VersionNpmExpression,
-)
-from lj_spider_core.version.expression.nuget_version_expression import (
-    VersionNugetExpression,
-)
-from lj_spider_core.version.expression.nvd_version_expression import (
-    VersionNvdExpression,
-)
-from lj_spider_core.version.expression.other_version_expression import VersionOtherExpression
-from lj_spider_core.version.expression.pip_version_expression import (
-    VersionPipExpression,
-)
-from lj_spider_core.version.expression.ruby_version_expression import (
-    VersionRubyExpression,
-)
+# flake8:noqa
+from version.expression.base_method import arrangement_version, \
+    handle_version_change_source, handle_version_compatible, dest_change_source, \
+    handle_version_comma, find_str_index, handle_version_or
+from version.expression.c_version_expression import VersionCExpression
+from version.expression.cargo_version_expression import VersionCargoExpression
+from version.expression.cocoapods_version_expression import VersionCocoExpression
+from version.expression.composer_version_expression import VersionComposerExpression
+from version.expression.go_version_expression import VersionGoExpression
+from version.expression.hex_version_expression import VersionHexExpression
+from version.expression.linux_version_expression import VersionLinuxExpression
+from version.expression.maven_version_expression import VersionMavenExpression
+from version.expression.npm_version_expression import VersionNpmExpression
+from version.expression.nuget_version_expression import VersionNugetExpression
+from version.expression.nvd_version_expression import VersionNvdExpression
+from version.expression.other_version_expression import VersionOtherExpression
+from version.expression.pip_version_expression import VersionPipExpression
+from version.expression.ruby_version_expression import VersionRubyExpression
+from version.expression.snyk_version_expression import VersionSnykExpression
 
-from lj_spider_core.version.expression.snyk_version_expression import (
-    VersionSnykExpression,
-)
-
-__all__ = [
+__all__ = {
     "arrangement_version",
     "handle_version_change_source",
     "handle_version_compatible",
     "dest_change_source",
     "handle_version_comma",
     "find_str_index",
     "handle_version_or",
@@ -63,16 +31,15 @@
     "VersionRubyExpression",
     "VersionPipExpression",
     "VersionNvdExpression",
     "VersionNugetExpression",
     "VersionNpmExpression",
     "VersionMavenExpression",
     "VersionHexExpression",
-    "VersionMavenExpression",
     "VersionGoExpression",
     "VersionComposerExpression",
     "VersionCargoExpression",
     "VersionCocoExpression",
     "VersionCExpression",
     "VersionLinuxExpression",
     "VersionOtherExpression",
-]
+}
```

### Comparing `common_version-0.0.1/version/expression/base_method.py` & `common_version-0.0.2/version/expression/base_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import re
 
-from lj_spider_core.version.version_base import VersionSort
+from version.version_base import VersionSort
 
 sort_values = []
 for i in VersionSort.__members__.values():
     sort_values.append(i.values[0])
 
 
 def fun(mat):
@@ -39,15 +39,15 @@
 def arrangement_version(
         version,
         package_type,
         is_del_identifier=False,
         is_format=True,
         is_del_brackets=False,
 ):
-    from lj_spider_core.version import get_base_version
+    from version import get_base_version
     """
     版本号格式化
     is_del_identifier 是否删除其他标识符  例如：> < = !
     :param is_format:
     :param package_type: 包类型
     :param version:
     :param is_del_identifier:
@@ -377,15 +377,15 @@
         elif pos == -1 and previous_pos == 0:
             if version_dest[previous_pos:]:
                 version_dest_list.append(version_dest[previous_pos:])
     return version_dest_list
 
 
 # def compare_version_size(left_version, right_version, package_type=None):
-#     from lj_spider_core.version.version_base import Version
+#     from version.version_base import Version
 #     """
 #     比较两个版本的大小
 #         1 大于
 #         0 等于
 #         -1 小于
 #     :param left_version:左边版本
 #     :param right_version:右边版本
@@ -417,16 +417,16 @@
 #         flag_num = 1
 #     if less_flag and not greater_flag:
 #         flag_num = -1
 #     return flag_num
 
 
 def handle_version_compatible(version_dest, package_type):
-    from lj_spider_core.version.version_base import Item, Version
-    from lj_spider_core.version import PackageType
+    from version.version_base import Item, Version
+    from version import PackageType
     """
     此函数用于处理   获取大于当前版本的最小版本
     :param package_type:包类型
     :param version_dest: 版本表达式
     :return:Item()
     """
     if package_type == PackageType.Npm.value:
@@ -495,15 +495,15 @@
         version_item = Item(
             left_open=True, left=version_dest, right_open=False, right=max_version
         )
     return version_item
 
 
 def dest_change_source(version_dest):
-    from lj_spider_core.version.version_base import Item
+    from version.version_base import Item
 
     """
     大于、大于等于、小于、小于等于逻辑范围
     :param package_type:
     :param version_dest:
     :return:
     """
@@ -554,15 +554,15 @@
                 version[msg_index + len(msg):], msg
             )
     else:
         return version
 
 
 def handle_version_change_source(version_dest, package_type):
-    from lj_spider_core.version.version_base import Version
+    from version.version_base import Version
 
     """
     小于等于逻辑、大于等于逻辑、大于逻辑、小于逻辑
     :param package_type:
     :param version_dest:
     :return:
     """
@@ -605,15 +605,15 @@
         right_open = True
     elif ")" in version:
         right_open = False
     return left_open, right_open
 
 
 def get_cut_version_item(left_open, right_open, format_version, is_left=True):
-    from lj_spider_core.version.version_base import Item, Version
+    from version.version_base import Item, Version
 
     if left_open is None:
         if isinstance(format_version, Version):
             right = format_version.new_version
         else:
             right = format_version
         final_item = Item(
@@ -635,30 +635,30 @@
             final_item = Item(
                 left_open=left_open, left="", right_open=right_open, right=left
             )
     return final_item
 
 
 def cut_not_in(left_version, right_version, package_type):
-    from lj_spider_core.version.version_base import Item
-    from lj_spider_core.version import get_base_version
+    from version.version_base import Item
+    from version import get_base_version
     left_item = Item(valid=False)
     right_item = Item(valid=False)
     if len(left_version) > 1:
         format_left_version = get_base_version(package_type, left_version[1:])
         if len(right_version) == 1:
             final_version = left_version + "," + right_version
         elif len(right_version) > 1:
             final_version = left_version + ",]"
         else:
             final_version = left_version
         left_open, right_open = find_left_or_right_identifier(final_version)
         left_item = get_cut_version_item(left_open, right_open, format_left_version)
     if len(right_version) > 1:
-        # format_right_version = change_to_lj_expression(package_type, right_version[:-1]).get_value()
+        # format_right_version = change_to_expression(package_type, right_version[:-1]).get_value()
         format_right_version = get_base_version(package_type, right_version[:-1])
         if len(left_version) == 1:
             final_version = left_version + "," + right_version
         elif len(left_version) > 1:
             final_version = "[," + right_version
         else:
             final_version = right_version
@@ -681,15 +681,15 @@
             new_item = left_item
         else:
             new_item = right_item
     return new_item
 
 
 def cut_left_and_right_dest(version_dest_list, package_type):
-    from lj_spider_core.version.version_base import ItemGroup
+    from version.version_base import ItemGroup
     """
     比较大小取交集
     仅适用与 ['>1','<2]此种情况
     :param version_dest_list:
     :return:
     """
     left_version = version_dest_list[0].replace(" ", "")
@@ -701,15 +701,15 @@
         left_item = handle_version_change_source(left_version, package_type)
         right_item = handle_version_change_source(right_version, package_type)
         new_item = ItemGroup(left_item, right_item, is_or=False).merge()
     return new_item
 
 
 def handle_version_or(version_dest, package_type):
-    from lj_spider_core.version.version_base import Item, Version
+    from version.version_base import Item, Version
 
     """
     :param version_dest:
     :return:
     """
     left_open, right_open = find_left_or_right_identifier(version_dest)
     new_version_dest = arrangement_version(
@@ -725,16 +725,16 @@
         version_item = Item(
             left_open=True, right_open=right_open, right=new_version_dest, left=""
         )
     return version_item
 
 
 def handle_version_comma(version_dest, package_type):
-    from lj_spider_core.version.version_base import Item
-    from lj_spider_core.version import PackageType
+    from version.version_base import Item
+    from version import PackageType
     """
     比较左右大小 取交集
     :param package_type:
     :param version_dest:
     :return:
     """
     version_dest = version_dest.strip(" ")
@@ -746,15 +746,15 @@
         versions = version_dest.split(",")
     if versions:
         new_item = cut_left_and_right_dest(versions, package_type)
     return new_item
 
 
 def get_equal_item(version_expression, package_type, is_del_brackets=False):
-    from lj_spider_core.version.version_base import Version, Item
+    from version.version_base import Version, Item
 
     format_version_dest = arrangement_version(
         version_expression, package_type, is_del_identifier=True, is_del_brackets=is_del_brackets
     )
     if isinstance(format_version_dest, Version):
         if format_version_dest.new_version:
             format_version = format_version_dest.new_version
```

### Comparing `common_version-0.0.1/version/expression/c_version_expression.py` & `common_version-0.0.2/version/expression/c_version_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import re
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import chinese_to_english_version, handle_version_or, \
+from version.expression.base import VersionExpression
+from version.expression.base_method import chinese_to_english_version, handle_version_or, \
     handle_version_compatible
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionCExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
+    def change_to_expression(self, package_type, version_expression):
         """
-        将表达式改变为棱镜表达式
+        将表达式改变为通用版本表达式
         :param package_type: 包类型
         :param version_expression: 各组件版本表达式
         :return:
         """
         version_expression = version_expression.replace('[', "")
         version_expression = version_expression.replace(']', "")
         version_expression = chinese_to_english_version(version_expression)
```

### Comparing `common_version-0.0.1/version/expression/cargo_version_expression.py` & `common_version-0.0.2/version/expression/cargo_version_expression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import get_equal_item, chinese_to_english_version, handle_version_or
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.expression.base import VersionExpression
+from version.expression.base_method import get_equal_item, chinese_to_english_version, handle_version_or
+from version.version_base import Item, ItemGroup
 
 
 class VersionCargoExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
+    def change_to_expression(self, package_type, version_expression):
         """
-        将表达式改变为棱镜表达式
+        将表达式改变为通用版本表达式
         :param package_type: 包类型
         :param version_expression: 各组件版本表达式
         :return:
         """
         version_expression = chinese_to_english_version(version_expression)
         if ',' in version_expression:
             versions = version_expression.split(",")
@@ -25,15 +25,15 @@
         else:
             version_item = self.handle_cargo_compare(version_expression, package_type)
         if isinstance(version_item, ItemGroup):
             version_item = version_item.merge()
         return version_item
 
     def handle_cargo_compare(self, version_expression, package_type):
-        from lj_spider_core.version.expression import (
+        from version.expression import (
             handle_version_compatible,
         )
         if "~" in version_expression:
             version_item = handle_version_compatible(version_expression, package_type)
         elif "*" in version_expression:
             if "*" != version_expression.replace(" ", ""):
                 version_item = handle_version_compatible(
```

### Comparing `common_version-0.0.1/version/expression/cocoapods_version_expression.py` & `common_version-0.0.2/version/expression/cocoapods_version_expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import chinese_to_english_version
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.expression.base import VersionExpression
+from version.expression.base_method import chinese_to_english_version
+from version.version_base import Item, ItemGroup
 
 
 class VersionCocoExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-
+    def change_to_expression(self, package_type, version_expression):
         """
-        将表达式改变为棱镜表达式
+        将表达式改变为通用版本表达式
         :param package_type: 包类型
         :param version_expression: 各组件版本表达式
         :return:
         """
         version_expression = chinese_to_english_version(version_expression)
         if ',' in version_expression:
             versions = version_expression.split(",")
@@ -26,15 +25,15 @@
         else:
             version_item = self.handle_cocoapods_compare(version_expression, package_type)
         if isinstance(version_item, ItemGroup):
             version_item = version_item.merge()
         return version_item
 
     def handle_cocoapods_compare(self, version_expression, package_type):
-        from lj_spider_core.version.expression import (
+        from version.expression import (
             dest_change_source,
             handle_version_compatible,
         )
         if "~>" in version_expression:
             version_item = handle_version_compatible(version_expression, package_type)
         elif ">" in version_expression or "<" in version_expression:
             version_item = dest_change_source(version_expression)
```

### Comparing `common_version-0.0.1/version/expression/composer_version_expression.py` & `common_version-0.0.2/version/expression/composer_version_expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import chinese_to_english_version
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.exceptions import VersionDestError
+from version.expression.base import VersionExpression
+from version.expression.base_method import chinese_to_english_version
+from version.version_base import Item, ItemGroup
 
 
 class VersionComposerExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        from lj_spider_core.version.expression import find_str_index
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param pacage_type: 组件类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+        from version.expression import find_str_index
+
         version_expression = chinese_to_english_version(version_expression)
         version_dest = find_str_index(version_expression, " ")
         version_dest = version_dest.replace("||", "|")
         if "|" in version_dest:
             version_dest_list = version_dest.split("|")
             items = []
             for version in version_dest_list:
@@ -40,16 +34,16 @@
         else:
             version_item = self.handle_composer_compare(version_dest, package_type)
         if isinstance(version_item, ItemGroup):
             version_item = version_item.merge()
         return version_item
 
     def handle_composer_compare(self, version_dest, package_type):
-        from lj_spider_core.version.version_base import Version
-        from lj_spider_core.version.expression import (
+        from version.version_base import Version
+        from version.expression import (
             arrangement_version,
             handle_version_compatible,
             handle_version_or,
         )
         version_dest = version_dest.lower()
 
         if " as" in version_dest:
```

### Comparing `common_version-0.0.1/version/expression/hex_version_expression.py` & `common_version-0.0.2/version/expression/hex_version_expression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     handle_version_compatible,
     chinese_to_english_version, handle_version_or,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionHexExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+
         version_expression = chinese_to_english_version(version_expression)
         version_item = Item(valid=False)
         if "and" in version_expression or "or" in version_expression:
             # todo 暂时未考虑一个表达式中既有and又有or的情况
             if "and" in version_expression:
                 version_dest_list = version_expression.split("and")
                 items = []
```

### Comparing `common_version-0.0.1/version/expression/linux_version_expression.py` & `common_version-0.0.2/version/expression/linux_version_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # -*- coding: utf-8 -*-
 import re
 from abc import ABC
 
-from lj_spider_core.version.expression import handle_version_change_source
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.expression import handle_version_change_source
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     cut_left_and_right_dest, get_equal_item, chinese_to_english_version,
     # handle_version_compatible,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionLinuxExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+
         version_expression = chinese_to_english_version(version_expression)
         version_expression = re.sub(r"[,<>=&|\^~]+ *", lambda matched: self.func(matched), version_expression)
         if "||" in version_expression:
             versions = version_expression.split("||")
             items = []
             for version in versions:
                 part_item = self.handle_linux_compare(version, package_type)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `common_version-0.0.1/version/expression/maven_version_expression.py` & `common_version-0.0.2/version/expression/maven_version_expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     cut_left_and_right_dest,
     get_equal_item,
     chinese_to_english_version,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionMavenExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
         version_expression = chinese_to_english_version(version_expression)
         version_expression = version_expression.replace(" ", "")
         version_expression = version_expression.replace(")(", ")&(")
         version_expression = version_expression.replace("][", "]&[")
         version_expression = version_expression.replace("](", "]&(")
         version_expression = version_expression.replace(")[", ")&[")
         version_expression = version_expression.replace("),[", ")||[")
```

### Comparing `common_version-0.0.1/version/expression/npm_version_expression.py` & `common_version-0.0.2/version/expression/npm_version_expression.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # -*- coding: utf-8 -*-
 import re
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.exceptions import VersionDestError
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     arrangement_version,
     # find_str_index,
     handle_version_comma,
     handle_version_compatible,
     handle_version_or,
     chinese_to_english_version,
     # fun
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionNpmExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param pacage_type: 组件类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
         version_expression = chinese_to_english_version(version_expression)
         version_dest = re.sub(r"[,<>=&|\^~]+ *", lambda matched: self.func(matched), version_expression)
         # version_dest = re.sub(r'([><=\^~][><=\^~]* *\d)', lambda matched: fun(matched), version_expression)
         # version_dest = find_str_index(version_expression, " ")
         if "||" in version_dest or "|" in version_dest:
             version_dest_list = []
             if "||" in version_dest:
@@ -51,15 +44,15 @@
         else:
             version_item = self.handle_npm_compare(version_dest, package_type)
         if isinstance(version_item, ItemGroup):
             version_item = version_item.merge()
         return version_item
 
     def handle_npm_compare(self, version_dest, package_type):
-        from lj_spider_core.version.version_base import Version
+        from version.version_base import Version
         if version_dest:
             if version_dest[0] == " ":
                 version_dest = version_dest[1:]
             if version_dest[-1] == " ":
                 version_dest = version_dest[0:-1]
         if "~" in version_dest or (".x" in version_dest and "/" not in version_dest):
             if "-" in version_dest:
```

### Comparing `common_version-0.0.1/version/expression/nuget_version_expression.py` & `common_version-0.0.2/version/expression/nuget_version_expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.exceptions import VersionDestError
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     arrangement_version,
     find_left_or_right_identifier,
     handle_version_comma, get_equal_item, cut_left_and_right_dest, handle_version_change_source,
     chinese_to_english_version, handle_version_compatible,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base import Item, ItemGroup
+from version.version_base.base_version import Version
 
 
 class VersionNugetExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+
         version_expression = chinese_to_english_version(version_expression)
         if version_expression and version_expression != "-1":
             version_item = self.handle_nuget_compare(version_expression, package_type)
         else:
             version_expression = version_expression.replace(" ", "")
             if version_expression != "-1":
                 raise VersionDestError(version_expression + "version_expression格式无效")
```

### Comparing `common_version-0.0.1/version/expression/nvd_version_expression.py` & `common_version-0.0.2/version/expression/nvd_version_expression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import get_equal_item, chinese_to_english_version
-from lj_spider_core.version.version_base import ItemGroup, Item
+from version.expression.base import VersionExpression
+from version.expression.base_method import get_equal_item, chinese_to_english_version
+from version.version_base import ItemGroup, Item
 
 
 class VersionNvdExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
         version_expression = chinese_to_english_version(version_expression)
         if "||" in version_expression:
             version_expressions = version_expression.split("||")
             items = []
             for version in version_expressions:
                 part_item = get_equal_item(version, package_type, is_del_brackets=True)
                 items.append(part_item)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `common_version-0.0.1/version/expression/other_version_expression.py` & `common_version-0.0.2/version/expression/other_version_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # -*- coding: utf-8 -*-
 import re
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression import handle_version_change_source
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.exceptions import VersionDestError
+from version.expression import handle_version_change_source
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     cut_left_and_right_dest,
     chinese_to_english_version, handle_version_compatible, arrangement_version,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionOtherExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+
         version_expression = chinese_to_english_version(version_expression)
         version_expression = re.sub(r"[,<>=&|\^~]+ *", lambda matched: self.func(matched), version_expression)
         # version_expression = re.sub(r'([><=\^~][><=\^~]* *\d)', lambda matched: fun(matched), version_expression)
         if "|" in version_expression:
             versions = version_expression.split("|")
             items = []
             for version in versions:
@@ -50,15 +45,15 @@
                     version_expression, package_type
                 )
         if isinstance(version_item, ItemGroup):
             version_item = version_item.merge()
         return version_item
 
     def handle_other_compare(self, version, package_type):
-        from lj_spider_core.version.version_base import Version
+        from version.version_base import Version
         if "[" in version or "]" in version or "(" in version or ")" in version:
             version_dest_list = version.split(",")
             version_item = cut_left_and_right_dest(version_dest_list, package_type)
         elif "!=" in version:
             new_version_dest = arrangement_version(
                 version, package_type, is_del_identifier=True
             )
```

### Comparing `common_version-0.0.1/version/expression/pip_version_expression.py` & `common_version-0.0.2/version/expression/pip_version_expression.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.exceptions import VersionDestError
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     arrangement_version,
     handle_version_change_source,
     handle_version_compatible, get_equal_item, chinese_to_english_version, handle_version_or,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base import Item, ItemGroup
+from version.version_base.base_version import Version
 
 
 class VersionPipExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
+        
         version_expression = chinese_to_english_version(version_expression)
         if version_expression:
             version_expression = version_expression.replace(" ", "")
         if "," in version_expression:
             version_dest_list = version_expression.split(",")
             items = []
             for version in version_dest_list:
@@ -110,15 +105,15 @@
                 left_open=True,
                 right_open=False,
                 left=format_version,
                 right=max_version,
             )
 
     def handle_pip_matching(self, package_type, version_dest):
-        from lj_spider_core.version.version_base import Version
+        from version.version_base import Version
 
         """
         不带有*的 != 和==逻辑
         处理==
             例1：==1.1.1  版本号必须与1.1.1完全相等才算作匹配
             例2：==1.1     版本号为1.1.0或1.1都算作与之匹配
             例3：==1.1.*   匹配前缀与1.1.相等的版本号，包括：1.1.post1
```

### Comparing `common_version-0.0.1/version/expression/ruby_version_expression.py` & `common_version-0.0.2/version/expression/ruby_version_expression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # -*- coding: utf-8 -*-
 from abc import ABC
 
-from lj_spider_core.version.exceptions import VersionDestError
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.exceptions import VersionDestError
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     arrangement_version,
     handle_version_compatible,
     # get_equal_item,
     chinese_to_english_version, handle_version_or,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionRubyExpression(VersionExpression, ABC):
-    def change_to_lj_expression(self, package_type, version_expression):
+    def change_to_expression(self, package_type, version_expression):
 
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
         version_expression = chinese_to_english_version(version_expression)
         version_expression = version_expression.replace(" ", "")
         if "," in version_expression:
             versions = version_expression.split(",")
             items = []
             for version in versions:
                 part_version_item = self.handle_ruby_compare(version, package_type)
@@ -53,15 +47,15 @@
             if version_expression and "*" != version_expression:
                 version_item = Item(left_open=True, left=version_expression, right_open=True, right=version_expression)
             else:
                 version_item = Item(left_open=True, right_open=True, left="", right="")
         return version_item
 
     def handle_ruby_matching(self, version_dest, package_type):
-        from lj_spider_core.version.version_base import Version
+        from version.version_base import Version
         """
          != 逻辑   例如  !=1.1.1   --->   [,1.1.1)||(1.1.1,]
         :param version_dest:
         :return:
         """
         format_version_dest = arrangement_version(
             version_dest, package_type, is_del_identifier=True
```

### Comparing `common_version-0.0.1/version/expression/snyk_version_expression.py` & `common_version-0.0.2/version/expression/snyk_version_expression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # -*- coding: utf-8 -*-
 import re
 from abc import ABC
 
-from lj_spider_core.version.expression import handle_version_change_source
-from lj_spider_core.version.expression.base import VersionExpression
-from lj_spider_core.version.expression.base_method import (
+from version.expression import handle_version_change_source
+from version.expression.base import VersionExpression
+from version.expression.base_method import (
     cut_left_and_right_dest, get_equal_item, chinese_to_english_version, handle_version_compatible, handle_version_or,
 )
-from lj_spider_core.version.version_base import Item, ItemGroup
+from version.version_base import Item, ItemGroup
 
 
 class VersionSnykExpression(VersionExpression, ABC):
 
-    def change_to_lj_expression(self, package_type, version_expression):
-        """
-        将表达式改变为棱镜表达式
-        :param package_type: 包类型
-        :param version_expression: 各组件版本表达式
-        :return:
-        """
+    def change_to_expression(self, package_type, version_expression):
         # version_expression = re.sub(r'([><=\^~][><=\^~]* +)', lambda matched: fun(matched), version_expression)
         version_expression = chinese_to_english_version(version_expression)
         version_expression = re.sub(r"[,<>=&|\^~]+ *", lambda matched: self.func(matched), version_expression)
         if "||" in version_expression:
             versions = version_expression.split("||")
             items = []
             for version in versions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `common_version-0.0.1/version/version_base/__init__.py` & `common_version-0.0.2/version/version_base/__init__.py`

 * *Files identical despite different names*

### Comparing `common_version-0.0.1/version/version_base/base_item.py` & `common_version-0.0.2/version/version_base/base_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import copy
 
 
-# from lj_spider_core.version import PackageType
+# from version import PackageType
 
 
 class Line:
     def __init__(self, start, end):
         self.start = start
         self.end = end
 
@@ -16,15 +16,15 @@
         if not start:
             start = "0"
         if not end:
             end = "9999999"
         return f"{start},{end}"
 
     def in_line(self, spot, is_end=True):
-        from lj_spider_core.version import get_base_version
+        from version import get_base_version
         """
         判断是否在范围内
         :param spot:
         :return:
         """
         is_in_line = False
         start = self.start
@@ -90,29 +90,29 @@
         elif part_right_flag == 0 and self.right_open:
             right_flag = True
         else:
             right_flag = False
         return right_flag
 
     def is_in_version_item(self, other, package_type):
-        from lj_spider_core.version.version_base import Equal_Not_Compare_Type, Equal_Or_Compare_Type
-        from lj_spider_core.version import get_base_version, change_to_lj_expression
+        from version.version_base import Equal_Not_Compare_Type, Equal_Or_Compare_Type
+        from version import get_base_version, change_to_expression
         if self.left == self.right and package_type in Equal_Not_Compare_Type:
             if self.left == other or self.right == other:
                 return True
             else:
                 return False
         elif self.left == self.right and package_type in Equal_Or_Compare_Type:
             if self.right == other:
                 final_flag = True
                 return final_flag
             else:
                 try:
                     if package_type != "cargo":
-                        left_version = change_to_lj_expression(package_type=package_type, version_expression=other)
+                        left_version = change_to_expression(package_type=package_type, version_expression=other)
                     else:
                         left_version_obj = get_base_version(package_type=package_type, version_name=other)
                         left_version = Item(left_open=True, right_open=True, left=left_version_obj.new_version,
                                             right=left_version_obj.new_version)
                     if left_version.left == left_version.right:
                         version1 = get_base_version(package_type=package_type, version_name=other)
                         flag = version1.__cmp__(self.left)
@@ -141,15 +141,15 @@
             right_flag = self.compare_right(part_right_flag)
             return left_flag and right_flag
 
     def is_valid(self):
         return self.valid
 
     def set_valid(self, valid):
-        from lj_spider_core.version import get_base_version
+        from version import get_base_version
         valid = valid
         if self.right and self.left:
             if self.left != self.right:
                 is_intersect = get_base_version(version_name=self.left).__cmp__(self.right)
                 if is_intersect > 0:
                     valid = False
         return valid
@@ -207,15 +207,15 @@
         """
         if isinstance(other, ItemGroup):
             return other.merge_or(self)
         new_item = self.is_intersect(other, is_or=True)
         return new_item
 
     def sort_match_line(self, first_line, other_line):
-        from lj_spider_core.version import sort_versions
+        from version import sort_versions
         if not first_line.start:
             first_line.start = "0"
         if not other_line.start:
             other_line.start = "0"
         if not first_line.end:
             first_line.end = "99999999"
         if not other_line.end:
@@ -610,15 +610,15 @@
     def __eq__(self, other):
         return self.__cmp__(other) == 0
 
     def __lt__(self, other):
         return self.__cmp__(other) < 0
 
     def to_compare(self, one_version, two_version):
-        from lj_spider_core.version import get_base_version
+        from version import get_base_version
         flag = 1
         is_compare = True
         try:
             one_version_obj = get_base_version(package_type="snyk", version_name=one_version)
             two_version_obj = get_base_version(package_type="snyk", version_name=two_version)
             flag = one_version_obj.__cmp__(two_version_obj)
         except Exception:
@@ -759,15 +759,15 @@
                 ret = ret.merge_and(item)
                 if not ret.is_valid():
                     return Item(valid=False)
         return ret.merge_finish() if isinstance(ret, ItemGroup) else ret
 
     def merge_finish(self):
         assert self.is_or
-        from lj_spider_core.version import get_base_version, version_compare
+        from version import get_base_version, version_compare
         for item in self.items:
             assert isinstance(item, Item)
         new_items = sorted(self.items)
         ret = []
         last = new_items[0]
         for i in range(1, len(new_items)):
             right = last.right
```

### Comparing `common_version-0.0.1/version/version_base/base_version.py` & `common_version-0.0.2/version/version_base/base_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import copy
 import enum
 import re
 
 from aenum import MultiValueEnum
 
-from lj_spider_core.version.version_base.common_method import is_match
+from version.version_base.common_method import is_match
 
 
 class VersionSort(MultiValueEnum):
     DEV = "dev", 10
     X_DEV = "x-dev", 11
     A = "a", 20
     B = "b", 30
@@ -190,24 +190,24 @@
     def __eq__(self, other):
         return self.__cmp__(other) == 0
 
     def __lt__(self, other):
         return self.__cmp__(other) < 0
 
     def __cmp__(self, other):
-        from lj_spider_core.version import get_base_version
+        from version import get_base_version
         if isinstance(other, str):
             other = get_base_version(self.package_type, other)
         other.cmp_versions = other.format_cmp_version(self)
         self.cmp_versions = self.format_cmp_version(other)
         flag = self.compare_to_versions(other)
         return flag if self.cmp_versions else 2
 
     def compare_to_versions(self, other):
-        from lj_spider_core.version.expression.base_method import supplement_zero, compare_str_change_list
+        from version.expression.base_method import supplement_zero, compare_str_change_list
         equal_num = 0
         version_source_list, version_dest_list = supplement_zero(
             self.cmp_versions, other.cmp_versions
         )
         version_source_list = [i if i != '0' else 0 for i in version_source_list]
         version_dest_list = [i if i != '0' else 0 for i in version_dest_list]
         flag = 0
@@ -264,15 +264,15 @@
                 version = self.format_release(version)
                 version = self.format_post(version)
                 version = self.format_dev(version)
                 version = self.format_del(version)
         return version
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/common_method.py` & `common_version-0.0.2/version/version_base/common_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import re
 
 
 # def sort_version(version_list, package_type=None):
-#     from lj_spider_core.version import Version
+#     from version import Version
 #     """
 #     快速排序
 #     version_list  版本列表   排序  从小到大
 #     :param version_list:
 #     :param package_type:
 #     :return:
 #     """
```

### Comparing `common_version-0.0.1/version/version_base/composer_version.py` & `common_version-0.0.2/version/version_base/composer_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 @Project:lj_spider_core
 @File:composer_version.py
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/9/21 16:01
 @function：
 """
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base.base_version import Version
 
 
 class ComposerVersion(Version):
 
     def __init__(self, version, package_type="composer", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/go_version.py` & `common_version-0.0.2/version/version_base/go_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 @Project:lj_spider_core
 @File:snyk_version.py
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/9/21 14:26
 @function：
 """
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base.base_version import Version
 
 
 class GoVersion(Version):
 
     def __init__(self, version, package_type="go", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
     def format_version(self):
-        # from lj_spider_core.version.expression import arrangement_version
+        # from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/linux_version.py` & `common_version-0.0.2/version/version_base/linux_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/10/25 15:17
 @function：
 """
 import re
 
-from lj_spider_core.version.version_base.snyk_version import SnykVersion
+from version.version_base.snyk_version import SnykVersion
 
 
 class LinuxVersion(SnykVersion):
     def __init__(self, version, package_type="linux", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/lj_version.py` & `common_version-0.0.2/version/version_base/lj_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import enum
 
-from lj_spider_core.version.version_base import ItemGroup, Item
+from version.version_base import ItemGroup, Item
 
 
 class CompareType(enum.Enum):
     COMPARE = "compare"
     EQUAL = "=="
 
 
@@ -23,26 +23,26 @@
         self.version_str = version_str
         self.format_version = ""
         self.package_type = package_type
         self.format_version_obj = self.format_compare_version()
         self.format_version_list = list()
 
     def format_compare_version(self):
-        from lj_spider_core.version import (
+        from version import (
             get_base_version
         )
         version_obj = get_base_version(self.package_type, self.version_str)
         if version_obj.new_version:
             self.format_version = version_obj.new_version
         else:
             self.format_version = version_obj.old_version
         return version_obj
 
     def version_compare(self, version1, version2):
-        from lj_spider_core.version import (
+        from version import (
             get_base_version
         )
         version1_obj = get_base_version(self.package_type, version1)
         version2_obj = get_base_version(self.package_type, version2)
         return version1_obj.__cmp__(version2_obj)
 
     def format_version_lj_list(self, lj_expression):
@@ -54,16 +54,16 @@
         """
         if "||" in lj_expression:
             self.format_version_list = lj_expression.split("||")
         else:
             self.format_version_list.append(lj_expression)
 
     # def compare_version(self, compare_type, version_dest):
-    #     from lj_spider_core.version.version_base import Version
-    #     from lj_spider_core.version import version_compare
+    #     from version.version_base import Version
+    #     from version import version_compare
     #     if isinstance(compare_type, str):
     #         compare_type = CompareType(compare_type)
     #     assert compare_type in CompareType
     #     flag = None
     #     if CompareType.EQUAL == compare_type:
     #         if version_dest == self.version_str:
     #             flag = 0
@@ -74,16 +74,16 @@
     #                                    )
     #         else:
     #             if version_dest == self.version_str:
     #                 flag = 0
     #     return flag
     #
     # def compare_version_equal(self, format_version1, format_version2):
-    #     from lj_spider_core.version import is_canonical
-    #     from lj_spider_core.version.expression.base_method import (
+    #     from version import is_canonical
+    #     from version.expression.base_method import (
     #         compare_version_size,
     #     )
     #     if is_canonical(self.package_type, format_version2.new_version) and is_canonical(
     #             self.package_type, format_version1.new_version,
     #     ):
     #         flag = compare_version_size(
     #             format_version1.new_version, format_version2.new_version, self.package_type
@@ -150,16 +150,16 @@
                     part_item = Item(left_open=True, left=version, right_open=True, right=version)
             all_item.append(part_item)
         ret = ItemGroup(*all_item, is_or=True)
         ret = ret.merge()
         return ret
 
     def check_version_in_expression(self, lj_expression):
-        from lj_spider_core.version import get_base_version
-        from lj_spider_core.version.version_base import Equal_Or_Compare_Type
+        from version import get_base_version
+        from version.version_base import Equal_Or_Compare_Type
         """
         检查版本是否属于棱镜表达式
         :param lj_expression:
         :return:
         """
         if isinstance(lj_expression, Item) or isinstance(lj_expression, ItemGroup):
             if lj_expression.get_value() == "*":
@@ -202,15 +202,15 @@
                 for ret_item in ret.all_other:
                     part_flag = ret_item.is_in_version_item(self.version_str, self.package_type)
                     if part_flag:
                         break
             return part_flag
 
     def sort_versions2(self, versions, remove_not_final):
-        from lj_spider_core.version import get_base_version
+        from version import get_base_version
         not_version_objs = []
         final_version_objs = []
         fail_versions = []
         for version in versions:
             # new_version_obj = get_base_version(self.package_type, version, is_sort=True)
             new_version_obj = get_base_version(self.package_type, version)
             if new_version_obj.new_version:
@@ -235,40 +235,40 @@
             version_objs = not_version_objs
         else:
             version_objs = final_version_objs
         last_sort_versions = sorted(version_objs)
         return list(map(str, last_sort_versions)), sorted(list(map(str, fail_versions)))
 
     # def merge_versions_expression(self, versions, is_or):
-    #     from lj_spider_core.version import change_to_lj_expression
+    #     from version import change_to_expression
     #     if is_or:
     #         items = []
     #         for version in versions:
-    #             part_item = change_to_lj_expression(package_type=self.package_type, version_expression=version)
+    #             part_item = change_to_expression(package_type=self.package_type, version_expression=version)
     #             if isinstance(part_item, Item):
     #                 items.append(part_item)
     #             else:
     #                 items += part_item.items
     #         new_group = ItemGroup(*items, is_or=True)
     #     else:
     #         items = None
     #         for version in versions:
-    #             part_item = change_to_lj_expression(package_type=self.package_type, version_expression=version)
+    #             part_item = change_to_expression(package_type=self.package_type, version_expression=version)
     #             if items:
     #                 items = ItemGroup(items, part_item, is_or=is_or)
     #             else:
     #                 items = part_item
     #         new_group = items
     #     return new_group.merge()
 
     def merge_versions_expression(self, versions, is_or):
-        from lj_spider_core.version import change_to_lj_expression
+        from version import change_to_expression
         if is_or:
             version = "||".join(versions)
-            new_group = change_to_lj_expression(package_type=self.package_type, version_expression=version)
+            new_group = change_to_expression(package_type=self.package_type, version_expression=version)
         else:
             items = []
             for version in versions:
-                part_item = change_to_lj_expression(package_type=self.package_type, version_expression=version)
+                part_item = change_to_expression(package_type=self.package_type, version_expression=version)
                 items.append(part_item)
             new_group = ItemGroup(*items, is_or=is_or)
         return new_group.merge()
```

### Comparing `common_version-0.0.1/version/version_base/maven_version.py` & `common_version-0.0.2/version/version_base/maven_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @Project:lj_spider_core
 @File:composer_version.py
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/9/21 16:01
 @function：
 """
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base.base_version import Version
 
 
 class MavenVersion(Version):
 
     def __init__(self, version, package_type="composer", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
@@ -25,15 +25,15 @@
         """
         version = super().format_release(version)
         if "m" in version:
             version = version.replace("m", "b")
         return version
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/npm_version.py` & `common_version-0.0.2/version/version_base/npm_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 @Project:lj_spider_core
 @File:snyk_version.py
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/9/21 14:26
 @function：
 """
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base.base_version import Version
 
 
 class NpmVersion(Version):
     def __init__(self, version, package_type="npm", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
```

### Comparing `common_version-0.0.1/version/version_base/snyk_version.py` & `common_version-0.0.2/version/version_base/snyk_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 @IDE: PyCharm
 @Author : hsc
 @Date:2022/9/21 14:26
 @function：
 """
 import re
 
-from lj_spider_core.version.version_base.base_version import Version
+from version.version_base.base_version import Version
 
 
 class SnykVersion(Version):
     def __init__(self, version, package_type="snyk", is_sort=False):
         super().__init__(version, package_type, is_sort)
 
     def format_version(self):
-        from lj_spider_core.version.expression import arrangement_version
+        from version.expression import arrangement_version
         """
         格式化版本
         :param version:
         :return:
         """
         new_version = ""
         if self.old_version:
@@ -80,15 +80,15 @@
                 other_del_version = other.del_replace(other.new_version)
             else:
                 other_del_version = other.del_replace(other.old_version)
             final_cmp_version = self.get_final_cmp_version(del_version, other_del_version)
         return final_cmp_version
 
     def get_final_cmp_version(self, del_version, other_del_version):
-        from lj_spider_core.version.expression.base_method import supplement_zero
+        from version.expression.base_method import supplement_zero
         final_cmp_version = []
         cmp_versions = []
         if "_" in del_version:
             part_versions = del_version.split("_")
             other_part_versions = []
             if "_" in other_del_version:
                 other_part_versions = other_del_version.split("_")
```

