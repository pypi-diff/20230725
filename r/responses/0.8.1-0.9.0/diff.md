# Comparing `tmp/responses-0.8.1.tar.gz` & `tmp/responses-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responses-0.8.1.tar", last modified: Mon Oct  2 17:02:17 2017, max compression
+gzip compressed data, was "dist/responses-0.9.0.tar", last modified: Wed Apr  4 16:59:20 2018, max compression
```

## Comparing `responses-0.8.1.tar` & `responses-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dcramer    (501) staff       (20)        0 2017-10-02 17:02:17.000000 responses-0.8.1/
--rw-r--r--   0 dcramer    (501) staff       (20)     1699 2017-10-02 17:00:51.000000 responses-0.8.1/CHANGES
--rw-r--r--   0 dcramer    (501) staff       (20)    10835 2016-01-25 20:48:16.000000 responses-0.8.1/LICENSE
--rw-r--r--   0 dcramer    (501) staff       (20)       53 2016-01-25 20:51:25.000000 responses-0.8.1/MANIFEST.in
--rw-r--r--   0 dcramer    (501) staff       (20)    10083 2017-10-02 17:02:17.000000 responses-0.8.1/PKG-INFO
--rw-r--r--   0 dcramer    (501) staff       (20)     7431 2017-09-26 21:58:49.000000 responses-0.8.1/README.rst
-drwxr-xr-x   0 dcramer    (501) staff       (20)        0 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/
--rw-r--r--   0 dcramer    (501) staff       (20)        1 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/dependency_links.txt
--rw-r--r--   0 dcramer    (501) staff       (20)        1 2016-01-25 21:16:56.000000 responses-0.8.1/responses.egg-info/not-zip-safe
--rw-r--r--   0 dcramer    (501) staff       (20)    10083 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/PKG-INFO
--rw-r--r--   0 dcramer    (501) staff       (20)      145 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/requires.txt
--rw-r--r--   0 dcramer    (501) staff       (20)      284 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/SOURCES.txt
--rw-r--r--   0 dcramer    (501) staff       (20)       25 2017-10-02 17:02:17.000000 responses-0.8.1/responses.egg-info/top_level.txt
--rw-r--r--   0 dcramer    (501) staff       (20)    17082 2017-10-02 17:00:38.000000 responses-0.8.1/responses.py
--rw-r--r--   0 dcramer    (501) staff       (20)      165 2017-10-02 17:02:17.000000 responses-0.8.1/setup.cfg
--rw-r--r--   0 dcramer    (501) staff       (20)     2428 2017-10-02 17:01:17.000000 responses-0.8.1/setup.py
--rw-r--r--   0 dcramer    (501) staff       (20)    23568 2017-10-02 17:00:38.000000 responses-0.8.1/test_responses.py
+drwxr-xr-x   0 dcramer    (501) staff       (20)        0 2018-04-04 16:59:20.000000 responses-0.9.0/
+-rw-r--r--   0 dcramer    (501) staff       (20)    10251 2018-04-04 16:59:20.000000 responses-0.9.0/PKG-INFO
+-rw-r--r--   0 dcramer    (501) staff       (20)    18075 2018-04-04 16:22:34.000000 responses-0.9.0/responses.py
+-rw-r--r--   0 dcramer    (501) staff       (20)    10835 2017-12-07 21:27:59.000000 responses-0.9.0/LICENSE
+-rw-r--r--   0 dcramer    (501) staff       (20)     1901 2018-04-04 16:25:37.000000 responses-0.9.0/CHANGES
+-rw-r--r--   0 dcramer    (501) staff       (20)       53 2017-12-07 21:27:59.000000 responses-0.9.0/MANIFEST.in
+-rw-r--r--   0 dcramer    (501) staff       (20)     2427 2018-04-04 16:27:26.000000 responses-0.9.0/setup.py
+-rw-r--r--   0 dcramer    (501) staff       (20)    24689 2018-04-04 15:47:12.000000 responses-0.9.0/test_responses.py
+-rw-r--r--   0 dcramer    (501) staff       (20)      165 2018-04-04 16:59:20.000000 responses-0.9.0/setup.cfg
+drwxr-xr-x   0 dcramer    (501) staff       (20)        0 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/
+-rw-r--r--   0 dcramer    (501) staff       (20)    10251 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/PKG-INFO
+-rw-r--r--   0 dcramer    (501) staff       (20)        1 2018-04-04 15:56:47.000000 responses-0.9.0/responses.egg-info/not-zip-safe
+-rw-r--r--   0 dcramer    (501) staff       (20)      284 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/SOURCES.txt
+-rw-r--r--   0 dcramer    (501) staff       (20)      145 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/requires.txt
+-rw-r--r--   0 dcramer    (501) staff       (20)       25 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/top_level.txt
+-rw-r--r--   0 dcramer    (501) staff       (20)        1 2018-04-04 16:59:20.000000 responses-0.9.0/responses.egg-info/dependency_links.txt
+-rw-r--r--   0 dcramer    (501) staff       (20)     7543 2018-04-04 15:47:12.000000 responses-0.9.0/README.rst
```

### Comparing `responses-0.8.1/CHANGES` & `responses-0.9.0/CHANGES`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-0.8.1
+0.9.0
 -----
 
-- Maintain 'method' param on 'add'
+- Support for Python 3.7 (#196)
+- Support streaming responses for BaseResponse (#192)
+- Support custom patch targets for mock (#189)
+- Fix unicode support for passthru urls (#178)
+- Fix support for unicode in domain names and tlds (177)
 
 0.8.0
 -----
 
 - Added the ability to passthru real requests via ``add_passthru()``
   and ``passthru_prefixes`` configurations.
```

