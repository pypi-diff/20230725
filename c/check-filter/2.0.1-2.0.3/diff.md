# Comparing `tmp/check_filter-2.0.1.tar.gz` & `tmp/check_filter-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_filter-2.0.1.tar", max compression
+gzip compressed data, was "check_filter-2.0.3.tar", max compression
```

## Comparing `check_filter-2.0.1.tar` & `check_filter-2.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-24 19:29:03.783034 check_filter-2.0.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-07-24 19:29:03.783034 check_filter-2.0.1/README.md
--rw-r--r--   0        0        0      266 2023-07-24 19:29:03.783034 check_filter-2.0.1/check_filter/__init__.py
--rw-r--r--   0        0        0      620 2023-07-24 19:29:03.783034 check_filter-2.0.1/check_filter/check.py
--rw-r--r--   0        0        0     2641 2023-07-24 19:29:03.783034 check_filter-2.0.1/check_filter/cli.py
--rw-r--r--   0        0        0     1314 2023-07-24 19:29:03.783034 check_filter-2.0.1/check_filter/utils.py
--rw-r--r--   0        0        0     1324 2023-07-24 19:29:03.783034 check_filter-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 check_filter-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 20:25:11.809928 check_filter-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2533 2023-07-25 20:25:11.809928 check_filter-2.0.3/README.md
+-rw-r--r--   0        0        0      266 2023-07-25 20:25:11.809928 check_filter-2.0.3/check_filter/__init__.py
+-rw-r--r--   0        0        0      680 2023-07-25 20:25:11.809928 check_filter-2.0.3/check_filter/check.py
+-rw-r--r--   0        0        0     2641 2023-07-25 20:25:11.809928 check_filter-2.0.3/check_filter/cli.py
+-rw-r--r--   0        0        0     1314 2023-07-25 20:25:11.809928 check_filter-2.0.3/check_filter/utils.py
+-rw-r--r--   0        0        0     1324 2023-07-25 20:25:11.809928 check_filter-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 check_filter-2.0.3/PKG-INFO
```

### Comparing `check_filter-2.0.1/LICENSE` & `check_filter-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `check_filter-2.0.1/README.md` & `check_filter-2.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Check Filtering
 
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub release](https://img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https://GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-asset-manager)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub release](https://img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https://GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-asset-manager) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/check-filter?label=Supported%20versions)
 
 Check URLs that filtered ( or not ) in Iran
 
 ## Requirements
 
 - Python 3.8+
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
 # Check Filtering [![made-with-python](https://img.shields.io/badge/
 Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub release]
 (https://img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https:
 //GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://
 github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/
 badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/
 release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-
-asset-manager) Check URLs that filtered ( or not ) in Iran ## Requirements -
-Python 3.8+ ## Install ```bash pip install check-filter ``` ## Usage You can
-use this package in three ways: 1. Single domain ```bash check-filter domain
-github.com ``` ![single](.github/single.png) 2. Multiple domains ```bash check-
-filter domains github.com,google.com ``` ![single](.github/multiple.png) 3.
-From a file Create a file from your website URLs. Put each URL in a new line.
-```text github.com arash-hatami.ir facebook.com gitlab.com google.com
-pornhub.com pypi.org twitter.com gsm.ir xnxx.com cloudflare.com
-stackoverflow.com ``` Then run the following command: ```bash check-filter file
-list ``` ![single](.github/file.png) --- ## Support ð [![Donate with
-Bitcoin](https://en.cryptobadges.io/badge/micro/
+asset-manager) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+check-filter?label=Supported%20versions) Check URLs that filtered ( or not ) in
+Iran ## Requirements - Python 3.8+ ## Install ```bash pip install check-filter
+``` ## Usage You can use this package in three ways: 1. Single domain ```bash
+check-filter domain github.com ``` ![single](.github/single.png) 2. Multiple
+domains ```bash check-filter domains github.com,google.com ``` ![single]
+(.github/multiple.png) 3. From a file Create a file from your website URLs. Put
+each URL in a new line. ```text github.com arash-hatami.ir facebook.com
+gitlab.com google.com pornhub.com pypi.org twitter.com gsm.ir xnxx.com
+cloudflare.com stackoverflow.com ``` Then run the following command: ```bash
+check-filter file list ``` ![single](.github/file.png) --- ## Support ð [!
+[Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/
 bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://en.cryptobadges.io/donate/
 bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://
 en.cryptobadges.io/badge/micro/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)]
 (https://en.cryptobadges.io/donate/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 [![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/
 D1D1WGU9)
 [https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg]
```

### Comparing `check_filter-2.0.1/check_filter/check.py` & `check_filter-2.0.3/check_filter/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """It's the checker module for filtering status"""
+import os
 import dns.resolver
 
 blocked_ips = {'10.10.34.34', '10.10.34.35', '10.10.34.36'}
 resolver = dns.resolver.Resolver()
