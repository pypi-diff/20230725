# Comparing `tmp/pwdriver-0.27.2.tar.gz` & `tmp/pwdriver-0.27.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdriver-0.27.2.tar", max compression
+gzip compressed data, was "pwdriver-0.27.3.tar", max compression
```

## Comparing `pwdriver-0.27.2.tar` & `pwdriver-0.27.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-05-29 16:32:27.591685 pwdriver-0.27.2/LICENSE
--rw-r--r--   0        0        0     5485 2023-05-29 16:32:27.591685 pwdriver-0.27.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/__init__.py
--rw-r--r--   0        0        0    11601 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/core.py
--rw-r--r--   0        0        0     1358 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/listener.py
--rw-r--r--   0        0        0     4199 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/page.py
--rw-r--r--   0        0        0     1333 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/util.py
--rw-r--r--   0        0        0     1024 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/val.py
--rw-r--r--   0        0        0     1352 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 pwdriver-0.27.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-25 11:28:51.206101 pwdriver-0.27.3/LICENSE
+-rw-r--r--   0        0        0     5514 2023-07-25 11:28:51.206101 pwdriver-0.27.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/__init__.py
+-rw-r--r--   0        0        0    11601 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/core.py
+-rw-r--r--   0        0        0     1358 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/listener.py
+-rw-r--r--   0        0        0     4199 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/page.py
+-rw-r--r--   0        0        0     1333 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/util.py
+-rw-r--r--   0        0        0     1024 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pwdriver/val.py
+-rw-r--r--   0        0        0     1353 2023-07-25 11:28:51.206101 pwdriver-0.27.3/pyproject.toml
+-rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 pwdriver-0.27.3/PKG-INFO
```

### Comparing `pwdriver-0.27.2/LICENSE` & `pwdriver-0.27.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/README.md` & `pwdriver-0.27.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # PWDriver (PyWebDriver)
 
 [![E2e test](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml)
-[![Code Coverage](https://codecov.io/gh/jinmoo21/pwdriver/branch/master/graph/badge.svg)](https://codecov.io/gh/jinmoo21/pwdriver)
+[![Code Coverage](https://codecov.io/gh/jinmoo21/pwdriver/branch/master/graph/badge.svg?branch=master&kill_cache=1)](https://codecov.io/gh/jinmoo21/pwdriver)
 
 [![Release status](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml)
 [![PyPI version](https://badge.fury.io/py/pwdriver.svg)](https://badge.fury.io/py/pwdriver)
 
 [![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jinmoo21/PWDriver/blob/master/LICENSE)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fjinmoo21%2FPWDriver.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fjinmoo21%2FPWDriver?ref=badge_shield)
 
@@ -145,15 +145,15 @@
         self.driver.quit()
 
     def test_something(self):
         page = BingPage(self.driver)
         page.get()
         keyword = 'chicken'
         page.type_keyword(keyword)
-        page.click_search()
+        page.submit_keyword()
         self.assertIn(f'https://www.bing.com/search?q={keyword}', self.driver.current_url)
         self.assertEqual(f'{keyword} - Search', self.driver.title)
 
 
 if __name__ == '__main__':
     unittest.main()
 ```
```

### Comparing `pwdriver-0.27.2/pwdriver/core.py` & `pwdriver-0.27.3/pwdriver/core.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/pwdriver/listener.py` & `pwdriver-0.27.3/pwdriver/listener.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/pwdriver/page.py` & `pwdriver-0.27.3/pwdriver/page.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/pwdriver/util.py` & `pwdriver-0.27.3/pwdriver/util.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/pwdriver/val.py` & `pwdriver-0.27.3/pwdriver/val.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.27.2/pyproject.toml` & `pwdriver-0.27.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pwdriver"
-version = "0.27.2"
+version = "0.27.3"
 description = "It will download a WebDriver, and then set basic configuration automatically."
 license = "MIT"
 authors = [
     "Jinmoo Han <jinmoo21@naver.com>",
 ]
 maintainers = [
     "Jinmoo Han <jinmoo21@naver.com>",
@@ -35,16 +35,16 @@
 ]
 packages = [
     { include = "pwdriver" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-selenium = "^4.9.1"
-Appium-Python-Client = "^2.10.1"
+selenium = "^4.10.0"
+Appium-Python-Client = "^2.11.1"
 requests = "^2.31.0"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/jinmoo21/pwdriver"
 "Bug Reports" = "https://github.com/jinmoo21/pwdriver/issues"
 
 [build-system]
```

### Comparing `pwdriver-0.27.2/PKG-INFO` & `pwdriver-0.27.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdriver
-Version: 0.27.2
+Version: 0.27.3
 Summary: It will download a WebDriver, and then set basic configuration automatically.
 Home-page: https://github.com/jinmoo21/pwdriver
 License: MIT
 Keywords: python,testing,automation,webdriver,selenium,test-automation,selenium-webdriver,appium,appium-webdriver
 Author: Jinmoo Han
 Author-email: jinmoo21@naver.com
 Maintainer: Jinmoo Han
@@ -16,25 +16,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: Appium-Python-Client (>=2.10.1,<3.0.0)
+Requires-Dist: Appium-Python-Client (>=2.11.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: selenium (>=4.9.1,<5.0.0)
+Requires-Dist: selenium (>=4.10.0,<5.0.0)
 Project-URL: Bug Reports, https://github.com/jinmoo21/pwdriver/issues
 Project-URL: Repository, https://github.com/jinmoo21/pwdriver
 Description-Content-Type: text/markdown
 
 # PWDriver (PyWebDriver)
 
 [![E2e test](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml)
-[![Code Coverage](https://codecov.io/gh/jinmoo21/pwdriver/branch/master/graph/badge.svg)](https://codecov.io/gh/jinmoo21/pwdriver)
+[![Code Coverage](https://codecov.io/gh/jinmoo21/pwdriver/branch/master/graph/badge.svg?branch=master&kill_cache=1)](https://codecov.io/gh/jinmoo21/pwdriver)
 
 [![Release status](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml)
 [![PyPI version](https://badge.fury.io/py/pwdriver.svg)](https://badge.fury.io/py/pwdriver)
 
 [![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jinmoo21/PWDriver/blob/master/LICENSE)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fjinmoo21%2FPWDriver.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fjinmoo21%2FPWDriver?ref=badge_shield)
 
@@ -174,15 +174,15 @@
         self.driver.quit()
 
     def test_something(self):
         page = BingPage(self.driver)
         page.get()
         keyword = 'chicken'
         page.type_keyword(keyword)
-        page.click_search()
+        page.submit_keyword()
         self.assertIn(f'https://www.bing.com/search?q={keyword}', self.driver.current_url)
         self.assertEqual(f'{keyword} - Search', self.driver.title)
 
 
 if __name__ == '__main__':
     unittest.main()
 ```
```

