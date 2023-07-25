# Comparing `tmp/check_rkn-0.1.1.tar.gz` & `tmp/check_rkn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_rkn-0.1.1.tar", max compression
+gzip compressed data, was "check_rkn-1.0.0.tar", max compression
```

## Comparing `check_rkn-0.1.1.tar` & `check_rkn-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-14 15:56:57.206827 check_rkn-0.1.1/check_rkn/__init__.py
--rw-r--r--   0        0        0     1891 2023-07-25 09:57:22.148188 check_rkn-0.1.1/check_rkn/check_rkn.py
--rw-r--r--   0        0        0    11555 2023-07-14 12:27:23.917420 check_rkn-0.1.1/LICENSE
--rw-r--r--   0        0        0      703 2023-07-25 10:04:19.154560 check_rkn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      718 2023-07-21 15:59:30.437665 check_rkn-0.1.1/README.md
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 check_rkn-0.1.1/setup.py
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 check_rkn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-14 15:56:57.206827 check_rkn-1.0.0/check_rkn/__init__.py
+-rw-r--r--   0        0        0     1891 2023-07-25 09:57:22.148188 check_rkn-1.0.0/check_rkn/check_rkn.py
+-rw-r--r--   0        0        0    11555 2023-07-14 12:27:23.917420 check_rkn-1.0.0/LICENSE
+-rw-r--r--   0        0        0      782 2023-07-25 12:29:27.706108 check_rkn-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      809 2023-07-25 12:15:11.579056 check_rkn-1.0.0/README.md
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 check_rkn-1.0.0/setup.py
+-rw-r--r--   0        0        0     1480 1970-01-01 00:00:00.000000 check_rkn-1.0.0/PKG-INFO
```

### Comparing `check_rkn-0.1.1/check_rkn/check_rkn.py` & `check_rkn-1.0.0/check_rkn/check_rkn.py`

 * *Files identical despite different names*

### Comparing `check_rkn-0.1.1/LICENSE` & `check_rkn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `check_rkn-0.1.1/pyproject.toml` & `check_rkn-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "check-rkn"
-version = "0.1.1"
+version = "1.0.0"
 description = "Library that check blocked website on blocklist.rkn.gov.ru"
+license = "Apache-2.0"
 authors = ["IvanyaK <ivanrus200519@gmail.com>"]
 readme = "README.md"
+repository = "https://codeberg.org/IvanyaK/check-rkn"
 packages = [{include = "check_rkn"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anticaptchaofficial = "^1.0.53"
 selenium = "^4.10.0"
```

### Comparing `check_rkn-0.1.1/README.md` & `check_rkn-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Check_rkn
 
+[![PyPI](https://img.shields.io/pypi/v/check-rkn)](https://pypi.org/project/check-rkn/)
+
 This is library, that check blocked websites on [blocklist.rkn.gov.ru](https://blocklist.rkn.gov.ru/). Library uses [Selenium](https://pypi.org/project/selenium/) and [anticaptchaofficial](https://pypi.org/project/anticaptchaofficial/). *WARNING!*  You need to register on [anti-captcha.com](https://anti-captcha.com/) to get the api key and top up your balance (For residents of the Russian federation: MIR cards are available, you can also pay with cryptocurrency)
 
 ## How to use
 
 ```python 
 from check_rkn.check_rkn import check_website
```

### Comparing `check_rkn-0.1.1/setup.py` & `check_rkn-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['anticaptchaofficial>=1.0.53,<2.0.0', 'selenium>=4.10.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'check-rkn',
-    'version': '0.1.1',
+    'version': '1.0.0',
     'description': 'Library that check blocked website on blocklist.rkn.gov.ru',
-    'long_description': '# Check_rkn\n\nThis is library, that check blocked websites on [blocklist.rkn.gov.ru](https://blocklist.rkn.gov.ru/). Library uses [Selenium](https://pypi.org/project/selenium/) and [anticaptchaofficial](https://pypi.org/project/anticaptchaofficial/). *WARNING!*  You need to register on [anti-captcha.com](https://anti-captcha.com/) to get the api key and top up your balance (For residents of the Russian federation: MIR cards are available, you can also pay with cryptocurrency)\n\n## How to use\n\n```python \nfrom check_rkn.check_rkn import check_website\n\nresult = check_website("your_url", "your_api_key")\nprint(result) # True if website is blocked or False if no\n\n```\n\n## License - [Apache 2.0](NOTICE)\n',
+    'long_description': '# Check_rkn\n\n[![PyPI](https://img.shields.io/pypi/v/check-rkn)](https://pypi.org/project/check-rkn/)\n\nThis is library, that check blocked websites on [blocklist.rkn.gov.ru](https://blocklist.rkn.gov.ru/). Library uses [Selenium](https://pypi.org/project/selenium/) and [anticaptchaofficial](https://pypi.org/project/anticaptchaofficial/). *WARNING!*  You need to register on [anti-captcha.com](https://anti-captcha.com/) to get the api key and top up your balance (For residents of the Russian federation: MIR cards are available, you can also pay with cryptocurrency)\n\n## How to use\n\n```python \nfrom check_rkn.check_rkn import check_website\n\nresult = check_website("your_url", "your_api_key")\nprint(result) # True if website is blocked or False if no\n\n```\n\n## License - [Apache 2.0](NOTICE)\n',
     'author': 'IvanyaK',
     'author_email': 'ivanrus200519@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://codeberg.org/IvanyaK/check-rkn',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `check_rkn-0.1.1/PKG-INFO` & `check_rkn-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: check-rkn
-Version: 0.1.1
+Version: 1.0.0
 Summary: Library that check blocked website on blocklist.rkn.gov.ru
+Home-page: https://codeberg.org/IvanyaK/check-rkn
+License: Apache-2.0
 Author: IvanyaK
 Author-email: ivanrus200519@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anticaptchaofficial (>=1.0.53,<2.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
+Project-URL: Repository, https://codeberg.org/IvanyaK/check-rkn
 Description-Content-Type: text/markdown
 
 # Check_rkn
 
+[![PyPI](https://img.shields.io/pypi/v/check-rkn)](https://pypi.org/project/check-rkn/)
+
 This is library, that check blocked websites on [blocklist.rkn.gov.ru](https://blocklist.rkn.gov.ru/). Library uses [Selenium](https://pypi.org/project/selenium/) and [anticaptchaofficial](https://pypi.org/project/anticaptchaofficial/). *WARNING!*  You need to register on [anti-captcha.com](https://anti-captcha.com/) to get the api key and top up your balance (For residents of the Russian federation: MIR cards are available, you can also pay with cryptocurrency)
 
 ## How to use
 
 ```python 
 from check_rkn.check_rkn import check_website
```

