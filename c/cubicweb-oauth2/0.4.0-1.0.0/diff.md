# Comparing `tmp/cubicweb-oauth2-0.4.0.tar.gz` & `tmp/cubicweb-oauth2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-oauth2-0.4.0.tar", last modified: Thu May  4 09:33:52 2023, max compression
+gzip compressed data, was "cubicweb-oauth2-1.0.0.tar", last modified: Tue Jul 25 14:58:27 2023, max compression
```

## Comparing `cubicweb-oauth2-0.4.0.tar` & `cubicweb-oauth2-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      436 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/MANIFEST.in
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2840 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/PKG-INFO
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2438 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/README.rst
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.129850 cubicweb-oauth2-0.4.0/cubicweb_oauth2/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      243 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/__init__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)      693 2023-05-04 08:51:51.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/__pkginfo__.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     8335 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/auth.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/
--rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/en.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/es.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)      298 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/i18n/fr.po
--rw-r--r--   0 fferry    (1000) fferry    (1000)     5123 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/site_cubicweb.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2701 2023-03-21 09:36:29.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2/views.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.129850 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2840 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 fferry    (1000) fferry    (1000)      646 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       42 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/entry_points.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-03-21 09:16:50.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 fferry    (1000) fferry    (1000)       72 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/requires.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       16 2023-05-04 09:33:52.000000 cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/top_level.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/setup.cfg
--rw-r--r--   0 fferry    (1000) fferry    (1000)     2637 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/setup.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/test/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        0 2023-03-21 09:36:32.000000 cubicweb-oauth2-0.4.0/test/__init__.py
-drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-05-04 09:33:52.133850 cubicweb-oauth2-0.4.0/test/data/
--rw-r--r--   0 fferry    (1000) fferry    (1000)        7 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/data/bootstrap_cubes
--rw-r--r--   0 fferry    (1000) fferry    (1000)     3243 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/jwt.key
--rw-r--r--   0 fferry    (1000) fferry    (1000)      800 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test/jwt.pub
--rw-r--r--   0 fferry    (1000) fferry    (1000)     6935 2023-03-21 09:36:32.000000 cubicweb-oauth2-0.4.0/test/test_oauth2.py
--rw-r--r--   0 fferry    (1000) fferry    (1000)       25 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/test-requirements.txt
--rw-r--r--   0 fferry    (1000) fferry    (1000)     1916 2023-03-21 09:16:09.000000 cubicweb-oauth2-0.4.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.830367 cubicweb-oauth2-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-25 14:58:27.830367 cubicweb-oauth2-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.822367 cubicweb-oauth2-1.0.0/cubicweb_oauth2/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.826367 cubicweb-oauth2-1.0.0/cubicweb_oauth2/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.826367 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-25 14:58:27.000000 cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:58:27.830367 cubicweb-oauth2-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.830367 cubicweb-oauth2-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:27.830367 cubicweb-oauth2-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test/jwt.key
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test/jwt.pub
+-rw-rw-rw-   0 root         (0) root         (0)     7115 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test/test_oauth2.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-25 14:57:32.000000 cubicweb-oauth2-1.0.0/tox.ini
```

### Comparing `cubicweb-oauth2-0.4.0/PKG-INFO` & `cubicweb-oauth2-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-oauth2
-Version: 0.4.0
+Version: 1.0.0
 Summary: Oauth2/OpenID authentication for cubicweb
 Home-page: http://www.cubicweb.org/project/cubicweb-oauth2
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-oauth2-0.4.0/README.rst` & `cubicweb-oauth2-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2/__pkginfo__.py` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2/__pkginfo__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: disable=W0622
 """cubicweb-oauth2 application packaging information"""
 
 
 modname = "cubicweb_oauth2"
 distname = "cubicweb-oauth2"
 
-numversion = (0, 4, 0)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Oauth2/OpenID authentication for cubicweb"
 web = "http://www.cubicweb.org/project/%s" % distname
 
 __depends__ = {
-    "cubicweb": ">=3.38.0,<3.39.0",
+    "cubicweb": ">=4.0.0,<5.0.0",
     "authlib": ">=1.2.0,<1.3.0",
     "requests": ">=2.28.0,<2.29.0",
 }
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
```

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2/auth.py` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2/site_cubicweb.py` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2/views.py` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/PKG-INFO` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-oauth2
-Version: 0.4.0
+Version: 1.0.0
 Summary: Oauth2/OpenID authentication for cubicweb
 Home-page: http://www.cubicweb.org/project/cubicweb-oauth2
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-oauth2-0.4.0/cubicweb_oauth2.egg-info/SOURCES.txt` & `cubicweb-oauth2-1.0.0/cubicweb_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/setup.py` & `cubicweb-oauth2-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/test/jwt.key` & `cubicweb-oauth2-1.0.0/test/jwt.key`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/test/jwt.pub` & `cubicweb-oauth2-1.0.0/test/jwt.pub`

 * *Files identical despite different names*

### Comparing `cubicweb-oauth2-0.4.0/test/test_oauth2.py` & `cubicweb-oauth2-1.0.0/test/test_oauth2.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 import os
 import unittest
 import urllib.parse
 
 from authlib.jose import jwt
 import responses
+from cubicweb.devtools import BASE_URL
 