-resolver.nameservers = ['8.8.8.8']
+resolver.nameservers = [
+    '178.22.122.100' if 'CI' in os.environ else '8.8.8.8'
+]
 headers = ['Address', 'Status']
 
 
 def check(domain: str) -> bool:
     """Check if domain is blocked
 
     Args:
```

### Comparing `check_filter-2.0.1/check_filter/cli.py` & `check_filter-2.0.3/check_filter/cli.py`

 * *Files identical despite different names*

### Comparing `check_filter-2.0.1/check_filter/utils.py` & `check_filter-2.0.3/check_filter/utils.py`

 * *Files identical despite different names*

### Comparing `check_filter-2.0.1/pyproject.toml` & `check_filter-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "check-filter"
-version = "2.0.1"
+version = "2.0.3"
 license = "MIT"
 description = "Check URLs that filtered ( or not ) in Iran."
 authors = ["Arash Hatami <hatamiarash7@gmail.com>"]
 readme = "README.md"
 homepage = "https://arash-hatami.ir"
 repository = "https://github.com/hatamiarash7/CheckFiltering"
 keywords = ["internet", "censorship", "filtering"]
```

### Comparing `check_filter-2.0.1/PKG-INFO` & `check_filter-2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-filter
-Version: 2.0.1
+Version: 2.0.3
 Summary: Check URLs that filtered ( or not ) in Iran.
 Home-page: https://arash-hatami.ir
 License: MIT
 Keywords: internet,censorship,filtering
 Author: Arash Hatami
 Author-email: hatamiarash7@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -22,15 +22,15 @@
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Bug Tracker, https://github.com/hatamiarash7/CheckFiltering/issues
 Project-URL: Repository, https://github.com/hatamiarash7/CheckFiltering
 Description-Content-Type: text/markdown
 
 # Check Filtering
 
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub release](https://img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https://GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-asset-manager)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub release](https://img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https://GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-asset-manager) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/check-filter?label=Supported%20versions)
 
 Check URLs that filtered ( or not ) in Iran
 
 ## Requirements
 
 - Python 3.8+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: check-filter Version: 2.0.1 Summary: Check URLs
+Metadata-Version: 2.1 Name: check-filter Version: 2.0.3 Summary: Check URLs
 that filtered ( or not ) in Iran. Home-page: https://arash-hatami.ir License:
 MIT Keywords: internet,censorship,filtering Author: Arash Hatami Author-email:
 hatamiarash7@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -15,25 +15,26 @@
 Filtering [![made-with-python](https://img.shields.io/badge/Made%20with-Python-
 1f425f.svg)](https://www.python.org/) [![GitHub release](https://
 img.shields.io/github/release/hatamiarash7/CheckFiltering.svg)](https://
 GitHub.com/hatamiarash7/CheckFiltering/releases/) [![Release](https://
 github.com/hatamiarash7/CheckFiltering/actions/workflows/release.yml/
 badge.svg)](https://github.com/hatamiarash7/CheckFiltering/actions/workflows/
 release.yml) ![GitHub](https://img.shields.io/github/license/hatamiarash7/jira-
-asset-manager) Check URLs that filtered ( or not ) in Iran ## Requirements -
-Python 3.8+ ## Install ```bash pip install check-filter ``` ## Usage You can
-use this package in three ways: 1. Single domain ```bash check-filter domain
-github.com ``` ![single](.github/single.png) 2. Multiple domains ```bash check-
-filter domains github.com,google.com ``` ![single](.github/multiple.png) 3.
-From a file Create a file from your website URLs. Put each URL in a new line.
-```text github.com arash-hatami.ir facebook.com gitlab.com google.com
-pornhub.com pypi.org twitter.com gsm.ir xnxx.com cloudflare.com
-stackoverflow.com ``` Then run the following command: ```bash check-filter file
-list ``` ![single](.github/file.png) --- ## Support ð [![Donate with
-Bitcoin](https://en.cryptobadges.io/badge/micro/
+asset-manager) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+check-filter?label=Supported%20versions) Check URLs that filtered ( or not ) in
+Iran ## Requirements - Python 3.8+ ## Install ```bash pip install check-filter
+``` ## Usage You can use this package in three ways: 1. Single domain ```bash
+check-filter domain github.com ``` ![single](.github/single.png) 2. Multiple
+domains ```bash check-filter domains github.com,google.com ``` ![single]
+(.github/multiple.png) 3. From a file Create a file from your website URLs. Put
+each URL in a new line. ```text github.com arash-hatami.ir facebook.com
+gitlab.com google.com pornhub.com pypi.org twitter.com gsm.ir xnxx.com
+cloudflare.com stackoverflow.com ``` Then run the following command: ```bash
+check-filter file list ``` ![single](.github/file.png) --- ## Support ð [!
+[Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/
 bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz)](https://en.cryptobadges.io/donate/
 bc1qmmh6vt366yzjt3grjxjjqynrrxs3frun8gnxrz) [![Donate with Ethereum](https://
 en.cryptobadges.io/badge/micro/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)]
 (https://en.cryptobadges.io/donate/0x0831bD72Ea8904B38Be9D6185Da2f930d6078094)
 [![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/
 D1D1WGU9)
 [https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg]
```