### Comparing `responses-0.8.1/LICENSE` & `responses-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `responses-0.8.1/PKG-INFO` & `responses-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: responses
-Version: 0.8.1
+Version: 0.9.0
 Summary: A utility library for mocking out the `requests` Python library.
 Home-page: https://github.com/getsentry/responses
 Author: David Cramer
-Author-email: UNKNOWN
 License: Apache 2.0
 Description: Responses
         =========
         
         .. image:: https://travis-ci.org/getsentry/responses.svg?branch=master
         	:target: https://travis-ci.org/getsentry/responses
         
         A utility library for mocking out the `requests` Python library.
         
         .. note:: Responses requires Python 2.7 or newer, and requests >= 2.0
         
+        Installing
+        ----------
+        ``pip install responses``
+        
         Basics
         ------
         
         The core of ``responses`` comes from registering mock responses:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             @responses.activate
             def test_simple():
                 responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                               json={'error': 'not found'}, status=404)
         
                 resp = requests.get('http://twitter.com/api/1/foobar')
@@ -40,27 +44,29 @@
         
         If you attempt to fetch a url which doesn't hit a match, ``responses`` will raise
         a ``ConnectionError``:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             from requests.exceptions import ConnectionError
         
             @responses.activate
             def test_simple():
                 with pytest.raises(ConnectionError):
                     requests.get('http://twitter.com/api/1/foobar')
         
         Lastly, you can pass an ``Exception`` as the body to trigger an error on the request:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             @responses.activate
             def test_simple():
                 responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                               body=Exception('...'))
                 with pytest.raises(Exception):
                     requests.get('http://twitter.com/api/1/foobar')
@@ -272,7 +278,8 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
+Provides-Extra: tests
```

### Comparing `responses-0.8.1/README.rst` & `responses-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 .. image:: https://travis-ci.org/getsentry/responses.svg?branch=master
 	:target: https://travis-ci.org/getsentry/responses
 
 A utility library for mocking out the `requests` Python library.
 
 .. note:: Responses requires Python 2.7 or newer, and requests >= 2.0
 
+Installing
+----------
+``pip install responses``
+
 Basics
 ------
 
 The core of ``responses`` comes from registering mock responses:
 
 .. code-block:: python
 
     import responses
+    import requests 
 
     @responses.activate
     def test_simple():
         responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                       json={'error': 'not found'}, status=404)
 
         resp = requests.get('http://twitter.com/api/1/foobar')
@@ -32,27 +37,29 @@
 
 If you attempt to fetch a url which doesn't hit a match, ``responses`` will raise
 a ``ConnectionError``:
 
 .. code-block:: python
 
     import responses
