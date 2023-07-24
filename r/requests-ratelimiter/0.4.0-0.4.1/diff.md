# Comparing `tmp/requests-ratelimiter-0.4.0.tar.gz` & `tmp/requests_ratelimiter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-ratelimiter-0.4.0.tar", max compression
+gzip compressed data, was "requests_ratelimiter-0.4.1.tar", max compression
```

## Comparing `requests-ratelimiter-0.4.0.tar` & `requests_ratelimiter-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1211 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/HISTORY.md
--rw-r--r--   0        0        0     1068 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/LICENSE
--rw-r--r--   0        0        0     9882 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/README.md
--rw-r--r--   0        0        0     1909 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      466 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/requests_ratelimiter/__init__.py
--rw-r--r--   0        0        0       21 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/requests_ratelimiter/py.typed
--rw-r--r--   0        0        0     7258 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/requests_ratelimiter/requests_ratelimiter.py
--rw-r--r--   0        0        0        0 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/test/__init__.py
--rw-r--r--   0        0        0     1749 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/test/conftest.py
--rw-r--r--   0        0        0     3579 2022-09-27 18:55:25.783927 requests-ratelimiter-0.4.0/test/test_requests_ratelimiter.py
--rw-r--r--   0        0        0    11084 1970-01-01 00:00:00.000000 requests-ratelimiter-0.4.0/setup.py
--rw-r--r--   0        0        0    11141 1970-01-01 00:00:00.000000 requests-ratelimiter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1254 2023-07-24 22:39:10.071464 requests_ratelimiter-0.4.1/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-07-24 22:39:10.071464 requests_ratelimiter-0.4.1/LICENSE
+-rw-r--r--   0        0        0     9889 2023-07-24 22:39:10.071464 requests_ratelimiter-0.4.1/README.md
+-rw-r--r--   0        0        0     1793 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      466 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/requests_ratelimiter/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/requests_ratelimiter/py.typed
+-rw-r--r--   0        0        0     7304 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/requests_ratelimiter/requests_ratelimiter.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/test/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/test/conftest.py
+-rw-r--r--   0        0        0     3909 2023-07-24 22:39:10.075464 requests_ratelimiter-0.4.1/test/test_requests_ratelimiter.py
+-rw-r--r--   0        0        0    11211 1970-01-01 00:00:00.000000 requests_ratelimiter-0.4.1/PKG-INFO
```

### Comparing `requests-ratelimiter-0.4.0/HISTORY.md` & `requests_ratelimiter-0.4.1/HISTORY.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # History
 
+## 0.4.1 (2023-07-24)
+* Add support for python 3.12
+
 ## 0.4.0 (2022-09-27)
 * Drop support for python 3.6
 * Add support for python 3.11
-* Remove upper version constraint for non-dev dependencies
+* Remove upper version constraint for `requests`
 
 ## 0.3.2 (2022-05-09)
 * Default to not using monotonic time if using a persistent backend (SQLite or Redis)
 
 ## 0.3.1 (2022-04-06)
 * Fix 429 response handling: if multiple rate limits are defined, fill bucket according to smallest rate limit
 * Default to not passing `bucket_name` argument to backend
```

### Comparing `requests-ratelimiter-0.4.0/LICENSE` & `requests_ratelimiter-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-ratelimiter-0.4.0/README.md` & `requests_ratelimiter-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 <!-- TODO: Section explaining burst rate limit -->
 
 ### Advanced Settings
 If you need to define more complex rate limits, you can create a `Limiter` object instead:
 ```python
 from pyrate_limiter import Duration, RequestRate, Limiter
-from requests_ratelimiter LimiterSession
+from requests_ratelimiter import LimiterSession
 
 nanocentury_rate = RequestRate(10, Duration.SECOND * 3.156)
 fortnight_rate = RequestRate(1000, Duration.DAY * 14)
 trimonthly_rate = RequestRate(10000, Duration.MONTH * 3)
 limiter = Limiter(nanocentury_rate, fortnight_rate, trimonthly_rate)
 
 session = LimiterSession(limiter=limiter)
```