-from cubicweb.pyramid.test import PyramidCWTest
+from cubicweb_web.devtools.testlib import PyramidWebCWTC
 
 from cubicweb_oauth2.auth import Oauth2
 
 HERE = os.path.dirname(__file__)
 
 
 def create_token(payload):
@@ -33,16 +34,19 @@
     # ssh-keygen -t rsa -b 4096 -m PEM -f jwt.key
     # openssl rsa -in jwt.key -pubout -outform PEM -out jwt.pub
     with open(os.path.join(HERE, "jwt.key")) as f:
         privkey = f.read()
     return jwt.encode({"alg": "RS256"}, payload, privkey).decode()
 
 
-class AuthenticationTC(PyramidCWTest):
-    settings = {"cubicweb.bwcompat": False}
+class AuthenticationTC(PyramidWebCWTC):
+    settings = {
+        **PyramidWebCWTC.settings,
+        "cubicweb.includes": ["cubicweb.pyramid.auth", "cubicweb.pyramid.session"],
+    }
 
     @classmethod
     def init_config(cls, config):
         super().init_config(config)
         config.global_set_option("oauth2-enabled", True)
         config.global_set_option("oauth2-client-id", "id")
         config.global_set_option("oauth2-client-secret", "secret")
@@ -50,58 +54,60 @@
         config.global_set_option("oauth2-token-url", "https://provider/token")
         config.global_set_option("oauth2-jwk-path", os.path.join(HERE, "jwt.pub"))
         config.global_set_option("oauth2-provider-name", "Logilab")
 
     def test_login_page(self):
         resp = self.webapp.get("/login?postlogin_path=/schema", status=200)
         assert (
-            b'<a href="https://localhost:80/oauth2/start?rd=%2Fschema">'
-            b'<button class="validateButton" type="button" '
-            b'value="Log in with Logilab">Log in with Logilab</button></a>'
-        ) in resp.body
+            f'<a href="{BASE_URL}oauth2/start?rd=%2Fschema">'
+            f'<button class="validateButton" type="button" '
+            f'value="Log in with Logilab">Log in with Logilab</button></a>'
+        ).encode("utf-8") in resp.body
 
     def test_login_page_auto_login(self):
         self.set_option("oauth2-auto-login", True)
         try:
             resp = self.webapp.get("/login?postlogin_path=/schema", status=302)
         finally:
             self.set_option("oauth2-auto-login", False)
-        assert resp.location == "https://localhost:80/oauth2/start?rd=%2Fschema"
+        assert resp.location == f"{BASE_URL}oauth2/start?rd=%2Fschema"
 
     def test_force_login(self):
         self.set_option("oauth2-force-login", True)
         try:
-            resp = self.webapp.get("/1", status=401)
+            resp = self.webapp.get("/poulet", status=401)
         finally:
             self.set_option("oauth2-force-login", False)
         assert resp.body == (
-            b'<!DOCTYPE html><html><head><meta http-equiv="refresh" content="0; '
-            b'url=https://localhost:80/oauth2/start?rd=https%3A%2F%2Flocalhost%3A80%2F1" />'
-            b"</head></html>"
-        )
+            f'<!DOCTYPE html><html><head><meta http-equiv="refresh" content="0; '
+            f'url={BASE_URL}oauth2/start?rd={urllib.parse.quote(BASE_URL, safe="")}poulet" />'
+            f"</head></html>"
+        ).encode("utf-8")
 
     def test_force_login_signedrequest(self):
         # we should not block requests with signedrequest token authentication
         self.set_option("oauth2-force-login", True)
         try:
-            self.webapp.get("/1", headers={"Authorization": "Cubicweb foo"}, status=404)
+            self.webapp.get(
+                "/poulet", headers={"Authorization": "Cubicweb foo"}, status=404
+            )
         finally:
             self.set_option("oauth2-force-login", False)
 
     @responses.activate
     def test_full_login(self):
         resp = self.webapp.get("/oauth2/start?rd=/page", status=302)
         url = urllib.parse.urlparse(resp.location)
         assert url.scheme + "://" + url.netloc + url.path == "https://provider/auth"
         qs = urllib.parse.parse_qs(url.query)
         state = qs["state"][0]
         assert qs == {
             "response_type": ["code"],
             "client_id": ["id"],
-            "redirect_uri": ["https://localhost:80/oauth2/callback?rd=%2Fpage"],
+            "redirect_uri": [f"{BASE_URL}oauth2/callback?rd=%2Fpage"],
             "scope": ["openid email profile"],
             "state": [state],
         }
         resp = self.webapp.get(
             "/oauth2/callback?rd=%2Fpage&state=invalid",
             status=400,
         )
@@ -122,15 +128,15 @@
             json={"id_token": create_token(token)},
             status=200,
         )
         resp = self.webapp.get(
             "/oauth2/callback?rd=%2Fpage&state={}&code=sesame".format(state),
             status=302,
         )
-        assert resp.location == "https://localhost:80/page"
+        assert resp.location == f"{BASE_URL}page"
         with self.admin_access.cnx() as cnx:
             user = cnx.find("CWUser", login="jdoe").one()
             assert (user.surname, user.firstname) == ("Doe", "John")
             assert [a.address for a in user.use_email] == ["jdoe@logilab.fr"]
 
 
 class Oauth2TC(unittest.TestCase):
```

### Comparing `cubicweb-oauth2-0.4.0/tox.ini` & `cubicweb-oauth2-1.0.0/tox.ini`

 * *Files identical despite different names*