+    import requests 
 
     from requests.exceptions import ConnectionError
 
     @responses.activate
     def test_simple():
         with pytest.raises(ConnectionError):
             requests.get('http://twitter.com/api/1/foobar')
 
 Lastly, you can pass an ``Exception`` as the body to trigger an error on the request:
 
 .. code-block:: python
 
     import responses
+    import requests 
 
     @responses.activate
     def test_simple():
         responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                       body=Exception('...'))
         with pytest.raises(Exception):
             requests.get('http://twitter.com/api/1/foobar')
```

### Comparing `responses-0.8.1/responses.egg-info/PKG-INFO` & `responses-0.9.0/responses.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: responses
-Version: 0.8.1
+Version: 0.9.0
 Summary: A utility library for mocking out the `requests` Python library.
 Home-page: https://github.com/getsentry/responses
 Author: David Cramer
-Author-email: UNKNOWN
 License: Apache 2.0
 Description: Responses
         =========
         
         .. image:: https://travis-ci.org/getsentry/responses.svg?branch=master
         	:target: https://travis-ci.org/getsentry/responses
         
         A utility library for mocking out the `requests` Python library.
         
         .. note:: Responses requires Python 2.7 or newer, and requests >= 2.0
         
+        Installing
+        ----------
+        ``pip install responses``
+        
         Basics
         ------
         
         The core of ``responses`` comes from registering mock responses:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             @responses.activate
             def test_simple():
                 responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                               json={'error': 'not found'}, status=404)
         
                 resp = requests.get('http://twitter.com/api/1/foobar')
@@ -40,27 +44,29 @@
         
         If you attempt to fetch a url which doesn't hit a match, ``responses`` will raise
         a ``ConnectionError``:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             from requests.exceptions import ConnectionError
         
             @responses.activate
             def test_simple():
                 with pytest.raises(ConnectionError):
                     requests.get('http://twitter.com/api/1/foobar')
         
         Lastly, you can pass an ``Exception`` as the body to trigger an error on the request:
         
         .. code-block:: python
         
             import responses
+            import requests 
         
             @responses.activate
             def test_simple():
                 responses.add(responses.GET, 'http://twitter.com/api/1/foobar',
                               body=Exception('...'))
                 with pytest.raises(Exception):
                     requests.get('http://twitter.com/api/1/foobar')
@@ -272,7 +278,8 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
+Provides-Extra: tests
```

### Comparing `responses-0.8.1/responses.py` & `responses-0.9.0/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,37 @@
 try:
     from requests.packages.urllib3.response import HTTPResponse
 except ImportError:
     from urllib3.response import HTTPResponse
 
 if six.PY2:
     from urlparse import urlparse, parse_qsl, urlsplit, urlunsplit
+    from urllib import quote
 else:
-    from urllib.parse import urlparse, parse_qsl, urlsplit, urlunsplit
+    from urllib.parse import urlparse, parse_qsl, urlsplit, urlunsplit, quote
 
 if six.PY2:
     try:
         from six import cStringIO as BufferIO
     except ImportError:
         from six import StringIO as BufferIO
 else:
     from io import BytesIO as BufferIO
 