### Comparing `requests-ratelimiter-0.4.0/pyproject.toml` & `requests_ratelimiter-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-ratelimiter"
-version = "0.4.0"
+version = "0.4.1"
 description = "Rate-limiting for the requests library"
 authors = ["Jordan Cook"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/JWCook/requests-ratelimiter"
 repository = "https://github.com/JWCook/requests-ratelimiter"
 documentation = "https://requests-ratelimiter.readthedocs.io"
@@ -14,43 +14,39 @@
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
 include = [
     {format="sdist", path="*.md"},
     {format="sdist", path="test"},
 ]
+
 [tool.poetry.dependencies]
 python = "^3.7"
-pyrate-limiter = ">=2.8"
+pyrate-limiter = "^2.8"
 requests = ">=2.20"
 
 # Documentation dependencies needed for Readthedocs builds
-furo = {version="2022.9.15", optional=true}
+furo = {version="^2022.12", optional=true}
 myst-parser = {version=">=0.17", optional=true}
-sphinx = {version="^4.3.0", optional=true}
-sphinx-autodoc-typehints = {version="^1.17", optional=true}
+sphinx = {version="^5.2", optional=true}
+sphinx-autodoc-typehints = {version="^1.22", optional=true}
 sphinx-copybutton = {version=">=0.5", optional=true}
 
-
 [tool.poetry.extras]
 docs = ["furo", "myst-parser", "sphinx", "sphinx-autodoc-typehints",
         "sphinx-copybutton", "sphinxcontrib-apidoc"]
 
 [tool.poetry.dev-dependencies]
-coverage = "^6.2"
-pre-commit = "^2.17"
-pytest = "^7.0"
-pytest-cov = ">=2.11"
-pytest-xdist = ">=2.2"
+coverage = "^7.2"
+pre-commit = "^2.21"
+pytest = "^7.2"
+pytest-cov = ">=4.0"
+pytest-xdist = ">=3.1"
 requests-mock = "^1.10"
 
-# Workarounds for possible dependency issues with importlib-metadata
-typing-extensions = "^4.3"
-zipp = "^3.7"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 skip-string-normalization = true
```

### Comparing `requests-ratelimiter-0.4.0/requests_ratelimiter/requests_ratelimiter.py` & `requests_ratelimiter-0.4.1/requests_ratelimiter/requests_ratelimiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inspect import signature
 from logging import getLogger
 from time import time
-from typing import TYPE_CHECKING, Callable, Dict, Iterable, Type, Union
+from typing import TYPE_CHECKING, Callable, Dict, Iterable, Optional, Type, Union
 from urllib.parse import urlparse
 from uuid import uuid4
 
 from pyrate_limiter import Duration, Limiter, RequestRate
 from pyrate_limiter.bucket import AbstractBucket, MemoryListBucket, MemoryQueueBucket
 from requests import PreparedRequest, Response, Session
 from requests.adapters import HTTPAdapter
@@ -28,18 +28,18 @@
         per_second: float = 0,
         per_minute: float = 0,
         per_hour: float = 0,
         per_day: float = 0,
         per_month: float = 0,
         burst: float = 1,
         bucket_class: Type[AbstractBucket] = MemoryListBucket,
-        bucket_kwargs: Dict = None,
-        time_function: Callable[..., float] = None,
-        limiter: Limiter = None,
-        max_delay: Union[int, float] = None,
+        bucket_kwargs: Optional[Dict] = None,
+        time_function: Optional[Callable[..., float]] = None,
+        limiter: Optional[Limiter] = None,
+        max_delay: Union[int, float, None] = None,
         per_host: bool = True,
         limit_statuses: Iterable[int] = (429,),
         **kwargs,
     ):
         # Translate request rate values into RequestRate objects
         rates = [
             RequestRate(limit, interval)
```

### Comparing `requests-ratelimiter-0.4.0/test/conftest.py` & `requests_ratelimiter-0.4.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `requests-ratelimiter-0.4.0/test/test_requests_ratelimiter.py` & `requests_ratelimiter-0.4.1/test/test_requests_ratelimiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     get_mock_session,
     mount_mock_adapter,
 )
 from time import sleep
 from unittest.mock import patch
 
 from pyrate_limiter import Duration, Limiter, RequestRate
-from requests import Session
+from requests import Response, Session
+from requests.adapters import HTTPAdapter
 
 from requests_ratelimiter import LimiterAdapter, LimiterMixin, LimiterSession
 
 patch_sleep = patch('pyrate_limiter.limit_context_decorator.sleep', side_effect=sleep)
 rate = RequestRate(5, Duration.SECOND)
 
 
@@ -32,24 +33,32 @@
     assert mock_sleep.called is False
 
     session.get(MOCKED_URL)
     assert mock_sleep.called is True
 
 
 @patch_sleep
-def test_limiter_adapter(mock_sleep):
+@patch.object(HTTPAdapter, 'send')
+def test_limiter_adapter(mock_send, mock_sleep):
+    # To allow mounting a mock:// URL, we need to patch HTTPAdapter.send()
+    # so it doesn't validate the protocol
+    mock_response = Response()
+    mock_response.url = MOCKED_URL
+    mock_response.status = 200
+    mock_send.return_value = mock_response
+
     session = Session()
     adapter = LimiterAdapter(per_second=5)
-    session.mount('https://', adapter)
+    session.mount('http+mock://', adapter)
 
     for _ in range(5):
-        session.get('https://httpbin.org/get')
+        session.get(MOCKED_URL)
     assert mock_sleep.called is False
 
-    session.get('https://httpbin.org/get')
+    session.get(MOCKED_URL)
     assert mock_sleep.called is True
 
 
 @patch_sleep
 def test_custom_limiter(mock_sleep):
     limiter = Limiter(RequestRate(5, Duration.SECOND))
     session = get_mock_session(limiter=limiter)
```

### Comparing `requests-ratelimiter-0.4.0/setup.py` & `requests_ratelimiter-0.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,277 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: requests-ratelimiter
+Version: 0.4.1
+Summary: Rate-limiting for the requests library
+Home-page: https://github.com/JWCook/requests-ratelimiter
+License: MIT
+Keywords: requests,rate-limiting,leaky-bucket
+Author: Jordan Cook
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Provides-Extra: docs
+Requires-Dist: furo (>=2022.12,<2023.0) ; extra == "docs"
+Requires-Dist: myst-parser (>=0.17) ; extra == "docs"
+Requires-Dist: pyrate-limiter (>=2.8,<3.0)
+Requires-Dist: requests (>=2.20)
+Requires-Dist: sphinx (>=5.2,<6.0) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.22,<2.0) ; extra == "docs"
+Requires-Dist: sphinx-copybutton (>=0.5) ; extra == "docs"
+Project-URL: Documentation, https://requests-ratelimiter.readthedocs.io
+Project-URL: Repository, https://github.com/JWCook/requests-ratelimiter
+Description-Content-Type: text/markdown
 
-packages = \
-['requests_ratelimiter']
+# Requests-Ratelimiter
+[![Build
+status](https://github.com/JWCook/requests-ratelimiter/workflows/Build/badge.svg)](https://github.com/JWCook/requests-ratelimiter/actions)
+[![Codecov](https://codecov.io/gh/JWCook/requests-ratelimiter/branch/main/graph/badge.svg)](https://codecov.io/gh/JWCook/requests-ratelimiter)
+[![Documentation Status](https://img.shields.io/readthedocs/requests-ratelimiter/stable?label=docs)](https://requests-ratelimiter.readthedocs.io)
+[![PyPI](https://img.shields.io/pypi/v/requests-ratelimiter?color=blue)](https://pypi.org/project/requests-ratelimiter)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/requests-ratelimiter?color=blue)](https://anaconda.org/conda-forge/requests-ratelimiter)
+[![PyPI - Python Versions](https://img.shields.io/pypi/pyversions/requests-ratelimiter)](https://pypi.org/project/requests-ratelimiter)
+[![PyPI - Format](https://img.shields.io/pypi/format/requests-ratelimiter?color=blue)](https://pypi.org/project/requests-ratelimiter)
 
-package_data = \
-{'': ['*']}
+This package is a simple wrapper around [pyrate-limiter](https://pyratelimiter.readthedocs.io)
+that adds convenient integration with the [requests](https://requests.readthedocs.io) library.
 
-install_requires = \
-['pyrate-limiter>=2.8', 'requests>=2.20']
-
-extras_require = \
-{'docs': ['furo==2022.9.15',
-          'myst-parser>=0.17',
-          'sphinx>=4.3.0,<5.0.0',
-          'sphinx-autodoc-typehints>=1.17,<2.0',
-          'sphinx-copybutton>=0.5']}
-
-setup_kwargs = {
-    'name': 'requests-ratelimiter',
-    'version': '0.4.0',
-    'description': 'Rate-limiting for the requests library',
-    'long_description': '# Requests-Ratelimiter\n[![Build\nstatus](https://github.com/JWCook/requests-ratelimiter/workflows/Build/badge.svg)](https://github.com/JWCook/requests-ratelimiter/actions)\n[![Codecov](https://codecov.io/gh/JWCook/requests-ratelimiter/branch/main/graph/badge.svg)](https://codecov.io/gh/JWCook/requests-ratelimiter)\n[![Documentation Status](https://img.shields.io/readthedocs/requests-ratelimiter/stable?label=docs)](https://requests-ratelimiter.readthedocs.io)\n[![PyPI](https://img.shields.io/pypi/v/requests-ratelimiter?color=blue)](https://pypi.org/project/requests-ratelimiter)\n[![Conda](https://img.shields.io/conda/vn/conda-forge/requests-ratelimiter?color=blue)](https://anaconda.org/conda-forge/requests-ratelimiter)\n[![PyPI - Python Versions](https://img.shields.io/pypi/pyversions/requests-ratelimiter)](https://pypi.org/project/requests-ratelimiter)\n[![PyPI - Format](https://img.shields.io/pypi/format/requests-ratelimiter?color=blue)](https://pypi.org/project/requests-ratelimiter)\n\nThis package is a simple wrapper around [pyrate-limiter](https://pyratelimiter.readthedocs.io)\nthat adds convenient integration with the [requests](https://requests.readthedocs.io) library.\n\nFull project documentation can be found at [requests-ratelimiter.readthedocs.io](https://requests-ratelimiter.readthedocs.io).\n\n\n# Features\n* `pyrate-limiter` is a general-purpose rate limiting library that implements the leaky bucket\n  algorithm, supports multiple rate limits, and has optional persistence with SQLite and Redis\n  backends\n* `requests-ratelimiter` adds some extra conveniences specific to sending HTTP requests with the\n  `requests` library\n* It can be used as either a\n  [session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) or a\n  [transport adapter](https://requests.readthedocs.io/en/latest/user/advanced/#transport-adapters)\n* It can also be used as a mixin, for compatibility with other `requests`-based libraries\n* Rate limits are tracked separately per host\n* Different rate limits can optionally be applied to different hosts\n\n# Installation\n```\npip install requests-ratelimiter\n```\n\n# Usage\n\n## Usage Options\nThere are three ways to use `requests-ratelimiter`:\n\n### Session\nThe simplest option is\n[`LimiterSession`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterSession),\nwhich can be used as a drop-in replacement for\n[`requests.Session`](https://requests.readthedocs.io/en/latest/api/#requests.Session).\n\nExample:\n```python\nfrom requests_ratelimiter import LimiterSession\nfrom time import time\n\n# Apply a rate limit of 5 requests per second to all requests\nsession = LimiterSession(per_second=5)\nstart = time()\n\n# Send requests that stay within the defined rate limit\nfor i in range(20):\n    response = session.get(\'https://httpbin.org/get\')\n    print(f\'[t+{time()-start:.2f}] Sent request {i+1}\')\n```\n\nExample output:\n```bash\n[t+0.22] Sent request 1\n[t+0.26] Sent request 2\n[t+0.30] Sent request 3\n[t+0.34] Sent request 4\n[t+0.39] Sent request 5\n[t+1.24] Sent request 6\n[t+1.28] Sent request 7\n[t+1.32] Sent request 8\n[t+1.37] Sent request 9\n[t+1.41] Sent request 10\n[t+2.04] Sent request 11\n...\n```\n\n### Adapter\nFor more advanced usage,\n[`LimiterAdapter`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterAdapter)\nis available to be used as a\n[transport adapter](https://requests.readthedocs.io/en/latest/user/advanced/#transport-adapters).\n\nExample:\n```python\nfrom requests import Session\nfrom requests_ratelimiter import LimiterAdapter\n\nsession = Session()\n\n# Apply a rate-limit (5 requests per second) to all requests\nadapter = LimiterAdapter(per_second=5)\nsession.mount(\'http://\', adapter)\nsession.mount(\'https://\', adapter)\n\n# Send rate-limited requests\nfor user_id in range(100):\n    response = session.get(f\'https://api.some_site.com/v1/users/{user_id}\')\n    print(response.json())\n```\n\n### Mixin\nFinally,\n[`LimiterMixin`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterMixin)\nis available for advanced use cases in which you want add rate-limiting features to a custom session\nor adapter class. See\n[Custom Session Example](#custom-session-example-requests-cache) below for an example.\n\n## Rate Limit Settings\n### Basic Settings\nThe following parameters are available for the most common rate limit intervals:\n* `per_second`: Max requests per second\n* `per_minute`: Max requests per minute\n* `per_hour`: Max requests per hour\n* `per_day`: Max requests per day\n* `per_month`: Max requests per month\n* `burst`: Max number of consecutive requests allowed before applying per-second rate-limiting\n\n<!-- TODO: Section explaining burst rate limit -->\n\n### Advanced Settings\nIf you need to define more complex rate limits, you can create a `Limiter` object instead:\n```python\nfrom pyrate_limiter import Duration, RequestRate, Limiter\nfrom requests_ratelimiter LimiterSession\n\nnanocentury_rate = RequestRate(10, Duration.SECOND * 3.156)\nfortnight_rate = RequestRate(1000, Duration.DAY * 14)\ntrimonthly_rate = RequestRate(10000, Duration.MONTH * 3)\nlimiter = Limiter(nanocentury_rate, fortnight_rate, trimonthly_rate)\n\nsession = LimiterSession(limiter=limiter)\n```\n\nSee [pyrate-limiter docs](https://pyratelimiter.readthedocs.io/en/latest/#basic-usage) for more `Limiter` usage details.\n\n## Backends\nBy default, rate limits are tracked in memory and are not persistent. You can optionally use either\nSQLite or Redis to persist rate limits across threads, processes, and/or application restarts.\nYou can specify which backend to use with the `bucket_class` argument. For example, to use SQLite:\n```python\nfrom pyrate_limiter import SQLiteBucket\nfrom requests_ratelimiter import LimiterSession\n\nsession = LimiterSession(per_second=5, bucket_class=SQLiteBucket)\n```\n\nSee [pyrate-limiter docs](https://pyratelimiter.readthedocs.io/en/latest/#backends) for more details.\n\n## Other Features\n### Per-Host Rate Limit Tracking\nWith either `LimiterSession` or `LimiterAdapter`, rate limits are tracked separately for each host.\nIn other words, requests sent to one host will not count against the rate limit for any other hosts:\n\n```python\nsession = LimiterSession(per_second=5)\n\n# Make requests for two different hosts\nfor _ in range(10):\n    response = session.get(f\'https://httpbin.org/get\')\n    print(response.json())\n    session.get(f\'https://httpbingo.org/get\')\n    print(response.json())\n```\n\nIf you have a case where multiple hosts share the same rate limit, you can disable this behavior\nwith the `per_host` option:\n```python\nsession = LimiterSession(per_second=5, per_host=False)\n```\n\n### Per-Host Rate Limit Definitions\nWith `LimiterAdapter`, you can apply different rate limits to different hosts or URLs:\n```python\n# Apply a different set of rate limits (2/second and 100/minute) to a specific host\nadapter_2 = LimiterAdapter(per_second=2, per_minute=100)\nsession.mount(\'https://api.some_site.com\', adapter_2)\n```\n\nBehavior for matching requests is the same as other transport adapters: `requests` will use the\nadapter with the most specific (i.e., longest) URL prefix that matches a given request. For example:\n```python\nsession.mount(\'https://api.some_site.com/v1\', adapter_3)\nsession.mount(\'https://api.some_site.com/v1/users\', adapter_4)\n\n# This request will use adapter_3\nsession.get(\'https://api.some_site.com/v1/\')\n\n# This request will use adapter_4\nsession.get(\'https://api.some_site.com/v1/users/1234\')\n```\n\n### Rate Limit Error Handling\nSometimes, server-side rate limiting may not behave exactly as documented (or may not be documented\nat all). Or you might encounter other scenarios where your client-side limit gets out of sync with\nthe server-side limit. Typically, a server will send a `429: Too Many Requests` response for an\nexceeded rate limit.\n\nWhen this happens, `requests-ratelimiter` will adjust its request log in an attempt to catch up to\nthe server-side limit. If a server sends a different status code other than 429 to indicate an\nexceeded limit, you can set this with `limit_statuses`:\n```python\nsession = LimiterSession(per_second=5, limit_statuses=[429, 500])\n```\n\nOr if you would prefer to disable this behavior and handle it yourself:\n```python\nsession = LimiterSession(per_second=5, limit_statuses=[])\n```\n\n# Compatibility\nThere are many other useful libraries out there that add features to `requests`, most commonly by\nextending or modifying\n[requests.Session](https://requests.readthedocs.io/en/latest/api/#requests.Session) or\n[requests.HTTPAdapter](https://requests.readthedocs.io/en/latest/api/#requests.adapters.HTTPAdapter).\n\nTo use `requests-ratelimiter` with one of these libraries, you have a few different options:\n1. If the library provides a custom `Session` class, mount a `LimiterAdapter` on it\n2. Or use `LimiterMixin` to create a custom `Session` class with features from both libraries\n3. If the library provides a custom `Adapter` class, use `LimiterMixin` to create a custom `Adapter`\n   class with features from both libraries\n\n## Custom Session Example: Requests-Cache\nFor example, to combine with [requests-cache](https://github.com/requests-cache/requests-cache), which\nalso includes a separate mixin class:\n```python\nfrom requests import Session\nfrom requests_cache import CacheMixin, RedisCache\nfrom requests_ratelimiter import LimiterMixin, RedisBucket\n\n\nclass CachedLimiterSession(CacheMixin, LimiterMixin, Session):\n    """Session class with caching and rate-limiting behavior. Accepts arguments for both\n    LimiterSession and CachedSession.\n    """\n\n\n# Optionally use Redis as both the bucket backend and the cache backend\nsession = CachedLimiterSession(\n    per_second=5,\n    bucket_class=RedisBucket,\n    backend=RedisCache(),\n)\n```\n\nThis example has an extra benefit: cache hits won\'t count against your rate limit!\n',
-    'author': 'Jordan Cook',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/JWCook/requests-ratelimiter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Full project documentation can be found at [requests-ratelimiter.readthedocs.io](https://requests-ratelimiter.readthedocs.io).
 
 
-setup(**setup_kwargs)
+# Features
+* `pyrate-limiter` is a general-purpose rate limiting library that implements the leaky bucket
+  algorithm, supports multiple rate limits, and has optional persistence with SQLite and Redis
+  backends
+* `requests-ratelimiter` adds some extra conveniences specific to sending HTTP requests with the
+  `requests` library
+* It can be used as either a
+  [session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) or a
+  [transport adapter](https://requests.readthedocs.io/en/latest/user/advanced/#transport-adapters)
+* It can also be used as a mixin, for compatibility with other `requests`-based libraries
+* Rate limits are tracked separately per host
+* Different rate limits can optionally be applied to different hosts
+
+# Installation
+```
+pip install requests-ratelimiter
+```
+
+# Usage
+
+## Usage Options
+There are three ways to use `requests-ratelimiter`:
+
+### Session
+The simplest option is
+[`LimiterSession`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterSession),
+which can be used as a drop-in replacement for
+[`requests.Session`](https://requests.readthedocs.io/en/latest/api/#requests.Session).
+
+Example:
+```python
+from requests_ratelimiter import LimiterSession
+from time import time
+
+# Apply a rate limit of 5 requests per second to all requests
+session = LimiterSession(per_second=5)
+start = time()
+
+# Send requests that stay within the defined rate limit
+for i in range(20):
+    response = session.get('https://httpbin.org/get')
+    print(f'[t+{time()-start:.2f}] Sent request {i+1}')
+```
+
+Example output:
+```bash
+[t+0.22] Sent request 1
+[t+0.26] Sent request 2
+[t+0.30] Sent request 3
+[t+0.34] Sent request 4
+[t+0.39] Sent request 5
+[t+1.24] Sent request 6
+[t+1.28] Sent request 7
+[t+1.32] Sent request 8
+[t+1.37] Sent request 9
+[t+1.41] Sent request 10
+[t+2.04] Sent request 11
+...
+```
+
+### Adapter
+For more advanced usage,
+[`LimiterAdapter`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterAdapter)
+is available to be used as a
+[transport adapter](https://requests.readthedocs.io/en/latest/user/advanced/#transport-adapters).
+
+Example:
+```python
+from requests import Session
+from requests_ratelimiter import LimiterAdapter
+
+session = Session()
+
+# Apply a rate-limit (5 requests per second) to all requests
+adapter = LimiterAdapter(per_second=5)
+session.mount('http://', adapter)
+session.mount('https://', adapter)
+
+# Send rate-limited requests
+for user_id in range(100):
+    response = session.get(f'https://api.some_site.com/v1/users/{user_id}')
+    print(response.json())
+```
+
+### Mixin
+Finally,
+[`LimiterMixin`](https://requests-ratelimiter.readthedocs.io/en/stable/reference.html#requests_ratelimiter.LimiterMixin)
+is available for advanced use cases in which you want add rate-limiting features to a custom session
+or adapter class. See
+[Custom Session Example](#custom-session-example-requests-cache) below for an example.
+
+## Rate Limit Settings
+### Basic Settings
+The following parameters are available for the most common rate limit intervals:
+* `per_second`: Max requests per second
+* `per_minute`: Max requests per minute
+* `per_hour`: Max requests per hour
+* `per_day`: Max requests per day
+* `per_month`: Max requests per month
+* `burst`: Max number of consecutive requests allowed before applying per-second rate-limiting
+
+<!-- TODO: Section explaining burst rate limit -->
+
+### Advanced Settings
+If you need to define more complex rate limits, you can create a `Limiter` object instead:
+```python
+from pyrate_limiter import Duration, RequestRate, Limiter
+from requests_ratelimiter import LimiterSession
+
+nanocentury_rate = RequestRate(10, Duration.SECOND * 3.156)
+fortnight_rate = RequestRate(1000, Duration.DAY * 14)
+trimonthly_rate = RequestRate(10000, Duration.MONTH * 3)
+limiter = Limiter(nanocentury_rate, fortnight_rate, trimonthly_rate)
+
+session = LimiterSession(limiter=limiter)
+```
+
+See [pyrate-limiter docs](https://pyratelimiter.readthedocs.io/en/latest/#basic-usage) for more `Limiter` usage details.
+
+## Backends
+By default, rate limits are tracked in memory and are not persistent. You can optionally use either
+SQLite or Redis to persist rate limits across threads, processes, and/or application restarts.
+You can specify which backend to use with the `bucket_class` argument. For example, to use SQLite:
+```python
+from pyrate_limiter import SQLiteBucket
+from requests_ratelimiter import LimiterSession
+
+session = LimiterSession(per_second=5, bucket_class=SQLiteBucket)
+```
+
+See [pyrate-limiter docs](https://pyratelimiter.readthedocs.io/en/latest/#backends) for more details.
+
+## Other Features
+### Per-Host Rate Limit Tracking
+With either `LimiterSession` or `LimiterAdapter`, rate limits are tracked separately for each host.
+In other words, requests sent to one host will not count against the rate limit for any other hosts:
+
+```python
+session = LimiterSession(per_second=5)
+
+# Make requests for two different hosts
+for _ in range(10):
+    response = session.get(f'https://httpbin.org/get')
+    print(response.json())
+    session.get(f'https://httpbingo.org/get')
+    print(response.json())
+```
+
+If you have a case where multiple hosts share the same rate limit, you can disable this behavior
+with the `per_host` option:
+```python
+session = LimiterSession(per_second=5, per_host=False)
+```
+
+### Per-Host Rate Limit Definitions
+With `LimiterAdapter`, you can apply different rate limits to different hosts or URLs:
+```python
+# Apply a different set of rate limits (2/second and 100/minute) to a specific host
+adapter_2 = LimiterAdapter(per_second=2, per_minute=100)
+session.mount('https://api.some_site.com', adapter_2)
+```
+
+Behavior for matching requests is the same as other transport adapters: `requests` will use the
+adapter with the most specific (i.e., longest) URL prefix that matches a given request. For example:
+```python
+session.mount('https://api.some_site.com/v1', adapter_3)
+session.mount('https://api.some_site.com/v1/users', adapter_4)
+
+# This request will use adapter_3
+session.get('https://api.some_site.com/v1/')
+
+# This request will use adapter_4
+session.get('https://api.some_site.com/v1/users/1234')
+```
+
+### Rate Limit Error Handling
+Sometimes, server-side rate limiting may not behave exactly as documented (or may not be documented
+at all). Or you might encounter other scenarios where your client-side limit gets out of sync with
+the server-side limit. Typically, a server will send a `429: Too Many Requests` response for an
+exceeded rate limit.
+
+When this happens, `requests-ratelimiter` will adjust its request log in an attempt to catch up to
+the server-side limit. If a server sends a different status code other than 429 to indicate an
+exceeded limit, you can set this with `limit_statuses`:
+```python
+session = LimiterSession(per_second=5, limit_statuses=[429, 500])
+```
+
+Or if you would prefer to disable this behavior and handle it yourself:
+```python
+session = LimiterSession(per_second=5, limit_statuses=[])
+```
+
+# Compatibility
+There are many other useful libraries out there that add features to `requests`, most commonly by
+extending or modifying
+[requests.Session](https://requests.readthedocs.io/en/latest/api/#requests.Session) or
+[requests.HTTPAdapter](https://requests.readthedocs.io/en/latest/api/#requests.adapters.HTTPAdapter).
+
+To use `requests-ratelimiter` with one of these libraries, you have a few different options:
+1. If the library provides a custom `Session` class, mount a `LimiterAdapter` on it
+2. Or use `LimiterMixin` to create a custom `Session` class with features from both libraries
+3. If the library provides a custom `Adapter` class, use `LimiterMixin` to create a custom `Adapter`
+   class with features from both libraries
+
+## Custom Session Example: Requests-Cache
+For example, to combine with [requests-cache](https://github.com/requests-cache/requests-cache), which
+also includes a separate mixin class:
+```python
+from requests import Session
+from requests_cache import CacheMixin, RedisCache
+from requests_ratelimiter import LimiterMixin, RedisBucket
+
+
+class CachedLimiterSession(CacheMixin, LimiterMixin, Session):
+    """Session class with caching and rate-limiting behavior. Accepts arguments for both
+    LimiterSession and CachedSession.
+    """
+
+
+# Optionally use Redis as both the bucket backend and the cache backend
+session = CachedLimiterSession(
+    per_second=5,
+    bucket_class=RedisBucket,
+    backend=RedisCache(),
+)
+```
+
+This example has an extra benefit: cache hits won't count against your rate limit!
+
```