+try:
+    from unittest import mock as std_mock
+except ImportError:
+    import mock as std_mock
+
+try:
+    Pattern = re._pattern_type
+except AttributeError:
+    # Python 3.7
+    Pattern = re.Pattern
+
 UNSET = object()
 
 Call = namedtuple('Call', ['request', 'response'])
 
 _real_send = HTTPAdapter.send
 
 _wrapper_template = """\
@@ -49,14 +61,42 @@
 logger = logging.getLogger('responses')
 
 
 def _is_string(s):
     return isinstance(s, six.string_types)
 
 
+def _has_unicode(s):
+    return any(ord(char) > 128 for char in s)
+
+
+def _clean_unicode(url):
+    # Clean up domain names, which use punycode to handle unicode chars
+    urllist = list(urlsplit(url))
+    netloc = urllist[1]
+    if _has_unicode(netloc):
+        domains = netloc.split('.')
+        for i, d in enumerate(domains):
+            if _has_unicode(d):
+                d = 'xn--' + d.encode('punycode').decode('ascii')
+                domains[i] = d
+        urllist[1] = '.'.join(domains)
+        url = urlunsplit(urllist)
+
+    # Clean up path/query/params, which use url-encoding to handle unicode chars
+    if isinstance(url.encode('utf8'), six.string_types):
+        url = url.encode('utf8')
+    chars = list(url)
+    for i, x in enumerate(chars):
+        if ord(x) > 128:
+            chars[i] = quote(x)
+
+    return ''.join(chars)
+
+
 def _is_redirect(response):
     try:
         # 2.0.0 <= requests <= 2.2
         return response.is_redirect
     except AttributeError:
         # requests > 2.2
         return (
@@ -128,14 +168,16 @@
     return BufferIO(body)
 
 
 class BaseResponse(object):
     content_type = None
     headers = None
 
+    stream = False
+
     def __init__(self, method, url, match_querystring=False):
         self.method = method
         self.match_querystring = match_querystring
         # ensure the url has a default path set if the url is a string
         self.url = _ensure_url_default_path(url)
         self.call_count = 0
 
@@ -145,18 +187,18 @@
 
         if self.method != other.method:
             return False
 
         # Can't simply do a equality check on the objects directly here since __eq__ isn't
         # implemented for regex. It might seem to work as regex is using a cache to return
         # the same regex instances, but it doesn't in all cases.
-        self_url = self.url.pattern if isinstance(
-            self.url, re._pattern_type) else self.url
-        other_url = other.url.pattern if isinstance(
-            other.url, re._pattern_type) else other.url
+        self_url = self.url.pattern if isinstance(self.url,
+                                                  Pattern) else self.url
+        other_url = other.url.pattern if isinstance(other.url,
+                                                    Pattern) else other.url
 
         return self_url == other_url
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def _url_matches_strict(self, url, other):
@@ -169,37 +211,33 @@
         url_qsl = sorted(parse_qsl(url_parsed.query))
         other_qsl = sorted(parse_qsl(other_parsed.query))
 
         if len(url_qsl) != len(other_qsl):
             return False
 
         for (a_k, a_v), (b_k, b_v) in zip(url_qsl, other_qsl):
-            if not isinstance(a_k, six.text_type):
-                a_k = a_k.decode('utf-8')
-            if not isinstance(b_k, six.text_type):
-                b_k = b_k.decode('utf-8')
             if a_k != b_k:
                 return False
-            if not isinstance(a_v, six.text_type):
-                a_v = a_v.decode('utf-8')
-            if not isinstance(b_v, six.text_type):
-                b_v = b_v.decode('utf-8')
             if a_v != b_v:
                 return False
         return True
 
     def _url_matches(self, url, other, match_querystring=False):
         if _is_string(url):
+            if _has_unicode(url):
+                url = _clean_unicode(url)
+                if not isinstance(other, six.text_type):
+                    other = other.encode('ascii').decode('utf8')
             if match_querystring:
                 return self._url_matches_strict(url, other)
             else:
                 url_without_qs = url.split('?', 1)[0]
                 other_without_qs = other.split('?', 1)[0]
                 return url_without_qs == other_without_qs
-        elif isinstance(url, re._pattern_type) and url.match(other):
+        elif isinstance(url, Pattern) and url.match(other):
             return True
         else:
             return False
 
     def get_headers(self):
         headers = {}
         if self.content_type is not None:
@@ -312,20 +350,22 @@
     POST = 'POST'
     PUT = 'PUT'
     response_callback = None
 
     def __init__(self,
                  assert_all_requests_are_fired=True,
                  response_callback=None,
-                 passthru_prefixes=()):
+                 passthru_prefixes=(),
+                 target='requests.adapters.HTTPAdapter.send'):
         self._calls = CallList()
         self.reset()
         self.assert_all_requests_are_fired = assert_all_requests_are_fired
         self.response_callback = response_callback
         self.passthru_prefixes = tuple(passthru_prefixes)
+        self.target = target
 
     def reset(self):
         self._matches = []
         self._calls.reset()
 
     def add(
             self,
@@ -385,14 +425,16 @@
         Register a URL prefix to passthru any non-matching mock requests to.
 
         For example, to allow any request to 'https://example.com', but require
         mocks for the remainder, you would add the prefix as so:
 
         >>> responses.add_passthru('https://example.com')
         """
+        if _has_unicode(prefix):
+            prefix = _clean_unicode(prefix)
         self.passthru_prefixes += (prefix, )
 
     def remove(self, method_or_response=None, url=None):
         """
         Removes a response previously added using ``add()``, identified
         either by a response object inheriting ``BaseResponse`` or
         ``method`` and ``url``. Removes all matching responses.
@@ -522,24 +564,18 @@
 
         response = resp_callback(response) if resp_callback else response
         match.call_count += 1
         self._calls.add(request, response)
         return response
 
     def start(self):
-        try:
-            from unittest import mock
-        except ImportError:
-            import mock
-
         def unbound_on_send(adapter, request, *a, **kwargs):
             return self._on_request(adapter, request, *a, **kwargs)
 
-        self._patcher = mock.patch('requests.adapters.HTTPAdapter.send',
-                                   unbound_on_send)
+        self._patcher = std_mock.patch(target=self.target, new=unbound_on_send)
         self._patcher.start()
 
     def stop(self, allow_assert=True):
         self._patcher.stop()
         if not self.assert_all_requests_are_fired:
             return
         if not allow_assert:
```

### Comparing `responses-0.8.1/setup.py` & `responses-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 if 'test' in sys.argv:
     setup_requires.append('pytest')
 
 install_requires = [
     'requests>=2.0',
     'cookies',
-    'six',
+    'six'
 ]
 
 tests_require = [
     'pytest',
     'coverage >= 3.7.1, < 5.0.0',
     'pytest-cov',
     'pytest-localserver',
@@ -65,15 +65,15 @@
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 setup(
     name='responses',
-    version='0.8.1',
+    version='0.9.0',
     author='David Cramer',
     description=(
         'A utility library for mocking out the `requests` Python library.'),
     url='https://github.com/getsentry/responses',
     license='Apache 2.0',
     long_description=open('README.rst').read(),
     py_modules=['responses', 'test_responses'],
```

### Comparing `responses-0.8.1/test_responses.py` & `responses-0.9.0/test_responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -644,29 +644,44 @@
             assert status_codes == [301, 301, 200]
         assert_reset()
 
     run()
     assert_reset()
 
 
-def test_handles_chinese_url():
+def test_handles_unicode_querystring():
     url = u'http://example.com/test?type=2&ie=utf8&query=汉字'
 
     @responses.activate
     def run():
         responses.add(responses.GET, url, body='test', match_querystring=True)
 
         resp = requests.get(url)
 
         assert_response(resp, 'test')
 
     run()
     assert_reset()
 
 
+def test_handles_unicode_url():
+    url = u'http://www.संजाल.भारत/hi/वेबसाइट-डिजाइन'
+
+    @responses.activate
+    def run():
+        responses.add(responses.GET, url, body='test')
+
+        resp = requests.get(url)
+
+        assert_response(resp, 'test')
+
+    run()
+    assert_reset()
+
+
 def test_headers():
     @responses.activate
     def run():
         responses.add(
             responses.GET,
             'http://example.com',
             body='',
@@ -757,7 +772,30 @@
         responses.add(
             method=responses.GET, url='http://example.com', body='OK')
         resp = requests.get('http://example.com')
         assert_response(resp, 'OK')
 
     run()
     assert_reset()
+
+
+def test_passthru_unicode():
+    @responses.activate
+    def run():
+        with responses.RequestsMock() as m:
+            url = u'http://موقع.وزارة-الاتصالات.مصر/'
+            clean_url = 'http://xn--4gbrim.xn----ymcbaaajlc6dj7bxne2c.xn--wgbh1c/'
+            m.add_passthru(url)
+            assert m.passthru_prefixes[0] == clean_url
+
+    run()
+    assert_reset()
+
+
+def test_custom_target(monkeypatch):
+    requests_mock = responses.RequestsMock(target='something.else')
+    std_mock_mock = responses.std_mock.MagicMock()
+    patch_mock = std_mock_mock.patch
+    monkeypatch.setattr(responses, 'std_mock', std_mock_mock)
+    requests_mock.start()
+    assert len(patch_mock.call_args_list) == 1
+    assert patch_mock.call_args[1]['target'] == 'something.else'
```

