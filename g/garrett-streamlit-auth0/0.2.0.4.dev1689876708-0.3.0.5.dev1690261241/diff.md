# Comparing `tmp/garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar.gz` & `tmp/garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar", last modified: Thu Jul 20 18:11:48 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar", last modified: Tue Jul 25 05:00:42 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708.tar` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   337460 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.13833558.js
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.1dbfa948.css
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:11:48.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:11:48.524284 garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 18:11:36.000000 garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.024566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.016566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.1dbfa948.css
+-rw-r--r--   0 runner    (1001) docker     (123)   337632 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.84bf3e3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:00:42.032566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.py
```

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/LICENSE` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/README.md` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/README.md`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import streamlit.components.v1 as components
 
-# _RELEASE = False
-_RELEASE = True
-
+_RELEASE = False if "auth0_component_develop" in os.environ else True
 
 if not _RELEASE:
     _login_button = components.declare_component(
         "login_button",
         url="http://localhost:3000",  # vite dev server port
     )
 else:
@@ -117,33 +115,33 @@
             return False
     elif type(val) is int:
         return False if val == 0 else True
     elif type(val) is float:
         return False if val == 0 else True
     raise ValueError("invalid truth value %r" % (val,))
 
-if not _RELEASE:
-    import streamlit as st
-    from dotenv import load_dotenv
-    import os
-
-    load_dotenv()
-
-    clientId = os.environ["clientId"]
-    domain = os.environ["domain"]
-    audience = os.getenv("audience")
-    issuer = os.getenv("issuer")
-    debug_logs = os.getenv("debug_logs", False)
-
-    st.subheader("Login component")
-    user_info = login_button(
-        clientId,
-        domain=domain,
-        audience=audience,
-        issuer=issuer,
-        debug_logs=debug_logs
-    )
-    # user_info = login_button(clientId = "...", domain = "...")
-    st.write("User info")
-    st.write(user_info)
-    if st.button("rerun"):
-        st.experimental_rerun()
+# if not _RELEASE:
+#     import streamlit as st
+#     from dotenv import load_dotenv
+#     import os
+
+#     load_dotenv()
+
+#     clientId = os.environ["clientId"]
+#     domain = os.environ["domain"]
+#     audience = os.getenv("audience")
+#     issuer = os.getenv("issuer")
+#     debug_logs = os.getenv("debug_logs", False)
+
+#     st.subheader("Login component")
+#     user_info = login_button(
+#         clientId,
+#         domain=domain,
+#         audience=audience,
+#         issuer=issuer,
+#         debug_logs=debug_logs
+#     )
+#     # user_info = login_button(clientId = "...", domain = "...")
+#     st.write("User info")
+#     st.write(user_info)
+#     if st.button("rerun"):
+#         st.experimental_rerun()
```

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.13833558.js` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.84bf3e3f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,58 +19,58 @@
     function r(s) {
         if (s.ep) return;
         s.ep = !0;
         const o = n(s);
         fetch(s.href, o)
     }
 })();
-var xd = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+var Ld = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-function Ld(e) {
+function Dd(e) {
     return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e
 }
-var bl = {
+var gl = {
         exports: {}
     },
     X = {};
 /** @license React v16.13.1
  * react-is.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 var pt = typeof Symbol == "function" && Symbol.for,
-    na = pt ? Symbol.for("react.element") : 60103,
-    ra = pt ? Symbol.for("react.portal") : 60106,
+    Qo = pt ? Symbol.for("react.element") : 60103,
+    ta = pt ? Symbol.for("react.portal") : 60106,
     cs = pt ? Symbol.for("react.fragment") : 60107,
     us = pt ? Symbol.for("react.strict_mode") : 60108,
     ls = pt ? Symbol.for("react.profiler") : 60114,
     fs = pt ? Symbol.for("react.provider") : 60109,
     hs = pt ? Symbol.for("react.context") : 60110,
-    ia = pt ? Symbol.for("react.async_mode") : 60111,
+    ea = pt ? Symbol.for("react.async_mode") : 60111,
     ds = pt ? Symbol.for("react.concurrent_mode") : 60111,
     ps = pt ? Symbol.for("react.forward_ref") : 60112,
     ys = pt ? Symbol.for("react.suspense") : 60113,
-    Dd = pt ? Symbol.for("react.suspense_list") : 60120,
+    kd = pt ? Symbol.for("react.suspense_list") : 60120,
     bs = pt ? Symbol.for("react.memo") : 60115,
     ms = pt ? Symbol.for("react.lazy") : 60116,
-    kd = pt ? Symbol.for("react.block") : 60121,
-    Ed = pt ? Symbol.for("react.fundamental") : 60117,
-    Ud = pt ? Symbol.for("react.responder") : 60118,
-    Nd = pt ? Symbol.for("react.scope") : 60119;
+    Ed = pt ? Symbol.for("react.block") : 60121,
+    Ud = pt ? Symbol.for("react.fundamental") : 60117,
+    Nd = pt ? Symbol.for("react.responder") : 60118,
+    Md = pt ? Symbol.for("react.scope") : 60119;
 
-function Rt(e) {
+function Vt(e) {
     if (typeof e == "object" && e !== null) {
         var t = e.$$typeof;
         switch (t) {
-            case na:
+            case Qo:
                 switch (e = e.type, e) {
-                    case ia:
+                    case ea:
                     case ds:
                     case cs:
                     case ls:
                     case us:
                     case ys:
                         return e;
                     default:
@@ -81,118 +81,118 @@
                             case bs:
                             case fs:
                                 return e;
                             default:
                                 return t
                         }
                 }
-            case ra:
+            case ta:
                 return t
         }
     }
 }
 
-function ml(e) {
-    return Rt(e) === ds
+function vl(e) {
+    return Vt(e) === ds
 }
-X.AsyncMode = ia;
+X.AsyncMode = ea;
 X.ConcurrentMode = ds;
 X.ContextConsumer = hs;
 X.ContextProvider = fs;
-X.Element = na;
+X.Element = Qo;
 X.ForwardRef = ps;
 X.Fragment = cs;
 X.Lazy = ms;
 X.Memo = bs;
-X.Portal = ra;
+X.Portal = ta;
 X.Profiler = ls;
 X.StrictMode = us;
 X.Suspense = ys;
 X.isAsyncMode = function(e) {
-    return ml(e) || Rt(e) === ia
+    return vl(e) || Vt(e) === ea
 };
-X.isConcurrentMode = ml;
+X.isConcurrentMode = vl;
 X.isContextConsumer = function(e) {
-    return Rt(e) === hs
+    return Vt(e) === hs
 };
 X.isContextProvider = function(e) {
-    return Rt(e) === fs
+    return Vt(e) === fs
 };
 X.isElement = function(e) {
-    return typeof e == "object" && e !== null && e.$$typeof === na
+    return typeof e == "object" && e !== null && e.$$typeof === Qo
 };
 X.isForwardRef = function(e) {
-    return Rt(e) === ps
+    return Vt(e) === ps
 };
 X.isFragment = function(e) {
-    return Rt(e) === cs
+    return Vt(e) === cs
 };
 X.isLazy = function(e) {
-    return Rt(e) === ms
+    return Vt(e) === ms
 };
 X.isMemo = function(e) {
-    return Rt(e) === bs
+    return Vt(e) === bs
 };
 X.isPortal = function(e) {
-    return Rt(e) === ra
+    return Vt(e) === ta
 };
 X.isProfiler = function(e) {
-    return Rt(e) === ls
+    return Vt(e) === ls
 };
 X.isStrictMode = function(e) {
-    return Rt(e) === us
+    return Vt(e) === us
 };
 X.isSuspense = function(e) {
-    return Rt(e) === ys
+    return Vt(e) === ys
 };
 X.isValidElementType = function(e) {
-    return typeof e == "string" || typeof e == "function" || e === cs || e === ds || e === ls || e === us || e === ys || e === Dd || typeof e == "object" && e !== null && (e.$$typeof === ms || e.$$typeof === bs || e.$$typeof === fs || e.$$typeof === hs || e.$$typeof === ps || e.$$typeof === Ed || e.$$typeof === Ud || e.$$typeof === Nd || e.$$typeof === kd)
+    return typeof e == "string" || typeof e == "function" || e === cs || e === ds || e === ls || e === us || e === ys || e === kd || typeof e == "object" && e !== null && (e.$$typeof === ms || e.$$typeof === bs || e.$$typeof === fs || e.$$typeof === hs || e.$$typeof === ps || e.$$typeof === Ud || e.$$typeof === Nd || e.$$typeof === Md || e.$$typeof === Ed)
 };
-X.typeOf = Rt;
+X.typeOf = Vt;
 (function(e) {
     e.exports = X
-})(bl);
-var gl = bl.exports,
-    Md = {
+})(gl);
+var wl = gl.exports,
+    Cd = {
         $$typeof: !0,
         render: !0,
         defaultProps: !0,
         displayName: !0,
         propTypes: !0
     },
-    Cd = {
+    Rd = {
         $$typeof: !0,
         compare: !0,
         defaultProps: !0,
         displayName: !0,
         propTypes: !0,
         type: !0
     },
-    vl = {};
-vl[gl.ForwardRef] = Md;
-vl[gl.Memo] = Cd;
-var wl = {
+    _l = {};
+_l[wl.ForwardRef] = Cd;
+_l[wl.Memo] = Rd;
+var Sl = {
         exports: {}
     },
     q = {};
 /*
 object-assign
 (c) Sindre Sorhus
 @license MIT
 */
-var Lc = Object.getOwnPropertySymbols,
-    Rd = Object.prototype.hasOwnProperty,
-    Vd = Object.prototype.propertyIsEnumerable;
+var kc = Object.getOwnPropertySymbols,
+    Vd = Object.prototype.hasOwnProperty,
+    jd = Object.prototype.propertyIsEnumerable;
 
-function jd(e) {
+function Pd(e) {
     if (e == null) throw new TypeError("Object.assign cannot be called with null or undefined");
     return Object(e)
 }
 
-function Pd() {
+function zd() {
     try {
         if (!Object.assign) return !1;
         var e = new String("abc");
         if (e[5] = "de", Object.getOwnPropertyNames(e)[0] === "5") return !1;
         for (var t = {}, n = 0; n < 10; n++) t["_" + String.fromCharCode(n)] = n;
         var r = Object.getOwnPropertyNames(t).map(function(o) {
             return t[o]
@@ -202,161 +202,161 @@
         return "abcdefghijklmnopqrst".split("").forEach(function(o) {
             s[o] = o
         }), Object.keys(Object.assign({}, s)).join("") === "abcdefghijklmnopqrst"
     } catch {
         return !1
     }
 }
-var zd = Pd() ? Object.assign : function(e, t) {
-    for (var n, r = jd(e), s, o = 1; o < arguments.length; o++) {
+var Wd = zd() ? Object.assign : function(e, t) {
+    for (var n, r = Pd(e), s, o = 1; o < arguments.length; o++) {
         n = Object(arguments[o]);
-        for (var i in n) Rd.call(n, i) && (r[i] = n[i]);
-        if (Lc) {
-            s = Lc(n);
-            for (var a = 0; a < s.length; a++) Vd.call(n, s[a]) && (r[s[a]] = n[s[a]])
+        for (var i in n) Vd.call(n, i) && (r[i] = n[i]);
+        if (kc) {
+            s = kc(n);
+            for (var a = 0; a < s.length; a++) jd.call(n, s[a]) && (r[s[a]] = n[s[a]])
         }
     }
     return r
 };
 /** @license React v16.14.0
  * react.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
-var sa = zd,
-    te = typeof Symbol == "function" && Symbol.for,
-    Wr = te ? Symbol.for("react.element") : 60103,
-    Wd = te ? Symbol.for("react.portal") : 60106,
-    $d = te ? Symbol.for("react.fragment") : 60107,
-    Yd = te ? Symbol.for("react.strict_mode") : 60108,
-    Gd = te ? Symbol.for("react.profiler") : 60114,
-    Kd = te ? Symbol.for("react.provider") : 60109,
-    Zd = te ? Symbol.for("react.context") : 60110,
-    Hd = te ? Symbol.for("react.forward_ref") : 60112,
-    Jd = te ? Symbol.for("react.suspense") : 60113,
-    Xd = te ? Symbol.for("react.memo") : 60115,
-    qd = te ? Symbol.for("react.lazy") : 60116,
-    Dc = typeof Symbol == "function" && Symbol.iterator;
+var na = Wd,
+    ee = typeof Symbol == "function" && Symbol.for,
+    Wr = ee ? Symbol.for("react.element") : 60103,
+    $d = ee ? Symbol.for("react.portal") : 60106,
+    Yd = ee ? Symbol.for("react.fragment") : 60107,
+    Gd = ee ? Symbol.for("react.strict_mode") : 60108,
+    Kd = ee ? Symbol.for("react.profiler") : 60114,
+    Zd = ee ? Symbol.for("react.provider") : 60109,
+    Hd = ee ? Symbol.for("react.context") : 60110,
+    Jd = ee ? Symbol.for("react.forward_ref") : 60112,
+    Xd = ee ? Symbol.for("react.suspense") : 60113,
+    qd = ee ? Symbol.for("react.memo") : 60115,
+    Qd = ee ? Symbol.for("react.lazy") : 60116,
+    Ec = typeof Symbol == "function" && Symbol.iterator;
 
 function $r(e) {
     for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
     return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
 }
-var _l = {
+var Il = {
         isMounted: function() {
             return !1
         },
         enqueueForceUpdate: function() {},
         enqueueReplaceState: function() {},
         enqueueSetState: function() {}
     },
-    Sl = {};
+    Tl = {};
 
 function cr(e, t, n) {
-    this.props = e, this.context = t, this.refs = Sl, this.updater = n || _l
+    this.props = e, this.context = t, this.refs = Tl, this.updater = n || Il
 }
 cr.prototype.isReactComponent = {};
 cr.prototype.setState = function(e, t) {
     if (typeof e != "object" && typeof e != "function" && e != null) throw Error($r(85));
     this.updater.enqueueSetState(this, e, t, "setState")
 };
 cr.prototype.forceUpdate = function(e) {
     this.updater.enqueueForceUpdate(this, e, "forceUpdate")
 };
 
-function Il() {}
-Il.prototype = cr.prototype;
+function Al() {}
+Al.prototype = cr.prototype;
 
-function oa(e, t, n) {
-    this.props = e, this.context = t, this.refs = Sl, this.updater = n || _l
+function ra(e, t, n) {
+    this.props = e, this.context = t, this.refs = Tl, this.updater = n || Il
 }
-var aa = oa.prototype = new Il;
-aa.constructor = oa;
-sa(aa, cr.prototype);
-aa.isPureReactComponent = !0;
-var ca = {
+var ia = ra.prototype = new Al;
+ia.constructor = ra;
+na(ia, cr.prototype);
+ia.isPureReactComponent = !0;
+var sa = {
         current: null
     },
-    Tl = Object.prototype.hasOwnProperty,
-    Al = {
+    Bl = Object.prototype.hasOwnProperty,
+    Ol = {
         key: !0,
         ref: !0,
         __self: !0,
         __source: !0
     };
 
-function Bl(e, t, n) {
+function Fl(e, t, n) {
     var r, s = {},
         o = null,
         i = null;
     if (t != null)
-        for (r in t.ref !== void 0 && (i = t.ref), t.key !== void 0 && (o = "" + t.key), t) Tl.call(t, r) && !Al.hasOwnProperty(r) && (s[r] = t[r]);
+        for (r in t.ref !== void 0 && (i = t.ref), t.key !== void 0 && (o = "" + t.key), t) Bl.call(t, r) && !Ol.hasOwnProperty(r) && (s[r] = t[r]);
     var a = arguments.length - 2;
     if (a === 1) s.children = n;
     else if (1 < a) {
         for (var c = Array(a), u = 0; u < a; u++) c[u] = arguments[u + 2];
         s.children = c
     }
     if (e && e.defaultProps)
         for (r in a = e.defaultProps, a) s[r] === void 0 && (s[r] = a[r]);
     return {
         $$typeof: Wr,
         type: e,
         key: o,
         ref: i,
         props: s,
-        _owner: ca.current
+        _owner: sa.current
     }
 }
 
-function Qd(e, t) {
+function tp(e, t) {
     return {
         $$typeof: Wr,
         type: e.type,
         key: t,
         ref: e.ref,
         props: e.props,
         _owner: e._owner
     }
 }
 
-function ua(e) {
+function oa(e) {
     return typeof e == "object" && e !== null && e.$$typeof === Wr
 }
 
-function tp(e) {
+function ep(e) {
     var t = {
         "=": "=0",
         ":": "=2"
     };
     return "$" + ("" + e).replace(/[=:]/g, function(n) {
         return t[n]
     })
 }
-var Ol = /\/+/g,
+var xl = /\/+/g,
     Ui = [];
 
-function Fl(e, t, n, r) {
+function Ll(e, t, n, r) {
     if (Ui.length) {
         var s = Ui.pop();
         return s.result = e, s.keyPrefix = t, s.func = n, s.context = r, s.count = 0, s
     }
     return {
         result: e,
         keyPrefix: t,
         func: n,
         context: r,
         count: 0
     }
 }
 
-function xl(e) {
+function Dl(e) {
     e.result = null, e.keyPrefix = null, e.func = null, e.context = null, e.count = 0, 10 > Ui.length && Ui.push(e)
 }
 
 function wo(e, t, n, r) {
     var s = typeof e;
     (s === "undefined" || s === "boolean") && (e = null);
     var o = !1;
@@ -365,116 +365,116 @@
         case "string":
         case "number":
             o = !0;
             break;
         case "object":
             switch (e.$$typeof) {
                 case Wr:
-                case Wd:
+                case $d:
                     o = !0
             }
     }
     if (o) return n(r, e, t === "" ? "." + js(e, 0) : t), 1;
     if (o = 0, t = t === "" ? "." : t + ":", Array.isArray(e))
         for (var i = 0; i < e.length; i++) {
             s = e[i];
             var a = t + js(s, i);
             o += wo(s, a, n, r)
-        } else if (e === null || typeof e != "object" ? a = null : (a = Dc && e[Dc] || e["@@iterator"], a = typeof a == "function" ? a : null), typeof a == "function")
+        } else if (e === null || typeof e != "object" ? a = null : (a = Ec && e[Ec] || e["@@iterator"], a = typeof a == "function" ? a : null), typeof a == "function")
             for (e = a.call(e), i = 0; !(s = e.next()).done;) s = s.value, a = t + js(s, i++), o += wo(s, a, n, r);
         else if (s === "object") throw n = "" + e, Error($r(31, n === "[object Object]" ? "object with keys {" + Object.keys(e).join(", ") + "}" : n, ""));
     return o
 }
 
 function _o(e, t, n) {
     return e == null ? 0 : wo(e, "", t, n)
 }
 
 function js(e, t) {
-    return typeof e == "object" && e !== null && e.key != null ? tp(e.key) : t.toString(36)
+    return typeof e == "object" && e !== null && e.key != null ? ep(e.key) : t.toString(36)
 }
 
-function ep(e, t) {
+function np(e, t) {
     e.func.call(e.context, t, e.count++)
 }
 
-function np(e, t, n) {
+function rp(e, t, n) {
     var r = e.result,
         s = e.keyPrefix;
     e = e.func.call(e.context, t, e.count++), Array.isArray(e) ? So(e, r, n, function(o) {
         return o
-    }) : e != null && (ua(e) && (e = Qd(e, s + (!e.key || t && t.key === e.key ? "" : ("" + e.key).replace(Ol, "$&/") + "/") + n)), r.push(e))
+    }) : e != null && (oa(e) && (e = tp(e, s + (!e.key || t && t.key === e.key ? "" : ("" + e.key).replace(xl, "$&/") + "/") + n)), r.push(e))
 }
 
 function So(e, t, n, r, s) {
     var o = "";
-    n != null && (o = ("" + n).replace(Ol, "$&/") + "/"), t = Fl(t, o, r, s), _o(e, np, t), xl(t)
+    n != null && (o = ("" + n).replace(xl, "$&/") + "/"), t = Ll(t, o, r, s), _o(e, rp, t), Dl(t)
 }
-var Ll = {
+var kl = {
     current: null
 };
 
 function Le() {
-    var e = Ll.current;
+    var e = kl.current;
     if (e === null) throw Error($r(321));
     return e
 }
-var rp = {
-    ReactCurrentDispatcher: Ll,
+var ip = {
+    ReactCurrentDispatcher: kl,
     ReactCurrentBatchConfig: {
         suspense: null
     },
-    ReactCurrentOwner: ca,
+    ReactCurrentOwner: sa,
     IsSomeRendererActing: {
         current: !1
     },
-    assign: sa
+    assign: na
 };
 q.Children = {
     map: function(e, t, n) {
         if (e == null) return e;
         var r = [];
         return So(e, r, null, t, n), r
     },
     forEach: function(e, t, n) {
         if (e == null) return e;
-        t = Fl(null, null, t, n), _o(e, ep, t), xl(t)
+        t = Ll(null, null, t, n), _o(e, np, t), Dl(t)
     },
     count: function(e) {
         return _o(e, function() {
             return null
         }, null)
     },
     toArray: function(e) {
         var t = [];
         return So(e, t, null, function(n) {
             return n
         }), t
     },
     only: function(e) {
-        if (!ua(e)) throw Error($r(143));
+        if (!oa(e)) throw Error($r(143));
         return e
     }
 };
 q.Component = cr;
-q.Fragment = $d;
-q.Profiler = Gd;
-q.PureComponent = oa;
-q.StrictMode = Yd;
-q.Suspense = Jd;
-q.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = rp;
+q.Fragment = Yd;
+q.Profiler = Kd;
+q.PureComponent = ra;
+q.StrictMode = Gd;
+q.Suspense = Xd;
+q.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = ip;
 q.cloneElement = function(e, t, n) {
     if (e == null) throw Error($r(267, e));
-    var r = sa({}, e.props),
+    var r = na({}, e.props),
         s = e.key,
         o = e.ref,
         i = e._owner;
     if (t != null) {
-        if (t.ref !== void 0 && (o = t.ref, i = ca.current), t.key !== void 0 && (s = "" + t.key), e.type && e.type.defaultProps) var a = e.type.defaultProps;
-        for (c in t) Tl.call(t, c) && !Al.hasOwnProperty(c) && (r[c] = t[c] === void 0 && a !== void 0 ? a[c] : t[c])
+        if (t.ref !== void 0 && (o = t.ref, i = sa.current), t.key !== void 0 && (s = "" + t.key), e.type && e.type.defaultProps) var a = e.type.defaultProps;
+        for (c in t) Bl.call(t, c) && !Ol.hasOwnProperty(c) && (r[c] = t[c] === void 0 && a !== void 0 ? a[c] : t[c])
     }
     var c = arguments.length - 2;
     if (c === 1) r.children = n;
     else if (1 < c) {
         a = Array(c);
         for (var u = 0; u < c; u++) a[u] = arguments[u + 2];
         r.children = a
@@ -486,54 +486,54 @@
         ref: o,
         props: r,
         _owner: i
     }
 };
 q.createContext = function(e, t) {
     return t === void 0 && (t = null), e = {
-        $$typeof: Zd,
+        $$typeof: Hd,
         _calculateChangedBits: t,
         _currentValue: e,
         _currentValue2: e,
         _threadCount: 0,
         Provider: null,
         Consumer: null
     }, e.Provider = {
-        $$typeof: Kd,
+        $$typeof: Zd,
         _context: e
     }, e.Consumer = e
 };
-q.createElement = Bl;
+q.createElement = Fl;
 q.createFactory = function(e) {
-    var t = Bl.bind(null, e);
+    var t = Fl.bind(null, e);
     return t.type = e, t
 };
 q.createRef = function() {
     return {
         current: null
     }
 };
 q.forwardRef = function(e) {
     return {
-        $$typeof: Hd,
+        $$typeof: Jd,
         render: e
     }
 };
-q.isValidElement = ua;
+q.isValidElement = oa;
 q.lazy = function(e) {
     return {
-        $$typeof: qd,
+        $$typeof: Qd,
         _ctor: e,
         _status: -1,
         _result: null
     }
 };
 q.memo = function(e, t) {
     return {
-        $$typeof: Xd,
+        $$typeof: qd,
         type: e,
         compare: t === void 0 ? null : t
     }
 };
 q.useCallback = function(e, t) {
     return Le().useCallback(e, t)
 };
@@ -561,33 +561,33 @@
 };
 q.useState = function(e) {
     return Le().useState(e)
 };
 q.version = "16.14.0";
 (function(e) {
     e.exports = q
-})(wl);
-const ip = Ld(wl.exports),
-    Dl = new WeakMap,
+})(Sl);
+const sp = Dd(Sl.exports),
+    El = new WeakMap,
     Io = new WeakMap;
 
 function et(e) {
-    const t = Dl.get(e);
+    const t = El.get(e);
     return console.assert(t != null, "'this' is expected an Event object, but got", e), t
 }
 
-function kc(e) {
+function Uc(e) {
     if (e.passiveListener != null) {
         typeof console < "u" && typeof console.error == "function" && console.error("Unable to preventDefault inside passive event listener invocation.", e.passiveListener);
         return
     }!e.event.cancelable || (e.canceled = !0, typeof e.event.preventDefault == "function" && e.event.preventDefault())
 }
 
 function Kn(e, t) {
-    Dl.set(this, {
+    El.set(this, {
         eventTarget: e,
         event: t,
         eventPhase: 2,
         currentTarget: e,
         canceled: !1,
         stopped: !1,
         immediateStopped: !1,
@@ -596,15 +596,15 @@
     }), Object.defineProperty(this, "isTrusted", {
         value: !1,
         enumerable: !0
     });
     const n = Object.keys(t);
     for (let r = 0; r < n.length; ++r) {
         const s = n[r];
-        s in this || Object.defineProperty(this, s, kl(s))
+        s in this || Object.defineProperty(this, s, Ul(s))
     }
 }
 Kn.prototype = {
     get type() {
         return et(this).event.type
     },
     get target() {
@@ -643,15 +643,15 @@
     get bubbles() {
         return Boolean(et(this).event.bubbles)
     },
     get cancelable() {
         return Boolean(et(this).event.cancelable)
     },
     preventDefault() {
-        kc(et(this))
+        Uc(et(this))
     },
     get defaultPrevented() {
         return et(this).canceled
     },
     get composed() {
         return Boolean(et(this).event.composed)
     },
@@ -669,50 +669,50 @@
         const t = et(this);
         t.stopped = !0, typeof t.event.cancelBubble == "boolean" && (t.event.cancelBubble = !0)
     },
     get returnValue() {
         return !et(this).canceled
     },
     set returnValue(e) {
-        e || kc(et(this))
+        e || Uc(et(this))
     },
     initEvent() {}
 };
 Object.defineProperty(Kn.prototype, "constructor", {
     value: Kn,
     configurable: !0,
     writable: !0
 });
 typeof window < "u" && typeof window.Event < "u" && (Object.setPrototypeOf(Kn.prototype, window.Event.prototype), Io.set(window.Event.prototype, Kn));
 
-function kl(e) {
+function Ul(e) {
     return {
         get() {
             return et(this).event[e]
         },
         set(t) {
             et(this).event[e] = t
         },
         configurable: !0,
         enumerable: !0
     }
 }
 
-function sp(e) {
+function op(e) {
     return {
         value() {
             const t = et(this).event;
             return t[e].apply(t, arguments)
         },
         configurable: !0,
         enumerable: !0
     }
 }
 
-function op(e, t) {
+function ap(e, t) {
     const n = Object.keys(t);
     if (n.length === 0) return e;
 
     function r(s, o) {
         e.call(this, s, o)
     }
     r.prototype = Object.create(e.prototype, {
@@ -722,62 +722,62 @@
             writable: !0
         }
     });
     for (let s = 0; s < n.length; ++s) {
         const o = n[s];
         if (!(o in e.prototype)) {
             const a = typeof Object.getOwnPropertyDescriptor(t, o).value == "function";
-            Object.defineProperty(r.prototype, o, a ? sp(o) : kl(o))
+            Object.defineProperty(r.prototype, o, a ? op(o) : Ul(o))
         }
     }
     return r
 }
 
-function El(e) {
+function Nl(e) {
     if (e == null || e === Object.prototype) return Kn;
     let t = Io.get(e);
-    return t == null && (t = op(El(Object.getPrototypeOf(e)), e), Io.set(e, t)), t
+    return t == null && (t = ap(Nl(Object.getPrototypeOf(e)), e), Io.set(e, t)), t
 }
 
-function ap(e, t) {
-    const n = El(Object.getPrototypeOf(t));
+function cp(e, t) {
+    const n = Nl(Object.getPrototypeOf(t));
     return new n(e, t)
 }
 
-function cp(e) {
+function up(e) {
     return et(e).immediateStopped
 }
 
-function up(e, t) {
+function lp(e, t) {
     et(e).eventPhase = t
 }
 
-function lp(e, t) {
+function fp(e, t) {
     et(e).currentTarget = t
 }
 
-function Ec(e, t) {
+function Nc(e, t) {
     et(e).passiveListener = t
 }
-const Ul = new WeakMap,
-    Uc = 1,
-    Nc = 2,
+const Ml = new WeakMap,
+    Mc = 1,
+    Cc = 2,
     Ti = 3;
 
 function Ai(e) {
     return e !== null && typeof e == "object"
 }
 
 function Sr(e) {
-    const t = Ul.get(e);
+    const t = Ml.get(e);
     if (t == null) throw new TypeError("'this' is expected an EventTarget object, but got another value.");
     return t
 }
 
-function fp(e) {
+function hp(e) {
     return {
         get() {
             let n = Sr(this).get(e);
             for (; n != null;) {
                 if (n.listenerType === Ti) return n.listener;
                 n = n.next
             }
@@ -801,53 +801,53 @@
             }
         },
         configurable: !0,
         enumerable: !0
     }
 }
 
-function hp(e, t) {
-    Object.defineProperty(e, `on${t}`, fp(t))
+function dp(e, t) {
+    Object.defineProperty(e, `on${t}`, hp(t))
 }
 
-function Mc(e) {
+function Rc(e) {
     function t() {
-        Ye.call(this)
+        Ge.call(this)
     }
-    t.prototype = Object.create(Ye.prototype, {
+    t.prototype = Object.create(Ge.prototype, {
         constructor: {
             value: t,
             configurable: !0,
             writable: !0
         }
     });
-    for (let n = 0; n < e.length; ++n) hp(t.prototype, e[n]);
+    for (let n = 0; n < e.length; ++n) dp(t.prototype, e[n]);
     return t
 }
 
-function Ye() {
-    if (this instanceof Ye) {
-        Ul.set(this, new Map);
+function Ge() {
+    if (this instanceof Ge) {
+        Ml.set(this, new Map);
         return
     }
-    if (arguments.length === 1 && Array.isArray(arguments[0])) return Mc(arguments[0]);
+    if (arguments.length === 1 && Array.isArray(arguments[0])) return Rc(arguments[0]);
     if (arguments.length > 0) {
         const e = new Array(arguments.length);
         for (let t = 0; t < arguments.length; ++t) e[t] = arguments[t];
-        return Mc(e)
+        return Rc(e)
     }
     throw new TypeError("Cannot call a class as a function")
 }
-Ye.prototype = {
+Ge.prototype = {
     addEventListener(e, t, n) {
         if (t == null) return;
         if (typeof t != "function" && !Ai(t)) throw new TypeError("'listener' should be a function or an object.");
         const r = Sr(this),
             s = Ai(n),
-            i = Boolean(s ? n.capture : n) ? Uc : Nc,
+            i = Boolean(s ? n.capture : n) ? Mc : Cc,
             a = {
                 listener: t,
                 listenerType: i,
                 passive: s && Boolean(n.passive),
                 once: s && Boolean(n.once),
                 next: null
             };
@@ -862,15 +862,15 @@
             u = c, c = c.next
         }
         u.next = a
     },
     removeEventListener(e, t, n) {
         if (t == null) return;
         const r = Sr(this),
-            o = (Ai(n) ? Boolean(n.capture) : Boolean(n)) ? Uc : Nc;
+            o = (Ai(n) ? Boolean(n.capture) : Boolean(n)) ? Mc : Cc;
         let i = null,
             a = r.get(e);
         for (; a != null;) {
             if (a.listener === t && a.listenerType === o) {
                 i !== null ? i.next = a.next : a.next !== null ? r.set(e, a.next) : r.delete(e);
                 return
             }
@@ -879,34 +879,34 @@
     },
     dispatchEvent(e) {
         if (e == null || typeof e.type != "string") throw new TypeError('"event.type" should be a string.');
         const t = Sr(this),
             n = e.type;
         let r = t.get(n);
         if (r == null) return !0;
-        const s = ap(this, e);
+        const s = cp(this, e);
         let o = null;
         for (; r != null;) {
-            if (r.once ? o !== null ? o.next = r.next : r.next !== null ? t.set(n, r.next) : t.delete(n) : o = r, Ec(s, r.passive ? r.listener : null), typeof r.listener == "function") try {
+            if (r.once ? o !== null ? o.next = r.next : r.next !== null ? t.set(n, r.next) : t.delete(n) : o = r, Nc(s, r.passive ? r.listener : null), typeof r.listener == "function") try {
                 r.listener.call(this, s)
             } catch (i) {
                 typeof console < "u" && typeof console.error == "function" && console.error(i)
             } else r.listenerType !== Ti && typeof r.listener.handleEvent == "function" && r.listener.handleEvent(s);
-            if (cp(s)) break;
+            if (up(s)) break;
             r = r.next
         }
-        return Ec(s, null), up(s, 0), lp(s, null), !s.defaultPrevented
+        return Nc(s, null), lp(s, 0), fp(s, null), !s.defaultPrevented
     }
 };
-Object.defineProperty(Ye.prototype, "constructor", {
-    value: Ye,
+Object.defineProperty(Ge.prototype, "constructor", {
+    value: Ge,
     configurable: !0,
     writable: !0
 });
-typeof window < "u" && typeof window.EventTarget < "u" && Object.setPrototypeOf(Ye.prototype, window.EventTarget.prototype);
+typeof window < "u" && typeof window.EventTarget < "u" && Object.setPrototypeOf(Ge.prototype, window.EventTarget.prototype);
 var y = {};
 y.SIZEOF_SHORT = 2;
 y.SIZEOF_INT = 4;
 y.FILE_IDENTIFIER_LENGTH = 4;
 y.Encoding = {
     UTF8_BYTES: 1,
     UTF16_STRING: 2
@@ -1247,15 +1247,15 @@
 
 function gs(e) {
     if (e === void 0) return {};
     if (e === Object(e)) return e;
     throw TypeError("Could not convert argument to dictionary")
 }
 
-function dp(e) {
+function pp(e) {
     for (var t = String(e), n = t.length, r = 0, s = []; r < n;) {
         var o = t.charCodeAt(r);
         if (o < 55296 || o > 57343) s.push(o);
         else if (56320 <= o && o <= 57343) s.push(65533);
         else if (55296 <= o && o <= 56319)
             if (r === n - 1) s.push(65533);
             else {
@@ -1266,27 +1266,27 @@
                     s.push(65536 + (a << 10) + c), r += 1
                 } else s.push(65533)
             } r += 1
     }
     return s
 }
 
-function pp(e) {
+function yp(e) {
     for (var t = "", n = 0; n < e.length; ++n) {
         var r = e[n];
         r <= 65535 ? t += String.fromCharCode(r) : (r -= 65536, t += String.fromCharCode((r >> 10) + 55296, (r & 1023) + 56320))
     }
     return t
 }
 var Ni = -1;
 
-function la(e) {
+function aa(e) {
     this.tokens = [].slice.call(e)
 }
-la.prototype = {
+aa.prototype = {
     endOfStream: function() {
         return !this.tokens.length
     },
     read: function() {
         return this.tokens.length ? this.tokens.shift() : Ni
     },
     prepend: function(e) {
@@ -1318,51 +1318,51 @@
     }), Object.defineProperty(this, "ignoreBOM", {
         value: this._ignoreBOM
     })
 }
 Ci.prototype = {
     decode: function(t, n) {
         var r;
-        typeof t == "object" && t instanceof ArrayBuffer ? r = new Uint8Array(t) : typeof t == "object" && "buffer" in t && t.buffer instanceof ArrayBuffer ? r = new Uint8Array(t.buffer, t.byteOffset, t.byteLength) : r = new Uint8Array(0), n = gs(n), this._streaming || (this._decoder = new yp({
+        typeof t == "object" && t instanceof ArrayBuffer ? r = new Uint8Array(t) : typeof t == "object" && "buffer" in t && t.buffer instanceof ArrayBuffer ? r = new Uint8Array(t.buffer, t.byteOffset, t.byteLength) : r = new Uint8Array(0), n = gs(n), this._streaming || (this._decoder = new bp({
             fatal: this._fatal
         }), this._BOMseen = !1), this._streaming = Boolean(n.stream);
-        for (var s = new la(r), o = [], i; !s.endOfStream() && (i = this._decoder.handler(s, s.read()), i !== Zn);) i !== null && (Array.isArray(i) ? o.push.apply(o, i) : o.push(i));
+        for (var s = new aa(r), o = [], i; !s.endOfStream() && (i = this._decoder.handler(s, s.read()), i !== Zn);) i !== null && (Array.isArray(i) ? o.push.apply(o, i) : o.push(i));
         if (!this._streaming) {
             do {
                 if (i = this._decoder.handler(s, s.read()), i === Zn) break;
                 i !== null && (Array.isArray(i) ? o.push.apply(o, i) : o.push(i))
             } while (!s.endOfStream());
             this._decoder = null
         }
-        return o.length && ["utf-8"].indexOf(this.encoding) !== -1 && !this._ignoreBOM && !this._BOMseen && (o[0] === 65279 ? (this._BOMseen = !0, o.shift()) : this._BOMseen = !0), pp(o)
+        return o.length && ["utf-8"].indexOf(this.encoding) !== -1 && !this._ignoreBOM && !this._BOMseen && (o[0] === 65279 ? (this._BOMseen = !0, o.shift()) : this._BOMseen = !0), yp(o)
     }
 };
 
 function Ri(e, t) {
     if (!(this instanceof Ri)) return new Ri(e, t);
     if (e = e !== void 0 ? String(e).toLowerCase() : Mi, e !== Mi) throw new Error("Encoding not supported. Only utf-8 is supported");
     t = gs(t), this._streaming = !1, this._encoder = null, this._options = {
         fatal: Boolean(t.fatal)
     }, Object.defineProperty(this, "encoding", {
         value: "utf-8"
     })
 }
 Ri.prototype = {
     encode: function(t, n) {
-        t = t ? String(t) : "", n = gs(n), this._streaming || (this._encoder = new bp(this._options)), this._streaming = Boolean(n.stream);
-        for (var r = [], s = new la(dp(t)), o; !s.endOfStream() && (o = this._encoder.handler(s, s.read()), o !== Zn);) Array.isArray(o) ? r.push.apply(r, o) : r.push(o);
+        t = t ? String(t) : "", n = gs(n), this._streaming || (this._encoder = new mp(this._options)), this._streaming = Boolean(n.stream);
+        for (var r = [], s = new aa(pp(t)), o; !s.endOfStream() && (o = this._encoder.handler(s, s.read()), o !== Zn);) Array.isArray(o) ? r.push.apply(r, o) : r.push(o);
         if (!this._streaming) {
             for (; o = this._encoder.handler(s, s.read()), o !== Zn;) Array.isArray(o) ? r.push.apply(r, o) : r.push(o);
             this._encoder = null
         }
         return new Uint8Array(r)
     }
 };
 
-function yp(e) {
+function bp(e) {
     var t = e.fatal,
         n = 0,
         r = 0,
         s = 0,
         o = 128,
         i = 191;
     this.handler = function(a, c) {
@@ -1379,69 +1379,69 @@
         if (!_e(c, o, i)) return n = s = r = 0, o = 128, i = 191, a.prepend(c), Ps(t);
         if (o = 128, i = 191, r += 1, n += c - 128 << 6 * (s - r), r !== s) return null;
         var u = n;
         return n = s = r = 0, u
     }
 }
 
-function bp(e) {
+function mp(e) {
     e.fatal, this.handler = function(t, n) {
         if (n === Ni) return Zn;
         if (_e(n, 0, 127)) return n;
         var r, s;
         _e(n, 128, 2047) ? (r = 1, s = 192) : _e(n, 2048, 65535) ? (r = 2, s = 224) : _e(n, 65536, 1114111) && (r = 3, s = 240);
         for (var o = [(n >> 6 * r) + s]; r > 0;) {
             var i = n >> 6 * (r - 1);
             o.push(128 | i & 63), r -= 1
         }
         return o
     }
 }
 const Vi = typeof Buffer == "function" ? Buffer : null,
-    Nl = typeof TextDecoder == "function" && typeof TextEncoder == "function",
+    Cl = typeof TextDecoder == "function" && typeof TextEncoder == "function",
     To = (e => {
-        if (Nl || !Vi) {
+        if (Cl || !Vi) {
             const t = new e("utf-8");
             return n => t.decode(n)
         }
         return t => {
             const {
                 buffer: n,
                 byteOffset: r,
                 length: s
             } = j(t);
             return Vi.from(n, r, s).toString()
         }
     })(typeof TextDecoder < "u" ? TextDecoder : Ci),
     vs = (e => {
-        if (Nl || !Vi) {
+        if (Cl || !Vi) {
             const t = new e;
             return n => t.encode(n)
         }
         return (t = "") => j(Vi.from(t, "utf8"))
     })(typeof TextEncoder < "u" ? TextEncoder : Ri),
     ot = Object.freeze({
         done: !0,
         value: void 0
     });
-class Cc {
+class Vc {
     constructor(t) {
         this._json = t
     }
     get schema() {
         return this._json.schema
     }
     get batches() {
         return this._json.batches || []
     }
     get dictionaries() {
         return this._json.dictionaries || []
     }
 }
-class _n {
+class Sn {
     tee() {
         return this._getDOMStream().tee()
     }
     pipe(t, n) {
         return this._getNodeStream().pipe(t, n)
     }
     pipeTo(t, n) {
@@ -1453,15 +1453,15 @@
     _getDOMStream() {
         return this._DOMStream || (this._DOMStream = this.toDOMStream())
     }
     _getNodeStream() {
         return this._nodeStream || (this._nodeStream = this.toNodeStream())
     }
 }
-class mp extends _n {
+class gp extends Sn {
     constructor() {
         super(), this._values = [], this.resolvers = [], this._closedPromise = new Promise(t => this._closedPromiseResolve = t)
     }
     get closed() {
         return this._closedPromise
     }
     async cancel(t) {
@@ -1525,28 +1525,28 @@
         }) : Promise.resolve(ot)
     }
     _ensureOpen() {
         if (this._closedPromiseResolve) return !0;
         throw new Error(`${this} is closed`)
     }
 }
-const [gp, ws] = (() => {
+const [vp, ws] = (() => {
     const e = () => {
         throw new Error("BigInt is not available in this environment")
     };
 
     function t() {
         throw e()
     }
     return t.asIntN = () => {
         throw e()
     }, t.asUintN = () => {
         throw e()
     }, typeof BigInt < "u" ? [BigInt, !0] : [t, !1]
-})(), [ur, L_] = (() => {
+})(), [ur, D_] = (() => {
     const e = () => {
         throw new Error("BigInt64Array is not available in this environment")
     };
     class t {
         static get BYTES_PER_ELEMENT() {
             return 8
         }
@@ -1557,15 +1557,15 @@
             throw e()
         }
         constructor() {
             throw e()
         }
     }
     return typeof BigInt64Array < "u" ? [BigInt64Array, !0] : [t, !1]
-})(), [Yr, D_] = (() => {
+})(), [Yr, k_] = (() => {
     const e = () => {
         throw new Error("BigUint64Array is not available in this environment")
     };
     class t {
         static get BYTES_PER_ELEMENT() {
             return 8
         }
@@ -1576,19 +1576,19 @@
             throw e()
         }
         constructor() {
             throw e()
         }
     }
     return typeof BigUint64Array < "u" ? [BigUint64Array, !0] : [t, !1]
-})(), vp = e => typeof e == "number", Ml = e => typeof e == "boolean", zt = e => typeof e == "function", Mt = e => e != null && Object(e) === e, Ge = e => Mt(e) && zt(e.then), Xt = e => Mt(e) && zt(e[Symbol.iterator]), De = e => Mt(e) && zt(e[Symbol.asyncIterator]), Ao = e => Mt(e) && Mt(e.schema), Cl = e => Mt(e) && "done" in e && "value" in e, Rl = e => Mt(e) && zt(e.stat) && vp(e.fd), Vl = e => Mt(e) && fa(e.body), wp = e => Mt(e) && zt(e.abort) && zt(e.getWriter) && !(e instanceof _n), fa = e => Mt(e) && zt(e.cancel) && zt(e.getReader) && !(e instanceof _n), _p = e => Mt(e) && zt(e.end) && zt(e.write) && Ml(e.writable) && !(e instanceof _n), jl = e => Mt(e) && zt(e.read) && zt(e.pipe) && Ml(e.readable) && !(e instanceof _n);
-var Sp = y.ByteBuffer;
-const ha = typeof SharedArrayBuffer < "u" ? SharedArrayBuffer : ArrayBuffer;
+})(), wp = e => typeof e == "number", Rl = e => typeof e == "boolean", Wt = e => typeof e == "function", Ct = e => e != null && Object(e) === e, Ke = e => Ct(e) && Wt(e.then), qt = e => Ct(e) && Wt(e[Symbol.iterator]), De = e => Ct(e) && Wt(e[Symbol.asyncIterator]), Ao = e => Ct(e) && Ct(e.schema), Vl = e => Ct(e) && "done" in e && "value" in e, jl = e => Ct(e) && Wt(e.stat) && wp(e.fd), Pl = e => Ct(e) && ca(e.body), _p = e => Ct(e) && Wt(e.abort) && Wt(e.getWriter) && !(e instanceof Sn), ca = e => Ct(e) && Wt(e.cancel) && Wt(e.getReader) && !(e instanceof Sn), Sp = e => Ct(e) && Wt(e.end) && Wt(e.write) && Rl(e.writable) && !(e instanceof Sn), zl = e => Ct(e) && Wt(e.read) && Wt(e.pipe) && Rl(e.readable) && !(e instanceof Sn);
+var Ip = y.ByteBuffer;
+const ua = typeof SharedArrayBuffer < "u" ? SharedArrayBuffer : ArrayBuffer;
 
-function Ip(e) {
+function Tp(e) {
     let t = e[0] ? [e[0]] : [],
         n, r, s, o;
     for (let i, a, c = 0, u = 0, l = e.length; ++c < l;) {
         if (i = t[u], a = e[c], !i || !a || i.buffer !== a.buffer || a.byteOffset < i.byteOffset) {
             a && (t[++u] = a);
             continue
         }
@@ -1610,16 +1610,16 @@
 function Fr(e, t, n = 0, r = t.byteLength) {
     const s = e.byteLength,
         o = new Uint8Array(e.buffer, e.byteOffset, s),
         i = new Uint8Array(t.buffer, t.byteOffset, Math.min(r, s));
     return o.set(i, n), e
 }
 
-function qt(e, t) {
-    let n = Ip(e),
+function Qt(e, t) {
+    let n = Tp(e),
         r = n.reduce((l, f) => l + f.byteLength, 0),
         s, o, i, a = 0,
         c = -1,
         u = Math.min(t || 1 / 0, r);
     for (let l = n.length; ++c < l;) {
         if (s = n[c], o = s.subarray(0, Math.min(s.length, u - a)), u <= a + o.length) {
             o.length < s.length ? n[c] = s.subarray(o.length) : o.length === s.length && c++, i ? Fr(i, o, a) : i = o;
@@ -1627,166 +1627,166 @@
         }
         Fr(i || (i = new Uint8Array(u)), o, a), a += o.length
     }
     return [i || new Uint8Array(0), n.slice(c), r - (i ? i.byteLength : 0)]
 }
 
 function R(e, t) {
-    let n = Cl(t) ? t.value : t;
-    return n instanceof e ? e === Uint8Array ? new e(n.buffer, n.byteOffset, n.byteLength) : n : n ? (typeof n == "string" && (n = vs(n)), n instanceof ArrayBuffer ? new e(n) : n instanceof ha ? new e(n) : n instanceof Sp ? R(e, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new e(0) : new e(n.buffer, n.byteOffset, n.byteLength / e.BYTES_PER_ELEMENT) : e.from(n)) : new e(0)
+    let n = Vl(t) ? t.value : t;
+    return n instanceof e ? e === Uint8Array ? new e(n.buffer, n.byteOffset, n.byteLength) : n : n ? (typeof n == "string" && (n = vs(n)), n instanceof ArrayBuffer ? new e(n) : n instanceof ua ? new e(n) : n instanceof Ip ? R(e, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new e(0) : new e(n.buffer, n.byteOffset, n.byteLength / e.BYTES_PER_ELEMENT) : e.from(n)) : new e(0)
 }
-const Tp = e => R(Int8Array, e),
-    Ap = e => R(Int16Array, e),
-    kn = e => R(Int32Array, e),
-    Pl = e => R(ur, e),
+const Ap = e => R(Int8Array, e),
+    Bp = e => R(Int16Array, e),
+    En = e => R(Int32Array, e),
+    Wl = e => R(ur, e),
     j = e => R(Uint8Array, e),
-    Bp = e => R(Uint16Array, e),
-    Op = e => R(Uint32Array, e),
-    zl = e => R(Yr, e),
-    Fp = e => R(Float32Array, e),
-    xp = e => R(Float64Array, e),
-    Lp = e => R(Uint8ClampedArray, e),
+    Op = e => R(Uint16Array, e),
+    Fp = e => R(Uint32Array, e),
+    $l = e => R(Yr, e),
+    xp = e => R(Float32Array, e),
+    Lp = e => R(Float64Array, e),
+    Dp = e => R(Uint8ClampedArray, e),
     Bo = e => (e.next(), e);
 
 function* de(e, t) {
     const n = function*(s) {
             yield s
         },
-        r = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof ha ? n(t) : Xt(t) ? t : n(t);
+        r = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof ua ? n(t) : qt(t) ? t : n(t);
     yield* Bo(function*(s) {
         let o = null;
         do o = s.next(yield R(e, o)); while (!o.done)
     }(r[Symbol.iterator]()))
 }
-const Dp = e => de(Int8Array, e),
-    kp = e => de(Int16Array, e),
-    Ep = e => de(Int32Array, e),
-    Wl = e => de(Uint8Array, e),
-    Up = e => de(Uint16Array, e),
-    Np = e => de(Uint32Array, e),
-    Mp = e => de(Float32Array, e),
-    Cp = e => de(Float64Array, e),
-    Rp = e => de(Uint8ClampedArray, e);
-async function* ee(e, t) {
-    if (Ge(t)) return yield* ee(e, await t);
+const kp = e => de(Int8Array, e),
+    Ep = e => de(Int16Array, e),
+    Up = e => de(Int32Array, e),
+    Yl = e => de(Uint8Array, e),
+    Np = e => de(Uint16Array, e),
+    Mp = e => de(Uint32Array, e),
+    Cp = e => de(Float32Array, e),
+    Rp = e => de(Float64Array, e),
+    Vp = e => de(Uint8ClampedArray, e);
+async function* ne(e, t) {
+    if (Ke(t)) return yield* ne(e, await t);
     const n = async function*(o) {
         yield await o
     }, r = async function*(o) {
         yield* Bo(function*(i) {
             let a = null;
             do a = i.next(yield a && a.value); while (!a.done)
         }(o[Symbol.iterator]()))
-    }, s = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof ha ? n(t) : Xt(t) ? r(t) : De(t) ? t : n(t);
+    }, s = typeof t == "string" || ArrayBuffer.isView(t) || t instanceof ArrayBuffer || t instanceof ua ? n(t) : qt(t) ? r(t) : De(t) ? t : n(t);
     yield* Bo(async function*(o) {
         let i = null;
         do i = await o.next(yield R(e, i)); while (!i.done)
     }(s[Symbol.asyncIterator]()))
 }
-const Vp = e => ee(Int8Array, e),
-    jp = e => ee(Int16Array, e),
-    Pp = e => ee(Int32Array, e),
-    $l = e => ee(Uint8Array, e),
-    zp = e => ee(Uint16Array, e),
-    Wp = e => ee(Uint32Array, e),
-    $p = e => ee(Float32Array, e),
-    Yp = e => ee(Float64Array, e),
-    Gp = e => ee(Uint8ClampedArray, e);
+const jp = e => ne(Int8Array, e),
+    Pp = e => ne(Int16Array, e),
+    zp = e => ne(Int32Array, e),
+    Gl = e => ne(Uint8Array, e),
+    Wp = e => ne(Uint16Array, e),
+    $p = e => ne(Uint32Array, e),
+    Yp = e => ne(Float32Array, e),
+    Gp = e => ne(Float64Array, e),
+    Kp = e => ne(Uint8ClampedArray, e);
 
 function _s(e, t, n) {
     if (e !== 0) {
         n = n.slice(0, t + 1);
         for (let r = -1; ++r <= t;) n[r] += e
     }
     return n
 }
 
-function Yl(e, t) {
+function Kl(e, t) {
     let n = 0,
         r = e.length;
     if (r !== t.length) return !1;
     if (r > 0)
         do
             if (e[n] !== t[n]) return !1; while (++n < r);
     return !0
 }
-const Kp = Object.freeze(Object.defineProperty({
+const Zp = Object.freeze(Object.defineProperty({
         __proto__: null,
         memcpy: Fr,
-        joinUint8Arrays: qt,
+        joinUint8Arrays: Qt,
         toArrayBufferView: R,
-        toInt8Array: Tp,
-        toInt16Array: Ap,
-        toInt32Array: kn,
-        toBigInt64Array: Pl,
+        toInt8Array: Ap,
+        toInt16Array: Bp,
+        toInt32Array: En,
+        toBigInt64Array: Wl,
         toUint8Array: j,
-        toUint16Array: Bp,
-        toUint32Array: Op,
-        toBigUint64Array: zl,
-        toFloat32Array: Fp,
-        toFloat64Array: xp,
-        toUint8ClampedArray: Lp,
+        toUint16Array: Op,
+        toUint32Array: Fp,
+        toBigUint64Array: $l,
+        toFloat32Array: xp,
+        toFloat64Array: Lp,
+        toUint8ClampedArray: Dp,
         toArrayBufferViewIterator: de,
-        toInt8ArrayIterator: Dp,
-        toInt16ArrayIterator: kp,
-        toInt32ArrayIterator: Ep,
-        toUint8ArrayIterator: Wl,
-        toUint16ArrayIterator: Up,
-        toUint32ArrayIterator: Np,
-        toFloat32ArrayIterator: Mp,
-        toFloat64ArrayIterator: Cp,
-        toUint8ClampedArrayIterator: Rp,
-        toArrayBufferViewAsyncIterator: ee,
-        toInt8ArrayAsyncIterator: Vp,
-        toInt16ArrayAsyncIterator: jp,
-        toInt32ArrayAsyncIterator: Pp,
-        toUint8ArrayAsyncIterator: $l,
-        toUint16ArrayAsyncIterator: zp,
-        toUint32ArrayAsyncIterator: Wp,
-        toFloat32ArrayAsyncIterator: $p,
-        toFloat64ArrayAsyncIterator: Yp,
-        toUint8ClampedArrayAsyncIterator: Gp,
+        toInt8ArrayIterator: kp,
+        toInt16ArrayIterator: Ep,
+        toInt32ArrayIterator: Up,
+        toUint8ArrayIterator: Yl,
+        toUint16ArrayIterator: Np,
+        toUint32ArrayIterator: Mp,
+        toFloat32ArrayIterator: Cp,
+        toFloat64ArrayIterator: Rp,
+        toUint8ClampedArrayIterator: Vp,
+        toArrayBufferViewAsyncIterator: ne,
+        toInt8ArrayAsyncIterator: jp,
+        toInt16ArrayAsyncIterator: Pp,
+        toInt32ArrayAsyncIterator: zp,
+        toUint8ArrayAsyncIterator: Gl,
+        toUint16ArrayAsyncIterator: Wp,
+        toUint32ArrayAsyncIterator: $p,
+        toFloat32ArrayAsyncIterator: Yp,
+        toFloat64ArrayAsyncIterator: Gp,
+        toUint8ClampedArrayAsyncIterator: Kp,
         rebaseValueOffsets: _s,
-        compareArrayLike: Yl
+        compareArrayLike: Kl
     }, Symbol.toStringTag, {
         value: "Module"
     })),
     Ut = {
         fromIterable(e) {
-            return li(Zp(e))
+            return li(Hp(e))
         },
         fromAsyncIterable(e) {
-            return li(Hp(e))
+            return li(Jp(e))
         },
         fromDOMStream(e) {
-            return li(Jp(e))
+            return li(Xp(e))
         },
         fromNodeStream(e) {
-            return li(qp(e))
+            return li(Qp(e))
         },
         toDOMStream(e, t) {
             throw new Error('"toDOMStream" not available in this environment')
         },
         toNodeStream(e, t) {
             throw new Error('"toNodeStream" not available in this environment')
         }
     },
     li = e => (e.next(), e);
 
-function* Zp(e) {
+function* Hp(e) {
     let t, n = !1,
         r = [],
         s, o, i, a = 0;
 
     function c() {
-        return o === "peek" ? qt(r, i)[0] : ([s, r, a] = qt(r, i), s)
+        return o === "peek" ? Qt(r, i)[0] : ([s, r, a] = Qt(r, i), s)
     }({
         cmd: o,
         size: i
     } = yield null);
-    let u = Wl(e)[Symbol.iterator]();
+    let u = Yl(e)[Symbol.iterator]();
     try {
         do
             if ({
                     done: t,
                     value: s
                 } = isNaN(i - a) ? u.next(void 0) : u.next(i - a), !t && s.byteLength > 0 && (r.push(s), a += s.byteLength), t || i <= a)
                 do({
@@ -1795,26 +1795,26 @@
                 } = yield c()); while (i < a); while (!t)
     } catch (l) {
         (n = !0) && typeof u.throw == "function" && u.throw(l)
     } finally {
         n === !1 && typeof u.return == "function" && u.return()
     }
 }
-async function* Hp(e) {
+async function* Jp(e) {
     let t, n = !1,
         r = [],
         s, o, i, a = 0;
 
     function c() {
-        return o === "peek" ? qt(r, i)[0] : ([s, r, a] = qt(r, i), s)
+        return o === "peek" ? Qt(r, i)[0] : ([s, r, a] = Qt(r, i), s)
     }({
         cmd: o,
         size: i
     } = yield null);
-    let u = $l(e)[Symbol.asyncIterator]();
+    let u = Gl(e)[Symbol.asyncIterator]();
     try {
         do
             if ({
                     done: t,
                     value: s
                 } = isNaN(i - a) ? await u.next(void 0) : await u.next(i - a), !t && s.byteLength > 0 && (r.push(s), a += s.byteLength), t || i <= a)
                 do({
@@ -1823,27 +1823,27 @@
                 } = yield c()); while (i < a); while (!t)
     } catch (l) {
         (n = !0) && typeof u.throw == "function" && await u.throw(l)
     } finally {
         n === !1 && typeof u.return == "function" && await u.return()
     }
 }
-async function* Jp(e) {
+async function* Xp(e) {
     let t = !1,
         n = !1,
         r = [],
         s, o, i, a = 0;
 
     function c() {
-        return o === "peek" ? qt(r, i)[0] : ([s, r, a] = qt(r, i), s)
+        return o === "peek" ? Qt(r, i)[0] : ([s, r, a] = Qt(r, i), s)
     }({
         cmd: o,
         size: i
     } = yield null);
-    let u = new Xp(e);
+    let u = new qp(e);
     try {
         do
             if ({
                     done: t,
                     value: s
                 } = isNaN(i - a) ? await u.read(void 0) : await u.read(i - a), !t && s.byteLength > 0 && (r.push(j(s)), a += s.byteLength), t || i <= a)
                 do({
@@ -1852,15 +1852,15 @@
                 } = yield c()); while (i < a); while (!t)
     } catch (l) {
         (n = !0) && await u.cancel(l)
     } finally {
         n === !1 ? await u.cancel() : e.locked && u.releaseLock()
     }
 }
-class Xp {
+class qp {
     constructor(t) {
         this.source = t, this.byobReader = null, this.defaultReader = null;
         try {
             this.supportsBYOB = !!(this.reader = this.getBYOBReader())
         } catch {
             this.supportsBYOB = !(this.reader = this.getDefaultReader())
         }
@@ -1891,47 +1891,47 @@
     }
     getBYOBReader() {
         return this.defaultReader && this.releaseLock(), this.byobReader || (this.byobReader = this.source.getReader({
             mode: "byob"
         }), this.byobReader.closed.catch(() => {})), this.reader = this.byobReader
     }
     async readFromBYOBReader(t) {
-        return await Gl(this.getBYOBReader(), new ArrayBuffer(t), 0, t)
+        return await Zl(this.getBYOBReader(), new ArrayBuffer(t), 0, t)
     }
 }
-async function Gl(e, t, n, r) {
+async function Zl(e, t, n, r) {
     if (n >= r) return {
         done: !1,
         value: new Uint8Array(t, 0, r)
     };
     const {
         done: s,
         value: o
     } = await e.read(new Uint8Array(t, n, r - n));
-    return (n += o.byteLength) < r && !s ? await Gl(e, o.buffer, n, r) : {
+    return (n += o.byteLength) < r && !s ? await Zl(e, o.buffer, n, r) : {
         done: s,
         value: new Uint8Array(o.buffer, 0, n)
     }
 }
 const zs = (e, t) => {
     let n = s => r([t, s]),
         r;
     return [t, n, new Promise(s => (r = s) && e.once(t, n))]
 };
-async function* qp(e) {
+async function* Qp(e) {
     let t = [],
         n = "error",
         r = !1,
         s = null,
         o, i, a = 0,
         c = [],
         u;
 
     function l() {
-        return o === "peek" ? qt(c, i)[0] : ([u, c, a] = qt(c, i), u)
+        return o === "peek" ? Qt(c, i)[0] : ([u, c, a] = Qt(c, i), u)
     }
     if ({
             cmd: o,
             size: i
         } = yield null, e.isTTY) return yield new Uint8Array(0);
     try {
         t[0] = zs(e, "end"), t[1] = zs(e, "error");
@@ -3332,45 +3332,45 @@
             })(n.flatbuf || (n.flatbuf = {}))
         })(t.arrow || (t.arrow = {}))
     })(e.apache || (e.apache = {}))
 })(gt || (gt = {}));
 m.apache.arrow.flatbuf.Type;
 var le = m.apache.arrow.flatbuf.DateUnit,
     Z = m.apache.arrow.flatbuf.TimeUnit,
-    Pt = m.apache.arrow.flatbuf.Precision,
+    zt = m.apache.arrow.flatbuf.Precision,
     Be = m.apache.arrow.flatbuf.UnionMode,
     Hn = m.apache.arrow.flatbuf.IntervalUnit,
     Q = gt.apache.arrow.flatbuf.MessageHeader,
-    Gt = m.apache.arrow.flatbuf.MetadataVersion,
+    Kt = m.apache.arrow.flatbuf.MetadataVersion,
     d;
 (function(e) {
     e[e.NONE = 0] = "NONE", e[e.Null = 1] = "Null", e[e.Int = 2] = "Int", e[e.Float = 3] = "Float", e[e.Binary = 4] = "Binary", e[e.Utf8 = 5] = "Utf8", e[e.Bool = 6] = "Bool", e[e.Decimal = 7] = "Decimal", e[e.Date = 8] = "Date", e[e.Time = 9] = "Time", e[e.Timestamp = 10] = "Timestamp", e[e.Interval = 11] = "Interval", e[e.List = 12] = "List", e[e.Struct = 13] = "Struct", e[e.Union = 14] = "Union", e[e.FixedSizeBinary = 15] = "FixedSizeBinary", e[e.FixedSizeList = 16] = "FixedSizeList", e[e.Map = 17] = "Map", e[e.Dictionary = -1] = "Dictionary", e[e.Int8 = -2] = "Int8", e[e.Int16 = -3] = "Int16", e[e.Int32 = -4] = "Int32", e[e.Int64 = -5] = "Int64", e[e.Uint8 = -6] = "Uint8", e[e.Uint16 = -7] = "Uint16", e[e.Uint32 = -8] = "Uint32", e[e.Uint64 = -9] = "Uint64", e[e.Float16 = -10] = "Float16", e[e.Float32 = -11] = "Float32", e[e.Float64 = -12] = "Float64", e[e.DateDay = -13] = "DateDay", e[e.DateMillisecond = -14] = "DateMillisecond", e[e.TimestampSecond = -15] = "TimestampSecond", e[e.TimestampMillisecond = -16] = "TimestampMillisecond", e[e.TimestampMicrosecond = -17] = "TimestampMicrosecond", e[e.TimestampNanosecond = -18] = "TimestampNanosecond", e[e.TimeSecond = -19] = "TimeSecond", e[e.TimeMillisecond = -20] = "TimeMillisecond", e[e.TimeMicrosecond = -21] = "TimeMicrosecond", e[e.TimeNanosecond = -22] = "TimeNanosecond", e[e.DenseUnion = -23] = "DenseUnion", e[e.SparseUnion = -24] = "SparseUnion", e[e.IntervalDayTime = -25] = "IntervalDayTime", e[e.IntervalYearMonth = -26] = "IntervalYearMonth"
 })(d || (d = {}));
 var T;
 (function(e) {
     e[e.OFFSET = 0] = "OFFSET", e[e.DATA = 1] = "DATA", e[e.VALIDITY = 2] = "VALIDITY", e[e.TYPE = 3] = "TYPE"
 })(T || (T = {}));
 
-function da(e, t, n, r) {
+function la(e, t, n, r) {
     return (n & 1 << r) !== 0
 }
 
-function Kl(e, t, n, r) {
+function Hl(e, t, n, r) {
     return (n & 1 << r) >> r
 }
 
-function Zl(e, t, n) {
+function Jl(e, t, n) {
     return n ? !!(e[t >> 3] |= 1 << t % 8) || !0 : !(e[t >> 3] &= ~(1 << t % 8)) && !1
 }
 
 function Ss(e, t, n) {
     const r = n.byteLength + 7 & -8;
     if (e > 0 || n.byteLength < r) {
         const s = new Uint8Array(r);
-        return s.set(e % 8 === 0 ? n.subarray(e >> 3) : xr(Gr(n, e, t, null, da)).subarray(0, r)), s
+        return s.set(e % 8 === 0 ? n.subarray(e >> 3) : xr(Gr(n, e, t, null, la)).subarray(0, r)), s
     }
     return n
 }
 
 function xr(e) {
     let t = [],
         n = 0,
@@ -3393,60 +3393,60 @@
     }
 }
 
 function ji(e, t, n) {
     if (n - t <= 0) return 0;
     if (n - t < 8) {
         let o = 0;
-        for (const i of Gr(e, t, n - t, e, Kl)) o += i;
+        for (const i of Gr(e, t, n - t, e, Hl)) o += i;
         return o
     }
     const r = n >> 3 << 3,
         s = t + (t % 8 === 0 ? 0 : 8 - t % 8);
-    return ji(e, t, s) + ji(e, r, n) + Hl(e, s >> 3, r - s >> 3)
+    return ji(e, t, s) + ji(e, r, n) + Xl(e, s >> 3, r - s >> 3)
 }
 
-function Hl(e, t, n) {
+function Xl(e, t, n) {
     let r = 0,
         s = t | 0;
     const o = new DataView(e.buffer, e.byteOffset, e.byteLength),
         i = n === void 0 ? e.byteLength : s + n;
     for (; i - s >= 4;) r += Bi(o.getUint32(s)), s += 4;
     for (; i - s >= 2;) r += Bi(o.getUint16(s)), s += 2;
     for (; i - s >= 1;) r += Bi(o.getUint8(s)), s += 1;
     return r
 }
 
 function Bi(e) {
     let t = e | 0;
     return t = t - (t >>> 1 & 1431655765), t = (t & 858993459) + (t >>> 2 & 858993459), (t + (t >>> 4) & 252645135) * 16843009 >>> 24
 }
-const Qp = Object.freeze(Object.defineProperty({
+const ty = Object.freeze(Object.defineProperty({
     __proto__: null,
-    getBool: da,
-    getBit: Kl,
-    setBool: Zl,
+    getBool: la,
+    getBit: Hl,
+    setBool: Jl,
     truncateBitmap: Ss,
     packBools: xr,
     iterateBits: Gr,
     popcnt_bit_range: ji,
-    popcnt_array: Hl,
+    popcnt_array: Xl,
     popcnt_uint32: Bi
 }, Symbol.toStringTag, {
     value: "Module"
 }));
 class V {
     visitMany(t, ...n) {
         return t.map((r, s) => this.visit(r, ...n.map(o => o[s])))
     }
     visit(...t) {
         return this.getVisitFn(t[0], !1).apply(this, t)
     }
     getVisitFn(t, n = !0) {
-        return ty(this, t, n)
+        return ey(this, t, n)
     }
     visitNull(t, ...n) {
         return null
     }
     visitBool(t, ...n) {
         return null
     }
@@ -3496,15 +3496,15 @@
         return null
     }
     visitMap(t, ...n) {
         return null
     }
 }
 
-function ty(e, t, n = !0) {
+function ey(e, t, n = !0) {
     let r = null,
         s = d.NONE;
     switch (t instanceof S || t instanceof z ? s = Ws(t.type) : t instanceof U ? s = Ws(t) : typeof(s = t) != "number" && (s = d[t]), s) {
         case d.Null:
             r = e.visitNull;
             break;
         case d.Bool:
@@ -3656,19 +3656,19 @@
                     return n ? d.Int32 : d.Uint32;
                 case 64:
                     return n ? d.Int64 : d.Uint64
             }
             return d.Int;
         case d.Float:
             switch (e.precision) {
-                case Pt.HALF:
+                case zt.HALF:
                     return d.Float16;
-                case Pt.SINGLE:
+                case zt.SINGLE:
                     return d.Float32;
-                case Pt.DOUBLE:
+                case zt.DOUBLE:
                     return d.Float64
             }
             return d.Float;
         case d.Binary:
             return d.Binary;
         case d.Utf8:
             return d.Utf8;
@@ -3762,21 +3762,21 @@
 V.prototype.visitTimeNanosecond = null;
 V.prototype.visitDenseUnion = null;
 V.prototype.visitSparseUnion = null;
 V.prototype.visitIntervalDayTime = null;
 V.prototype.visitIntervalYearMonth = null;
 class B extends V {
     compareSchemas(t, n) {
-        return t === n || n instanceof t.constructor && Nt.compareFields(t.fields, n.fields)
+        return t === n || n instanceof t.constructor && Mt.compareFields(t.fields, n.fields)
     }
     compareFields(t, n) {
-        return t === n || Array.isArray(t) && Array.isArray(n) && t.length === n.length && t.every((r, s) => Nt.compareField(r, n[s]))
+        return t === n || Array.isArray(t) && Array.isArray(n) && t.length === n.length && t.every((r, s) => Mt.compareField(r, n[s]))
     }
     compareField(t, n) {
-        return t === n || n instanceof t.constructor && t.name === n.name && t.nullable === n.nullable && Nt.visit(t.type, n.type)
+        return t === n || n instanceof t.constructor && t.name === n.name && t.nullable === n.nullable && Mt.visit(t.type, n.type)
     }
 }
 
 function Lt(e, t) {
     return t instanceof e.constructor
 }
 
@@ -3788,56 +3788,56 @@
     return e === t || Lt(e, t) && e.bitWidth === t.bitWidth && e.isSigned === t.isSigned
 }
 
 function Is(e, t) {
     return e === t || Lt(e, t) && e.precision === t.precision
 }
 
-function ey(e, t) {
+function ny(e, t) {
     return e === t || Lt(e, t) && e.byteWidth === t.byteWidth
 }
 
-function pa(e, t) {
+function fa(e, t) {
     return e === t || Lt(e, t) && e.unit === t.unit
 }
 
 function Zr(e, t) {
     return e === t || Lt(e, t) && e.unit === t.unit && e.timezone === t.timezone
 }
 
 function Hr(e, t) {
     return e === t || Lt(e, t) && e.unit === t.unit && e.bitWidth === t.bitWidth
 }
 
-function ny(e, t) {
-    return e === t || Lt(e, t) && e.children.length === t.children.length && Nt.compareFields(e.children, t.children)
+function ry(e, t) {
+    return e === t || Lt(e, t) && e.children.length === t.children.length && Mt.compareFields(e.children, t.children)
 }
 
-function ry(e, t) {
-    return e === t || Lt(e, t) && e.children.length === t.children.length && Nt.compareFields(e.children, t.children)
+function iy(e, t) {
+    return e === t || Lt(e, t) && e.children.length === t.children.length && Mt.compareFields(e.children, t.children)
 }
 
-function ya(e, t) {
-    return e === t || Lt(e, t) && e.mode === t.mode && e.typeIds.every((n, r) => n === t.typeIds[r]) && Nt.compareFields(e.children, t.children)
+function ha(e, t) {
+    return e === t || Lt(e, t) && e.mode === t.mode && e.typeIds.every((n, r) => n === t.typeIds[r]) && Mt.compareFields(e.children, t.children)
 }
 
-function iy(e, t) {
-    return e === t || Lt(e, t) && e.id === t.id && e.isOrdered === t.isOrdered && Nt.visit(e.indices, t.indices) && Nt.visit(e.dictionary, t.dictionary)
+function sy(e, t) {
+    return e === t || Lt(e, t) && e.id === t.id && e.isOrdered === t.isOrdered && Mt.visit(e.indices, t.indices) && Mt.visit(e.dictionary, t.dictionary)
 }
 
-function ba(e, t) {
+function da(e, t) {
     return e === t || Lt(e, t) && e.unit === t.unit
 }
 
-function sy(e, t) {
-    return e === t || Lt(e, t) && e.listSize === t.listSize && e.children.length === t.children.length && Nt.compareFields(e.children, t.children)
+function oy(e, t) {
+    return e === t || Lt(e, t) && e.listSize === t.listSize && e.children.length === t.children.length && Mt.compareFields(e.children, t.children)
 }
 
-function oy(e, t) {
-    return e === t || Lt(e, t) && e.keysSorted === t.keysSorted && e.children.length === t.children.length && Nt.compareFields(e.children, t.children)
+function ay(e, t) {
+    return e === t || Lt(e, t) && e.keysSorted === t.keysSorted && e.children.length === t.children.length && Mt.compareFields(e.children, t.children)
 }
 B.prototype.visitNull = Kr;
 B.prototype.visitBool = Kr;
 B.prototype.visitInt = ke;
 B.prototype.visitInt8 = ke;
 B.prototype.visitInt16 = ke;
 B.prototype.visitInt32 = ke;
@@ -3848,41 +3848,41 @@
 B.prototype.visitUint64 = ke;
 B.prototype.visitFloat = Is;
 B.prototype.visitFloat16 = Is;
 B.prototype.visitFloat32 = Is;
 B.prototype.visitFloat64 = Is;
 B.prototype.visitUtf8 = Kr;
 B.prototype.visitBinary = Kr;
-B.prototype.visitFixedSizeBinary = ey;
-B.prototype.visitDate = pa;
-B.prototype.visitDateDay = pa;
-B.prototype.visitDateMillisecond = pa;
+B.prototype.visitFixedSizeBinary = ny;
+B.prototype.visitDate = fa;
+B.prototype.visitDateDay = fa;
+B.prototype.visitDateMillisecond = fa;
 B.prototype.visitTimestamp = Zr;
 B.prototype.visitTimestampSecond = Zr;
 B.prototype.visitTimestampMillisecond = Zr;
 B.prototype.visitTimestampMicrosecond = Zr;
 B.prototype.visitTimestampNanosecond = Zr;
 B.prototype.visitTime = Hr;
 B.prototype.visitTimeSecond = Hr;
 B.prototype.visitTimeMillisecond = Hr;
 B.prototype.visitTimeMicrosecond = Hr;
 B.prototype.visitTimeNanosecond = Hr;
 B.prototype.visitDecimal = Kr;
-B.prototype.visitList = ny;
-B.prototype.visitStruct = ry;
-B.prototype.visitUnion = ya;
-B.prototype.visitDenseUnion = ya;
-B.prototype.visitSparseUnion = ya;
-B.prototype.visitDictionary = iy;
-B.prototype.visitInterval = ba;
-B.prototype.visitIntervalDayTime = ba;
-B.prototype.visitIntervalYearMonth = ba;
-B.prototype.visitFixedSizeList = sy;
-B.prototype.visitMap = oy;
-const Nt = new B;
+B.prototype.visitList = ry;
+B.prototype.visitStruct = iy;
+B.prototype.visitUnion = ha;
+B.prototype.visitDenseUnion = ha;
+B.prototype.visitSparseUnion = ha;
+B.prototype.visitDictionary = sy;
+B.prototype.visitInterval = da;
+B.prototype.visitIntervalDayTime = da;
+B.prototype.visitIntervalYearMonth = da;
+B.prototype.visitFixedSizeList = oy;
+B.prototype.visitMap = ay;
+const Mt = new B;
 class U {
     static isNull(t) {
         return t && t.typeId === d.Null
     }
     static isInt(t) {
         return t && t.typeId === d.Int
     }
@@ -3934,15 +3934,15 @@
     static isDictionary(t) {
         return t && t.typeId === d.Dictionary
     }
     get typeId() {
         return d.NONE
     }
     compareTo(t) {
-        return Nt.visit(this, t)
+        return Mt.visit(this, t)
     }
 }
 U[Symbol.toStringTag] = (e => (e.children = null, e.ArrayType = Array, e[Symbol.toStringTag] = "DataType"))(U.prototype);
 class Jn extends U {
     toString() {
         return "Null"
     }
@@ -3972,123 +3972,123 @@
         throw new Error(`Unrecognized ${this[Symbol.toStringTag]} type`)
     }
     toString() {
         return `${this.isSigned?"I":"Ui"}nt${this.bitWidth}`
     }
 }
 xt[Symbol.toStringTag] = (e => (e.isSigned = null, e.bitWidth = null, e[Symbol.toStringTag] = "Int"))(xt.prototype);
-class ma extends xt {
+class pa extends xt {
     constructor() {
         super(!0, 8)
     }
 }
-class ga extends xt {
+class ya extends xt {
     constructor() {
         super(!0, 16)
     }
 }
-class hn extends xt {
+class pn extends xt {
     constructor() {
         super(!0, 32)
     }
 }
 class Xn extends xt {
     constructor() {
         super(!0, 64)
     }
 }
-class va extends xt {
+class ba extends xt {
     constructor() {
         super(!1, 8)
     }
 }
-class wa extends xt {
+class ma extends xt {
     constructor() {
         super(!1, 16)
     }
 }
-class _a extends xt {
+class ga extends xt {
     constructor() {
         super(!1, 32)
     }
 }
 class qn extends xt {
     constructor() {
         super(!1, 64)
     }
 }
-Object.defineProperty(ma.prototype, "ArrayType", {
+Object.defineProperty(pa.prototype, "ArrayType", {
     value: Int8Array
 });
-Object.defineProperty(ga.prototype, "ArrayType", {
+Object.defineProperty(ya.prototype, "ArrayType", {
     value: Int16Array
 });
-Object.defineProperty(hn.prototype, "ArrayType", {
+Object.defineProperty(pn.prototype, "ArrayType", {
     value: Int32Array
 });
 Object.defineProperty(Xn.prototype, "ArrayType", {
     value: Int32Array
 });
-Object.defineProperty(va.prototype, "ArrayType", {
+Object.defineProperty(ba.prototype, "ArrayType", {
     value: Uint8Array
 });
-Object.defineProperty(wa.prototype, "ArrayType", {
+Object.defineProperty(ma.prototype, "ArrayType", {
     value: Uint16Array
 });
-Object.defineProperty(_a.prototype, "ArrayType", {
+Object.defineProperty(ga.prototype, "ArrayType", {
     value: Uint32Array
 });
 Object.defineProperty(qn.prototype, "ArrayType", {
     value: Uint32Array
 });
-class dn extends U {
+class yn extends U {
     constructor(t) {
         super(), this.precision = t
     }
     get typeId() {
         return d.Float
     }
     get ArrayType() {
         switch (this.precision) {
-            case Pt.HALF:
+            case zt.HALF:
                 return Uint16Array;
-            case Pt.SINGLE:
+            case zt.SINGLE:
                 return Float32Array;
-            case Pt.DOUBLE:
+            case zt.DOUBLE:
                 return Float64Array
         }
         throw new Error(`Unrecognized ${this[Symbol.toStringTag]} type`)
     }
     toString() {
         return `Float${this.precision<<5||16}`
     }
 }
-dn[Symbol.toStringTag] = (e => (e.precision = null, e[Symbol.toStringTag] = "Float"))(dn.prototype);
-class Ts extends dn {
+yn[Symbol.toStringTag] = (e => (e.precision = null, e[Symbol.toStringTag] = "Float"))(yn.prototype);
+class Ts extends yn {
     constructor() {
-        super(Pt.HALF)
+        super(zt.HALF)
     }
 }
-class Sa extends dn {
+class va extends yn {
     constructor() {
-        super(Pt.SINGLE)
+        super(zt.SINGLE)
     }
 }
-class Ia extends dn {
+class wa extends yn {
     constructor() {
-        super(Pt.DOUBLE)
+        super(zt.DOUBLE)
     }
 }
 Object.defineProperty(Ts.prototype, "ArrayType", {
     value: Uint16Array
 });
-Object.defineProperty(Sa.prototype, "ArrayType", {
+Object.defineProperty(va.prototype, "ArrayType", {
     value: Float32Array
 });
-Object.defineProperty(Ia.prototype, "ArrayType", {
+Object.defineProperty(wa.prototype, "ArrayType", {
     value: Float64Array
 });
 class Lr extends U {
     constructor() {
         super()
     }
     get typeId() {
@@ -4143,20 +4143,20 @@
         return d.Date
     }
     toString() {
         return `Date${(this.unit+1)*32}<${le[this.unit]}>`
     }
 }
 tr[Symbol.toStringTag] = (e => (e.unit = null, e.ArrayType = Int32Array, e[Symbol.toStringTag] = "Date"))(tr.prototype);
-class ay extends tr {
+class cy extends tr {
     constructor() {
         super(le.DAY)
     }
 }
-class Rc extends tr {
+class jc extends tr {
     constructor() {
         super(le.MILLISECOND)
     }
 }
 class zi extends U {
     constructor(t, n) {
         super(), this.unit = t, this.bitWidth = n
@@ -4210,26 +4210,26 @@
         return this.children[0]
     }
     get ArrayType() {
         return this.valueType.ArrayType
     }
 }
 er[Symbol.toStringTag] = (e => (e.children = null, e[Symbol.toStringTag] = "List"))(er.prototype);
-class Qt extends U {
+class te extends U {
     constructor(t) {
         super(), this.children = t
     }
     get typeId() {
         return d.Struct
     }
     toString() {
         return `Struct<{${this.children.map(t=>`${t.name}:${t.type}`).join(", ")}}>`
     }
 }
-Qt[Symbol.toStringTag] = (e => (e.children = null, e[Symbol.toStringTag] = "Struct"))(Qt.prototype);
+te[Symbol.toStringTag] = (e => (e.children = null, e[Symbol.toStringTag] = "Struct"))(te.prototype);
 class kr extends U {
     constructor(t, n, r) {
         super(), this.mode = t, this.children = r, this.typeIds = n = Int32Array.from(n), this.typeIdToChildIndex = n.reduce((s, o, i) => (s[o] = i) && s || s, Object.create(null))
     }
     get typeId() {
         return d.Union
     }
@@ -4285,18 +4285,18 @@
         return this.children[0].type.children[1].type
     }
     toString() {
         return `Map<{${this.children[0].type.children.map(t=>`${t.name}:${t.type}`).join(", ")}}>`
     }
 }
 Ur[Symbol.toStringTag] = (e => (e.children = null, e.keysSorted = null, e[Symbol.toStringTag] = "Map_"))(Ur.prototype);
-const cy = (e => () => ++e)(-1);
-class Ke extends U {
+const uy = (e => () => ++e)(-1);
+class Ze extends U {
     constructor(t, n, r, s) {
-        super(), this.indices = n, this.dictionary = t, this.isOrdered = s || !1, this.id = r == null ? cy() : typeof r == "number" ? r : r.low
+        super(), this.indices = n, this.dictionary = t, this.isOrdered = s || !1, this.id = r == null ? uy() : typeof r == "number" ? r : r.low
     }
     get typeId() {
         return d.Dictionary
     }
     get children() {
         return this.dictionary.children
     }
@@ -4306,17 +4306,17 @@
     get ArrayType() {
         return this.dictionary.ArrayType
     }
     toString() {
         return `Dictionary<${this.indices}, ${this.dictionary}>`
     }
 }
-Ke[Symbol.toStringTag] = (e => (e.id = null, e.indices = null, e.isOrdered = null, e.dictionary = null, e[Symbol.toStringTag] = "Dictionary"))(Ke.prototype);
+Ze[Symbol.toStringTag] = (e => (e.id = null, e.indices = null, e.isOrdered = null, e.dictionary = null, e[Symbol.toStringTag] = "Dictionary"))(Ze.prototype);
 
-function Jl(e) {
+function ql(e) {
     let t = e;
     switch (e.typeId) {
         case d.Decimal:
             return 4;
         case d.Timestamp:
             return 2;
         case d.Date:
@@ -4331,20 +4331,20 @@
             return t.listSize;
         case d.FixedSizeBinary:
             return t.byteWidth;
         default:
             return 1
     }
 }
-const uy = -1;
+const ly = -1;
 class S {
     constructor(t, n, r, s, o, i, a) {
         this.type = t, this.dictionary = a, this.offset = Math.floor(Math.max(n || 0, 0)), this.length = Math.floor(Math.max(r || 0, 0)), this._nullCount = Math.floor(Math.max(s || 0, -1)), this.childData = (i || []).map(u => u instanceof S ? u : u.data);
         let c;
-        o instanceof S ? (this.stride = o.stride, this.values = o.values, this.typeIds = o.typeIds, this.nullBitmap = o.nullBitmap, this.valueOffsets = o.valueOffsets) : (this.stride = Jl(t), o && ((c = o[0]) && (this.valueOffsets = c), (c = o[1]) && (this.values = c), (c = o[2]) && (this.nullBitmap = c), (c = o[3]) && (this.typeIds = c)))
+        o instanceof S ? (this.stride = o.stride, this.values = o.values, this.typeIds = o.typeIds, this.nullBitmap = o.nullBitmap, this.valueOffsets = o.valueOffsets) : (this.stride = ql(t), o && ((c = o[0]) && (this.valueOffsets = c), (c = o[1]) && (this.values = c), (c = o[2]) && (this.nullBitmap = c), (c = o[3]) && (this.typeIds = c)))
     }
     get typeId() {
         return this.type.typeId
     }
     get ArrayType() {
         return this.type.ArrayType
     }
@@ -4360,15 +4360,15 @@
                 typeIds: o
             } = this;
         return n && (t += n.byteLength), r && (t += r.byteLength), s && (t += s.byteLength), o && (t += o.byteLength), this.childData.reduce((i, a) => i + a.byteLength, t)
     }
     get nullCount() {
         let t = this._nullCount,
             n;
-        return t <= uy && (n = this.nullBitmap) && (this._nullCount = t = this.length - ji(n, this.offset, this.offset + this.length)), t
+        return t <= ly && (n = this.nullBitmap) && (this._nullCount = t = this.length - ji(n, this.offset, this.offset + this.length)), t
     }
     clone(t, n = this.offset, r = this.length, s = this._nullCount, o = this, i = this.childData) {
         return new S(t, n, r, s, o, i, this.dictionary)
     }
     slice(t, n) {
         const {
             stride: r,
@@ -4467,73 +4467,73 @@
     static Interval(t, n, r, s, o, i) {
         return new S(t, n, r, s, [void 0, R(t.ArrayType, i), j(o)])
     }
     static FixedSizeBinary(t, n, r, s, o, i) {
         return new S(t, n, r, s, [void 0, R(t.ArrayType, i), j(o)])
     }
     static Binary(t, n, r, s, o, i, a) {
-        return new S(t, n, r, s, [kn(i), j(a), j(o)])
+        return new S(t, n, r, s, [En(i), j(a), j(o)])
     }
     static Utf8(t, n, r, s, o, i, a) {
-        return new S(t, n, r, s, [kn(i), j(a), j(o)])
+        return new S(t, n, r, s, [En(i), j(a), j(o)])
     }
     static List(t, n, r, s, o, i, a) {
-        return new S(t, n, r, s, [kn(i), void 0, j(o)], [a])
+        return new S(t, n, r, s, [En(i), void 0, j(o)], [a])
     }
     static FixedSizeList(t, n, r, s, o, i) {
         return new S(t, n, r, s, [void 0, void 0, j(o)], [i])
     }
     static Struct(t, n, r, s, o, i) {
         return new S(t, n, r, s, [void 0, void 0, j(o)], i)
     }
     static Map(t, n, r, s, o, i, a) {
-        return new S(t, n, r, s, [kn(i), void 0, j(o)], [a])
+        return new S(t, n, r, s, [En(i), void 0, j(o)], [a])
     }
     static Union(t, n, r, s, o, i, a, c) {
         const u = [void 0, void 0, j(o), R(t.ArrayType, i)];
-        return t.mode === Be.Sparse ? new S(t, n, r, s, u, a) : (u[T.OFFSET] = kn(a), new S(t, n, r, s, u, c))
+        return t.mode === Be.Sparse ? new S(t, n, r, s, u, a) : (u[T.OFFSET] = En(a), new S(t, n, r, s, u, c))
     }
 }
 S.prototype.childData = Object.freeze([]);
-const ly = void 0;
+const fy = void 0;
 
 function Ir(e) {
     if (e === null) return "null";
-    if (e === ly) return "undefined";
+    if (e === fy) return "undefined";
     switch (typeof e) {
         case "number":
             return `${e}`;
         case "bigint":
             return `${e}`;
         case "string":
             return `"${e}"`
     }
     return typeof e[Symbol.toPrimitive] == "function" ? e[Symbol.toPrimitive]("string") : ArrayBuffer.isView(e) ? `[${e}]` : JSON.stringify(e)
 }
 
-function fy(e) {
+function hy(e) {
     if (!e || e.length <= 0) return function(s) {
         return !0
     };
     let t = "",
         n = e.filter(r => r === r);
     return n.length > 0 && (t = `
     switch (x) {${n.map(r=>`
-        case ${hy(r)}:`).join("")}
+        case ${dy(r)}:`).join("")}
             return false;
     }`), e.length !== n.length && (t = `if (x !== x) return false;
 ${t}`), new Function("x", `${t}
 return true;`)
 }
 
-function hy(e) {
+function dy(e) {
     return typeof e != "bigint" ? Ir(e) : ws ? `${Ir(e)}n` : `"${Ir(e)}"`
 }
 const $s = (e, t) => (e * t + 63 & -64 || 64) / t,
-    dy = (e, t = 0) => e.length >= t ? e.subarray(0, t) : Fr(new e.constructor(t), e, 0);
+    py = (e, t = 0) => e.length >= t ? e.subarray(0, t) : Fr(new e.constructor(t), e, 0);
 class Jr {
     constructor(t, n = 1) {
         this.buffer = t, this.stride = n, this.BYTES_PER_ELEMENT = t.BYTES_PER_ELEMENT, this.ArrayType = t.constructor, this._resize(this.length = t.length / n | 0)
     }
     get byteLength() {
         return this.length * this.stride * this.BYTES_PER_ELEMENT | 0
     }
@@ -4557,15 +4557,15 @@
                 s = this.buffer.length;
             r >= s && this._resize(s === 0 ? $s(r * 1, this.BYTES_PER_ELEMENT) : $s(r * 2, this.BYTES_PER_ELEMENT))
         }
         return this
     }
     flush(t = this.length) {
         t = $s(t * this.stride, this.BYTES_PER_ELEMENT);
-        const n = dy(this.buffer, t);
+        const n = py(this.buffer, t);
         return this.clear(), n
     }
     clear() {
         return this.length = 0, this._resize(0), this
     }
     _resize(t) {
         return this.buffer = Fr(new this.ArrayType(t), this.buffer)
@@ -4579,15 +4579,15 @@
     get(t) {
         return this.buffer[t]
     }
     set(t, n) {
         return this.reserve(t - this.length + 1), this.buffer[t * this.stride] = n, this
     }
 }
-class Xl extends Xr {
+class Ql extends Xr {
     constructor(t = new Uint8Array(0)) {
         super(t, 1 / 8), this.numValid = 0
     }
     get numInvalid() {
         return this.length - this.numValid
     }
     get(t) {
@@ -4599,15 +4599,15 @@
         } = this.reserve(t - this.length + 1), s = t >> 3, o = t % 8, i = r[s] >> o & 1;
         return n ? i === 0 && (r[s] |= 1 << o, ++this.numValid) : i === 1 && (r[s] &= ~(1 << o), --this.numValid), this
     }
     clear() {
         return this.numValid = 0, super.clear()
     }
 }
-class ql extends Xr {
+class tf extends Xr {
     constructor(t = new Int32Array(1)) {
         super(t, 1)
     }
     append(t) {
         return this.set(this.length - 1, t)
     }
     set(t, n) {
@@ -4615,15 +4615,15 @@
             s = this.reserve(t - r + 1).buffer;
         return r < t++ && s.fill(s[r], r, t), s[t] = s[t - 1] + n, this
     }
     flush(t = this.length - 1) {
         return t > this.length && this.set(t - 1, 0), super.flush(t + 1)
     }
 }
-class Ql extends Jr {
+class ef extends Jr {
     get ArrayType64() {
         return this._ArrayType64 || (this._ArrayType64 = this.buffer instanceof Int32Array ? ur : Yr)
     }
     set(t, n) {
         switch (this.reserve(t - this.length + 1), typeof n) {
             case "bigint":
                 this.buffer64[t] = n;
@@ -4643,28 +4643,28 @@
     }
 }
 class at {
     constructor({
         type: t,
         nullValues: n
     }) {
-        this.length = 0, this.finished = !1, this.type = t, this.children = [], this.nullValues = n, this.stride = Jl(t), this._nulls = new Xl, n && n.length > 0 && (this._isValid = fy(n))
+        this.length = 0, this.finished = !1, this.type = t, this.children = [], this.nullValues = n, this.stride = ql(t), this._nulls = new Ql, n && n.length > 0 && (this._isValid = hy(n))
     }
     static new(t) {}
     static throughNode(t) {
         throw new Error('"throughNode" not available in this environment')
     }
     static throughDOM(t) {
         throw new Error('"throughDOM" not available in this environment')
     }
     static throughIterable(t) {
-        return py(t)
+        return yy(t)
     }
     static throughAsyncIterable(t) {
-        return yy(t)
+        return by(t)
     }
     toVector() {
         return z.new(this.flush())
     }
     get ArrayType() {
         return this.type.ArrayType
     }
@@ -4740,26 +4740,26 @@
 }
 at.prototype.length = 1;
 at.prototype.stride = 1;
 at.prototype.children = null;
 at.prototype.finished = !1;
 at.prototype.nullValues = null;
 at.prototype._isValid = () => !0;
-class Xe extends at {
+class Qe extends at {
     constructor(t) {
         super(t), this._values = new Xr(new this.ArrayType(0), this.stride)
     }
     setValue(t, n) {
         const r = this._values;
         return r.reserve(t - r.length + 1), super.setValue(t, n)
     }
 }
 class As extends at {
     constructor(t) {
-        super(t), this._pendingLength = 0, this._offsets = new ql
+        super(t), this._pendingLength = 0, this._offsets = new tf
     }
     setValue(t, n) {
         const r = this._pending || (this._pending = new Map),
             s = r.get(t);
         s && (this._pendingLength -= s.length), this._pendingLength += n.length, r.set(t, n)
     }
     setValid(t, n) {
@@ -4777,67 +4777,67 @@
     _flush() {
         const t = this._pending,
             n = this._pendingLength;
         return this._pendingLength = 0, this._pending = void 0, t && t.size > 0 && this._flushPending(t, n), this
     }
 }
 
-function py(e) {
+function yy(e) {
     const {
         ["queueingStrategy"]: t = "count"
     } = e, {
         ["highWaterMark"]: n = t !== "bytes" ? 1e3 : 2 ** 14
     } = e, r = t !== "bytes" ? "length" : "byteLength";
     return function*(s) {
         let o = 0,
             i = at.new(e);
         for (const a of s) i.append(a)[r] >= n && ++o && (yield i.toVector());
         (i.finish().length > 0 || o === 0) && (yield i.toVector())
     }
 }
 
-function yy(e) {
+function by(e) {
     const {
         ["queueingStrategy"]: t = "count"
     } = e, {
         ["highWaterMark"]: n = t !== "bytes" ? 1e3 : 2 ** 14
     } = e, r = t !== "bytes" ? "length" : "byteLength";
     return async function*(s) {
         let o = 0,
             i = at.new(e);
         for await (const a of s) i.append(a)[r] >= n && ++o && (yield i.toVector());
         (i.finish().length > 0 || o === 0) && (yield i.toVector())
     }
 }
-class by extends at {
+class my extends at {
     constructor(t) {
-        super(t), this._values = new Xl
+        super(t), this._values = new Ql
     }
     setValue(t, n) {
         this._values.set(t, +n)
     }
 }
-class my extends at {
+class gy extends at {
     setValue(t, n) {}
     setValid(t, n) {
         return this.length = Math.max(t + 1, this.length), n
     }
 }
-class Ta extends Xe {}
-class gy extends Ta {}
-class vy extends Ta {}
-class wy extends Xe {}
-class _y extends at {
+class _a extends Qe {}
+class vy extends _a {}
+class wy extends _a {}
+class _y extends Qe {}
+class Sy extends at {
     constructor({
         type: t,
         nullValues: n,
         dictionaryHashFunction: r
     }) {
         super({
-            type: new Ke(t.dictionary, t.indices, t.id, t.isOrdered)
+            type: new Ze(t.dictionary, t.indices, t.id, t.isOrdered)
         }), this._nulls = null, this._dictionaryOffset = 0, this._keysToIndices = Object.create(null), this.indices = at.new({
             type: this.type.indices,
             nullValues: n
         }), this.dictionary = at.new({
             type: this.type.dictionary,
             nullValues: null
         }), typeof r == "function" && (this.valueToKey = r)
@@ -4886,151 +4886,151 @@
     clear() {
         return this.indices.clear(), this.dictionary.clear(), super.clear()
     }
     valueToKey(t) {
         return typeof t == "string" ? t : `${t}`
     }
 }
-class Sy extends Xe {}
-const tf = new Float64Array(1),
-    On = new Uint32Array(tf.buffer);
+class Iy extends Qe {}
+const nf = new Float64Array(1),
+    Fn = new Uint32Array(nf.buffer);
 
-function ef(e) {
+function rf(e) {
     let t = (e & 31744) >> 10,
         n = (e & 1023) / 1024,
         r = (-1) ** ((e & 32768) >> 15);
     switch (t) {
         case 31:
             return r * (n ? NaN : 1 / 0);
         case 0:
             return r * (n ? 6103515625e-14 * n : 0)
     }
     return r * 2 ** (t - 15) * (1 + n)
 }
 
-function Aa(e) {
+function Sa(e) {
     if (e !== e) return 32256;
-    tf[0] = e;
-    let t = (On[1] & 2147483648) >> 16 & 65535,
-        n = On[1] & 2146435072,
+    nf[0] = e;
+    let t = (Fn[1] & 2147483648) >> 16 & 65535,
+        n = Fn[1] & 2146435072,
         r = 0;
-    return n >= 1089470464 ? On[0] > 0 ? n = 31744 : (n = (n & 2080374784) >> 16, r = (On[1] & 1048575) >> 10) : n <= 1056964608 ? (r = 1048576 + (On[1] & 1048575), r = 1048576 + (r << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, r = (On[1] & 1048575) + 512 >> 10), t | n | r & 65535
+    return n >= 1089470464 ? Fn[0] > 0 ? n = 31744 : (n = (n & 2080374784) >> 16, r = (Fn[1] & 1048575) >> 10) : n <= 1056964608 ? (r = 1048576 + (Fn[1] & 1048575), r = 1048576 + (r << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, r = (Fn[1] & 1048575) + 512 >> 10), t | n | r & 65535
 }
-const Iy = Object.freeze(Object.defineProperty({
+const Ty = Object.freeze(Object.defineProperty({
     __proto__: null,
-    uint16ToFloat64: ef,
-    float64ToUint16: Aa
+    uint16ToFloat64: rf,
+    float64ToUint16: Sa
 }, Symbol.toStringTag, {
     value: "Module"
 }));
-class Bs extends Xe {}
-class Ty extends Bs {
+class Bs extends Qe {}
+class Ay extends Bs {
     setValue(t, n) {
-        this._values.set(t, Aa(n))
+        this._values.set(t, Sa(n))
     }
 }
-class Ay extends Bs {
+class By extends Bs {
     setValue(t, n) {
         this._values.set(t, n)
     }
 }
-class By extends Bs {
+class Oy extends Bs {
     setValue(t, n) {
         this._values.set(t, n)
     }
 }
-const nf = Symbol.for("isArrowBigNum");
+const sf = Symbol.for("isArrowBigNum");
 
-function ne(e, ...t) {
+function re(e, ...t) {
     return t.length === 0 ? Object.setPrototypeOf(R(this.TypedArray, e), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(e, ...t), this.constructor.prototype)
 }
-ne.prototype[nf] = !0;
-ne.prototype.toJSON = function() {
-    return `"${ze(this)}"`
+re.prototype[sf] = !0;
+re.prototype.toJSON = function() {
+    return `"${We(this)}"`
 };
-ne.prototype.valueOf = function() {
-    return rf(this)
+re.prototype.valueOf = function() {
+    return of(this)
 };
-ne.prototype.toString = function() {
-    return ze(this)
+re.prototype.toString = function() {
+    return We(this)
 };
-ne.prototype[Symbol.toPrimitive] = function(e = "default") {
+re.prototype[Symbol.toPrimitive] = function(e = "default") {
     switch (e) {
         case "number":
-            return rf(this);
+            return of(this);
         case "string":
-            return ze(this);
+            return We(this);
         case "default":
             return Mr(this)
     }
-    return ze(this)
+    return We(this)
 };
 
 function Pn(...e) {
-    return ne.apply(this, e)
+    return re.apply(this, e)
 }
 
 function zn(...e) {
-    return ne.apply(this, e)
+    return re.apply(this, e)
 }
 
 function Nr(...e) {
-    return ne.apply(this, e)
+    return re.apply(this, e)
 }
 Object.setPrototypeOf(Pn.prototype, Object.create(Int32Array.prototype));
 Object.setPrototypeOf(zn.prototype, Object.create(Uint32Array.prototype));
 Object.setPrototypeOf(Nr.prototype, Object.create(Uint32Array.prototype));
-Object.assign(Pn.prototype, ne.prototype, {
+Object.assign(Pn.prototype, re.prototype, {
     constructor: Pn,
     signed: !0,
     TypedArray: Int32Array,
     BigIntArray: ur
 });
-Object.assign(zn.prototype, ne.prototype, {
+Object.assign(zn.prototype, re.prototype, {
     constructor: zn,
     signed: !1,
     TypedArray: Uint32Array,
     BigIntArray: Yr
 });
-Object.assign(Nr.prototype, ne.prototype, {
+Object.assign(Nr.prototype, re.prototype, {
     constructor: Nr,
     signed: !0,
     TypedArray: Uint32Array,
     BigIntArray: Yr
 });
 
-function rf(e) {
+function of(e) {
     let {
         buffer: t,
         byteOffset: n,
         length: r,
         signed: s
     } = e, o = new Int32Array(t, n, r), i = 0, a = 0, c = o.length, u, l;
     for (; a < c;) l = o[a++], u = o[a++], s || (u = u >>> 0), i += (l >>> 0) + u * a ** 32;
     return i
 }
-let ze, Mr;
-ws ? (Mr = e => e.byteLength === 8 ? new e.BigIntArray(e.buffer, e.byteOffset, 1)[0] : Ys(e), ze = e => e.byteLength === 8 ? `${new e.BigIntArray(e.buffer,e.byteOffset,1)[0]}` : Ys(e)) : (ze = Ys, Mr = ze);
+let We, Mr;
+ws ? (Mr = e => e.byteLength === 8 ? new e.BigIntArray(e.buffer, e.byteOffset, 1)[0] : Ys(e), We = e => e.byteLength === 8 ? `${new e.BigIntArray(e.buffer,e.byteOffset,1)[0]}` : Ys(e)) : (We = Ys, Mr = We);
 
 function Ys(e) {
     let t = "",
         n = new Uint32Array(2),
         r = new Uint16Array(e.buffer, e.byteOffset, e.byteLength / 2),
         s = new Uint32Array((r = new Uint16Array(r).reverse()).buffer),
         o = -1,
         i = r.length - 1;
     do {
         for (n[0] = r[o = 0]; o < i;) r[o++] = n[1] = n[0] / 10, n[0] = (n[0] - n[1] * 10 << 16) + r[o];
         r[o] = n[1] = n[0] / 10, n[0] = n[0] - n[1] * 10, t = `${n[0]}${t}`
     } while (s[0] || s[1] || s[2] || s[3]);
     return t || "0"
 }
-class Sn {
+class In {
     constructor(t, n) {
-        return Sn.new(t, n)
+        return In.new(t, n)
     }
     static new(t, n) {
         switch (n) {
             case !0:
                 return new Pn(t);
             case !1:
                 return new zn(t)
@@ -5050,77 +5050,77 @@
     static unsigned(t) {
         return new zn(t)
     }
     static decimal(t) {
         return new Nr(t)
     }
 }
-const Oy = Object.freeze(Object.defineProperty({
+const Fy = Object.freeze(Object.defineProperty({
     __proto__: null,
-    isArrowBigNumSymbol: nf,
+    isArrowBigNumSymbol: sf,
     get bignumToString() {
-        return ze
+        return We
     },
     get bignumToBigInt() {
         return Mr
     },
-    BN: Sn
+    BN: In
 }, Symbol.toStringTag, {
     value: "Module"
 }));
-class Ee extends Xe {
+class Ee extends Qe {
     setValue(t, n) {
         this._values.set(t, n)
     }
 }
-class Fy extends Ee {}
 class xy extends Ee {}
 class Ly extends Ee {}
-class Dy extends Ee {
+class Dy extends Ee {}
+class ky extends Ee {
     constructor(t) {
-        t.nullValues && (t.nullValues = t.nullValues.map(Gi)), super(t), this._values = new Ql(new Int32Array(0), 2)
+        t.nullValues && (t.nullValues = t.nullValues.map(Gi)), super(t), this._values = new ef(new Int32Array(0), 2)
     }
     get values64() {
         return this._values.buffer64
     }
     isValid(t) {
         return super.isValid(Gi(t))
     }
 }
-class ky extends Ee {}
 class Ey extends Ee {}
 class Uy extends Ee {}
-class Ny extends Ee {
+class Ny extends Ee {}
+class My extends Ee {
     constructor(t) {
-        t.nullValues && (t.nullValues = t.nullValues.map(Gi)), super(t), this._values = new Ql(new Uint32Array(0), 2)
+        t.nullValues && (t.nullValues = t.nullValues.map(Gi)), super(t), this._values = new ef(new Uint32Array(0), 2)
     }
     get values64() {
         return this._values.buffer64
     }
     isValid(t) {
         return super.isValid(Gi(t))
     }
 }
 const Gi = (e => t => (ArrayBuffer.isView(t) && (e.buffer = t.buffer, e.byteOffset = t.byteOffset, e.byteLength = t.byteLength, t = Mr(e), e.buffer = null), t))({
     BigIntArray: ur
 });
-class qr extends Xe {}
-class My extends qr {}
+class qr extends Qe {}
 class Cy extends qr {}
 class Ry extends qr {}
 class Vy extends qr {}
-class Qr extends Xe {}
-class jy extends Qr {}
+class jy extends qr {}
+class Qr extends Qe {}
 class Py extends Qr {}
 class zy extends Qr {}
 class Wy extends Qr {}
-class Ba extends Xe {}
-class $y extends Ba {}
-class Yy extends Ba {}
-class sf extends As {
+class $y extends Qr {}
+class Ia extends Qe {}
+class Yy extends Ia {}
+class Gy extends Ia {}
+class af extends As {
     constructor(t) {
         super(t), this._values = new Jr(new Uint8Array(0))
     }
     get byteLength() {
         let t = this._pendingLength + this.length * 4;
         return this._offsets && (t += this._offsets.byteLength), this._values && (t += this._values.byteLength), this._nulls && (t += this._nulls.byteLength), t
     }
@@ -5133,29 +5133,29 @@
         let o = 0,
             i = 0,
             a = 0,
             c;
         for ([o, c] of t) c === void 0 ? r.set(o, 0) : (i = c.length, s.set(c, a), r.set(o, i), a += i)
     }
 }
-class Oa extends As {
+class Ta extends As {
     constructor(t) {
         super(t), this._values = new Jr(new Uint8Array(0))
     }
     get byteLength() {
         let t = this._pendingLength + this.length * 4;
         return this._offsets && (t += this._offsets.byteLength), this._values && (t += this._values.byteLength), this._nulls && (t += this._nulls.byteLength), t
     }
     setValue(t, n) {
         return super.setValue(t, vs(n))
     }
     _flushPending(t, n) {}
 }
-Oa.prototype._flushPending = sf.prototype._flushPending;
-class of {
+Ta.prototype._flushPending = af.prototype._flushPending;
+class cf {
     get length() {
         return this._values.length
     }
     get(t) {
         return this._values[t]
     }
     clear() {
@@ -5262,17 +5262,17 @@
     [Wn]: {
         writable: !0,
         enumerable: !1,
         configurable: !1,
         value: -1
     }
 }), e[Symbol.toStringTag] = "Row"))(Se.prototype);
-class af extends Se {
+class uf extends Se {
     constructor(t) {
-        return super(t, t.length), Gy(this)
+        return super(t, t.length), Ky(this)
     }
     keys() {
         return this[bt].getChildAt(0)[Symbol.iterator]()
     }
     values() {
         return this[bt].getChildAt(1)[Symbol.iterator]()
     }
@@ -5285,17 +5285,17 @@
     getValue(t) {
         return this[bt].getChildAt(1).get(t)
     }
     setValue(t, n) {
         this[bt].getChildAt(1).set(t, n)
     }
 }
-class cf extends Se {
+class lf extends Se {
     constructor(t) {
-        return super(t, t.type.children.length), uf(this)
+        return super(t, t.type.children.length), ff(this)
     }* keys() {
         for (const t of this[bt].type.children) yield t.name
     }* values() {
         for (const t of this[bt].type.children) yield this[t.name]
     }
     getKey(t) {
         return this[bt].type.children[t].name
@@ -5307,15 +5307,15 @@
         return this[bt].getChildAt(t).get(this[Wn])
     }
     setValue(t, n) {
         return this[bt].getChildAt(t).set(this[Wn], n)
     }
 }
 Object.setPrototypeOf(Se.prototype, Map.prototype);
-const uf = (() => {
+const ff = (() => {
         const e = {
             enumerable: !0,
             configurable: !1,
             get: null,
             set: null
         };
         return t => {
@@ -5327,16 +5327,16 @@
                 o = i => function(a) {
                     return this.set(i, a)
                 };
             for (const i of t.keys()) r.set(i, ++n), e.get = s(i), e.set = o(i), t.hasOwnProperty(i) || (e.enumerable = !0, Object.defineProperty(t, i, e)), t.hasOwnProperty(n) || (e.enumerable = !1, Object.defineProperty(t, n, e));
             return e.get = e.set = null, t
         }
     })(),
-    Gy = (() => {
-        if (typeof Proxy > "u") return uf;
+    Ky = (() => {
+        if (typeof Proxy > "u") return ff;
         const e = Se.prototype.has,
             t = Se.prototype.get,
             n = Se.prototype.set,
             r = Se.prototype.getKey,
             s = {
                 isExtensible() {
                     return !1
@@ -5476,126 +5476,126 @@
                     }
                     return typeof i == "number" && !e.call(c, i) && (i = r.call(c, i)), e.call(c, i) ? !!n.call(c, i, a) : !1
                 }
             };
         return o => new Proxy(o, s)
     })();
 
-function Ky(e, t, n) {
+function Zy(e, t, n) {
     const r = e.length,
         s = t > -1 ? t : r + t % r;
     return n ? n(e, s) : s
 }
-let Vc;
+let Pc;
 
-function Fa(e, t, n, r) {
+function Aa(e, t, n, r) {
     let {
         length: s = 0
     } = e, o = typeof t != "number" ? 0 : t, i = typeof n != "number" ? s : n;
-    return o < 0 && (o = (o % s + s) % s), i < 0 && (i = (i % s + s) % s), i < o && (Vc = o, o = i, i = Vc), i > s && (i = s), r ? r(e, o, i) : [o, i]
+    return o < 0 && (o = (o % s + s) % s), i < 0 && (i = (i % s + s) % s), i < o && (Pc = o, o = i, i = Pc), i > s && (i = s), r ? r(e, o, i) : [o, i]
 }
-const Zy = ws ? gp(0) : 0,
-    jc = e => e !== e;
+const Hy = ws ? vp(0) : 0,
+    zc = e => e !== e;
 
-function In(e) {
+function Tn(e) {
     let t = typeof e;
-    if (t !== "object" || e === null) return jc(e) ? jc : t !== "bigint" ? n => n === e : n => Zy + n === e;
+    if (t !== "object" || e === null) return zc(e) ? zc : t !== "bigint" ? n => n === e : n => Hy + n === e;
     if (e instanceof Date) {
         const n = e.valueOf();
         return r => r instanceof Date ? r.valueOf() === n : !1
     }
-    return ArrayBuffer.isView(e) ? n => n ? Yl(e, n) : !1 : e instanceof Map ? Jy(e) : Array.isArray(e) ? Hy(e) : e instanceof z ? Xy(e) : qy(e)
+    return ArrayBuffer.isView(e) ? n => n ? Kl(e, n) : !1 : e instanceof Map ? Xy(e) : Array.isArray(e) ? Jy(e) : e instanceof z ? qy(e) : Qy(e)
 }
 
-function Hy(e) {
+function Jy(e) {
     const t = [];
-    for (let n = -1, r = e.length; ++n < r;) t[n] = In(e[n]);
+    for (let n = -1, r = e.length; ++n < r;) t[n] = Tn(e[n]);
     return Os(t)
 }
 
-function Jy(e) {
+function Xy(e) {
     let t = -1;
     const n = [];
-    return e.forEach(r => n[++t] = In(r)), Os(n)
+    return e.forEach(r => n[++t] = Tn(r)), Os(n)
 }
 
-function Xy(e) {
+function qy(e) {
     const t = [];
-    for (let n = -1, r = e.length; ++n < r;) t[n] = In(e.get(n));
+    for (let n = -1, r = e.length; ++n < r;) t[n] = Tn(e.get(n));
     return Os(t)
 }
 
-function qy(e) {
+function Qy(e) {
     const t = Object.keys(e);
     if (t.length === 0) return () => !1;
     const n = [];
-    for (let r = -1, s = t.length; ++r < s;) n[r] = In(e[t[r]]);
+    for (let r = -1, s = t.length; ++r < s;) n[r] = Tn(e[t[r]]);
     return Os(n, t)
 }
 
 function Os(e, t) {
     return n => {
         if (!n || typeof n != "object") return !1;
         switch (n.constructor) {
             case Array:
-                return Qy(e, n);
+                return tb(e, n);
             case Map:
-            case af:
-            case cf:
-                return Pc(e, n, n.keys());
+            case uf:
+            case lf:
+                return Wc(e, n, n.keys());
             case Object:
             case void 0:
-                return Pc(e, n, t || Object.keys(n))
+                return Wc(e, n, t || Object.keys(n))
         }
-        return n instanceof z ? tb(e, n) : !1
+        return n instanceof z ? eb(e, n) : !1
     }
 }
 
-function Qy(e, t) {
+function tb(e, t) {
     const n = e.length;
     if (t.length !== n) return !1;
     for (let r = -1; ++r < n;)
         if (!e[r](t[r])) return !1;
     return !0
 }
 
-function tb(e, t) {
+function eb(e, t) {
     const n = e.length;
     if (t.length !== n) return !1;
     for (let r = -1; ++r < n;)
         if (!e[r](t.get(r))) return !1;
     return !0
 }
 
-function Pc(e, t, n) {
+function Wc(e, t, n) {
     const r = n[Symbol.iterator](),
         s = t instanceof Map ? t.keys() : Object.keys(t)[Symbol.iterator](),
         o = t instanceof Map ? t.values() : Object.values(t)[Symbol.iterator]();
     let i = 0,
         a = e.length,
         c = o.next(),
         u = r.next(),
         l = s.next();
     for (; i < a && !u.done && !l.done && !c.done && !(u.value !== l.value || !e[i](c.value)); ++i, u = r.next(), l = s.next(), c = o.next());
     return i === a && u.done && l.done && c.done ? !0 : (r.return && r.return(), s.return && s.return(), o.return && o.return(), !1)
 }
-const eb = Object.freeze(Object.defineProperty({
+const nb = Object.freeze(Object.defineProperty({
     __proto__: null,
-    clampIndex: Ky,
-    clampRange: Fa,
-    createElementComparator: In
+    clampIndex: Zy,
+    clampRange: Aa,
+    createElementComparator: Tn
 }, Symbol.toStringTag, {
     value: "Module"
 }));
 class mt extends z {
-    constructor(t, n = [], r = nb(n)) {
+    constructor(t, n = [], r = rb(n)) {
         super(), this._nullCount = -1, this._type = t, this._chunks = n, this._chunkOffsets = r, this._length = r[r.length - 1], this._numChildren = (this._type.children || []).length
     }
     static flatten(...t) {
-        return ob(z, t)
+        return ab(z, t)
     }
     static concat(...t) {
         const n = mt.flatten(...t);
         return new mt(n[0].type, n)
     }
     get type() {
         return this._type
@@ -5651,15 +5651,15 @@
     clone(t = this._chunks) {
         return new mt(this._type, t)
     }
     concat(...t) {
         return this.clone(mt.flatten(this, ...t))
     }
     slice(t, n) {
-        return Fa(this, t, n, this._sliceInternal)
+        return Aa(this, t, n, this._sliceInternal)
     }
     getChildAt(t) {
         if (t < 0 || t >= this._numChildren) return null;
         let n = this._children || (this._children = []),
             r, s, o;
         return (r = n[t]) ? r : (s = (this._type.children || [])[t]) && (o = this._chunks.map(i => i.getChildAt(t)).filter(i => i != null), o.length > 0) ? n[t] = new mt(s.type, o) : null
     }
@@ -5700,15 +5700,15 @@
         if (n <= 0) return new r(0);
         if (n <= 1) return t[0].toArray();
         let s = 0,
             o = new Array(n);
         for (let c = -1; ++c < n;) s += (o[c] = t[c].toArray()).length;
         r !== o[0].constructor && (r = o[0].constructor);
         let i = new r(s),
-            a = r === Array ? ib : rb;
+            a = r === Array ? sb : ib;
         for (let c = -1, u = 0; ++c < n;) u = a(o[c], i, u);
         return i
     }
     getInternal({
         _chunks: t
     }, n, r) {
         return t[n].get(r)
@@ -5752,66 +5752,66 @@
                 p = Math.min(r - f, l);
             s.push(u.slice(h, p))
         }
         return t.clone(s)
     }
 }
 
-function nb(e) {
+function rb(e) {
     let t = new Uint32Array((e || []).length + 1),
         n = t[0] = 0,
         r = t.length;
     for (let s = 0; ++s < r;) t[s] = n += e[s - 1].length;
     return t
 }
-const rb = (e, t, n) => (t.set(e, n), n + e.length),
-    ib = (e, t, n) => {
+const ib = (e, t, n) => (t.set(e, n), n + e.length),
+    sb = (e, t, n) => {
         let r = n;
         for (let s = -1, o = e.length; ++s < o;) t[r++] = e[s];
         return r
     };
-class Kt extends mt {
+class Zt extends mt {
     constructor(t, n = [], r) {
-        if (n = mt.flatten(...n), super(t.type, n, r), this._field = t, n.length === 1 && !(this instanceof zc)) return new zc(t, n[0], this._chunkOffsets)
+        if (n = mt.flatten(...n), super(t.type, n, r), this._field = t, n.length === 1 && !(this instanceof $c)) return new $c(t, n[0], this._chunkOffsets)
     }
     static new(t, n, ...r) {
         const s = mt.flatten(Array.isArray(n) ? [...n, ...r] : n instanceof z ? [n, ...r] : [z.new(n, ...r)]);
         if (typeof t == "string") {
             const o = s[0].data.type;
             t = new W(t, o, !0)
         } else !t.nullable && s.some(({
             nullCount: o
         }) => o > 0) && (t = t.clone({
             nullable: !0
         }));
-        return new Kt(t, s)
+        return new Zt(t, s)
     }
     get field() {
         return this._field
     }
     get name() {
         return this._field.name
     }
     get nullable() {
         return this._field.nullable
     }
     get metadata() {
         return this._field.metadata
     }
     clone(t = this._chunks) {
-        return new Kt(this._field, t)
+        return new Zt(this._field, t)
     }
     getChildAt(t) {
         if (t < 0 || t >= this.numChildren) return null;
         let n = this._children || (this._children = []),
             r, s, o;
-        return (r = n[t]) ? r : (s = (this.type.children || [])[t]) && (o = this._chunks.map(i => i.getChildAt(t)).filter(i => i != null), o.length > 0) ? n[t] = new Kt(s, o) : null
+        return (r = n[t]) ? r : (s = (this.type.children || [])[t]) && (o = this._chunks.map(i => i.getChildAt(t)).filter(i => i != null), o.length > 0) ? n[t] = new Zt(s, o) : null
     }
 }
-class zc extends Kt {
+class $c extends Zt {
     constructor(t, n, r) {
         super(t, [n], r), this._chunk = n
     }
     search(t, n) {
         return n ? n(this, 0, t) : [0, t]
     }
     isValid(t) {
@@ -5823,106 +5823,106 @@
     set(t, n) {
         this._chunk.set(t, n)
     }
     indexOf(t, n) {
         return this._chunk.indexOf(t, n)
     }
 }
-const cn = Array.isArray,
-    lf = (e, t) => xa(e, t, [], 0),
-    sb = e => {
-        const [t, n] = La(e, [
+const ln = Array.isArray,
+    hf = (e, t) => Ba(e, t, [], 0),
+    ob = e => {
+        const [t, n] = Oa(e, [
             [],
             []
         ]);
-        return n.map((r, s) => r instanceof Kt ? Kt.new(r.field.clone(t[s]), r) : r instanceof z ? Kt.new(t[s], r) : Kt.new(t[s], []))
+        return n.map((r, s) => r instanceof Zt ? Zt.new(r.field.clone(t[s]), r) : r instanceof z ? Zt.new(t[s], r) : Zt.new(t[s], []))
     },
-    ff = e => La(e, [
+    df = e => Oa(e, [
         [],
         []
     ]),
-    ob = (e, t) => Fo(e, t, [], 0),
-    ab = (e, t) => hf(e, t, [], 0);
+    ab = (e, t) => Fo(e, t, [], 0),
+    cb = (e, t) => pf(e, t, [], 0);
 
-function xa(e, t, n, r) {
+function Ba(e, t, n, r) {
     let s, o = r,
         i = -1,
         a = t.length;
-    for (; ++i < a;) cn(s = t[i]) ? o = xa(e, s, n, o).length : s instanceof e && (n[o++] = s);
+    for (; ++i < a;) ln(s = t[i]) ? o = Ba(e, s, n, o).length : s instanceof e && (n[o++] = s);
     return n
 }
 
 function Fo(e, t, n, r) {
     let s, o = r,
         i = -1,
         a = t.length;
-    for (; ++i < a;) cn(s = t[i]) ? o = Fo(e, s, n, o).length : s instanceof mt ? o = Fo(e, s.chunks, n, o).length : s instanceof e && (n[o++] = s);
+    for (; ++i < a;) ln(s = t[i]) ? o = Fo(e, s, n, o).length : s instanceof mt ? o = Fo(e, s.chunks, n, o).length : s instanceof e && (n[o++] = s);
     return n
 }
 
-function hf(e, t, n, r) {
+function pf(e, t, n, r) {
     let s, o = r,
         i = -1,
         a = t.length;
-    for (; ++i < a;) cn(s = t[i]) ? o = hf(e, s, n, o).length : s instanceof e ? o = xa(z, s.schema.fields.map((c, u) => s.getChildAt(u)), n, o).length : s instanceof z && (n[o++] = s);
+    for (; ++i < a;) ln(s = t[i]) ? o = pf(e, s, n, o).length : s instanceof e ? o = Ba(z, s.schema.fields.map((c, u) => s.getChildAt(u)), n, o).length : s instanceof z && (n[o++] = s);
     return n
 }
-const cb = (e, [t, n], r) => (e[0][r] = t, e[1][r] = n, e);
+const ub = (e, [t, n], r) => (e[0][r] = t, e[1][r] = n, e);
 
-function La(e, t) {
+function Oa(e, t) {
     let n, r;
     switch (r = e.length) {
         case 0:
             return t;
         case 1:
             if (n = t[0], !e[0]) return t;
-            if (cn(e[0])) return La(e[0], t);
-            e[0] instanceof S || e[0] instanceof z || e[0] instanceof U || ([n, e] = Object.entries(e[0]).reduce(cb, t));
+            if (ln(e[0])) return Oa(e[0], t);
+            e[0] instanceof S || e[0] instanceof z || e[0] instanceof U || ([n, e] = Object.entries(e[0]).reduce(ub, t));
             break;
         default:
-            cn(n = e[r - 1]) ? e = cn(e[0]) ? e[0] : e.slice(0, r - 1) : (e = cn(e[0]) ? e[0] : e, n = [])
+            ln(n = e[r - 1]) ? e = ln(e[0]) ? e[0] : e.slice(0, r - 1) : (e = ln(e[0]) ? e[0] : e, n = [])
     }
     let s = -1,
         o = -1,
         i = -1,
         a = e.length,
         c, u, [l, f] = t;
-    for (; ++i < a;) u = e[i], u instanceof Kt && (f[++o] = u) ? l[++s] = u.field.clone(n[i], u.type, !0) : ({
+    for (; ++i < a;) u = e[i], u instanceof Zt && (f[++o] = u) ? l[++s] = u.field.clone(n[i], u.type, !0) : ({
         [i]: c = i
     } = n, u instanceof U && (f[++o] = u) ? l[++s] = W.new(c, u, !0) : u && u.type && (f[++o] = u) && (u instanceof S && (f[o] = u = z.new(u)), l[++s] = W.new(c, u.type, !0)));
     return t
 }
 class H {
     constructor(t = [], n, r) {
         this.fields = t || [], this.metadata = n || new Map, r || (r = xo(t)), this.dictionaries = r
     }
     static from(...t) {
         return H.new(t[0], t[1])
     }
     static new(...t) {
-        return new H(ff(t)[0])
+        return new H(df(t)[0])
     }
     get[Symbol.toStringTag]() {
         return "Schema"
     }
     toString() {
         return `Schema<{ ${this.fields.map((t,n)=>`${n}: ${t}`).join(", ")} }>`
     }
     compareTo(t) {
-        return Nt.compareSchemas(this, t)
+        return Mt.compareSchemas(this, t)
     }
     select(...t) {
         const n = t.reduce((r, s) => (r[s] = !0) && r, Object.create(null));
         return new H(this.fields.filter(r => n[r.name]), this.metadata)
     }
     selectAt(...t) {
         return new H(t.map(n => this.fields[n]).filter(Boolean), this.metadata)
     }
     assign(...t) {
-        const n = t[0] instanceof H ? t[0] : new H(lf(W, t)),
+        const n = t[0] instanceof H ? t[0] : new H(hf(W, t)),
             r = [...this.fields],
             s = fi(fi(new Map, this.metadata), n.metadata),
             o = n.fields.filter(a => {
                 const c = r.findIndex(u => u.name === a.name);
                 return ~c ? (r[c] = a.clone({
                     metadata: fi(fi(new Map, r[c].metadata), a.metadata)
                 })) && !1 : !0
@@ -5947,15 +5947,15 @@
     get[Symbol.toStringTag]() {
         return "Field"
     }
     toString() {
         return `${this.name}: ${this.type}`
     }
     compareTo(t) {
-        return Nt.compareField(this, t)
+        return Mt.compareField(this, t)
     }
     clone(...t) {
         let [n, r, s, o] = t;
         return !t[0] || typeof t[0] != "object" ? [n = this.name, r = this.type, s = this.nullable, o = this.metadata] = t : {
             name: n = this.name,
             type: r = this.type,
             nullable: s = this.nullable,
@@ -5982,17 +5982,17 @@
 H.prototype.fields = null;
 H.prototype.metadata = null;
 H.prototype.dictionaries = null;
 W.prototype.type = null;
 W.prototype.name = null;
 W.prototype.nullable = null;
 W.prototype.metadata = null;
-class ub extends As {
+class lb extends As {
     constructor(t) {
-        super(t), this._run = new of, this._offsets = new ql
+        super(t), this._run = new cf, this._offsets = new tf
     }
     addChild(t, n = "0") {
         if (this.numChildren > 0) throw new Error("ListBuilder can only have one child.");
         return this.children[this.numChildren] = t, this.type = new er(new W(n, t.type, !0)), this.numChildren - 1
     }
     clear() {
         return this._run.clear(), super.clear()
@@ -6002,31 +6002,31 @@
             r = this._offsets,
             s = this._setValue;
         let o = 0,
             i;
         for ([o, i] of t) i === void 0 ? r.set(o, 0) : (r.set(o, i.length), s(this, o, n.bind(i)))
     }
 }
-class lb extends at {
+class fb extends at {
     constructor() {
-        super(...arguments), this._run = new of
+        super(...arguments), this._run = new cf
     }
     setValue(t, n) {
         super.setValue(t, this._run.bind(n))
     }
     addChild(t, n = "0") {
         if (this.numChildren > 0) throw new Error("FixedSizeListBuilder can only have one child.");
         const r = this.children.push(t);
         return this.type = new Er(this.type.listSize, new W(n, t.type, !0)), r
     }
     clear() {
         return this._run.clear(), super.clear()
     }
 }
-class fb extends As {
+class hb extends As {
     set(t, n) {
         return super.set(t, n)
     }
     setValue(t, n) {
         n = n instanceof Map ? n : new Map(Object.entries(n));
         const r = this._pending || (this._pending = new Map),
             s = r.get(t);
@@ -6040,21 +6040,21 @@
         const n = this._offsets,
             r = this._setValue;
         t.forEach((s, o) => {
             s === void 0 ? n.set(o, 0) : (n.set(o, s.size), r(this, o, s))
         })
     }
 }
-class hb extends at {
+class db extends at {
     addChild(t, n = `${this.numChildren}`) {
         const r = this.children.push(t);
-        return this.type = new Qt([...this.type.children, new W(n, t.type, !0)]), r
+        return this.type = new te([...this.type.children, new W(n, t.type, !0)]), r
     }
 }
-class Da extends at {
+class Fa extends at {
     constructor(t) {
         super(t), this._typeIds = new Xr(new Int8Array(0), 1), typeof t.valueToChildTypeId == "function" && (this._valueToChildTypeId = t.valueToChildTypeId)
     }
     get typeIdToChildIndex() {
         return this.type.typeIdToChildIndex
     }
     append(t, n) {
@@ -6078,73 +6078,73 @@
             a = [...s, new W(n, t.type)];
         return this.type = new kr(o, [...i, r], a), r
     }
     _valueToChildTypeId(t, n, r) {
         throw new Error("Cannot map UnionBuilder value to child typeId. Pass the `childTypeId` as the second argument to unionBuilder.append(), or supply a `valueToChildTypeId` function as part of the UnionBuilder constructor options.")
     }
 }
-class db extends Da {}
-class pb extends Da {
+class pb extends Fa {}
+class yb extends Fa {
     constructor(t) {
         super(t), this._offsets = new Xr(new Int32Array(0))
     }
     setValue(t, n, r) {
         const s = this.type.typeIdToChildIndex[r];
         return this._offsets.set(t, this.getChildAt(s).length), super.setValue(t, n, r)
     }
 }
 class D extends V {}
-const yb = (e, t, n) => {
+const bb = (e, t, n) => {
         e[t] = n / 864e5 | 0
     },
-    ka = (e, t, n) => {
+    xa = (e, t, n) => {
         e[t] = n % 4294967296 | 0, e[t + 1] = n / 4294967296 | 0
     },
-    bb = (e, t, n) => {
+    mb = (e, t, n) => {
         e[t] = n * 1e3 % 4294967296 | 0, e[t + 1] = n * 1e3 / 4294967296 | 0
     },
-    mb = (e, t, n) => {
+    gb = (e, t, n) => {
         e[t] = n * 1e6 % 4294967296 | 0, e[t + 1] = n * 1e6 / 4294967296 | 0
     },
-    df = (e, t, n, r) => {
+    yf = (e, t, n, r) => {
         const {
             [n]: s, [n + 1]: o
         } = t;
         s != null && o != null && e.set(r.subarray(0, o - s), s)
     },
-    gb = ({
+    vb = ({
         offset: e,
         values: t
     }, n, r) => {
         const s = e + n;
         r ? t[s >> 3] |= 1 << s % 8 : t[s >> 3] &= ~(1 << s % 8)
     },
-    pf = ({
+    bf = ({
         values: e
     }, t, n) => {
-        yb(e, t, n.valueOf())
+        bb(e, t, n.valueOf())
     },
-    yf = ({
+    mf = ({
         values: e
     }, t, n) => {
-        ka(e, t * 2, n.valueOf())
+        xa(e, t * 2, n.valueOf())
     },
     pe = ({
         stride: e,
         values: t
     }, n, r) => {
         t[e * n] = r
     },
-    bf = ({
+    gf = ({
         stride: e,
         values: t
     }, n, r) => {
-        t[e * n] = Aa(r)
+        t[e * n] = Sa(r)
     },
-    Ea = (e, t, n) => {
+    La = (e, t, n) => {
         switch (typeof n) {
             case "bigint":
                 e.values64[t] = n;
                 break;
             case "number":
                 e.values[t * e.stride] = n;
                 break;
@@ -6154,363 +6154,363 @@
                         stride: s,
                         ArrayType: o
                     } = e,
                     i = R(o, r);
                 e.values.set(i.subarray(0, s), s * t)
         }
     },
-    vb = ({
+    wb = ({
         stride: e,
         values: t
     }, n, r) => {
         t.set(r.subarray(0, e), e * n)
     },
-    wb = ({
+    _b = ({
         values: e,
         valueOffsets: t
-    }, n, r) => df(e, t, n, r),
-    _b = ({
+    }, n, r) => yf(e, t, n, r),
+    Sb = ({
         values: e,
         valueOffsets: t
     }, n, r) => {
-        df(e, t, n, vs(r))
-    },
-    Sb = (e, t, n) => {
-        e.type.bitWidth < 64 ? pe(e, t, n) : Ea(e, t, n)
+        yf(e, t, n, vs(r))
     },
     Ib = (e, t, n) => {
-        e.type.precision !== Pt.HALF ? pe(e, t, n) : bf(e, t, n)
+        e.type.bitWidth < 64 ? pe(e, t, n) : La(e, t, n)
     },
     Tb = (e, t, n) => {
-        e.type.unit === le.DAY ? pf(e, t, n) : yf(e, t, n)
+        e.type.precision !== zt.HALF ? pe(e, t, n) : gf(e, t, n)
+    },
+    Ab = (e, t, n) => {
+        e.type.unit === le.DAY ? bf(e, t, n) : mf(e, t, n)
     },
-    mf = ({
-        values: e
-    }, t, n) => ka(e, t * 2, n / 1e3),
-    gf = ({
-        values: e
-    }, t, n) => ka(e, t * 2, n),
     vf = ({
         values: e
-    }, t, n) => bb(e, t * 2, n),
+    }, t, n) => xa(e, t * 2, n / 1e3),
     wf = ({
         values: e
+    }, t, n) => xa(e, t * 2, n),
+    _f = ({
+        values: e
     }, t, n) => mb(e, t * 2, n),
-    Ab = (e, t, n) => {
+    Sf = ({
+        values: e
+    }, t, n) => gb(e, t * 2, n),
+    Bb = (e, t, n) => {
         switch (e.type.unit) {
             case Z.SECOND:
-                return mf(e, t, n);
+                return vf(e, t, n);
             case Z.MILLISECOND:
-                return gf(e, t, n);
+                return wf(e, t, n);
             case Z.MICROSECOND:
-                return vf(e, t, n);
+                return _f(e, t, n);
             case Z.NANOSECOND:
-                return wf(e, t, n)
+                return Sf(e, t, n)
         }
     },
-    _f = ({
+    If = ({
         values: e,
         stride: t
     }, n, r) => {
         e[t * n] = r
     },
-    Sf = ({
+    Tf = ({
         values: e,
         stride: t
     }, n, r) => {
         e[t * n] = r
     },
-    If = ({
+    Af = ({
         values: e
     }, t, n) => {
         e.set(n.subarray(0, 2), 2 * t)
     },
-    Tf = ({
+    Bf = ({
         values: e
     }, t, n) => {
         e.set(n.subarray(0, 2), 2 * t)
     },
-    Bb = (e, t, n) => {
+    Ob = (e, t, n) => {
         switch (e.type.unit) {
             case Z.SECOND:
-                return _f(e, t, n);
+                return If(e, t, n);
             case Z.MILLISECOND:
-                return Sf(e, t, n);
+                return Tf(e, t, n);
             case Z.MICROSECOND:
-                return If(e, t, n);
+                return Af(e, t, n);
             case Z.NANOSECOND:
-                return Tf(e, t, n)
+                return Bf(e, t, n)
         }
     },
-    Ob = ({
+    Fb = ({
         values: e
     }, t, n) => {
         e.set(n.subarray(0, 4), 4 * t)
     },
-    Fb = (e, t, n) => {
+    xb = (e, t, n) => {
         const r = e.getChildAt(0),
             s = e.valueOffsets;
         for (let o = -1, i = s[t], a = s[t + 1]; i < a;) r.set(i++, n.get(++o))
     },
-    xb = (e, t, n) => {
+    Lb = (e, t, n) => {
         const r = e.getChildAt(0),
             s = e.valueOffsets,
             o = n instanceof Map ? [...n] : Object.entries(n);
         for (let i = -1, a = s[t], c = s[t + 1]; a < c;) r.set(a++, o[++i])
     },
-    Lb = (e, t) => (n, r, s) => n && n.set(e, t[s]),
-    Db = (e, t) => (n, r, s) => n && n.set(e, t.get(s)),
-    kb = (e, t) => (n, r, s) => n && n.set(e, t.get(r.name)),
-    Eb = (e, t) => (n, r, s) => n && n.set(e, t[r.name]),
-    Ub = (e, t, n) => {
-        const r = n instanceof Map ? kb(t, n) : n instanceof z ? Db(t, n) : Array.isArray(n) ? Lb(t, n) : Eb(t, n);
+    Db = (e, t) => (n, r, s) => n && n.set(e, t[s]),
+    kb = (e, t) => (n, r, s) => n && n.set(e, t.get(s)),
+    Eb = (e, t) => (n, r, s) => n && n.set(e, t.get(r.name)),
+    Ub = (e, t) => (n, r, s) => n && n.set(e, t[r.name]),
+    Nb = (e, t, n) => {
+        const r = n instanceof Map ? Eb(t, n) : n instanceof z ? kb(t, n) : Array.isArray(n) ? Db(t, n) : Ub(t, n);
         e.type.children.forEach((s, o) => r(e.getChildAt(o), s, o))
     },
-    Nb = (e, t, n) => {
-        e.type.mode === Be.Dense ? Af(e, t, n) : Bf(e, t, n)
+    Mb = (e, t, n) => {
+        e.type.mode === Be.Dense ? Of(e, t, n) : Ff(e, t, n)
     },
-    Af = (e, t, n) => {
+    Of = (e, t, n) => {
         const r = e.typeIdToChildIndex[e.typeIds[t]],
             s = e.getChildAt(r);
         s && s.set(e.valueOffsets[t], n)
     },
-    Bf = (e, t, n) => {
+    Ff = (e, t, n) => {
         const r = e.typeIdToChildIndex[e.typeIds[t]],
             s = e.getChildAt(r);
         s && s.set(t, n)
     },
-    Mb = (e, t, n) => {
+    Cb = (e, t, n) => {
         const r = e.getKey(t);
         r !== null && e.setValue(r, n)
     },
-    Cb = (e, t, n) => {
-        e.type.unit === Hn.DAY_TIME ? Of(e, t, n) : Ff(e, t, n)
+    Rb = (e, t, n) => {
+        e.type.unit === Hn.DAY_TIME ? xf(e, t, n) : Lf(e, t, n)
     },
-    Of = ({
+    xf = ({
         values: e
     }, t, n) => {
         e.set(n.subarray(0, 2), 2 * t)
     },
-    Ff = ({
+    Lf = ({
         values: e
     }, t, n) => {
         e[t] = n[0] * 12 + n[1] % 12
     },
-    Rb = (e, t, n) => {
+    Vb = (e, t, n) => {
         const r = e.getChildAt(0),
             {
                 stride: s
             } = e;
         for (let o = -1, i = t * s; ++o < s;) r.set(i + o, n.get(o))
     };
-D.prototype.visitBool = gb;
-D.prototype.visitInt = Sb;
+D.prototype.visitBool = vb;
+D.prototype.visitInt = Ib;
 D.prototype.visitInt8 = pe;
 D.prototype.visitInt16 = pe;
 D.prototype.visitInt32 = pe;
-D.prototype.visitInt64 = Ea;
+D.prototype.visitInt64 = La;
 D.prototype.visitUint8 = pe;
 D.prototype.visitUint16 = pe;
 D.prototype.visitUint32 = pe;
-D.prototype.visitUint64 = Ea;
-D.prototype.visitFloat = Ib;
-D.prototype.visitFloat16 = bf;
+D.prototype.visitUint64 = La;
+D.prototype.visitFloat = Tb;
+D.prototype.visitFloat16 = gf;
 D.prototype.visitFloat32 = pe;
 D.prototype.visitFloat64 = pe;
-D.prototype.visitUtf8 = _b;
-D.prototype.visitBinary = wb;
-D.prototype.visitFixedSizeBinary = vb;
-D.prototype.visitDate = Tb;
-D.prototype.visitDateDay = pf;
-D.prototype.visitDateMillisecond = yf;
-D.prototype.visitTimestamp = Ab;
-D.prototype.visitTimestampSecond = mf;
-D.prototype.visitTimestampMillisecond = gf;
-D.prototype.visitTimestampMicrosecond = vf;
-D.prototype.visitTimestampNanosecond = wf;
-D.prototype.visitTime = Bb;
-D.prototype.visitTimeSecond = _f;
-D.prototype.visitTimeMillisecond = Sf;
-D.prototype.visitTimeMicrosecond = If;
-D.prototype.visitTimeNanosecond = Tf;
-D.prototype.visitDecimal = Ob;
-D.prototype.visitList = Fb;
-D.prototype.visitStruct = Ub;
-D.prototype.visitUnion = Nb;
-D.prototype.visitDenseUnion = Af;
-D.prototype.visitSparseUnion = Bf;
-D.prototype.visitDictionary = Mb;
-D.prototype.visitInterval = Cb;
-D.prototype.visitIntervalDayTime = Of;
-D.prototype.visitIntervalYearMonth = Ff;
-D.prototype.visitFixedSizeList = Rb;
-D.prototype.visitMap = xb;
+D.prototype.visitUtf8 = Sb;
+D.prototype.visitBinary = _b;
+D.prototype.visitFixedSizeBinary = wb;
+D.prototype.visitDate = Ab;
+D.prototype.visitDateDay = bf;
+D.prototype.visitDateMillisecond = mf;
+D.prototype.visitTimestamp = Bb;
+D.prototype.visitTimestampSecond = vf;
+D.prototype.visitTimestampMillisecond = wf;
+D.prototype.visitTimestampMicrosecond = _f;
+D.prototype.visitTimestampNanosecond = Sf;
+D.prototype.visitTime = Ob;
+D.prototype.visitTimeSecond = If;
+D.prototype.visitTimeMillisecond = Tf;
+D.prototype.visitTimeMicrosecond = Af;
+D.prototype.visitTimeNanosecond = Bf;
+D.prototype.visitDecimal = Fb;
+D.prototype.visitList = xb;
+D.prototype.visitStruct = Nb;
+D.prototype.visitUnion = Mb;
+D.prototype.visitDenseUnion = Of;
+D.prototype.visitSparseUnion = Ff;
+D.prototype.visitDictionary = Cb;
+D.prototype.visitInterval = Rb;
+D.prototype.visitIntervalDayTime = xf;
+D.prototype.visitIntervalYearMonth = Lf;
+D.prototype.visitFixedSizeList = Vb;
+D.prototype.visitMap = Lb;
 const Fs = new D;
-class Vb extends V {
+class jb extends V {
     visitNull() {
-        return my
+        return gy
     }
     visitBool() {
-        return by
+        return my
     }
     visitInt() {
         return Ee
     }
     visitInt8() {
-        return Fy
+        return xy
     }
     visitInt16() {
-        return xy
+        return Ly
     }
     visitInt32() {
-        return Ly
+        return Dy
     }
     visitInt64() {
-        return Dy
+        return ky
     }
     visitUint8() {
-        return ky
+        return Ey
     }
     visitUint16() {
-        return Ey
+        return Uy
     }
     visitUint32() {
-        return Uy
+        return Ny
     }
     visitUint64() {
-        return Ny
+        return My
     }
     visitFloat() {
         return Bs
     }
     visitFloat16() {
-        return Ty
+        return Ay
     }
     visitFloat32() {
-        return Ay
+        return By
     }
     visitFloat64() {
-        return By
+        return Oy
     }
     visitUtf8() {
-        return Oa
+        return Ta
     }
     visitBinary() {
-        return sf
+        return af
     }
     visitFixedSizeBinary() {
-        return Sy
+        return Iy
     }
     visitDate() {
-        return Ta
+        return _a
     }
     visitDateDay() {
-        return gy
+        return vy
     }
     visitDateMillisecond() {
-        return vy
+        return wy
     }
     visitTimestamp() {
         return Qr
     }
     visitTimestampSecond() {
-        return jy
+        return Py
     }
     visitTimestampMillisecond() {
-        return Py
+        return zy
     }
     visitTimestampMicrosecond() {
-        return zy
+        return Wy
     }
     visitTimestampNanosecond() {
-        return Wy
+        return $y
     }
     visitTime() {
         return qr
     }
     visitTimeSecond() {
-        return My
+        return Cy
     }
     visitTimeMillisecond() {
-        return Cy
+        return Ry
     }
     visitTimeMicrosecond() {
-        return Ry
+        return Vy
     }
     visitTimeNanosecond() {
-        return Vy
+        return jy
     }
     visitDecimal() {
-        return wy
+        return _y
     }
     visitList() {
-        return ub
+        return lb
     }
     visitStruct() {
-        return hb
+        return db
     }
     visitUnion() {
-        return Da
+        return Fa
     }
     visitDenseUnion() {
-        return pb
+        return yb
     }
     visitSparseUnion() {
-        return db
+        return pb
     }
     visitDictionary() {
-        return _y
+        return Sy
     }
     visitInterval() {
-        return Ba
+        return Ia
     }
     visitIntervalDayTime() {
-        return $y
+        return Yy
     }
     visitIntervalYearMonth() {
-        return Yy
+        return Gy
     }
     visitFixedSizeList() {
-        return lb
+        return fb
     }
     visitMap() {
-        return fb
+        return hb
     }
 }
-const xf = new Vb;
-at.new = Lf;
+const Df = new jb;
+at.new = kf;
 
-function Lf(e) {
+function kf(e) {
     const t = e.type,
-        n = new(xf.getVisitFn(t)())(e);
+        n = new(Df.getVisitFn(t)())(e);
     if (t.children && t.children.length > 0) {
         const r = e.children || [],
             s = {
                 nullValues: e.nullValues
             },
             o = Array.isArray(r) ? (i, a) => r[a] || s : ({
                 name: i
             }) => r[i] || s;
         t.children.forEach((i, a) => {
             const {
                 type: c
             } = i, u = o(i, a);
-            n.children.push(Lf({
+            n.children.push(kf({
                 ...u,
                 type: c
             }))
         })
     }
     return n
 }
 Object.keys(d).map(e => d[e]).filter(e => typeof e == "number" && e !== d.NONE).forEach(e => {
-    const t = xf.visit(e);
+    const t = Df.visit(e);
     t.prototype._setValue = Fs.getVisitFn(e)
 });
-Oa.prototype._setValue = Fs.visitBinary;
+Ta.prototype._setValue = Fs.visitBinary;
 var nr;
 (function(e) {
     (function(t) {
         (function(n) {
             (function(r) {
                 class s {
                     constructor() {
@@ -6607,37 +6607,37 @@
                     }
                 }
                 r.Block = s
             })(n.flatbuf || (n.flatbuf = {}))
         })(t.arrow || (t.arrow = {}))
     })(e.apache || (e.apache = {}))
 })(nr || (nr = {}));
-var Wc = y.Long,
-    jb = y.Builder,
-    Pb = y.ByteBuffer,
-    zb = nr.apache.arrow.flatbuf.Block,
-    se = nr.apache.arrow.flatbuf.Footer;
+var Yc = y.Long,
+    Pb = y.Builder,
+    zb = y.ByteBuffer,
+    Wb = nr.apache.arrow.flatbuf.Block,
+    oe = nr.apache.arrow.flatbuf.Footer;
 class Cr {
-    constructor(t, n = Gt.V4, r, s) {
+    constructor(t, n = Kt.V4, r, s) {
         this.schema = t, this.version = n, r && (this._recordBatches = r), s && (this._dictionaryBatches = s)
     }
     static decode(t) {
-        t = new Pb(j(t));
-        const n = se.getRootAsFooter(t),
+        t = new zb(j(t));
+        const n = oe.getRootAsFooter(t),
             r = H.decode(n.schema());
-        return new Wb(r, n)
+        return new $b(r, n)
     }
     static encode(t) {
-        const n = new jb,
+        const n = new Pb,
             r = H.encode(n, t.schema);
-        se.startRecordBatchesVector(n, t.numRecordBatches), [...t.recordBatches()].slice().reverse().forEach(i => Ze.encode(n, i));
+        oe.startRecordBatchesVector(n, t.numRecordBatches), [...t.recordBatches()].slice().reverse().forEach(i => He.encode(n, i));
         const s = n.endVector();
-        se.startDictionariesVector(n, t.numDictionaries), [...t.dictionaryBatches()].slice().reverse().forEach(i => Ze.encode(n, i));
+        oe.startDictionariesVector(n, t.numDictionaries), [...t.dictionaryBatches()].slice().reverse().forEach(i => He.encode(n, i));
         const o = n.endVector();
-        return se.startFooter(n), se.addSchema(n, r), se.addVersion(n, Gt.V4), se.addRecordBatches(n, s), se.addDictionaries(n, o), se.finishFooterBuffer(n, se.endFooter(n)), n.asUint8Array()
+        return oe.startFooter(n), oe.addSchema(n, r), oe.addVersion(n, Kt.V4), oe.addRecordBatches(n, s), oe.addDictionaries(n, o), oe.finishFooterBuffer(n, oe.endFooter(n)), n.asUint8Array()
     }
     get numRecordBatches() {
         return this._recordBatches.length
     }
     get numDictionaries() {
         return this._dictionaryBatches.length
     }* recordBatches() {
@@ -6648,72 +6648,72 @@
     getRecordBatch(t) {
         return t >= 0 && t < this.numRecordBatches && this._recordBatches[t] || null
     }
     getDictionaryBatch(t) {
         return t >= 0 && t < this.numDictionaries && this._dictionaryBatches[t] || null
     }
 }
-class Wb extends Cr {
+class $b extends Cr {
     constructor(t, n) {
         super(t, n.version()), this._footer = n
     }
     get numRecordBatches() {
         return this._footer.recordBatchesLength()
     }
     get numDictionaries() {
         return this._footer.dictionariesLength()
     }
     getRecordBatch(t) {
         if (t >= 0 && t < this.numRecordBatches) {
             const n = this._footer.recordBatches(t);
-            if (n) return Ze.decode(n)
+            if (n) return He.decode(n)
         }
         return null
     }
     getDictionaryBatch(t) {
         if (t >= 0 && t < this.numDictionaries) {
             const n = this._footer.dictionaries(t);
-            if (n) return Ze.decode(n)
+            if (n) return He.decode(n)
         }
         return null
     }
 }
-class Ze {
+class He {
     static decode(t) {
-        return new Ze(t.metaDataLength(), t.bodyLength(), t.offset())
+        return new He(t.metaDataLength(), t.bodyLength(), t.offset())
     }
     static encode(t, n) {
         const {
             metaDataLength: r
-        } = n, s = new Wc(n.offset, 0), o = new Wc(n.bodyLength, 0);
-        return zb.createBlock(t, s, r, o)
+        } = n, s = new Yc(n.offset, 0), o = new Yc(n.bodyLength, 0);
+        return Wb.createBlock(t, s, r, o)
     }
     constructor(t, n, r) {
         this.metaDataLength = t, this.offset = typeof r == "number" ? r : r.low, this.bodyLength = typeof n == "number" ? n : n.low
     }
 }
-class Tr extends mp {
+class Tr extends gp {
     write(t) {
         if ((t = j(t)).byteLength > 0) return super.write(t)
     }
     toString(t = !1) {
         return t ? To(this.toUint8Array(!0)) : this.toUint8Array(!1).then(To)
     }
     toUint8Array(t = !1) {
-        return t ? qt(this._values)[0] : (async () => {
+        return t ? Qt(this._values)[0] : (async () => {
             let n = [],
                 r = 0;
             for await (const s of this) n.push(s), r += s.byteLength;
-            return qt(n, r)[0]
+            return Qt(n, r)[0]
         })()
     }
 }
 class Ki {
     constructor(t) {
-        t && (this.source = new $b(Ut.fromIterable(t)))
+        t && (this.source = new Yb(Ut.fromIterable(t)))
     } [Symbol.iterator]() {
         return this
     }
     next(t) {
         return this.source.next(t)
     }
     throw (t) {
@@ -6725,17 +6725,17 @@
     peek(t) {
         return this.source.peek(t)
     }
     read(t) {
         return this.source.read(t)
     }
 }
-class pn {
+class bn {
     constructor(t) {
-        t instanceof pn ? this.source = t.source : t instanceof Tr ? this.source = new nn(Ut.fromAsyncIterable(t)) : jl(t) ? this.source = new nn(Ut.fromNodeStream(t)) : fa(t) ? this.source = new nn(Ut.fromDOMStream(t)) : Vl(t) ? this.source = new nn(Ut.fromDOMStream(t.body)) : Xt(t) ? this.source = new nn(Ut.fromIterable(t)) : Ge(t) ? this.source = new nn(Ut.fromAsyncIterable(t)) : De(t) && (this.source = new nn(Ut.fromAsyncIterable(t)))
+        t instanceof bn ? this.source = t.source : t instanceof Tr ? this.source = new sn(Ut.fromAsyncIterable(t)) : zl(t) ? this.source = new sn(Ut.fromNodeStream(t)) : ca(t) ? this.source = new sn(Ut.fromDOMStream(t)) : Pl(t) ? this.source = new sn(Ut.fromDOMStream(t.body)) : qt(t) ? this.source = new sn(Ut.fromIterable(t)) : Ke(t) ? this.source = new sn(Ut.fromAsyncIterable(t)) : De(t) && (this.source = new sn(Ut.fromAsyncIterable(t)))
     } [Symbol.asyncIterator]() {
         return this
     }
     next(t) {
         return this.source.next(t)
     }
     throw (t) {
@@ -6753,15 +6753,15 @@
     peek(t) {
         return this.source.peek(t)
     }
     read(t) {
         return this.source.read(t)
     }
 }
-class $b {
+class Yb {
     constructor(t) {
         this.source = t
     }
     cancel(t) {
         this.return(t)
     }
     peek(t) {
@@ -6779,15 +6779,15 @@
     throw (t) {
         return Object.create(this.source.throw && this.source.throw(t) || ot)
     }
     return (t) {
         return Object.create(this.source.return && this.source.return(t) || ot)
     }
 }
-class nn {
+class sn {
     constructor(t) {
         this.source = t, this._closedPromise = new Promise(n => this._closedPromiseResolve = n)
     }
     async cancel(t) {
         await this.return(t)
     }
     get closed() {
@@ -6810,15 +6810,15 @@
         return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(n)
     }
     async return (t) {
         const n = this.source.return && await this.source.return(t) || ot;
         return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(n)
     }
 }
-class $c extends Ki {
+class Gc extends Ki {
     constructor(t, n) {
         super(), this.position = 0, this.buffer = j(t), this.size = typeof n > "u" ? this.buffer.byteLength : n
     }
     readInt32(t) {
         const {
             buffer: n,
             byteOffset: r
@@ -6853,15 +6853,15 @@
     return (t) {
         return this.close(), {
             done: !0,
             value: t
         }
     }
 }
-class Zi extends pn {
+class Zi extends bn {
     constructor(t, n) {
         super(), this.position = 0, this._handle = t, typeof n == "number" ? this.size = n : this._pending = (async () => {
             this.size = (await t.stat()).size, delete this._pending
         })()
     }
     async readInt32(t) {
         const {
@@ -6921,22 +6921,22 @@
     async return (t) {
         return await this.close(), {
             done: !0,
             value: t
         }
     }
 }
-const Yb = 1 << 16;
+const Gb = 1 << 16;
 
-function Rn(e) {
+function Cn(e) {
     return e < 0 && (e = 4294967295 + e + 1), `0x${e.toString(16)}`
 }
 const rr = 8,
-    Ua = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
-class Na {
+    Da = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8];
+class ka {
     constructor(t) {
         this.buffer = t
     }
     high() {
         return this.buffer[1]
     }
     low() {
@@ -6944,15 +6944,15 @@
     }
     _times(t) {
         const n = new Uint32Array([this.buffer[1] >>> 16, this.buffer[1] & 65535, this.buffer[0] >>> 16, this.buffer[0] & 65535]),
             r = new Uint32Array([t.buffer[1] >>> 16, t.buffer[1] & 65535, t.buffer[0] >>> 16, t.buffer[0] & 65535]);
         let s = n[3] * r[3];
         this.buffer[0] = s & 65535;
         let o = s >>> 16;
-        return s = n[2] * r[3], o += s, s = n[3] * r[2] >>> 0, o += s, this.buffer[0] += o << 16, this.buffer[1] = o >>> 0 < s ? Yb : 0, this.buffer[1] += o >>> 16, this.buffer[1] += n[1] * r[3] + n[2] * r[2] + n[3] * r[1], this.buffer[1] += n[0] * r[3] + n[1] * r[2] + n[2] * r[1] + n[3] * r[0] << 16, this
+        return s = n[2] * r[3], o += s, s = n[3] * r[2] >>> 0, o += s, this.buffer[0] += o << 16, this.buffer[1] = o >>> 0 < s ? Gb : 0, this.buffer[1] += o >>> 16, this.buffer[1] += n[1] * r[3] + n[2] * r[2] + n[3] * r[1], this.buffer[1] += n[0] * r[3] + n[1] * r[2] + n[2] * r[1] + n[3] * r[0] << 16, this
     }
     _plus(t) {
         const n = this.buffer[0] + t.buffer[0] >>> 0;
         this.buffer[1] += t.buffer[1], n < this.buffer[0] >>> 0 && ++this.buffer[1], this.buffer[0] = n
     }
     lessThan(t) {
         return this.buffer[1] < t.buffer[1] || this.buffer[1] === t.buffer[1] && this.buffer[0] < t.buffer[0]
@@ -6960,18 +6960,18 @@
     equals(t) {
         return this.buffer[1] === t.buffer[1] && this.buffer[0] == t.buffer[0]
     }
     greaterThan(t) {
         return t.lessThan(this)
     }
     hex() {
-        return `${Rn(this.buffer[1])} ${Rn(this.buffer[0])}`
+        return `${Cn(this.buffer[1])} ${Cn(this.buffer[0])}`
     }
 }
-class K extends Na {
+class K extends ka {
     times(t) {
         return this._times(t), this
     }
     plus(t) {
         return this._plus(t), this
     }
     static from(t, n = new Uint32Array(2)) {
@@ -6982,15 +6982,15 @@
     }
     static fromString(t, n = new Uint32Array(2)) {
         const r = t.length;
         let s = new K(n);
         for (let o = 0; o < r;) {
             const i = rr < r - o ? rr : r - o,
                 a = new K(new Uint32Array([parseInt(t.substr(o, i), 10), 0])),
-                c = new K(new Uint32Array([Ua[i], 0]));
+                c = new K(new Uint32Array([Da[i], 0]));
             s.times(c), s.plus(a), o += i
         }
         return s
     }
     static convertArray(t) {
         const n = new Uint32Array(t.length * 2);
         for (let r = -1, s = t.length; ++r < s;) K.from(t[r], new Uint32Array(n.buffer, n.byteOffset + 2 * r * 4, 2));
@@ -6999,15 +6999,15 @@
     static multiply(t, n) {
         return new K(new Uint32Array(t.buffer)).times(n)
     }
     static add(t, n) {
         return new K(new Uint32Array(t.buffer)).plus(n)
     }
 }
-class wt extends Na {
+class wt extends ka {
     negate() {
         return this.buffer[0] = ~this.buffer[0] + 1, this.buffer[1] = ~this.buffer[1], this.buffer[0] == 0 && ++this.buffer[1], this
     }
     times(t) {
         return this._times(t), this
     }
     plus(t) {
@@ -7027,15 +7027,15 @@
     static fromString(t, n = new Uint32Array(2)) {
         const r = t.startsWith("-"),
             s = t.length;
         let o = new wt(n);
         for (let i = r ? 1 : 0; i < s;) {
             const a = rr < s - i ? rr : s - i,
                 c = new wt(new Uint32Array([parseInt(t.substr(i, a), 10), 0])),
-                u = new wt(new Uint32Array([Ua[a], 0]));
+                u = new wt(new Uint32Array([Da[a], 0]));
             o.times(u), o.plus(c), i += a
         }
         return r ? o.negate() : o
     }
     static convertArray(t) {
         const n = new Uint32Array(t.length * 2);
         for (let r = -1, s = t.length; ++r < s;) wt.from(t[r], new Uint32Array(n.buffer, n.byteOffset + 2 * r * 4, 2));
@@ -7044,15 +7044,15 @@
     static multiply(t, n) {
         return new wt(new Uint32Array(t.buffer)).times(n)
     }
     static add(t, n) {
         return new wt(new Uint32Array(t.buffer)).plus(n)
     }
 }
-class Yt {
+class Gt {
     constructor(t) {
         this.buffer = t
     }
     high() {
         return new wt(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
     }
     low() {
@@ -7076,56 +7076,56 @@
         return l = K.multiply(s, u), f.plus(l), l = K.multiply(o, c), f.plus(l), this.buffer[1] = f.low(), this.buffer[3] = f.lessThan(l) ? 1 : 0, this.buffer[2] = f.high(), new K(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(K.multiply(r, u)).plus(K.multiply(s, c)).plus(K.multiply(o, a)), this.buffer[3] += K.multiply(n, u).plus(K.multiply(r, c)).plus(K.multiply(s, a)).plus(K.multiply(o, i)).low(), this
     }
     plus(t) {
         let n = new Uint32Array(4);
         return n[3] = this.buffer[3] + t.buffer[3] >>> 0, n[2] = this.buffer[2] + t.buffer[2] >>> 0, n[1] = this.buffer[1] + t.buffer[1] >>> 0, n[0] = this.buffer[0] + t.buffer[0] >>> 0, n[0] < this.buffer[0] >>> 0 && ++n[1], n[1] < this.buffer[1] >>> 0 && ++n[2], n[2] < this.buffer[2] >>> 0 && ++n[3], this.buffer[3] = n[3], this.buffer[2] = n[2], this.buffer[1] = n[1], this.buffer[0] = n[0], this
     }
     hex() {
-        return `${Rn(this.buffer[3])} ${Rn(this.buffer[2])} ${Rn(this.buffer[1])} ${Rn(this.buffer[0])}`
+        return `${Cn(this.buffer[3])} ${Cn(this.buffer[2])} ${Cn(this.buffer[1])} ${Cn(this.buffer[0])}`
     }
     static multiply(t, n) {
-        return new Yt(new Uint32Array(t.buffer)).times(n)
+        return new Gt(new Uint32Array(t.buffer)).times(n)
     }
     static add(t, n) {
-        return new Yt(new Uint32Array(t.buffer)).plus(n)
+        return new Gt(new Uint32Array(t.buffer)).plus(n)
     }
     static from(t, n = new Uint32Array(4)) {
-        return Yt.fromString(typeof t == "string" ? t : t.toString(), n)
+        return Gt.fromString(typeof t == "string" ? t : t.toString(), n)
     }
     static fromNumber(t, n = new Uint32Array(4)) {
-        return Yt.fromString(t.toString(), n)
+        return Gt.fromString(t.toString(), n)
     }
     static fromString(t, n = new Uint32Array(4)) {
         const r = t.startsWith("-"),
             s = t.length;
-        let o = new Yt(n);
+        let o = new Gt(n);
         for (let i = r ? 1 : 0; i < s;) {
             const a = rr < s - i ? rr : s - i,
-                c = new Yt(new Uint32Array([parseInt(t.substr(i, a), 10), 0, 0, 0])),
-                u = new Yt(new Uint32Array([Ua[a], 0, 0, 0]));
+                c = new Gt(new Uint32Array([parseInt(t.substr(i, a), 10), 0, 0, 0])),
+                u = new Gt(new Uint32Array([Da[a], 0, 0, 0]));
             o.times(u), o.plus(c), i += a
         }
         return r ? o.negate() : o
     }
     static convertArray(t) {
         const n = new Uint32Array(t.length * 4);
-        for (let r = -1, s = t.length; ++r < s;) Yt.from(t[r], new Uint32Array(n.buffer, n.byteOffset + 4 * 4 * r, 4));
+        for (let r = -1, s = t.length; ++r < s;) Gt.from(t[r], new Uint32Array(n.buffer, n.byteOffset + 4 * 4 * r, 4));
         return n
     }
 }
-const Gb = Object.freeze(Object.defineProperty({
+const Kb = Object.freeze(Object.defineProperty({
     __proto__: null,
-    BaseInt64: Na,
+    BaseInt64: ka,
     Uint64: K,
     Int64: wt,
-    Int128: Yt
+    Int128: Gt
 }, Symbol.toStringTag, {
     value: "Module"
 }));
-class Df extends V {
+class Ef extends V {
     constructor(t, n, r, s) {
         super(), this.nodesIndex = -1, this.buffersIndex = -1, this.bytes = t, this.nodes = n, this.buffers = r, this.dictionaries = s
     }
     visit(t) {
         return super.visit(t instanceof W ? t.type : t)
     }
     visitNull(t, {
@@ -7265,15 +7265,15 @@
     } = this.nextBufferRange()) {
         return this.bytes.subarray(r, r + n)
     }
     readDictionary(t) {
         return this.dictionaries.get(t.id)
     }
 }
-class Kb extends Df {
+class Zb extends Ef {
     constructor(t, n, r, s) {
         super(new Uint8Array(0), n, r, s), this.sources = t
     }
     readNullBitmap(t, n, {
         offset: r
     } = this.nextBufferRange()) {
         return n <= 0 ? new Uint8Array(0) : xr(this.sources[r])
@@ -7290,64 +7290,64 @@
     }
     readData(t, {
         offset: n
     } = this.nextBufferRange()) {
         const {
             sources: r
         } = this;
-        return U.isTimestamp(t) || (U.isInt(t) || U.isTime(t)) && t.bitWidth === 64 || U.isDate(t) && t.unit === le.MILLISECOND ? R(Uint8Array, wt.convertArray(r[n])) : U.isDecimal(t) ? R(Uint8Array, Yt.convertArray(r[n])) : U.isBinary(t) || U.isFixedSizeBinary(t) ? Zb(r[n]) : U.isBool(t) ? xr(r[n]) : U.isUtf8(t) ? vs(r[n].join("")) : R(Uint8Array, R(t.ArrayType, r[n].map(s => +s)))
+        return U.isTimestamp(t) || (U.isInt(t) || U.isTime(t)) && t.bitWidth === 64 || U.isDate(t) && t.unit === le.MILLISECOND ? R(Uint8Array, wt.convertArray(r[n])) : U.isDecimal(t) ? R(Uint8Array, Gt.convertArray(r[n])) : U.isBinary(t) || U.isFixedSizeBinary(t) ? Hb(r[n]) : U.isBool(t) ? xr(r[n]) : U.isUtf8(t) ? vs(r[n].join("")) : R(Uint8Array, R(t.ArrayType, r[n].map(s => +s)))
     }
 }
 
-function Zb(e) {
+function Hb(e) {
     const t = e.join(""),
         n = new Uint8Array(t.length / 2);
     for (let r = 0; r < t.length; r += 2) n[r >> 1] = parseInt(t.substr(r, 2), 16);
     return n
 }
-var Hb = y.Long,
-    Yc = m.apache.arrow.flatbuf.Null,
+var Jb = y.Long,
+    Kc = m.apache.arrow.flatbuf.Null,
     hi = m.apache.arrow.flatbuf.Int,
     Gs = m.apache.arrow.flatbuf.FloatingPoint,
-    Gc = m.apache.arrow.flatbuf.Binary,
-    Kc = m.apache.arrow.flatbuf.Bool,
-    Zc = m.apache.arrow.flatbuf.Utf8,
+    Zc = m.apache.arrow.flatbuf.Binary,
+    Hc = m.apache.arrow.flatbuf.Bool,
+    Jc = m.apache.arrow.flatbuf.Utf8,
     di = m.apache.arrow.flatbuf.Decimal,
     Ks = m.apache.arrow.flatbuf.Date,
     pi = m.apache.arrow.flatbuf.Time,
     yi = m.apache.arrow.flatbuf.Timestamp,
     Zs = m.apache.arrow.flatbuf.Interval,
-    Hc = m.apache.arrow.flatbuf.List,
-    Jc = m.apache.arrow.flatbuf.Struct_,
-    Fn = m.apache.arrow.flatbuf.Union,
+    Xc = m.apache.arrow.flatbuf.List,
+    qc = m.apache.arrow.flatbuf.Struct_,
+    xn = m.apache.arrow.flatbuf.Union,
     yr = m.apache.arrow.flatbuf.DictionaryEncoding,
     Hs = m.apache.arrow.flatbuf.FixedSizeBinary,
     Js = m.apache.arrow.flatbuf.FixedSizeList,
     Xs = m.apache.arrow.flatbuf.Map;
-class Jb extends V {
+class Xb extends V {
     visit(t, n) {
         return t == null || n == null ? void 0 : super.visit(t, n)
     }
     visitNull(t, n) {
-        return Yc.startNull(n), Yc.endNull(n)
+        return Kc.startNull(n), Kc.endNull(n)
     }
     visitInt(t, n) {
         return hi.startInt(n), hi.addBitWidth(n, t.bitWidth), hi.addIsSigned(n, t.isSigned), hi.endInt(n)
     }
     visitFloat(t, n) {
         return Gs.startFloatingPoint(n), Gs.addPrecision(n, t.precision), Gs.endFloatingPoint(n)
     }
     visitBinary(t, n) {
-        return Gc.startBinary(n), Gc.endBinary(n)
+        return Zc.startBinary(n), Zc.endBinary(n)
     }
     visitBool(t, n) {
-        return Kc.startBool(n), Kc.endBool(n)
+        return Hc.startBool(n), Hc.endBool(n)
     }
     visitUtf8(t, n) {
-        return Zc.startUtf8(n), Zc.endUtf8(n)
+        return Jc.startUtf8(n), Jc.endUtf8(n)
     }
     visitDecimal(t, n) {
         return di.startDecimal(n), di.addScale(n, t.scale), di.addPrecision(n, t.precision), di.endDecimal(n)
     }
     visitDate(t, n) {
         return Ks.startDate(n), Ks.addUnit(n, t.unit), Ks.endDate(n)
     }
@@ -7358,90 +7358,90 @@
         const r = t.timezone && n.createString(t.timezone) || void 0;
         return yi.startTimestamp(n), yi.addUnit(n, t.unit), r !== void 0 && yi.addTimezone(n, r), yi.endTimestamp(n)
     }
     visitInterval(t, n) {
         return Zs.startInterval(n), Zs.addUnit(n, t.unit), Zs.endInterval(n)
     }
     visitList(t, n) {
-        return Hc.startList(n), Hc.endList(n)
+        return Xc.startList(n), Xc.endList(n)
     }
     visitStruct(t, n) {
-        return Jc.startStruct_(n), Jc.endStruct_(n)
+        return qc.startStruct_(n), qc.endStruct_(n)
     }
     visitUnion(t, n) {
-        Fn.startTypeIdsVector(n, t.typeIds.length);
-        const r = Fn.createTypeIdsVector(n, t.typeIds);
-        return Fn.startUnion(n), Fn.addMode(n, t.mode), Fn.addTypeIds(n, r), Fn.endUnion(n)
+        xn.startTypeIdsVector(n, t.typeIds.length);
+        const r = xn.createTypeIdsVector(n, t.typeIds);
+        return xn.startUnion(n), xn.addMode(n, t.mode), xn.addTypeIds(n, r), xn.endUnion(n)
     }
     visitDictionary(t, n) {
         const r = this.visit(t.indices, n);
-        return yr.startDictionaryEncoding(n), yr.addId(n, new Hb(t.id, 0)), yr.addIsOrdered(n, t.isOrdered), r !== void 0 && yr.addIndexType(n, r), yr.endDictionaryEncoding(n)
+        return yr.startDictionaryEncoding(n), yr.addId(n, new Jb(t.id, 0)), yr.addIsOrdered(n, t.isOrdered), r !== void 0 && yr.addIndexType(n, r), yr.endDictionaryEncoding(n)
     }
     visitFixedSizeBinary(t, n) {
         return Hs.startFixedSizeBinary(n), Hs.addByteWidth(n, t.byteWidth), Hs.endFixedSizeBinary(n)
     }
     visitFixedSizeList(t, n) {
         return Js.startFixedSizeList(n), Js.addListSize(n, t.listSize), Js.endFixedSizeList(n)
     }
     visitMap(t, n) {
         return Xs.startMap(n), Xs.addKeysSorted(n, t.keysSorted), Xs.endMap(n)
     }
 }
-const qs = new Jb;
+const qs = new Xb;
 
-function Xb(e, t = new Map) {
-    return new H(Qb(e, t), Oi(e.customMetadata), t)
+function qb(e, t = new Map) {
+    return new H(tm(e, t), Oi(e.customMetadata), t)
 }
 
-function kf(e) {
-    return new Ct(e.count, Ef(e.columns), Uf(e.columns))
+function Uf(e) {
+    return new Rt(e.count, Nf(e.columns), Mf(e.columns))
 }
 
-function qb(e) {
-    return new fe(kf(e.data), e.id, e.isDelta)
+function Qb(e) {
+    return new fe(Uf(e.data), e.id, e.isDelta)
 }
 
-function Qb(e, t) {
+function tm(e, t) {
     return (e.fields || []).filter(Boolean).map(n => W.fromJSON(n, t))
 }
 
-function Xc(e, t) {
+function Qc(e, t) {
     return (e.children || []).filter(Boolean).map(n => W.fromJSON(n, t))
 }
 
-function Ef(e) {
-    return (e || []).reduce((t, n) => [...t, new Tn(n.count, tm(n.VALIDITY)), ...Ef(n.children)], [])
+function Nf(e) {
+    return (e || []).reduce((t, n) => [...t, new An(n.count, em(n.VALIDITY)), ...Nf(n.children)], [])
 }
 
-function Uf(e, t = []) {
+function Mf(e, t = []) {
     for (let n = -1, r = (e || []).length; ++n < r;) {
         const s = e[n];
-        s.VALIDITY && t.push(new ae(t.length, s.VALIDITY.length)), s.TYPE && t.push(new ae(t.length, s.TYPE.length)), s.OFFSET && t.push(new ae(t.length, s.OFFSET.length)), s.DATA && t.push(new ae(t.length, s.DATA.length)), t = Uf(s.children, t)
+        s.VALIDITY && t.push(new ce(t.length, s.VALIDITY.length)), s.TYPE && t.push(new ce(t.length, s.TYPE.length)), s.OFFSET && t.push(new ce(t.length, s.OFFSET.length)), s.DATA && t.push(new ce(t.length, s.DATA.length)), t = Mf(s.children, t)
     }
     return t
 }
 
-function tm(e) {
+function em(e) {
     return (e || []).reduce((t, n) => t + +(n === 0), 0)
 }
 
-function em(e, t) {
+function nm(e, t) {
     let n, r, s, o, i, a;
-    return !t || !(o = e.dictionary) ? (i = Qc(e, Xc(e, t)), s = new W(e.name, i, e.nullable, Oi(e.customMetadata))) : t.has(n = o.id) ? (r = (r = o.indexType) ? qc(r) : new hn, a = new Ke(t.get(n), r, n, o.isOrdered), s = new W(e.name, a, e.nullable, Oi(e.customMetadata))) : (r = (r = o.indexType) ? qc(r) : new hn, t.set(n, i = Qc(e, Xc(e, t))), a = new Ke(i, r, n, o.isOrdered), s = new W(e.name, a, e.nullable, Oi(e.customMetadata))), s || null
+    return !t || !(o = e.dictionary) ? (i = eu(e, Qc(e, t)), s = new W(e.name, i, e.nullable, Oi(e.customMetadata))) : t.has(n = o.id) ? (r = (r = o.indexType) ? tu(r) : new pn, a = new Ze(t.get(n), r, n, o.isOrdered), s = new W(e.name, a, e.nullable, Oi(e.customMetadata))) : (r = (r = o.indexType) ? tu(r) : new pn, t.set(n, i = eu(e, Qc(e, t))), a = new Ze(i, r, n, o.isOrdered), s = new W(e.name, a, e.nullable, Oi(e.customMetadata))), s || null
 }
 
 function Oi(e) {
     return new Map(Object.entries(e || {}))
 }
 
-function qc(e) {
+function tu(e) {
     return new xt(e.isSigned, e.bitWidth)
 }
 
-function Qc(e, t) {
+function eu(e, t) {
     const n = e.type.name;
     switch (n) {
         case "NONE":
             return new Jn;
         case "null":
             return new Jn;
         case "binary":
@@ -7449,26 +7449,26 @@
         case "utf8":
             return new Qn;
         case "bool":
             return new Dr;
         case "list":
             return new er((t || [])[0]);
         case "struct":
-            return new Qt(t || []);
+            return new te(t || []);
         case "struct_":
-            return new Qt(t || [])
+            return new te(t || [])
     }
     switch (n) {
         case "int": {
             const r = e.type;
             return new xt(r.isSigned, r.bitWidth)
         }
         case "floatingpoint": {
             const r = e.type;
-            return new dn(Pt[r.precision])
+            return new yn(zt[r.precision])
         }
         case "decimal": {
             const r = e.type;
             return new Pi(r.scale, r.precision)
         }
         case "date": {
             const r = e.type;
@@ -7501,53 +7501,53 @@
         case "map": {
             const r = e.type;
             return new Ur((t || [])[0], r.keysSorted)
         }
     }
     throw new Error(`Unrecognized type: "${n}"`)
 }
-var yn = y.Long,
-    nm = y.Builder,
-    rm = y.ByteBuffer,
+var mn = y.Long,
+    rm = y.Builder,
+    im = y.ByteBuffer,
     ft = m.apache.arrow.flatbuf.Type,
-    $t = m.apache.arrow.flatbuf.Field,
+    Yt = m.apache.arrow.flatbuf.Field,
     ve = m.apache.arrow.flatbuf.Schema,
-    im = m.apache.arrow.flatbuf.Buffer,
+    sm = m.apache.arrow.flatbuf.Buffer,
     Ue = gt.apache.arrow.flatbuf.Message,
     je = m.apache.arrow.flatbuf.KeyValue,
-    sm = gt.apache.arrow.flatbuf.FieldNode,
-    tu = m.apache.arrow.flatbuf.Endianness,
+    om = gt.apache.arrow.flatbuf.FieldNode,
+    nu = m.apache.arrow.flatbuf.Endianness,
     Re = gt.apache.arrow.flatbuf.RecordBatch,
-    En = gt.apache.arrow.flatbuf.DictionaryBatch;
+    Un = gt.apache.arrow.flatbuf.DictionaryBatch;
 class _t {
     constructor(t, n, r, s) {
         this._version = n, this._headerType = r, this.body = new Uint8Array(0), s && (this._createHeader = () => s), this._bodyLength = typeof t == "number" ? t : t.low
     }
     static fromJSON(t, n) {
-        const r = new _t(0, Gt.V4, n);
-        return r._createHeader = om(t, n), r
+        const r = new _t(0, Kt.V4, n);
+        return r._createHeader = am(t, n), r
     }
     static decode(t) {
-        t = new rm(j(t));
+        t = new im(j(t));
         const n = Ue.getRootAsMessage(t),
             r = n.bodyLength(),
             s = n.version(),
             o = n.headerType(),
             i = new _t(r, s, o);
-        return i._createHeader = am(n, o), i
+        return i._createHeader = cm(n, o), i
     }
     static encode(t) {
-        let n = new nm,
+        let n = new rm,
             r = -1;
-        return t.isSchema() ? r = H.encode(n, t.header()) : t.isRecordBatch() ? r = Ct.encode(n, t.header()) : t.isDictionaryBatch() && (r = fe.encode(n, t.header())), Ue.startMessage(n), Ue.addVersion(n, Gt.V4), Ue.addHeader(n, r), Ue.addHeaderType(n, t.headerType), Ue.addBodyLength(n, new yn(t.bodyLength, 0)), Ue.finishMessageBuffer(n, Ue.endMessage(n)), n.asUint8Array()
+        return t.isSchema() ? r = H.encode(n, t.header()) : t.isRecordBatch() ? r = Rt.encode(n, t.header()) : t.isDictionaryBatch() && (r = fe.encode(n, t.header())), Ue.startMessage(n), Ue.addVersion(n, Kt.V4), Ue.addHeader(n, r), Ue.addHeaderType(n, t.headerType), Ue.addBodyLength(n, new mn(t.bodyLength, 0)), Ue.finishMessageBuffer(n, Ue.endMessage(n)), n.asUint8Array()
     }
     static from(t, n = 0) {
-        if (t instanceof H) return new _t(0, Gt.V4, Q.Schema, t);
-        if (t instanceof Ct) return new _t(n, Gt.V4, Q.RecordBatch, t);
-        if (t instanceof fe) return new _t(n, Gt.V4, Q.DictionaryBatch, t);
+        if (t instanceof H) return new _t(0, Kt.V4, Q.Schema, t);
+        if (t instanceof Rt) return new _t(n, Kt.V4, Q.RecordBatch, t);
+        if (t instanceof fe) return new _t(n, Kt.V4, Q.DictionaryBatch, t);
         throw new Error(`Unrecognized Message header: ${t}`)
     }
     get type() {
         return this.headerType
     }
     get version() {
         return this._version
@@ -7567,15 +7567,15 @@
     isRecordBatch() {
         return this.headerType === Q.RecordBatch
     }
     isDictionaryBatch() {
         return this.headerType === Q.DictionaryBatch
     }
 }
-class Ct {
+class Rt {
     get nodes() {
         return this._nodes
     }
     get length() {
         return this._length
     }
     get buffers() {
@@ -7604,131 +7604,131 @@
     get buffers() {
         return this.data.buffers
     }
     constructor(t, n, r = !1) {
         this._data = t, this._isDelta = r, this._id = typeof n == "number" ? n : n.low
     }
 }
-class ae {
+class ce {
     constructor(t, n) {
         this.offset = typeof t == "number" ? t : t.low, this.length = typeof n == "number" ? n : n.low
     }
 }
-class Tn {
+class An {
     constructor(t, n) {
         this.length = typeof t == "number" ? t : t.low, this.nullCount = typeof n == "number" ? n : n.low
     }
 }
 
-function om(e, t) {
+function am(e, t) {
     return () => {
         switch (t) {
             case Q.Schema:
                 return H.fromJSON(e);
             case Q.RecordBatch:
-                return Ct.fromJSON(e);
+                return Rt.fromJSON(e);
             case Q.DictionaryBatch:
                 return fe.fromJSON(e)
         }
         throw new Error(`Unrecognized Message type: { name: ${Q[t]}, type: ${t} }`)
     }
 }
 
-function am(e, t) {
+function cm(e, t) {
     return () => {
         switch (t) {
             case Q.Schema:
                 return H.decode(e.header(new ve));
             case Q.RecordBatch:
-                return Ct.decode(e.header(new Re), e.version());
+                return Rt.decode(e.header(new Re), e.version());
             case Q.DictionaryBatch:
-                return fe.decode(e.header(new En), e.version())
+                return fe.decode(e.header(new Un), e.version())
         }
         throw new Error(`Unrecognized Message type: { name: ${Q[t]}, type: ${t} }`)
     }
 }
-W.encode = gm;
-W.decode = bm;
-W.fromJSON = em;
-H.encode = mm;
-H.decode = cm;
-H.fromJSON = Xb;
-Ct.encode = vm;
-Ct.decode = um;
-Ct.fromJSON = kf;
-fe.encode = wm;
-fe.decode = lm;
-fe.fromJSON = qb;
-Tn.encode = _m;
-Tn.decode = hm;
-ae.encode = Sm;
-ae.decode = fm;
+W.encode = vm;
+W.decode = mm;
+W.fromJSON = nm;
+H.encode = gm;
+H.decode = um;
+H.fromJSON = qb;
+Rt.encode = wm;
+Rt.decode = lm;
+Rt.fromJSON = Uf;
+fe.encode = _m;
+fe.decode = fm;
+fe.fromJSON = Qb;
+An.encode = Sm;
+An.decode = dm;
+ce.encode = Im;
+ce.decode = hm;
 
-function cm(e, t = new Map) {
-    const n = ym(e, t);
+function um(e, t = new Map) {
+    const n = bm(e, t);
     return new H(n, Fi(e), t)
 }
 
-function um(e, t = Gt.V4) {
-    return new Ct(e.length(), dm(e), pm(e, t))
+function lm(e, t = Kt.V4) {
+    return new Rt(e.length(), pm(e), ym(e, t))
 }
 
-function lm(e, t = Gt.V4) {
-    return new fe(Ct.decode(e.data(), t), e.id(), e.isDelta())
-}
-
-function fm(e) {
-    return new ae(e.offset(), e.length())
+function fm(e, t = Kt.V4) {
+    return new fe(Rt.decode(e.data(), t), e.id(), e.isDelta())
 }
 
 function hm(e) {
-    return new Tn(e.length(), e.nullCount())
+    return new ce(e.offset(), e.length())
 }
 
 function dm(e) {
+    return new An(e.length(), e.nullCount())
+}
+
+function pm(e) {
     const t = [];
-    for (let n, r = -1, s = -1, o = e.nodesLength(); ++r < o;)(n = e.nodes(r)) && (t[++s] = Tn.decode(n));
+    for (let n, r = -1, s = -1, o = e.nodesLength(); ++r < o;)(n = e.nodes(r)) && (t[++s] = An.decode(n));
     return t
 }
 
-function pm(e, t) {
+function ym(e, t) {
     const n = [];
-    for (let r, s = -1, o = -1, i = e.buffersLength(); ++s < i;)(r = e.buffers(s)) && (t < Gt.V4 && (r.bb_pos += 8 * (s + 1)), n[++o] = ae.decode(r));
+    for (let r, s = -1, o = -1, i = e.buffersLength(); ++s < i;)(r = e.buffers(s)) && (t < Kt.V4 && (r.bb_pos += 8 * (s + 1)), n[++o] = ce.decode(r));
     return n
 }
 
-function ym(e, t) {
+function bm(e, t) {
     const n = [];
     for (let r, s = -1, o = -1, i = e.fieldsLength(); ++s < i;)(r = e.fields(s)) && (n[++o] = W.decode(r, t));
     return n
 }
 
-function eu(e, t) {
+function ru(e, t) {
     const n = [];
     for (let r, s = -1, o = -1, i = e.childrenLength(); ++s < i;)(r = e.children(s)) && (n[++o] = W.decode(r, t));
     return n
 }
 
-function bm(e, t) {
+function mm(e, t) {
     let n, r, s, o, i, a;
-    return !t || !(a = e.dictionary()) ? (s = ru(e, eu(e, t)), r = new W(e.name(), s, e.nullable(), Fi(e))) : t.has(n = a.id().low) ? (o = (o = a.indexType()) ? nu(o) : new hn, i = new Ke(t.get(n), o, n, a.isOrdered()), r = new W(e.name(), i, e.nullable(), Fi(e))) : (o = (o = a.indexType()) ? nu(o) : new hn, t.set(n, s = ru(e, eu(e, t))), i = new Ke(s, o, n, a.isOrdered()), r = new W(e.name(), i, e.nullable(), Fi(e))), r || null
+    return !t || !(a = e.dictionary()) ? (s = su(e, ru(e, t)), r = new W(e.name(), s, e.nullable(), Fi(e))) : t.has(n = a.id().low) ? (o = (o = a.indexType()) ? iu(o) : new pn, i = new Ze(t.get(n), o, n, a.isOrdered()), r = new W(e.name(), i, e.nullable(), Fi(e))) : (o = (o = a.indexType()) ? iu(o) : new pn, t.set(n, s = su(e, ru(e, t))), i = new Ze(s, o, n, a.isOrdered()), r = new W(e.name(), i, e.nullable(), Fi(e))), r || null
 }
 
 function Fi(e) {
     const t = new Map;
     if (e)
         for (let n, r, s = -1, o = e.customMetadataLength() | 0; ++s < o;)(n = e.customMetadata(s)) && (r = n.key()) != null && t.set(r, n.value());
     return t
 }
 
-function nu(e) {
+function iu(e) {
     return new xt(e.isSigned(), e.bitWidth())
 }
 
-function ru(e, t) {
+function su(e, t) {
     const n = e.typeType();
     switch (n) {
         case ft.NONE:
             return new Jn;
         case ft.Null:
             return new Jn;
         case ft.Binary:
@@ -7736,24 +7736,24 @@
         case ft.Utf8:
             return new Qn;
         case ft.Bool:
             return new Dr;
         case ft.List:
             return new er((t || [])[0]);
         case ft.Struct_:
-            return new Qt(t || [])
+            return new te(t || [])
     }
     switch (n) {
         case ft.Int: {
             const r = e.type(new m.apache.arrow.flatbuf.Int);
             return new xt(r.isSigned(), r.bitWidth())
         }
         case ft.FloatingPoint: {
             const r = e.type(new m.apache.arrow.flatbuf.FloatingPoint);
-            return new dn(r.precision())
+            return new yn(r.precision())
         }
         case ft.Decimal: {
             const r = e.type(new m.apache.arrow.flatbuf.Decimal);
             return new Pi(r.scale(), r.precision())
         }
         case ft.Date: {
             const r = e.type(new m.apache.arrow.flatbuf.Date);
@@ -7787,75 +7787,75 @@
             const r = e.type(new m.apache.arrow.flatbuf.Map);
             return new Ur((t || [])[0], r.keysSorted())
         }
     }
     throw new Error(`Unrecognized type: "${ft[n]}" (${n})`)
 }
 
-function mm(e, t) {
+function gm(e, t) {
     const n = t.fields.map(o => W.encode(e, o));
     ve.startFieldsVector(e, n.length);
     const r = ve.createFieldsVector(e, n),
         s = t.metadata && t.metadata.size > 0 ? ve.createCustomMetadataVector(e, [...t.metadata].map(([o, i]) => {
             const a = e.createString(`${o}`),
                 c = e.createString(`${i}`);
             return je.startKeyValue(e), je.addKey(e, a), je.addValue(e, c), je.endKeyValue(e)
         })) : -1;
-    return ve.startSchema(e), ve.addFields(e, r), ve.addEndianness(e, Im ? tu.Little : tu.Big), s !== -1 && ve.addCustomMetadata(e, s), ve.endSchema(e)
+    return ve.startSchema(e), ve.addFields(e, r), ve.addEndianness(e, Tm ? nu.Little : nu.Big), s !== -1 && ve.addCustomMetadata(e, s), ve.endSchema(e)
 }
 
-function gm(e, t) {
+function vm(e, t) {
     let n = -1,
         r = -1,
         s = -1,
         o = t.type,
         i = t.typeId;
     U.isDictionary(o) ? (i = o.dictionary.typeId, s = qs.visit(o, e), r = qs.visit(o.dictionary, e)) : r = qs.visit(o, e);
     const a = (o.children || []).map(l => W.encode(e, l)),
-        c = $t.createChildrenVector(e, a),
-        u = t.metadata && t.metadata.size > 0 ? $t.createCustomMetadataVector(e, [...t.metadata].map(([l, f]) => {
+        c = Yt.createChildrenVector(e, a),
+        u = t.metadata && t.metadata.size > 0 ? Yt.createCustomMetadataVector(e, [...t.metadata].map(([l, f]) => {
             const h = e.createString(`${l}`),
                 p = e.createString(`${f}`);
             return je.startKeyValue(e), je.addKey(e, h), je.addValue(e, p), je.endKeyValue(e)
         })) : -1;
-    return t.name && (n = e.createString(t.name)), $t.startField(e), $t.addType(e, r), $t.addTypeType(e, i), $t.addChildren(e, c), $t.addNullable(e, !!t.nullable), n !== -1 && $t.addName(e, n), s !== -1 && $t.addDictionary(e, s), u !== -1 && $t.addCustomMetadata(e, u), $t.endField(e)
+    return t.name && (n = e.createString(t.name)), Yt.startField(e), Yt.addType(e, r), Yt.addTypeType(e, i), Yt.addChildren(e, c), Yt.addNullable(e, !!t.nullable), n !== -1 && Yt.addName(e, n), s !== -1 && Yt.addDictionary(e, s), u !== -1 && Yt.addCustomMetadata(e, u), Yt.endField(e)
 }
 
-function vm(e, t) {
+function wm(e, t) {
     const n = t.nodes || [],
         r = t.buffers || [];
-    Re.startNodesVector(e, n.length), n.slice().reverse().forEach(i => Tn.encode(e, i));
+    Re.startNodesVector(e, n.length), n.slice().reverse().forEach(i => An.encode(e, i));
     const s = e.endVector();
-    Re.startBuffersVector(e, r.length), r.slice().reverse().forEach(i => ae.encode(e, i));
+    Re.startBuffersVector(e, r.length), r.slice().reverse().forEach(i => ce.encode(e, i));
     const o = e.endVector();
-    return Re.startRecordBatch(e), Re.addLength(e, new yn(t.length, 0)), Re.addNodes(e, s), Re.addBuffers(e, o), Re.endRecordBatch(e)
-}
-
-function wm(e, t) {
-    const n = Ct.encode(e, t.data);
-    return En.startDictionaryBatch(e), En.addId(e, new yn(t.id, 0)), En.addIsDelta(e, t.isDelta), En.addData(e, n), En.endDictionaryBatch(e)
+    return Re.startRecordBatch(e), Re.addLength(e, new mn(t.length, 0)), Re.addNodes(e, s), Re.addBuffers(e, o), Re.endRecordBatch(e)
 }
 
 function _m(e, t) {
-    return sm.createFieldNode(e, new yn(t.length, 0), new yn(t.nullCount, 0))
+    const n = Rt.encode(e, t.data);
+    return Un.startDictionaryBatch(e), Un.addId(e, new mn(t.id, 0)), Un.addIsDelta(e, t.isDelta), Un.addData(e, n), Un.endDictionaryBatch(e)
 }
 
 function Sm(e, t) {
-    return im.createBuffer(e, new yn(t.offset, 0), new yn(t.length, 0))
+    return om.createFieldNode(e, new mn(t.length, 0), new mn(t.nullCount, 0))
 }
-const Im = function() {
+
+function Im(e, t) {
+    return sm.createBuffer(e, new mn(t.offset, 0), new mn(t.length, 0))
+}
+const Tm = function() {
     const e = new ArrayBuffer(2);
     return new DataView(e).setInt16(0, 256, !0), new Int16Array(e)[0] === 256
 }();
-var Nf = y.ByteBuffer;
-const Ma = e => `Expected ${Q[e]} Message in stream, but was null or length 0.`,
-    Ca = e => `Header pointer of flatbuffer-encoded ${Q[e]} Message is null or length 0.`,
-    Mf = (e, t) => `Expected to read ${e} metadata bytes, but only read ${t}.`,
-    Cf = (e, t) => `Expected to read ${e} bytes for message body, but only read ${t}.`;
-class Rf {
+var Cf = y.ByteBuffer;
+const Ea = e => `Expected ${Q[e]} Message in stream, but was null or length 0.`,
+    Ua = e => `Header pointer of flatbuffer-encoded ${Q[e]} Message is null or length 0.`,
+    Rf = (e, t) => `Expected to read ${e} metadata bytes, but only read ${t}.`,
+    Vf = (e, t) => `Expected to read ${e} bytes for message body, but only read ${t}.`;
+class jf {
     constructor(t) {
         this.source = t instanceof Ki ? t : new Ki(t)
     } [Symbol.iterator]() {
         return this
     }
     next() {
         let t;
@@ -7866,52 +7866,52 @@
     }
     return (t) {
         return this.source.return(t)
     }
     readMessage(t) {
         let n;
         if ((n = this.next()).done) return null;
-        if (t != null && n.value.headerType !== t) throw new Error(Ma(t));
+        if (t != null && n.value.headerType !== t) throw new Error(Ea(t));
         return n.value
     }
     readMessageBody(t) {
         if (t <= 0) return new Uint8Array(0);
         const n = j(this.source.read(t));
-        if (n.byteLength < t) throw new Error(Cf(t, n.byteLength));
+        if (n.byteLength < t) throw new Error(Vf(t, n.byteLength));
         return n.byteOffset % 8 === 0 && n.byteOffset + n.byteLength <= n.buffer.byteLength ? n : n.slice()
     }
     readSchema(t = !1) {
         const n = Q.Schema,
             r = this.readMessage(n),
             s = r && r.header();
-        if (t && !s) throw new Error(Ca(n));
+        if (t && !s) throw new Error(Ua(n));
         return s
     }
     readMetadataLength() {
         const t = this.source.read(xs),
-            n = t && new Nf(t),
+            n = t && new Cf(t),
             r = n && n.readInt32(0) || 0;
         return {
             done: r === 0,
             value: r
         }
     }
     readMetadata(t) {
         const n = this.source.read(t);
         if (!n) return ot;
-        if (n.byteLength < t) throw new Error(Mf(t, n.byteLength));
+        if (n.byteLength < t) throw new Error(Rf(t, n.byteLength));
         return {
             done: !1,
             value: _t.decode(n)
         }
     }
 }
-class Tm {
+class Am {
     constructor(t, n) {
-        this.source = t instanceof pn ? t : Rl(t) ? new Zi(t, n) : new pn(t)
+        this.source = t instanceof bn ? t : jl(t) ? new Zi(t, n) : new bn(t)
     } [Symbol.asyncIterator]() {
         return this
     }
     async next() {
         let t;
         return (t = await this.readMetadataLength()).done || t.value === -1 && (t = await this.readMetadataLength()).done || (t = await this.readMetadata(t.value)).done ? ot : t
     }
@@ -7920,52 +7920,52 @@
     }
     async return (t) {
         return await this.source.return(t)
     }
     async readMessage(t) {
         let n;
         if ((n = await this.next()).done) return null;
-        if (t != null && n.value.headerType !== t) throw new Error(Ma(t));
+        if (t != null && n.value.headerType !== t) throw new Error(Ea(t));
         return n.value
     }
     async readMessageBody(t) {
         if (t <= 0) return new Uint8Array(0);
         const n = j(await this.source.read(t));
-        if (n.byteLength < t) throw new Error(Cf(t, n.byteLength));
+        if (n.byteLength < t) throw new Error(Vf(t, n.byteLength));
         return n.byteOffset % 8 === 0 && n.byteOffset + n.byteLength <= n.buffer.byteLength ? n : n.slice()
     }
     async readSchema(t = !1) {
         const n = Q.Schema,
             r = await this.readMessage(n),
             s = r && r.header();
-        if (t && !s) throw new Error(Ca(n));
+        if (t && !s) throw new Error(Ua(n));
         return s
     }
     async readMetadataLength() {
         const t = await this.source.read(xs),
-            n = t && new Nf(t),
+            n = t && new Cf(t),
             r = n && n.readInt32(0) || 0;
         return {
             done: r === 0,
             value: r
         }
     }
     async readMetadata(t) {
         const n = await this.source.read(t);
         if (!n) return ot;
-        if (n.byteLength < t) throw new Error(Mf(t, n.byteLength));
+        if (n.byteLength < t) throw new Error(Rf(t, n.byteLength));
         return {
             done: !1,
             value: _t.decode(n)
         }
     }
 }
-class Am extends Rf {
+class Bm extends jf {
     constructor(t) {
-        super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof Cc ? t : new Cc(t)
+        super(new Uint8Array(0)), this._schema = !1, this._body = [], this._batchIndex = 0, this._dictionaryIndex = 0, this._json = t instanceof Vc ? t : new Vc(t)
     }
     next() {
         const {
             _json: t
         } = this;
         if (!this._schema) {
             this._schema = !0;
@@ -8001,57 +8001,57 @@
         function n(r) {
             return (r || []).reduce((s, o) => [...s, ...o.VALIDITY && [o.VALIDITY] || [], ...o.TYPE && [o.TYPE] || [], ...o.OFFSET && [o.OFFSET] || [], ...o.DATA && [o.DATA] || [], ...n(o.children)], [])
         }
     }
     readMessage(t) {
         let n;
         if ((n = this.next()).done) return null;
-        if (t != null && n.value.headerType !== t) throw new Error(Ma(t));
+        if (t != null && n.value.headerType !== t) throw new Error(Ea(t));
         return n.value
     }
     readSchema() {
         const t = Q.Schema,
             n = this.readMessage(t),
             r = n && n.header();
-        if (!n || !r) throw new Error(Ca(t));
+        if (!n || !r) throw new Error(Ua(t));
         return r
     }
 }
 const xs = 4,
     Lo = "ARROW1",
     Rr = new Uint8Array(Lo.length);
 for (let e = 0; e < Lo.length; e += 1) Rr[e] = Lo.charCodeAt(e);
 
-function Ra(e, t = 0) {
+function Na(e, t = 0) {
     for (let n = -1, r = Rr.length; ++n < r;)
         if (Rr[n] !== e[t + n]) return !1;
     return !0
 }
 const ti = Rr.length,
-    Vf = ti + xs,
-    Bm = ti * 2 + xs;
+    Pf = ti + xs,
+    Om = ti * 2 + xs;
 class lt extends V {
     constructor() {
         super(), this._byteLength = 0, this._nodes = [], this._buffers = [], this._bufferRegions = []
     }
     static assemble(...t) {
         const n = new lt,
-            r = ab(Ot, t),
+            r = cb(Ot, t),
             [s = n] = n.visitMany(r);
         return s
     }
     visit(t) {
         if (!U.isDictionary(t.type)) {
             const {
                 data: n,
                 length: r,
                 nullCount: s
             } = t;
             if (r > 2147483647) throw new RangeError("Cannot write arrays larger than 2^31 - 1 in length");
-            U.isNull(t.type) || Ht.call(this, s <= 0 ? new Uint8Array(0) : Ss(n.offset, r, n.nullBitmap)), this.nodes.push(new Tn(r, s))
+            U.isNull(t.type) || Jt.call(this, s <= 0 ? new Uint8Array(0) : Ss(n.offset, r, n.nullBitmap)), this.nodes.push(new An(r, s))
         }
         return super.visit(t)
     }
     visitNull(t) {
         return this
     }
     visitDictionary(t) {
@@ -8067,95 +8067,95 @@
         return this._byteLength
     }
     get bufferRegions() {
         return this._bufferRegions
     }
 }
 
-function Ht(e) {
+function Jt(e) {
     const t = e.byteLength + 7 & -8;
-    return this.buffers.push(e), this.bufferRegions.push(new ae(this._byteLength, t)), this._byteLength += t, this
+    return this.buffers.push(e), this.bufferRegions.push(new ce(this._byteLength, t)), this._byteLength += t, this
 }
 
-function Om(e) {
+function Fm(e) {
     const {
         type: t,
         length: n,
         typeIds: r,
         valueOffsets: s
     } = e;
-    if (Ht.call(this, r), t.mode === Be.Sparse) return Do.call(this, e);
+    if (Jt.call(this, r), t.mode === Be.Sparse) return Do.call(this, e);
     if (t.mode === Be.Dense) {
-        if (e.offset <= 0) return Ht.call(this, s), Do.call(this, e); {
+        if (e.offset <= 0) return Jt.call(this, s), Do.call(this, e); {
             const o = r.reduce((l, f) => Math.max(l, f), r[0]),
                 i = new Int32Array(o + 1),
                 a = new Int32Array(o + 1).fill(-1),
                 c = new Int32Array(n),
                 u = _s(-s[0], n, s);
             for (let l, f, h = -1; ++h < n;)(f = a[l = r[h]]) === -1 && (f = a[l] = u[l]), c[h] = u[h] - f, ++i[l];
-            Ht.call(this, c);
+            Jt.call(this, c);
             for (let l, f = -1, h = t.children.length; ++f < h;)
                 if (l = e.getChildAt(f)) {
                     const p = t.typeIds[f],
                         w = Math.min(n, i[p]);
                     this.visit(l.slice(a[p], w))
                 }
         }
     }
     return this
 }
 
-function Fm(e) {
+function xm(e) {
     let t;
-    return e.nullCount >= e.length ? Ht.call(this, new Uint8Array(0)) : (t = e.values) instanceof Uint8Array ? Ht.call(this, Ss(e.offset, e.length, t)) : Ht.call(this, xr(e))
+    return e.nullCount >= e.length ? Jt.call(this, new Uint8Array(0)) : (t = e.values) instanceof Uint8Array ? Jt.call(this, Ss(e.offset, e.length, t)) : Jt.call(this, xr(e))
 }
 
-function qe(e) {
-    return Ht.call(this, e.values.subarray(0, e.length * e.stride))
+function tn(e) {
+    return Jt.call(this, e.values.subarray(0, e.length * e.stride))
 }
 
-function jf(e) {
+function zf(e) {
     const {
         length: t,
         values: n,
         valueOffsets: r
     } = e, s = r[0], o = r[t], i = Math.min(o - s, n.byteLength - s);
-    return Ht.call(this, _s(-r[0], t, r)), Ht.call(this, n.subarray(s, s + i)), this
+    return Jt.call(this, _s(-r[0], t, r)), Jt.call(this, n.subarray(s, s + i)), this
 }
 
-function Va(e) {
+function Ma(e) {
     const {
         length: t,
         valueOffsets: n
     } = e;
-    return n && Ht.call(this, _s(n[0], t, n)), this.visit(e.getChildAt(0))
+    return n && Jt.call(this, _s(n[0], t, n)), this.visit(e.getChildAt(0))
 }
 
 function Do(e) {
     return this.visitMany(e.type.children.map((t, n) => e.getChildAt(n)).filter(Boolean))[0]
 }
-lt.prototype.visitBool = Fm;
-lt.prototype.visitInt = qe;
-lt.prototype.visitFloat = qe;
-lt.prototype.visitUtf8 = jf;
-lt.prototype.visitBinary = jf;
-lt.prototype.visitFixedSizeBinary = qe;
-lt.prototype.visitDate = qe;
-lt.prototype.visitTimestamp = qe;
-lt.prototype.visitTime = qe;
-lt.prototype.visitDecimal = qe;
-lt.prototype.visitList = Va;
+lt.prototype.visitBool = xm;
+lt.prototype.visitInt = tn;
+lt.prototype.visitFloat = tn;
+lt.prototype.visitUtf8 = zf;
+lt.prototype.visitBinary = zf;
+lt.prototype.visitFixedSizeBinary = tn;
+lt.prototype.visitDate = tn;
+lt.prototype.visitTimestamp = tn;
+lt.prototype.visitTime = tn;
+lt.prototype.visitDecimal = tn;
+lt.prototype.visitList = Ma;
 lt.prototype.visitStruct = Do;
-lt.prototype.visitUnion = Om;
-lt.prototype.visitInterval = qe;
-lt.prototype.visitFixedSizeList = Va;
-lt.prototype.visitMap = Va;
-class ja extends _n {
+lt.prototype.visitUnion = Fm;
+lt.prototype.visitInterval = tn;
+lt.prototype.visitFixedSizeList = Ma;
+lt.prototype.visitMap = Ma;
+class Ca extends Sn {
     constructor(t) {
-        super(), this._position = 0, this._started = !1, this._sink = new Tr, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, Mt(t) || (t = {
+        super(), this._position = 0, this._started = !1, this._sink = new Tr, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, Ct(t) || (t = {
             autoDestroy: !0,
             writeLegacyIpcFormat: !1
         }), this._autoDestroy = typeof t.autoDestroy == "boolean" ? t.autoDestroy : !0, this._writeLegacyIpcFormat = typeof t.writeLegacyIpcFormat == "boolean" ? t.writeLegacyIpcFormat : !1
     }
     static throughNode(t) {
         throw new Error('"throughNode" not available in this environment')
     }
@@ -8165,15 +8165,15 @@
     toString(t = !1) {
         return this._sink.toString(t)
     }
     toUint8Array(t = !1) {
         return this._sink.toUint8Array(t)
     }
     writeAll(t) {
-        return Ge(t) ? t.then(n => this.writeAll(n)) : De(t) ? $a(this, t) : Wa(this, t)
+        return Ke(t) ? t.then(n => this.writeAll(n)) : De(t) ? Pa(this, t) : ja(this, t)
     }
     get closed() {
         return this._sink.closed
     } [Symbol.asyncIterator]() {
         return this._sink[Symbol.asyncIterator]()
     }
     toDOMStream(t) {
@@ -8188,41 +8188,41 @@
     abort(t) {
         return this.reset()._sink.abort(t)
     }
     finish() {
         return this._autoDestroy ? this.close() : this.reset(this._sink, this._schema), this
     }
     reset(t = this._sink, n = null) {
-        return t === this._sink || t instanceof Tr ? this._sink = t : (this._sink = new Tr, t && wp(t) ? this.toDOMStream({
+        return t === this._sink || t instanceof Tr ? this._sink = t : (this._sink = new Tr, t && _p(t) ? this.toDOMStream({
             type: "bytes"
-        }).pipeTo(t) : t && _p(t) && this.toNodeStream({
+        }).pipeTo(t) : t && Sp(t) && this.toNodeStream({
             objectMode: !1
         }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, (!n || !n.compareTo(this._schema)) && (n === null ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = n, this._writeSchema(n))), this
     }
     write(t) {
         let n = null;
         if (this._sink) {
             if (t == null) return this.finish() && void 0;
             if (t instanceof G && !(n = t.schema)) return this.finish() && void 0;
             if (t instanceof Ot && !(n = t.schema)) return this.finish() && void 0
         } else throw new Error("RecordBatchWriter is closed");
         if (n && !n.compareTo(this._schema)) {
             if (this._started && this._autoDestroy) return this.close();
             this.reset(this._sink, n)
         }
-        t instanceof Ot ? t instanceof Es || this._writeRecordBatch(t) : t instanceof G ? this.writeAll(t.chunks) : Xt(t) && this.writeAll(t)
+        t instanceof Ot ? t instanceof Es || this._writeRecordBatch(t) : t instanceof G ? this.writeAll(t.chunks) : qt(t) && this.writeAll(t)
     }
     _writeMessage(t, n = 8) {
         const r = n - 1,
             s = _t.encode(t),
             o = s.byteLength,
             i = this._writeLegacyIpcFormat ? 4 : 8,
             a = o + i + r & ~r,
             c = a - o - i;
-        return t.headerType === Q.RecordBatch ? this._recordBatchBlocks.push(new Ze(a, t.bodyLength, this._position)) : t.headerType === Q.DictionaryBatch && this._dictionaryBlocks.push(new Ze(a, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - i)), o > 0 && this._write(s), this._writePadding(c)
+        return t.headerType === Q.RecordBatch ? this._recordBatchBlocks.push(new He(a, t.bodyLength, this._position)) : t.headerType === Q.DictionaryBatch && this._dictionaryBlocks.push(new He(a, t.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - i)), o > 0 && this._write(s), this._writePadding(c)
     }
     _write(t) {
         if (this._started) {
             const n = j(t);
             n && n.byteLength > 0 && (this._sink.write(n), this._position += n.byteLength)
         }
         return this
@@ -8241,25 +8241,25 @@
     }
     _writeRecordBatch(t) {
         const {
             byteLength: n,
             nodes: r,
             bufferRegions: s,
             buffers: o
-        } = lt.assemble(t), i = new Ct(t.length, r, s), a = _t.from(i, n);
+        } = lt.assemble(t), i = new Rt(t.length, r, s), a = _t.from(i, n);
         return this._writeDictionaries(t)._writeMessage(a)._writeBodyBuffers(o)
     }
     _writeDictionaryBatch(t, n, r = !1) {
         this._dictionaryDeltaOffsets.set(n, t.length + (this._dictionaryDeltaOffsets.get(n) || 0));
         const {
             byteLength: s,
             nodes: o,
             bufferRegions: i,
             buffers: a
-        } = lt.assemble(t), c = new Ct(t.length, o, i), u = new fe(c, n, r), l = _t.from(u, s);
+        } = lt.assemble(t), c = new Rt(t.length, o, i), u = new fe(c, n, r), l = _t.from(u, s);
         return this._writeMessage(l)._writeBodyBuffers(a)
     }
     _writeBodyBuffers(t) {
         let n, r, s;
         for (let o = -1, i = t.length; ++o < i;)(n = t[o]) && (r = n.byteLength) > 0 && (this._write(n), (s = (r + 7 & -8) - r) > 0 && this._writePadding(s));
         return this
     }
@@ -8270,98 +8270,98 @@
                 const o = "chunks" in r ? r.chunks : [r];
                 for (const i of o) this._writeDictionaryBatch(i, n, s > 0), s += i.length
             }
         }
         return this
     }
 }
-class Pa extends ja {
+class Ra extends Ca {
     static writeAll(t, n) {
-        const r = new Pa(n);
-        return Ge(t) ? t.then(s => r.writeAll(s)) : De(t) ? $a(r, t) : Wa(r, t)
+        const r = new Ra(n);
+        return Ke(t) ? t.then(s => r.writeAll(s)) : De(t) ? Pa(r, t) : ja(r, t)
     }
 }
-class za extends ja {
+class Va extends Ca {
     constructor() {
         super(), this._autoDestroy = !0
     }
     static writeAll(t) {
-        const n = new za;
-        return Ge(t) ? t.then(r => n.writeAll(r)) : De(t) ? $a(n, t) : Wa(n, t)
+        const n = new Va;
+        return Ke(t) ? t.then(r => n.writeAll(r)) : De(t) ? Pa(n, t) : ja(n, t)
     }
     _writeSchema(t) {
         return this._writeMagic()._writePadding(2)
     }
     _writeFooter(t) {
-        const n = Cr.encode(new Cr(t, Gt.V4, this._recordBatchBlocks, this._dictionaryBlocks));
+        const n = Cr.encode(new Cr(t, Kt.V4, this._recordBatchBlocks, this._dictionaryBlocks));
         return super._writeFooter(t)._write(n)._write(Int32Array.of(n.byteLength))._writeMagic()
     }
 }
 
-function Wa(e, t) {
+function ja(e, t) {
     let n = t;
     t instanceof G && (n = t.chunks, e.reset(void 0, t.schema));
     for (const r of n) e.write(r);
     return e.finish()
 }
-async function $a(e, t) {
+async function Pa(e, t) {
     for await (const n of t) e.write(n);
     return e.finish()
 }
 const Qs = new Uint8Array(0),
-    Pf = e => [Qs, Qs, new Uint8Array(e), Qs];
+    Wf = e => [Qs, Qs, new Uint8Array(e), Qs];
 
-function xm(e, t, n = t.reduce((r, s) => Math.max(r, s.length), 0)) {
+function Lm(e, t, n = t.reduce((r, s) => Math.max(r, s.length), 0)) {
     let r, s, o = -1,
         i = t.length;
     const a = [...e.fields],
         c = [],
         u = (n + 63 & -64) >> 3;
     for (; ++o < i;)(r = t[o]) && r.length === n ? c[o] = r : ((s = a[o]).nullable || (a[o] = a[o].clone({
         nullable: !0
-    })), c[o] = r ? r._changeLengthAndBackfillNullBitmap(n) : S.new(s.type, 0, n, n, Pf(u)));
+    })), c[o] = r ? r._changeLengthAndBackfillNullBitmap(n) : S.new(s.type, 0, n, n, Wf(u)));
     return [new H(a), n, c]
 }
 
-function Lm(e) {
-    return zf(new H(e.map(({
+function Dm(e) {
+    return $f(new H(e.map(({
         field: t
     }) => t)), e)
 }
 
-function zf(e, t) {
-    return Dm(e, t.map(n => n instanceof mt ? n.chunks.map(r => r.data) : [n.data]))
+function $f(e, t) {
+    return km(e, t.map(n => n instanceof mt ? n.chunks.map(r => r.data) : [n.data]))
 }
 
-function Dm(e, t) {
+function km(e, t) {
     const n = [...e.fields],
         r = [],
         s = {
             numBatches: t.reduce((f, h) => Math.max(f, h.length), 0)
         };
     let o = 0,
         i = 0,
         a = -1,
         c = t.length,
         u, l = [];
     for (; s.numBatches-- > 0;) {
         for (i = Number.POSITIVE_INFINITY, a = -1; ++a < c;) l[a] = u = t[a].shift(), i = Math.min(i, u ? u.length : i);
-        isFinite(i) && (l = km(n, i, l, t, s), i > 0 && (r[o++] = [i, l.slice()]))
+        isFinite(i) && (l = Em(n, i, l, t, s), i > 0 && (r[o++] = [i, l.slice()]))
     }
     return [e = new H(n, e.metadata), r.map(f => new Ot(e, ...f))]
 }
 
-function km(e, t, n, r, s) {
+function Em(e, t, n, r, s) {
     let o, i, a = 0,
         c = -1,
         u = r.length;
     const l = (t + 63 & -64) >> 3;
     for (; ++c < u;)(o = n[c]) && (a = o.length) >= t ? a === t ? n[c] = o : (n[c] = o.slice(0, t), o = o.slice(t, a - t), s.numBatches = Math.max(s.numBatches, r[c].unshift(o))) : ((i = e[c]).nullable || (e[c] = i.clone({
         nullable: !0
-    })), n[c] = o ? o._changeLengthAndBackfillNullBitmap(t) : S.new(i.type, 0, t, t, Pf(l)));
+    })), n[c] = o ? o._changeLengthAndBackfillNullBitmap(t) : S.new(i.type, 0, t, t, Wf(l)));
     return n
 }
 class tt extends z {
     constructor(t, n) {
         super(), this._children = n, this.numChildren = t.childData.length, this._bindDataAccessors(this.data = t)
     }
     get type() {
@@ -8409,15 +8409,15 @@
     clone(t, n = this._children) {
         return z.new(t, n)
     }
     concat(...t) {
         return mt.concat(this, ...t)
     }
     slice(t, n) {
-        return Fa(this, t, n, this._sliceInternal)
+        return Aa(this, t, n, this._sliceInternal)
     }
     isValid(t) {
         if (this.nullCount > 0) {
             const n = this.offset + t;
             return (this.nullBitmap[n >> 3] & 1 << n % 8) !== 0
         }
         return !0
@@ -8430,42 +8430,42 @@
     }
     _sliceInternal(t, n, r) {
         return t.clone(t.data.slice(n, r - n), null)
     }
     _bindDataAccessors(t) {}
 }
 tt.prototype[Symbol.isConcatSpreadable] = !0;
-class Em extends tt {
+class Um extends tt {
     asUtf8() {
         return z.new(this.data.clone(new Qn))
     }
 }
-class Um extends tt {
+class Nm extends tt {
     static from(t) {
-        return bn(() => new Dr, t)
+        return gn(() => new Dr, t)
     }
 }
-class Ya extends tt {
+class za extends tt {
     static from(...t) {
-        return t.length === 2 ? bn(() => t[1] === le.DAY ? new ay : new Rc, t[0]) : bn(() => new Rc, t[0])
+        return t.length === 2 ? gn(() => t[1] === le.DAY ? new cy : new jc, t[0]) : gn(() => new jc, t[0])
     }
 }
-class Nm extends Ya {}
-class Mm extends Ya {}
-class Cm extends tt {}
-class Ga extends tt {
+class Mm extends za {}
+class Cm extends za {}
+class Rm extends tt {}
+class Wa extends tt {
     constructor(t) {
         super(t), this.indices = z.new(t.clone(this.type.indices))
     }
     static from(...t) {
         if (t.length === 3) {
-            const [n, r, s] = t, o = new Ke(n.type, r, null, null);
+            const [n, r, s] = t, o = new Ze(n.type, r, null, null);
             return z.new(S.Dictionary(o, 0, s.length, 0, null, s, n))
         }
-        return bn(() => t[0].type, t[0])
+        return gn(() => t[0].type, t[0])
     }
     get dictionary() {
         return this.data.dictionary
     }
     reverseLookup(t) {
         return this.dictionary.indexOf(t)
     }
@@ -8478,454 +8478,454 @@
     setKey(t, n) {
         return this.indices.set(t, n)
     }
     setValue(t, n) {
         return this.dictionary.set(t, n)
     }
 }
-Ga.prototype.indices = null;
-class Rm extends tt {}
+Wa.prototype.indices = null;
 class Vm extends tt {}
+class jm extends tt {}
 class Ls extends tt {
     static from(t) {
-        let n = zm(this);
+        let n = Wm(this);
         if (t instanceof ArrayBuffer || ArrayBuffer.isView(t)) {
-            let r = Pm(t.constructor) || n;
+            let r = zm(t.constructor) || n;
             if (n === null && (n = r), n && n === r) {
                 let s = new n,
                     o = t.byteLength / s.ArrayType.BYTES_PER_ELEMENT;
-                if (!jm(n, t.constructor)) return z.new(S.Float(s, 0, o, 0, null, t))
+                if (!Pm(n, t.constructor)) return z.new(S.Float(s, 0, o, 0, null, t))
             }
         }
-        if (n) return bn(() => new n, t);
+        if (n) return gn(() => new n, t);
         throw t instanceof DataView || t instanceof ArrayBuffer ? new TypeError(`Cannot infer float type from instance of ${t.constructor.name}`) : new TypeError("Unrecognized FloatVector input")
     }
 }
-class Wf extends Ls {
+class Yf extends Ls {
     toFloat32Array() {
         return new Float32Array(this)
     }
     toFloat64Array() {
         return new Float64Array(this)
     }
 }
-class $f extends Ls {}
-class Yf extends Ls {}
-const jm = (e, t) => e === Ts && t !== Uint16Array,
-    Pm = e => {
+class Gf extends Ls {}
+class Kf extends Ls {}
+const Pm = (e, t) => e === Ts && t !== Uint16Array,
+    zm = e => {
         switch (e) {
             case Uint16Array:
                 return Ts;
             case Float32Array:
-                return Sa;
+                return va;
             case Float64Array:
-                return Ia;
+                return wa;
             default:
                 return null
         }
     },
-    zm = e => {
+    Wm = e => {
         switch (e) {
-            case Wf:
-                return Ts;
-            case $f:
-                return Sa;
             case Yf:
-                return Ia;
+                return Ts;
+            case Gf:
+                return va;
+            case Kf:
+                return wa;
             default:
                 return null
         }
     };
-class Ka extends tt {}
-class Wm extends Ka {}
-class $m extends Ka {}
-class re extends tt {
+class $a extends tt {}
+class $m extends $a {}
+class Ym extends $a {}
+class ie extends tt {
     static from(...t) {
-        let [n, r = !1] = t, s = Km(this, r);
+        let [n, r = !1] = t, s = Zm(this, r);
         if (n instanceof ArrayBuffer || ArrayBuffer.isView(n)) {
-            let o = Gm(n.constructor, r) || s;
+            let o = Km(n.constructor, r) || s;
             if (s === null && (s = o), s && s === o) {
                 let i = new s,
                     a = n.byteLength / i.ArrayType.BYTES_PER_ELEMENT;
-                return Ym(s, n.constructor) && (a *= .5), z.new(S.Int(i, 0, a, 0, null, n))
+                return Gm(s, n.constructor) && (a *= .5), z.new(S.Int(i, 0, a, 0, null, n))
             }
         }
-        if (s) return bn(() => new s, n);
+        if (s) return gn(() => new s, n);
         throw n instanceof DataView || n instanceof ArrayBuffer ? new TypeError(`Cannot infer integer type from instance of ${n.constructor.name}`) : new TypeError("Unrecognized IntVector input")
     }
 }
-class Gf extends re {}
-class Kf extends re {}
-class Zf extends re {}
-class Hf extends re {
+class Zf extends ie {}
+class Hf extends ie {}
+class Jf extends ie {}
+class Xf extends ie {
     toBigInt64Array() {
-        return Pl(this.values)
+        return Wl(this.values)
     }
     get values64() {
         return this._values64 || (this._values64 = this.toBigInt64Array())
     }
 }
-class Jf extends re {}
-class Xf extends re {}
-class qf extends re {}
-class Qf extends re {
+class qf extends ie {}
+class Qf extends ie {}
+class th extends ie {}
+class eh extends ie {
     toBigUint64Array() {
-        return zl(this.values)
+        return $l(this.values)
     }
     get values64() {
         return this._values64 || (this._values64 = this.toBigUint64Array())
     }
 }
-const Ym = (e, t) => (e === Xn || e === qn) && (t === Int32Array || t === Uint32Array),
-    Gm = (e, t) => {
+const Gm = (e, t) => (e === Xn || e === qn) && (t === Int32Array || t === Uint32Array),
+    Km = (e, t) => {
         switch (e) {
             case Int8Array:
-                return ma;
+                return pa;
             case Int16Array:
-                return ga;
+                return ya;
             case Int32Array:
-                return t ? Xn : hn;
+                return t ? Xn : pn;
             case ur:
                 return Xn;
             case Uint8Array:
-                return va;
+                return ba;
             case Uint16Array:
-                return wa;
+                return ma;
             case Uint32Array:
-                return t ? qn : _a;
+                return t ? qn : ga;
             case Yr:
                 return qn;
             default:
                 return null
         }
     },
-    Km = (e, t) => {
+    Zm = (e, t) => {
         switch (e) {
-            case Gf:
-                return ma;
-            case Kf:
-                return ga;
             case Zf:
-                return t ? Xn : hn;
+                return pa;
             case Hf:
-                return Xn;
+                return ya;
             case Jf:
-                return va;
+                return t ? Xn : pn;
             case Xf:
-                return wa;
+                return Xn;
             case qf:
-                return t ? qn : _a;
+                return ba;
             case Qf:
+                return ma;
+            case th:
+                return t ? qn : ga;
+            case eh:
                 return qn;
             default:
                 return null
         }
     };
-class Zm extends tt {}
-class Hm extends tt {
+class Hm extends tt {}
+class Jm extends tt {
     asList() {
         const t = this.type.children[0];
         return z.new(this.data.clone(new er(t)))
     }
     bind(t) {
         const n = this.getChildAt(0),
             {
                 [t]: r,
                 [t + 1]: s
             } = this.valueOffsets;
-        return new af(n.slice(r, s))
+        return new uf(n.slice(r, s))
     }
 }
-class Jm extends tt {}
-const Xm = Symbol.for("rowIndex");
+class Xm extends tt {}
+const qm = Symbol.for("rowIndex");
 class Ds extends tt {
     bind(t) {
-        const n = this._row || (this._row = new cf(this)),
+        const n = this._row || (this._row = new lf(this)),
             r = Object.create(n);
-        return r[Xm] = t, r
+        return r[qm] = t, r
     }
 }
 class ei extends tt {}
-class qm extends ei {}
 class Qm extends ei {}
 class tg extends ei {}
 class eg extends ei {}
+class ng extends ei {}
 class ni extends tt {}
-class ng extends ni {}
 class rg extends ni {}
 class ig extends ni {}
 class sg extends ni {}
-class Za extends tt {
+class og extends ni {}
+class Ya extends tt {
     get typeIdToChildIndex() {
         return this.data.type.typeIdToChildIndex
     }
 }
-class og extends Za {
+class ag extends Ya {
     get valueOffsets() {
         return this.data.valueOffsets
     }
 }
-class ag extends Za {}
-class cg extends tt {
+class cg extends Ya {}
+class ug extends tt {
     static from(t) {
-        return bn(() => new Qn, t)
+        return gn(() => new Qn, t)
     }
     asBinary() {
         return z.new(this.data.clone(new Lr))
     }
 }
 
-function iu(e) {
+function ou(e) {
     return function() {
         return e(this)
     }
 }
 
-function ug(e) {
+function lg(e) {
     return function(t) {
         return e(this, t)
     }
 }
 
-function su(e) {
+function au(e) {
     return function(t, n) {
         return e(this, t, n)
     }
 }
 class O extends V {}
-const lg = (e, t) => 864e5 * e[t],
-    Ha = (e, t) => 4294967296 * e[t + 1] + (e[t] >>> 0),
-    fg = (e, t) => 4294967296 * (e[t + 1] / 1e3) + (e[t] >>> 0) / 1e3,
-    hg = (e, t) => 4294967296 * (e[t + 1] / 1e6) + (e[t] >>> 0) / 1e6,
-    th = e => new Date(e),
-    dg = (e, t) => th(lg(e, t)),
-    pg = (e, t) => th(Ha(e, t)),
-    yg = (e, t) => null,
-    eh = (e, t, n) => {
+const fg = (e, t) => 864e5 * e[t],
+    Ga = (e, t) => 4294967296 * e[t + 1] + (e[t] >>> 0),
+    hg = (e, t) => 4294967296 * (e[t + 1] / 1e3) + (e[t] >>> 0) / 1e3,
+    dg = (e, t) => 4294967296 * (e[t + 1] / 1e6) + (e[t] >>> 0) / 1e6,
+    nh = e => new Date(e),
+    pg = (e, t) => nh(fg(e, t)),
+    yg = (e, t) => nh(Ga(e, t)),
+    bg = (e, t) => null,
+    rh = (e, t, n) => {
         const {
             [n]: r, [n + 1]: s
         } = t;
         return r != null && s != null ? e.subarray(r, s) : null
     },
-    bg = ({
+    mg = ({
         offset: e,
         values: t
     }, n) => {
         const r = e + n;
         return (t[r >> 3] & 1 << r % 8) !== 0
     },
-    nh = ({
+    ih = ({
         values: e
-    }, t) => dg(e, t),
-    rh = ({
+    }, t) => pg(e, t),
+    sh = ({
         values: e
-    }, t) => pg(e, t * 2),
+    }, t) => yg(e, t * 2),
     ye = ({
         stride: e,
         values: t
     }, n) => t[e * n],
-    ih = ({
+    oh = ({
         stride: e,
         values: t
-    }, n) => ef(t[e * n]),
-    Ja = ({
+    }, n) => rf(t[e * n]),
+    Ka = ({
         stride: e,
         values: t,
         type: n
-    }, r) => Sn.new(t.subarray(e * r, e * (r + 1)), n.isSigned),
-    mg = ({
+    }, r) => In.new(t.subarray(e * r, e * (r + 1)), n.isSigned),
+    gg = ({
         stride: e,
         values: t
     }, n) => t.subarray(e * n, e * (n + 1)),
-    gg = ({
+    vg = ({
         values: e,
         valueOffsets: t
-    }, n) => eh(e, t, n),
-    vg = ({
+    }, n) => rh(e, t, n),
+    wg = ({
         values: e,
         valueOffsets: t
     }, n) => {
-        const r = eh(e, t, n);
+        const r = rh(e, t, n);
         return r !== null ? To(r) : null
     },
-    wg = (e, t) => e.type.bitWidth < 64 ? ye(e, t) : Ja(e, t),
-    _g = (e, t) => e.type.precision !== Pt.HALF ? ye(e, t) : ih(e, t),
-    Sg = (e, t) => e.type.unit === le.DAY ? nh(e, t) : rh(e, t),
-    sh = ({
-        values: e
-    }, t) => 1e3 * Ha(e, t * 2),
-    oh = ({
-        values: e
-    }, t) => Ha(e, t * 2),
+    _g = (e, t) => e.type.bitWidth < 64 ? ye(e, t) : Ka(e, t),
+    Sg = (e, t) => e.type.precision !== zt.HALF ? ye(e, t) : oh(e, t),
+    Ig = (e, t) => e.type.unit === le.DAY ? ih(e, t) : sh(e, t),
     ah = ({
         values: e
-    }, t) => fg(e, t * 2),
+    }, t) => 1e3 * Ga(e, t * 2),
     ch = ({
         values: e
+    }, t) => Ga(e, t * 2),
+    uh = ({
+        values: e
     }, t) => hg(e, t * 2),
-    Ig = (e, t) => {
+    lh = ({
+        values: e
+    }, t) => dg(e, t * 2),
+    Tg = (e, t) => {
         switch (e.type.unit) {
             case Z.SECOND:
-                return sh(e, t);
+                return ah(e, t);
             case Z.MILLISECOND:
-                return oh(e, t);
+                return ch(e, t);
             case Z.MICROSECOND:
-                return ah(e, t);
+                return uh(e, t);
             case Z.NANOSECOND:
-                return ch(e, t)
+                return lh(e, t)
         }
     },
-    uh = ({
+    fh = ({
         values: e,
         stride: t
     }, n) => e[t * n],
-    lh = ({
+    hh = ({
         values: e,
         stride: t
     }, n) => e[t * n],
-    fh = ({
+    dh = ({
         values: e
-    }, t) => Sn.signed(e.subarray(2 * t, 2 * (t + 1))),
-    hh = ({
+    }, t) => In.signed(e.subarray(2 * t, 2 * (t + 1))),
+    ph = ({
         values: e
-    }, t) => Sn.signed(e.subarray(2 * t, 2 * (t + 1))),
-    Tg = (e, t) => {
+    }, t) => In.signed(e.subarray(2 * t, 2 * (t + 1))),
+    Ag = (e, t) => {
         switch (e.type.unit) {
             case Z.SECOND:
-                return uh(e, t);
+                return fh(e, t);
             case Z.MILLISECOND:
-                return lh(e, t);
+                return hh(e, t);
             case Z.MICROSECOND:
-                return fh(e, t);
+                return dh(e, t);
             case Z.NANOSECOND:
-                return hh(e, t)
+                return ph(e, t)
         }
     },
-    Ag = ({
+    Bg = ({
         values: e
-    }, t) => Sn.decimal(e.subarray(4 * t, 4 * (t + 1))),
-    Bg = (e, t) => {
+    }, t) => In.decimal(e.subarray(4 * t, 4 * (t + 1))),
+    Og = (e, t) => {
         const n = e.getChildAt(0),
             {
                 valueOffsets: r,
                 stride: s
             } = e;
         return n.slice(r[t * s], r[t * s + 1])
     },
-    Og = (e, t) => e.bind(t),
     Fg = (e, t) => e.bind(t),
-    xg = (e, t) => e.type.mode === Be.Dense ? dh(e, t) : ph(e, t),
-    dh = (e, t) => {
+    xg = (e, t) => e.bind(t),
+    Lg = (e, t) => e.type.mode === Be.Dense ? yh(e, t) : bh(e, t),
+    yh = (e, t) => {
         const n = e.typeIdToChildIndex[e.typeIds[t]],
             r = e.getChildAt(n);
         return r ? r.get(e.valueOffsets[t]) : null
     },
-    ph = (e, t) => {
+    bh = (e, t) => {
         const n = e.typeIdToChildIndex[e.typeIds[t]],
             r = e.getChildAt(n);
         return r ? r.get(t) : null
     },
-    Lg = (e, t) => e.getValue(e.getKey(t)),
-    Dg = (e, t) => e.type.unit === Hn.DAY_TIME ? yh(e, t) : bh(e, t),
-    yh = ({
+    Dg = (e, t) => e.getValue(e.getKey(t)),
+    kg = (e, t) => e.type.unit === Hn.DAY_TIME ? mh(e, t) : gh(e, t),
+    mh = ({
         values: e
     }, t) => e.subarray(2 * t, 2 * (t + 1)),
-    bh = ({
+    gh = ({
         values: e
     }, t) => {
         const n = e[t],
             r = new Int32Array(2);
         return r[0] = n / 12 | 0, r[1] = n % 12 | 0, r
     },
-    kg = (e, t) => {
+    Eg = (e, t) => {
         const n = e.getChildAt(0),
             {
                 stride: r
             } = e;
         return n.slice(t * r, (t + 1) * r)
     };
-O.prototype.visitNull = yg;
-O.prototype.visitBool = bg;
-O.prototype.visitInt = wg;
+O.prototype.visitNull = bg;
+O.prototype.visitBool = mg;
+O.prototype.visitInt = _g;
 O.prototype.visitInt8 = ye;
 O.prototype.visitInt16 = ye;
 O.prototype.visitInt32 = ye;
-O.prototype.visitInt64 = Ja;
+O.prototype.visitInt64 = Ka;
 O.prototype.visitUint8 = ye;
 O.prototype.visitUint16 = ye;
 O.prototype.visitUint32 = ye;
-O.prototype.visitUint64 = Ja;
-O.prototype.visitFloat = _g;
-O.prototype.visitFloat16 = ih;
+O.prototype.visitUint64 = Ka;
+O.prototype.visitFloat = Sg;
+O.prototype.visitFloat16 = oh;
 O.prototype.visitFloat32 = ye;
 O.prototype.visitFloat64 = ye;
-O.prototype.visitUtf8 = vg;
-O.prototype.visitBinary = gg;
-O.prototype.visitFixedSizeBinary = mg;
-O.prototype.visitDate = Sg;
-O.prototype.visitDateDay = nh;
-O.prototype.visitDateMillisecond = rh;
-O.prototype.visitTimestamp = Ig;
-O.prototype.visitTimestampSecond = sh;
-O.prototype.visitTimestampMillisecond = oh;
-O.prototype.visitTimestampMicrosecond = ah;
-O.prototype.visitTimestampNanosecond = ch;
-O.prototype.visitTime = Tg;
-O.prototype.visitTimeSecond = uh;
-O.prototype.visitTimeMillisecond = lh;
-O.prototype.visitTimeMicrosecond = fh;
-O.prototype.visitTimeNanosecond = hh;
-O.prototype.visitDecimal = Ag;
-O.prototype.visitList = Bg;
-O.prototype.visitStruct = Fg;
-O.prototype.visitUnion = xg;
-O.prototype.visitDenseUnion = dh;
-O.prototype.visitSparseUnion = ph;
-O.prototype.visitDictionary = Lg;
-O.prototype.visitInterval = Dg;
-O.prototype.visitIntervalDayTime = yh;
-O.prototype.visitIntervalYearMonth = bh;
-O.prototype.visitFixedSizeList = kg;
-O.prototype.visitMap = Og;
+O.prototype.visitUtf8 = wg;
+O.prototype.visitBinary = vg;
+O.prototype.visitFixedSizeBinary = gg;
+O.prototype.visitDate = Ig;
+O.prototype.visitDateDay = ih;
+O.prototype.visitDateMillisecond = sh;
+O.prototype.visitTimestamp = Tg;
+O.prototype.visitTimestampSecond = ah;
+O.prototype.visitTimestampMillisecond = ch;
+O.prototype.visitTimestampMicrosecond = uh;
+O.prototype.visitTimestampNanosecond = lh;
+O.prototype.visitTime = Ag;
+O.prototype.visitTimeSecond = fh;
+O.prototype.visitTimeMillisecond = hh;
+O.prototype.visitTimeMicrosecond = dh;
+O.prototype.visitTimeNanosecond = ph;
+O.prototype.visitDecimal = Bg;
+O.prototype.visitList = Og;
+O.prototype.visitStruct = xg;
+O.prototype.visitUnion = Lg;
+O.prototype.visitDenseUnion = yh;
+O.prototype.visitSparseUnion = bh;
+O.prototype.visitDictionary = Dg;
+O.prototype.visitInterval = kg;
+O.prototype.visitIntervalDayTime = mh;
+O.prototype.visitIntervalYearMonth = gh;
+O.prototype.visitFixedSizeList = Eg;
+O.prototype.visitMap = Fg;
 const ks = new O;
 class F extends V {}
 
-function Eg(e, t) {
+function Ug(e, t) {
     return t === null && e.length > 0 ? 0 : -1
 }
 
-function Ug(e, t) {
+function Ng(e, t) {
     const {
         nullBitmap: n
     } = e;
     if (!n || e.nullCount <= 0) return -1;
     let r = 0;
-    for (const s of Gr(n, e.data.offset + (t || 0), e.length, n, da)) {
+    for (const s of Gr(n, e.data.offset + (t || 0), e.length, n, la)) {
         if (!s) return r;
         ++r
     }
     return -1
 }
 
 function C(e, t, n) {
     if (t === void 0) return -1;
-    if (t === null) return Ug(e, n);
-    const r = In(t);
+    if (t === null) return Ng(e, n);
+    const r = Tn(t);
     for (let s = (n || 0) - 1, o = e.length; ++s < o;)
         if (r(e.get(s))) return s;
     return -1
 }
 
-function mh(e, t, n) {
-    const r = In(t);
+function vh(e, t, n) {
+    const r = Tn(t);
     for (let s = (n || 0) - 1, o = e.length; ++s < o;)
         if (r(e.get(s))) return s;
     return -1
 }
-F.prototype.visitNull = Eg;
+F.prototype.visitNull = Ug;
 F.prototype.visitBool = C;
 F.prototype.visitInt = C;
 F.prototype.visitInt8 = C;
 F.prototype.visitInt16 = C;
 F.prototype.visitInt32 = C;
 F.prototype.visitInt64 = C;
 F.prototype.visitUint8 = C;
@@ -8952,32 +8952,32 @@
 F.prototype.visitTimeMillisecond = C;
 F.prototype.visitTimeMicrosecond = C;
 F.prototype.visitTimeNanosecond = C;
 F.prototype.visitDecimal = C;
 F.prototype.visitList = C;
 F.prototype.visitStruct = C;
 F.prototype.visitUnion = C;
-F.prototype.visitDenseUnion = mh;
-F.prototype.visitSparseUnion = mh;
+F.prototype.visitDenseUnion = vh;
+F.prototype.visitSparseUnion = vh;
 F.prototype.visitDictionary = C;
 F.prototype.visitInterval = C;
 F.prototype.visitIntervalDayTime = C;
 F.prototype.visitIntervalYearMonth = C;
 F.prototype.visitFixedSizeList = C;
 F.prototype.visitMap = C;
-const gh = new F;
+const wh = new F;
 class x extends V {}
 
-function Ng(e) {
+function Mg(e) {
     const t = ks.getVisitFn(e);
     return Gr(e.nullBitmap, e.offset, e.length, e, (n, r, s, o) => (s & 1 << o) !== 0 ? t(n, r) : null)
 }
 
 function k(e) {
-    if (e.nullCount > 0) return Ng(e);
+    if (e.nullCount > 0) return Mg(e);
     const {
         type: t,
         typeId: n,
         length: r
     } = e;
     return e.stride === 1 && (n === d.Timestamp || n === d.Int && t.bitWidth !== 64 || n === d.Time && t.bitWidth !== 64 || n === d.Float && t.precision > 0) ? e.values.subarray(0, r)[Symbol.iterator]() : function*(s) {
         for (let o = -1; ++o < r;) yield s(e, o)
@@ -9022,15 +9022,15 @@
 x.prototype.visitSparseUnion = k;
 x.prototype.visitDictionary = k;
 x.prototype.visitInterval = k;
 x.prototype.visitIntervalDayTime = k;
 x.prototype.visitIntervalYearMonth = k;
 x.prototype.visitFixedSizeList = k;
 x.prototype.visitMap = k;
-const Xa = new x;
+const Za = new x;
 class L extends V {}
 
 function E(e) {
     const {
         type: t,
         length: n,
         stride: r
@@ -9039,15 +9039,15 @@
         case d.Int:
         case d.Float:
         case d.Decimal:
         case d.Time:
         case d.Timestamp:
             return e.values.subarray(0, n * r)
     }
-    return [...Xa.visit(e)]
+    return [...Za.visit(e)]
 }
 L.prototype.visitNull = E;
 L.prototype.visitBool = E;
 L.prototype.visitInt = E;
 L.prototype.visitInt8 = E;
 L.prototype.visitInt16 = E;
 L.prototype.visitInt32 = E;
@@ -9084,18 +9084,18 @@
 L.prototype.visitSparseUnion = E;
 L.prototype.visitDictionary = E;
 L.prototype.visitInterval = E;
 L.prototype.visitIntervalDayTime = E;
 L.prototype.visitIntervalYearMonth = E;
 L.prototype.visitFixedSizeList = E;
 L.prototype.visitMap = E;
-const vh = new L,
+const _h = new L,
     br = (e, t) => e + t,
     to = e => `Cannot compute the byte width of variable-width column ${e}`;
-class Mg extends V {
+class Cg extends V {
     visitNull(t) {
         return 0
     }
     visitInt(t) {
         return t.bitWidth / 8
     }
     visitFloat(t) {
@@ -9149,156 +9149,156 @@
     visitFields(t) {
         return (t || []).map(n => this.visit(n.type))
     }
     visitSchema(t) {
         return this.visitFields(t.fields).reduce(br, 0)
     }
 }
-const wh = new Mg;
-class Cg extends V {
+const Sh = new Cg;
+class Rg extends V {
     visitNull() {
-        return Jm
+        return Xm
     }
     visitBool() {
-        return Um
+        return Nm
     }
     visitInt() {
-        return re
+        return ie
     }
     visitInt8() {
-        return Gf
+        return Zf
     }
     visitInt16() {
-        return Kf
+        return Hf
     }
     visitInt32() {
-        return Zf
+        return Jf
     }
     visitInt64() {
-        return Hf
+        return Xf
     }
     visitUint8() {
-        return Jf
+        return qf
     }
     visitUint16() {
-        return Xf
+        return Qf
     }
     visitUint32() {
-        return qf
+        return th
     }
     visitUint64() {
-        return Qf
+        return eh
     }
     visitFloat() {
         return Ls
     }
     visitFloat16() {
-        return Wf
+        return Yf
     }
     visitFloat32() {
-        return $f
+        return Gf
     }
     visitFloat64() {
-        return Yf
+        return Kf
     }
     visitUtf8() {
-        return cg
+        return ug
     }
     visitBinary() {
-        return Em
+        return Um
     }
     visitFixedSizeBinary() {
-        return Rm
+        return Vm
     }
     visitDate() {
-        return Ya
+        return za
     }
     visitDateDay() {
-        return Nm
+        return Mm
     }
     visitDateMillisecond() {
-        return Mm
+        return Cm
     }
     visitTimestamp() {
         return ei
     }
     visitTimestampSecond() {
-        return qm
+        return Qm
     }
     visitTimestampMillisecond() {
-        return Qm
+        return tg
     }
     visitTimestampMicrosecond() {
-        return tg
+        return eg
     }
     visitTimestampNanosecond() {
-        return eg
+        return ng
     }
     visitTime() {
         return ni
     }
     visitTimeSecond() {
-        return ng
+        return rg
     }
     visitTimeMillisecond() {
-        return rg
+        return ig
     }
     visitTimeMicrosecond() {
-        return ig
+        return sg
     }
     visitTimeNanosecond() {
-        return sg
+        return og
     }
     visitDecimal() {
-        return Cm
+        return Rm
     }
     visitList() {
-        return Zm
+        return Hm
     }
     visitStruct() {
         return Ds
     }
     visitUnion() {
-        return Za
+        return Ya
     }
     visitDenseUnion() {
-        return og
+        return ag
     }
     visitSparseUnion() {
-        return ag
+        return cg
     }
     visitDictionary() {
-        return Ga
+        return Wa
     }
     visitInterval() {
-        return Ka
+        return $a
     }
     visitIntervalDayTime() {
-        return Wm
+        return $m
     }
     visitIntervalYearMonth() {
-        return $m
+        return Ym
     }
     visitFixedSizeList() {
-        return Vm
+        return jm
     }
     visitMap() {
-        return Hm
+        return Jm
     }
 }
-const _h = new Cg;
-z.new = Rg;
-z.from = Vg;
+const Ih = new Rg;
+z.new = Vg;
+z.from = jg;
 
-function Rg(e, ...t) {
-    return new(_h.getVisitFn(e)())(e, ...t)
+function Vg(e, ...t) {
+    return new(Ih.getVisitFn(e)())(e, ...t)
 }
 
-function bn(e, t) {
-    if (Xt(t)) return z.from({
+function gn(e, t) {
+    if (qt(t)) return z.from({
         nullValues: [null, void 0],
         type: e(),
         values: t
     });
     if (De(t)) return z.from({
         nullValues: [null, void 0],
         type: e(),
@@ -9307,34 +9307,34 @@
     const {
         values: n = [],
         type: r = e(),
         nullValues: s = [null, void 0]
     } = {
         ...t
     };
-    return Xt(n) ? z.from({
+    return qt(n) ? z.from({
         nullValues: s,
         ...t,
         type: r
     }) : z.from({
         nullValues: s,
         ...t,
         type: r
     })
 }
 
-function Vg(e) {
+function jg(e) {
     const {
         values: t = [],
         ...n
     } = {
         nullValues: [null, void 0],
         ...e
     };
-    if (Xt(t)) {
+    if (qt(t)) {
         const r = [...at.throughIterable(n)(t)];
         return r.length === 1 ? r[0] : mt.concat(r)
     }
     return (async r => {
         const s = at.throughAsyncIterable(n);
         for await (const o of s(t)) r.push(o);
         return r.length === 1 ? r[0] : mt.concat(r)
@@ -9343,72 +9343,72 @@
 tt.prototype.get = function(t) {
     return ks.visit(this, t)
 };
 tt.prototype.set = function(t, n) {
     return Fs.visit(this, t, n)
 };
 tt.prototype.indexOf = function(t, n) {
-    return gh.visit(this, t, n)
+    return wh.visit(this, t, n)
 };
 tt.prototype.toArray = function() {
-    return vh.visit(this)
+    return _h.visit(this)
 };
 tt.prototype.getByteWidth = function() {
-    return wh.visit(this.type)
+    return Sh.visit(this.type)
 };
 tt.prototype[Symbol.iterator] = function() {
-    return Xa.visit(this)
+    return Za.visit(this)
 };
-tt.prototype._bindDataAccessors = Wg;
+tt.prototype._bindDataAccessors = $g;
 Object.keys(d).map(e => d[e]).filter(e => typeof e == "number").filter(e => e !== d.NONE).forEach(e => {
-    const t = _h.visit(e);
-    t.prototype.get = ug(ks.getVisitFn(e)), t.prototype.set = su(Fs.getVisitFn(e)), t.prototype.indexOf = su(gh.getVisitFn(e)), t.prototype.toArray = iu(vh.getVisitFn(e)), t.prototype.getByteWidth = jg(wh.getVisitFn(e)), t.prototype[Symbol.iterator] = iu(Xa.getVisitFn(e))
+    const t = Ih.visit(e);
+    t.prototype.get = lg(ks.getVisitFn(e)), t.prototype.set = au(Fs.getVisitFn(e)), t.prototype.indexOf = au(wh.getVisitFn(e)), t.prototype.toArray = ou(_h.getVisitFn(e)), t.prototype.getByteWidth = Pg(Sh.getVisitFn(e)), t.prototype[Symbol.iterator] = ou(Za.getVisitFn(e))
 });
 
-function jg(e) {
+function Pg(e) {
     return function() {
         return e(this.type)
     }
 }
 
-function Pg(e) {
+function zg(e) {
     return function(t) {
         return this.isValid(t) ? e.call(this, t) : null
     }
 }
 
-function zg(e) {
+function Wg(e) {
     return function(t, n) {
-        Zl(this.nullBitmap, this.offset + t, n != null) && e.call(this, t, n)
+        Jl(this.nullBitmap, this.offset + t, n != null) && e.call(this, t, n)
     }
 }
 
-function Wg() {
+function $g() {
     const e = this.nullBitmap;
-    e && e.byteLength > 0 && (this.get = Pg(this.get), this.set = zg(this.set))
+    e && e.byteLength > 0 && (this.get = zg(this.get), this.set = Wg(this.set))
 }
 class G extends mt {
     constructor(...t) {
         let n = null;
         t[0] instanceof H && (n = t.shift());
-        let r = lf(Ot, t);
+        let r = hf(Ot, t);
         if (!n && !(n = r[0] && r[0].schema)) throw new TypeError("Table must be initialized with a Schema or at least one RecordBatch");
-        r[0] || (r[0] = new Es(n)), super(new Qt(n.fields), r), this._schema = n, this._chunks = r
+        r[0] || (r[0] = new Es(n)), super(new te(n.fields), r), this._schema = n, this._chunks = r
     }
     static empty(t = new H([])) {
         return new G(t, [])
     }
     static from(t) {
         if (!t) return G.empty();
         if (typeof t == "object") {
-            let r = Xt(t.values) ? $g(t) : De(t.values) ? Yg(t) : null;
+            let r = qt(t.values) ? Yg(t) : De(t.values) ? Gg(t) : null;
             if (r !== null) return r
         }
-        let n = Jt.from(t);
-        return Ge(n) ? (async () => await G.from(await n))() : n.isSync() && (n = n.open()) ? n.schema ? new G(n.schema, [...n]) : G.empty() : (async r => {
+        let n = Xt.from(t);
+        return Ke(n) ? (async () => await G.from(await n))() : n.isSync() && (n = n.open()) ? n.schema ? new G(n.schema, [...n]) : G.empty() : (async r => {
             const s = await r,
                 o = s.schema,
                 i = [];
             if (o) {
                 for await (let a of s) i.push(a);
                 return new G(o, i)
             }
@@ -9418,15 +9418,15 @@
     static async fromAsync(t) {
         return await G.from(t)
     }
     static fromStruct(t) {
         return G.new(t.data.childData, t.type.children)
     }
     static new(...t) {
-        return new G(...Lm(sb(t)))
+        return new G(...Dm(ob(t)))
     }
     get schema() {
         return this._schema
     }
     get length() {
         return this._length
     }
@@ -9452,20 +9452,20 @@
         if (t < 0 || t >= this.numChildren) return null;
         let n, r;
         const s = this._schema.fields,
             o = this._children || (this._children = []);
         if (r = o[t]) return r;
         if (n = s[t]) {
             const i = this._chunks.map(a => a.getChildAt(t)).filter(a => a != null);
-            if (i.length > 0) return o[t] = new Kt(n, i)
+            if (i.length > 0) return o[t] = new Zt(n, i)
         }
         return null
     }
     serialize(t = "binary", n = !0) {
-        return (n ? Pa : za).writeAll(this).toUint8Array(!0)
+        return (n ? Ra : Va).writeAll(this).toUint8Array(!0)
     }
     count() {
         return this._length
     }
     select(...t) {
         const n = this._schema.fields.reduce((r, s, o) => r.set(s.name, o), new Map);
         return this.selectAt(...t.map(r => n.get(r)).filter(r => r > -1))
@@ -9486,49 +9486,49 @@
                 return ~h ? f[h] = u : l.push(u), a
             }, [
                 [],
                 []
             ]),
             o = this._schema.assign(t.schema),
             i = [...n.map((a, c, u, l = s[c]) => l === void 0 ? this.getColumnAt(c) : t.getColumnAt(l)), ...r.map(a => t.getColumnAt(a))].filter(Boolean);
-        return new G(...zf(o, i))
+        return new G(...$f(o, i))
     }
 }
 
-function $g(e) {
+function Yg(e) {
     const {
         type: t
     } = e;
-    return t instanceof Qt ? G.fromStruct(Ds.from(e)) : null
+    return t instanceof te ? G.fromStruct(Ds.from(e)) : null
 }
 
-function Yg(e) {
+function Gg(e) {
     const {
         type: t
     } = e;
-    return t instanceof Qt ? Ds.from(e).then(n => G.fromStruct(n)) : null
+    return t instanceof te ? Ds.from(e).then(n => G.fromStruct(n)) : null
 }
 class Ot extends Ds {
     constructor(...t) {
         let n, r = t[0],
             s;
         if (t[1] instanceof S)[, n, s] = t;
         else {
             const o = r.fields,
                 [, i, a] = t;
-            n = S.Struct(new Qt(o), 0, i, 0, null, a)
+            n = S.Struct(new te(o), 0, i, 0, null, a)
         }
         super(n, s), this._schema = r
     }
     static from(t) {
-        return Xt(t.values), G.from(t)
+        return qt(t.values), G.from(t)
     }
     static new(...t) {
-        const [n, r] = ff(t), s = r.filter(o => o instanceof z);
-        return new Ot(...xm(new H(n), s.map(o => o.data)))
+        const [n, r] = df(t), s = r.filter(o => o instanceof z);
+        return new Ot(...Lm(new H(n), s.map(o => o.data)))
     }
     clone(t, n = this._children) {
         return new Ot(this._schema, t, n)
     }
     concat(...t) {
         const n = this._schema,
             r = mt.flatten(this, ...t);
@@ -9539,15 +9539,15 @@
     get schema() {
         return this._schema
     }
     get numCols() {
         return this._schema.fields.length
     }
     get dictionaries() {
-        return this._dictionaries || (this._dictionaries = qa.collect(this))
+        return this._dictionaries || (this._dictionaries = Ha.collect(this))
     }
     select(...t) {
         const n = this._schema.fields.reduce((r, s, o) => r.set(s.name, o), new Map);
         return this.selectAt(...t.map(r => n.get(r)).filter(r => r > -1))
     }
     selectAt(...t) {
         const n = this._schema.selectAt(...t),
@@ -9556,30 +9556,30 @@
     }
 }
 class Es extends Ot {
     constructor(t) {
         super(t, 0, t.fields.map(n => S.new(n.type, 0, 0, 0)))
     }
 }
-class qa extends V {
+class Ha extends V {
     constructor() {
         super(...arguments), this.dictionaries = new Map
     }
     static collect(t) {
-        return new qa().visit(t.data, new Qt(t.schema.fields)).dictionaries
+        return new Ha().visit(t.data, new te(t.schema.fields)).dictionaries
     }
     visit(t, n) {
         return U.isDictionary(n) ? this.visitDictionary(t, n) : (t.childData.forEach((r, s) => this.visit(r, n.children[s].type)), this)
     }
     visitDictionary(t, n) {
         const r = t.dictionary;
         return r && r.length > 0 && this.dictionaries.set(n.id, r), this
     }
 }
-class Jt extends _n {
+class Xt extends Sn {
     constructor(t) {
         super(), this._impl = t
     }
     get closed() {
         return this._impl.closed
     }
     get schema() {
@@ -9625,15 +9625,15 @@
         return this._impl.cancel()
     }
     reset(t) {
         return this._impl.reset(t), this._DOMStream = void 0, this._nodeStream = void 0, this
     }
     open(t) {
         const n = this._impl.open(t);
-        return Ge(n) ? n.then(() => this) : this
+        return Ke(n) ? n.then(() => this) : this
     }
     readRecordBatch(t) {
         return this._impl.isFile() ? this._impl.readRecordBatch(t) : null
     } [Symbol.iterator]() {
         return this._impl[Symbol.iterator]()
     } [Symbol.asyncIterator]() {
         return this._impl[Symbol.asyncIterator]()
@@ -9657,50 +9657,50 @@
     static throughNode(t) {
         throw new Error('"throughNode" not available in this environment')
     }
     static throughDOM(t, n) {
         throw new Error('"throughDOM" not available in this environment')
     }
     static from(t) {
-        return t instanceof Jt ? t : Ao(t) ? Hg(t) : Rl(t) ? qg(t) : Ge(t) ? (async () => await Jt.from(await t))() : Vl(t) || fa(t) || jl(t) || De(t) ? Xg(new pn(t)) : Jg(new Ki(t))
+        return t instanceof Xt ? t : Ao(t) ? Jg(t) : jl(t) ? Qg(t) : Ke(t) ? (async () => await Xt.from(await t))() : Pl(t) || ca(t) || zl(t) || De(t) ? qg(new bn(t)) : Xg(new Ki(t))
     }
     static readAll(t) {
-        return t instanceof Jt ? t.isSync() ? ou(t) : au(t) : Ao(t) || ArrayBuffer.isView(t) || Xt(t) || Cl(t) ? ou(t) : au(t)
+        return t instanceof Xt ? t.isSync() ? cu(t) : uu(t) : Ao(t) || ArrayBuffer.isView(t) || qt(t) || Vl(t) ? cu(t) : uu(t)
     }
 }
-class Hi extends Jt {
+class Hi extends Xt {
     constructor(t) {
         super(t), this._impl = t
     } [Symbol.iterator]() {
         return this._impl[Symbol.iterator]()
     }
     async * [Symbol.asyncIterator]() {
         yield* this[Symbol.iterator]()
     }
 }
-class Ji extends Jt {
+class Ji extends Xt {
     constructor(t) {
         super(t), this._impl = t
     } [Symbol.iterator]() {
         throw new Error("AsyncRecordBatchStreamReader is not Iterable")
     } [Symbol.asyncIterator]() {
         return this._impl[Symbol.asyncIterator]()
     }
 }
-class Sh extends Hi {
+class Th extends Hi {
     constructor(t) {
         super(t), this._impl = t
     }
 }
-class Gg extends Ji {
+class Kg extends Ji {
     constructor(t) {
         super(t), this._impl = t
     }
 }
-class Ih {
+class Ah {
     constructor(t = new Map) {
         this.closed = !1, this.autoDestroy = !0, this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.dictionaries = t
     }
     get numDictionaries() {
         return this._dictionaryIndex
     }
     get numRecordBatches() {
@@ -9736,34 +9736,34 @@
         if (s || !c) {
             const u = a.dictionaries.get(r);
             return c && s ? c.concat(z.new(this._loadVectors(o, n, [u])[0])) : z.new(this._loadVectors(o, n, [u])[0])
         }
         return c
     }
     _loadVectors(t, n, r) {
-        return new Df(n, t.nodes, t.buffers, this.dictionaries).visitMany(r)
+        return new Ef(n, t.nodes, t.buffers, this.dictionaries).visitMany(r)
     }
 }
-class Xi extends Ih {
+class Xi extends Ah {
     constructor(t, n) {
-        super(n), this._reader = Ao(t) ? new Am(this._handle = t) : new Rf(this._handle = t)
+        super(n), this._reader = Ao(t) ? new Bm(this._handle = t) : new jf(this._handle = t)
     }
     isSync() {
         return !0
     }
     isStream() {
         return !0
     } [Symbol.iterator]() {
         return this
     }
     cancel() {
         !this.closed && (this.closed = !0) && (this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
     }
     open(t) {
-        return this.closed || (this.autoDestroy = Ah(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
+        return this.closed || (this.autoDestroy = Oh(this, t), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
     }
     throw (t) {
         return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(t) : ot
     }
     return (t) {
         return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.return(t) : ot
     }
@@ -9795,31 +9795,31 @@
             value: new Es(this.schema)
         }) : this.return()
     }
     _readNextMessageAndValidate(t) {
         return this._reader.readMessage(t)
     }
 }
-class qi extends Ih {
+class qi extends Ah {
     constructor(t, n) {
-        super(n), this._reader = new Tm(this._handle = t)
+        super(n), this._reader = new Am(this._handle = t)
     }
     isAsync() {
         return !0
     }
     isStream() {
         return !0
     } [Symbol.asyncIterator]() {
         return this
     }
     async cancel() {
         !this.closed && (this.closed = !0) && (await this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
     }
     async open(t) {
-        return this.closed || (this.autoDestroy = Ah(this, t), this.schema || (this.schema = await this._reader.readSchema()) || await this.cancel()), this
+        return this.closed || (this.autoDestroy = Oh(this, t), this.schema || (this.schema = await this._reader.readSchema()) || await this.cancel()), this
     }
     async throw (t) {
         return !this.closed && this.autoDestroy && (this.closed = !0) ? await this.reset()._reader.throw(t) : ot
     }
     async return (t) {
         return !this.closed && this.autoDestroy && (this.closed = !0) ? await this.reset()._reader.return(t) : ot
     }
@@ -9851,17 +9851,17 @@
             value: new Es(this.schema)
         }) : await this.return()
     }
     async _readNextMessageAndValidate(t) {
         return await this._reader.readMessage(t)
     }
 }
-class Th extends Xi {
+class Bh extends Xi {
     constructor(t, n) {
-        super(t instanceof $c ? t : new $c(t), n)
+        super(t instanceof Gc ? t : new Gc(t), n)
     }
     get footer() {
         return this._footer
     }
     get numDictionaries() {
         return this._footer ? this._footer.numDictionaries : 0
     }
@@ -9906,26 +9906,26 @@
                 this.dictionaries.set(s.id, i)
             }
         }
     }
     _readFooter() {
         const {
             _handle: t
-        } = this, n = t.size - Vf, r = t.readInt32(n), s = t.readAt(n - r, r);
+        } = this, n = t.size - Pf, r = t.readInt32(n), s = t.readAt(n - r, r);
         return Cr.decode(s)
     }
     _readNextMessageAndValidate(t) {
         if (this._footer || this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
             const n = this._footer && this._footer.getRecordBatch(this._recordBatchIndex);
             if (n && this._handle.seek(n.offset)) return this._reader.readMessage(t)
         }
         return null
     }
 }
-class Kg extends qi {
+class Zg extends qi {
     constructor(t, ...n) {
         const r = typeof n[0] != "number" ? n.shift() : void 0,
             s = n[0] instanceof Map ? n.shift() : void 0;
         super(t instanceof Zi ? t : new Zi(t, r), s)
     }
     get footer() {
         return this._footer
@@ -9976,89 +9976,89 @@
         }
     }
     async _readFooter() {
         const {
             _handle: t
         } = this;
         t._pending && await t._pending;
-        const n = t.size - Vf,
+        const n = t.size - Pf,
             r = await t.readInt32(n),
             s = await t.readAt(n - r, r);
         return Cr.decode(s)
     }
     async _readNextMessageAndValidate(t) {
         if (this._footer || await this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
             const n = this._footer.getRecordBatch(this._recordBatchIndex);
             if (n && await this._handle.seek(n.offset)) return await this._reader.readMessage(t)
         }
         return null
     }
 }
-class Zg extends Xi {
+class Hg extends Xi {
     constructor(t, n) {
         super(t, n)
     }
     _loadVectors(t, n, r) {
-        return new Kb(n, t.nodes, t.buffers, this.dictionaries).visitMany(r)
+        return new Zb(n, t.nodes, t.buffers, this.dictionaries).visitMany(r)
     }
 }
 
-function Ah(e, t) {
+function Oh(e, t) {
     return t && typeof t.autoDestroy == "boolean" ? t.autoDestroy : e.autoDestroy
 }
 
-function* ou(e) {
-    const t = Jt.from(e);
+function* cu(e) {
+    const t = Xt.from(e);
     try {
         if (!t.open({
                 autoDestroy: !1
             }).closed)
             do yield t; while (!t.reset().open().closed)
     } finally {
         t.cancel()
     }
 }
-async function* au(e) {
-    const t = await Jt.from(e);
+async function* uu(e) {
+    const t = await Xt.from(e);
     try {
         if (!(await t.open({
                 autoDestroy: !1
             })).closed)
             do yield t; while (!(await t.reset().open()).closed)
     } finally {
         await t.cancel()
     }
 }
 
-function Hg(e) {
-    return new Hi(new Zg(e))
+function Jg(e) {
+    return new Hi(new Hg(e))
 }
 
-function Jg(e) {
+function Xg(e) {
     const t = e.peek(ti + 7 & -8);
-    return t && t.byteLength >= 4 ? Ra(t) ? new Sh(new Th(e.read())) : new Hi(new Xi(e)) : new Hi(new Xi(function*() {}()))
+    return t && t.byteLength >= 4 ? Na(t) ? new Th(new Bh(e.read())) : new Hi(new Xi(e)) : new Hi(new Xi(function*() {}()))
 }
-async function Xg(e) {
+async function qg(e) {
     const t = await e.peek(ti + 7 & -8);
-    return t && t.byteLength >= 4 ? Ra(t) ? new Sh(new Th(await e.read())) : new Ji(new qi(e)) : new Ji(new qi(async function*() {}()))
+    return t && t.byteLength >= 4 ? Na(t) ? new Th(new Bh(await e.read())) : new Ji(new qi(e)) : new Ji(new qi(async function*() {}()))
 }
-async function qg(e) {
+async function Qg(e) {
     const {
         size: t
     } = await e.stat(), n = new Zi(e, t);
-    return t >= Bm && Ra(await n.readAt(0, ti + 7 & -8)) ? new Gg(new Kg(n)) : new Ji(new qi(n))
+    return t >= Om && Na(await n.readAt(0, ti + 7 & -8)) ? new Kg(new Zg(n)) : new Ji(new qi(n))
 }
 
-function Qg(e, t) {
-    if (De(e)) return e0(e, t);
-    if (Xt(e)) return t0(e, t);
+function t0(e, t) {
+    if (De(e)) return n0(e, t);
+    if (qt(e)) return e0(e, t);
     throw new Error("toDOMStream() must be called with an Iterable or AsyncIterable")
 }
 
-function t0(e, t) {
+function e0(e, t) {
     let n = null;
     const r = t && t.type === "bytes" || !1,
         s = t && t.highWaterMark || 2 ** 24;
     return new ReadableStream({
         ...t,
         start(i) {
             o(i, n || (n = e[Symbol.iterator]()))
@@ -10079,15 +10079,15 @@
             l = i.desiredSize || null;
         for (; !(u = a.next(r ? l : null)).done;)
             if (ArrayBuffer.isView(u.value) && (c = j(u.value)) && (l != null && r && (l = l - c.byteLength + 1), u.value = c), i.enqueue(u.value), l != null && --l <= 0) return;
         i.close()
     }
 }
 
-function e0(e, t) {
+function n0(e, t) {
     let n = null;
     const r = t && t.type === "bytes" || !1,
         s = t && t.highWaterMark || 2 ** 24;
     return new ReadableStream({
         ...t,
         async start(i) {
             await o(i, n || (n = e[Symbol.asyncIterator]()))
@@ -10107,24 +10107,24 @@
             l = i.desiredSize || null;
         for (; !(u = await a.next(r ? l : null)).done;)
             if (ArrayBuffer.isView(u.value) && (c = j(u.value)) && (l != null && r && (l = l - c.byteLength + 1), u.value = c), i.enqueue(u.value), l != null && --l <= 0) return;
         i.close()
     }
 }
 
-function n0(e) {
-    return new r0(e)
+function r0(e) {
+    return new i0(e)
 }
-class r0 {
+class i0 {
     constructor(t) {
         this._numChunks = 0, this._finished = !1, this._bufferedSize = 0;
         const {
             ["readableStrategy"]: n, ["writableStrategy"]: r, ["queueingStrategy"]: s = "count", ...o
         } = t;
-        this._controller = null, this._builder = at.new(o), this._getSize = s !== "bytes" ? cu : uu;
+        this._controller = null, this._builder = at.new(o), this._getSize = s !== "bytes" ? lu : fu;
         const {
             ["highWaterMark"]: i = s === "bytes" ? 2 ** 14 : 1e3
         } = {
             ...n
         }, {
             ["highWaterMark"]: a = s === "bytes" ? 2 ** 14 : 1e3
         } = {
@@ -10138,15 +10138,15 @@
                 this._maybeFlush(this._builder, this._controller = c)
             },
             start: c => {
                 this._maybeFlush(this._builder, this._controller = c)
             }
         }, {
             highWaterMark: i,
-            size: s !== "bytes" ? cu : uu
+            size: s !== "bytes" ? lu : fu
         }), this.writable = new WritableStream({
             abort: () => {
                 this._builder.clear()
             },
             write: () => {
                 this._maybeFlush(this._builder, this._controller)
             },
@@ -10165,18 +10165,18 @@
     _maybeFlush(t, n) {
         n !== null && (this._bufferedSize >= n.desiredSize && ++this._numChunks && this._enqueue(n, t.toVector()), t.finished && ((t.length > 0 || this._numChunks === 0) && ++this._numChunks && this._enqueue(n, t.toVector()), !this._finished && (this._finished = !0) && this._enqueue(n, null)))
     }
     _enqueue(t, n) {
         this._bufferedSize = 0, this._controller = null, n === null ? t.close() : t.enqueue(n)
     }
 }
-const cu = e => e.length,
-    uu = e => e.byteLength;
+const lu = e => e.length,
+    fu = e => e.byteLength;
 
-function i0(e, t) {
+function s0(e, t) {
     const n = new Tr;
     let r = null;
     const s = new ReadableStream({
         async cancel() {
             await n.close()
         },
         async start(a) {
@@ -10190,28 +10190,28 @@
         writable: new WritableStream(n, {
             highWaterMark: 2 ** 14,
             ...e
         }),
         readable: s
     };
     async function o() {
-        return await (await Jt.from(n)).open(t)
+        return await (await Xt.from(n)).open(t)
     }
     async function i(a, c) {
         let u = a.desiredSize,
             l = null;
         for (; !(l = await c.next()).done;)
             if (a.enqueue(l.value), u != null && --u <= 0) return;
         a.close()
     }
 }
 
-function s0(e, t) {
+function o0(e, t) {
     const n = new this(e),
-        r = new pn(n),
+        r = new bn(n),
         s = new ReadableStream({
             type: "bytes",
             async cancel() {
                 await r.cancel()
             },
             async pull(i) {
                 await o(i)
@@ -10233,21 +10233,21 @@
         for (; a = await r.read(c || null);)
             if (i.enqueue(a), c != null && (c -= a.byteLength) <= 0) return;
         i.close()
     }
 }
 class $n {
     eq(t) {
-        return t instanceof $n || (t = new Yn(t)), new o0(this, t)
+        return t instanceof $n || (t = new Yn(t)), new a0(this, t)
     }
     le(t) {
-        return t instanceof $n || (t = new Yn(t)), new a0(this, t)
+        return t instanceof $n || (t = new Yn(t)), new c0(this, t)
     }
     ge(t) {
-        return t instanceof $n || (t = new Yn(t)), new c0(this, t)
+        return t instanceof $n || (t = new Yn(t)), new u0(this, t)
     }
     lt(t) {
         return new xi(this.ge(t))
     }
     gt(t) {
         return new xi(this.le(t))
     }
@@ -10256,15 +10256,15 @@
     }
 }
 class Yn extends $n {
     constructor(t) {
         super(), this.v = t
     }
 }
-class Bh extends $n {
+class Fh extends $n {
     constructor(t) {
         super(), this.name = t
     }
     bind(t) {
         if (!this.colidx) {
             this.colidx = -1;
             const r = t.schema.fields;
@@ -10274,80 +10274,80 @@
                     break
                 } if (this.colidx < 0) throw new Error(`Failed to bind Col "${this.name}"`)
         }
         const n = this.vector = t.getChildAt(this.colidx);
         return r => n.get(r)
     }
 }
-class Qa {
+class Ja {
     and(...t) {
-        return new nc(this, ...t)
+        return new Qa(this, ...t)
     }
     or(...t) {
-        return new rc(this, ...t)
+        return new tc(this, ...t)
     }
     not() {
         return new xi(this)
     }
 }
-class tc extends Qa {
+class Xa extends Ja {
     constructor(t, n) {
         super(), this.left = t, this.right = n
     }
     bind(t) {
         return this.left instanceof Yn ? this.right instanceof Yn ? this._bindLitLit(t, this.left, this.right) : this._bindLitCol(t, this.left, this.right) : this.right instanceof Yn ? this._bindColLit(t, this.left, this.right) : this._bindColCol(t, this.left, this.right)
     }
 }
-class ec extends Qa {
+class qa extends Ja {
     constructor(...t) {
         super(), this.children = t
     }
 }
-ec.prototype.children = Object.freeze([]);
-class nc extends ec {
+qa.prototype.children = Object.freeze([]);
+class Qa extends qa {
     constructor(...t) {
-        t = t.reduce((n, r) => n.concat(r instanceof nc ? r.children : r), []), super(...t)
+        t = t.reduce((n, r) => n.concat(r instanceof Qa ? r.children : r), []), super(...t)
     }
     bind(t) {
         const n = this.children.map(r => r.bind(t));
         return (r, s) => n.every(o => o(r, s))
     }
 }
-class rc extends ec {
+class tc extends qa {
     constructor(...t) {
-        t = t.reduce((n, r) => n.concat(r instanceof rc ? r.children : r), []), super(...t)
+        t = t.reduce((n, r) => n.concat(r instanceof tc ? r.children : r), []), super(...t)
     }
     bind(t) {
         const n = this.children.map(r => r.bind(t));
         return (r, s) => n.some(o => o(r, s))
     }
 }
-class o0 extends tc {
+class a0 extends Xa {
     _bindLitLit(t, n, r) {
         const s = n.v == r.v;
         return () => s
     }
     _bindColCol(t, n, r) {
         const s = n.bind(t),
             o = r.bind(t);
         return (i, a) => s(i, a) == o(i, a)
     }
     _bindColLit(t, n, r) {
         const s = n.bind(t);
-        if (n.vector instanceof Ga) {
+        if (n.vector instanceof Wa) {
             let o;
             const i = n.vector;
             return i.dictionary !== this.lastDictionary ? (o = i.reverseLookup(r.v), this.lastDictionary = i.dictionary, this.lastKey = o) : o = this.lastKey, o === -1 ? () => !1 : a => i.getKey(a) === o
         } else return (o, i) => s(o, i) == r.v
     }
     _bindLitCol(t, n, r) {
         return this._bindColLit(t, r, n)
     }
 }
-class a0 extends tc {
+class c0 extends Xa {
     _bindLitLit(t, n, r) {
         const s = n.v <= r.v;
         return () => s
     }
     _bindColCol(t, n, r) {
         const s = n.bind(t),
             o = r.bind(t);
@@ -10358,15 +10358,15 @@
         return (o, i) => s(o, i) <= r.v
     }
     _bindLitCol(t, n, r) {
         const s = r.bind(t);
         return (o, i) => n.v <= s(o, i)
     }
 }
-class c0 extends tc {
+class u0 extends Xa {
     _bindLitLit(t, n, r) {
         const s = n.v >= r.v;
         return () => s
     }
     _bindColCol(t, n, r) {
         const s = n.bind(t),
             o = r.bind(t);
@@ -10377,15 +10377,15 @@
         return (o, i) => s(o, i) >= r.v
     }
     _bindLitCol(t, n, r) {
         const s = r.bind(t);
         return (o, i) => n.v >= s(o, i)
     }
 }
-class xi extends Qa {
+class xi extends Ja {
     constructor(t) {
         super(), this.child = t
     }
     bind(t) {
         const n = this.child.bind(t);
         return (r, s) => !n(r, s)
     }
@@ -10400,15 +10400,15 @@
     return new ri(this.chunks).scanReverse(e, t)
 };
 G.prototype.filter = function(e) {
     return new ri(this.chunks).filter(e)
 };
 class ri extends G {
     filter(t) {
-        return new ic(this.chunks, t)
+        return new ec(this.chunks, t)
     }
     scan(t, n) {
         const r = this.chunks,
             s = r.length;
         for (let o = -1; ++o < s;) {
             const i = r[o];
             n && n(i);
@@ -10423,15 +10423,15 @@
             n && n(i);
             for (let a = i.length; --a >= 0;) t(a, i)
         }
     }
     countBy(t) {
         const n = this.chunks,
             r = n.length,
-            s = typeof t == "string" ? new Bh(t) : t;
+            s = typeof t == "string" ? new Fh(t) : t;
         s.bind(n[r - 1]);
         const o = s.vector;
         if (!U.isDictionary(o.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
         const i = Math.ceil(Math.log(o.length) / Math.log(256)),
             a = i == 4 ? Uint32Array : i >= 2 ? Uint16Array : Uint8Array,
             c = new a(o.dictionary.length);
         for (let u = -1; ++u < r;) {
@@ -10439,31 +10439,31 @@
             s.bind(l);
             const f = s.vector.indices;
             for (let h = -1, p = l.length; ++h < p;) {
                 let w = f.get(h);
                 w !== null && c[w]++
             }
         }
-        return new Oh(o.dictionary, re.from(c))
+        return new xh(o.dictionary, ie.from(c))
     }
 }
-class Oh extends G {
+class xh extends G {
     constructor(t, n) {
         const r = new H([new W("values", t.type), new W("counts", n.type)]);
         super(new Ot(r, n.length, [t, n]))
     }
     toJSON() {
         const t = this.getColumnAt(0),
             n = this.getColumnAt(1),
             r = {};
         for (let s = -1; ++s < this.length;) r[t.get(s)] = n.get(s);
         return r
     }
 }
-class ic extends ri {
+class ec extends ri {
     constructor(t, n) {
         super(t), this._predicate = n
     }
     scan(t, n) {
         const r = this._chunks,
             s = r.length;
         for (let o = -1; ++o < s;) {
@@ -10499,20 +10499,20 @@
         for (let r = -1; ++r < n;) {
             const s = t[r],
                 o = this._predicate.bind(s);
             for (let i = -1, a = s.length; ++i < a;) o(i, s) && (yield s.get(i))
         }
     }
     filter(t) {
-        return new ic(this._chunks, this._predicate.and(t))
+        return new ec(this._chunks, this._predicate.and(t))
     }
     countBy(t) {
         const n = this._chunks,
             r = n.length,
-            s = typeof t == "string" ? new Bh(t) : t;
+            s = typeof t == "string" ? new Fh(t) : t;
         s.bind(n[r - 1]);
         const o = s.vector;
         if (!U.isDictionary(o.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
         const i = Math.ceil(Math.log(o.length) / Math.log(256)),
             a = i == 4 ? Uint32Array : i >= 2 ? Uint16Array : Uint8Array,
             c = new a(o.dictionary.length);
         for (let u = -1; ++u < r;) {
@@ -10521,28 +10521,28 @@
             s.bind(l);
             const h = s.vector.indices;
             for (let p = -1, w = l.length; ++p < w;) {
                 let _ = h.get(p);
                 _ !== null && f(p, l) && c[_]++
             }
         }
-        return new Oh(o.dictionary, re.from(c))
+        return new xh(o.dictionary, ie.from(c))
     }
 }({
-    ...Oy,
-    ...Gb,
-    ...Qp,
-    ...Iy,
-    ...Kp,
-    ...eb
+    ...Fy,
+    ...Kb,
+    ...ty,
+    ...Ty,
+    ...Zp,
+    ...nb
 });
-Ut.toDOMStream = Qg;
-at.throughDOM = n0;
-Jt.throughDOM = i0;
-ja.throughDOM = s0;
+Ut.toDOMStream = t0;
+at.throughDOM = r0;
+Xt.throughDOM = s0;
+Ca.throughDOM = o0;
 /**
  * @license
  * Copyright 2018-2021 Streamlit Inc.
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
@@ -10551,15 +10551,15 @@
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
-var lu = function() {
+var hu = function() {
     function e(t, n, r, s) {
         var o = this;
         this.getCell = function(i, a) {
             var c = i < o.headerRows && a < o.headerColumns,
                 u = i >= o.headerRows && a < o.headerColumns,
                 l = i < o.headerRows && a >= o.headerColumns;
             if (c) {
@@ -10724,27 +10724,27 @@
             return e
         }, Ar.apply(this, arguments)
     },
     Br;
 (function(e) {
     e.COMPONENT_READY = "streamlit:componentReady", e.SET_COMPONENT_VALUE = "streamlit:setComponentValue", e.SET_FRAME_HEIGHT = "streamlit:setFrameHeight"
 })(Br || (Br = {}));
-var mn = function() {
+var Je = function() {
         function e() {}
-        return e.API_VERSION = 1, e.RENDER_EVENT = "streamlit:render", e.events = new Ye, e.registeredMessageListener = !1, e.setComponentReady = function() {
+        return e.API_VERSION = 1, e.RENDER_EVENT = "streamlit:render", e.events = new Ge, e.registeredMessageListener = !1, e.setComponentReady = function() {
             e.registeredMessageListener || (window.addEventListener("message", e.onMessageEvent), e.registeredMessageListener = !0), e.sendBackMsg(Br.COMPONENT_READY, {
                 apiVersion: e.API_VERSION
             })
         }, e.setFrameHeight = function(t) {
             t === void 0 && (t = document.body.scrollHeight), t !== e.lastFrameHeight && (e.lastFrameHeight = t, e.sendBackMsg(Br.SET_FRAME_HEIGHT, {
                 height: t
             }))
         }, e.setComponentValue = function(t) {
             var n;
-            t instanceof lu ? (n = "dataframe", t = t.serialize()) : l0(t) ? (n = "bytes", t = new Uint8Array(t.buffer)) : t instanceof ArrayBuffer ? (n = "bytes", t = new Uint8Array(t)) : n = "json", e.sendBackMsg(Br.SET_COMPONENT_VALUE, {
+            t instanceof hu ? (n = "dataframe", t = t.serialize()) : f0(t) ? (n = "bytes", t = new Uint8Array(t.buffer)) : t instanceof ArrayBuffer ? (n = "bytes", t = new Uint8Array(t)) : n = "json", e.sendBackMsg(Br.SET_COMPONENT_VALUE, {
                 value: t,
                 dataType: n
             })
         }, e.onMessageEvent = function(t) {
             var n = t.data.type;
             switch (n) {
                 case e.RENDER_EVENT:
@@ -10754,15 +10754,15 @@
         }, e.onRenderMessage = function(t) {
             var n = t.args;
             n == null && (console.error("Got null args in onRenderMessage. This should never happen"), n = {});
             var r = t.dfs && t.dfs.length > 0 ? e.argsDataframeToObject(t.dfs) : {};
             n = Ar(Ar({}, n), r);
             var s = Boolean(t.disabled),
                 o = t.theme;
-            o && u0(o);
+            o && l0(o);
             var i = {
                     disabled: s,
                     args: n,
                     theme: o
                 },
                 a = new CustomEvent(e.RENDER_EVENT, {
                     detail: i
@@ -10777,23 +10777,23 @@
             return Object.fromEntries(n)
         }, e.toArrowTable = function(t) {
             var n = t.data,
                 r = n.data,
                 s = n.index,
                 o = n.columns,
                 i = n.styler;
-            return new lu(r, s, o, i)
+            return new hu(r, s, o, i)
         }, e.sendBackMsg = function(t, n) {
             window.parent.postMessage(Ar({
                 isStreamlitMessage: !0,
                 type: t
             }, n), "*")
         }, e
     }(),
-    u0 = function(e) {
+    l0 = function(e) {
         var t = document.createElement("style");
         document.head.appendChild(t), t.innerHTML = `
     :root {
       --primary-color: ` + e.primaryColor + `;
       --background-color: ` + e.backgroundColor + `;
       --secondary-background-color: ` + e.secondaryBackgroundColor + `;
       --text-color: ` + e.textColor + `;
@@ -10803,15 +10803,15 @@
     body {
       background-color: var(--background-color);
       color: var(--text-color);
     }
   `
     };
 
-function l0(e) {
+function f0(e) {
     var t = !1;
     try {
         t = e instanceof BigInt64Array || e instanceof BigUint64Array
     } catch {}
     return e instanceof Int8Array || e instanceof Uint8Array || e instanceof Uint8ClampedArray || e instanceof Int16Array || e instanceof Uint16Array || e instanceof Int32Array || e instanceof Uint32Array || e instanceof Float32Array || e instanceof Float64Array || t
 }
 /**
@@ -10826,15 +10826,15 @@
  *
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
-var f0 = globalThis && globalThis.__extends || function() {
+var h0 = globalThis && globalThis.__extends || function() {
     var e = function(t, n) {
         return e = Object.setPrototypeOf || {
             __proto__: []
         }
         instanceof Array && function(r, s) {
             r.__proto__ = s
         } || function(r, s) {
@@ -10847,37 +10847,37 @@
         function r() {
             this.constructor = t
         }
         t.prototype = n === null ? Object.create(n) : (r.prototype = n.prototype, new r)
     }
 }();
 (function(e) {
-    f0(t, e);
+    h0(t, e);
 
     function t() {
         return e !== null && e.apply(this, arguments) || this
     }
     return t.prototype.componentDidMount = function() {
-        mn.setFrameHeight()
+        Je.setFrameHeight()
     }, t.prototype.componentDidUpdate = function() {
-        mn.setFrameHeight()
+        Je.setFrameHeight()
     }, t
-})(ip.PureComponent);
+})(sp.PureComponent);
 var ko = function(e, t) {
     return ko = Object.setPrototypeOf || {
         __proto__: []
     }
     instanceof Array && function(n, r) {
         n.__proto__ = r
     } || function(n, r) {
         for (var s in r) Object.prototype.hasOwnProperty.call(r, s) && (n[s] = r[s])
     }, ko(e, t)
 };
 
-function An(e, t) {
+function Bn(e, t) {
     if (typeof t != "function" && t !== null) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
     function n() {
         this.constructor = e
     }
     ko(e, t), e.prototype = t === null ? Object.create(t) : (n.prototype = t.prototype, new n)
 }
@@ -11026,29 +11026,29 @@
 }
 
 function Eo(e, t, n) {
     if (n || arguments.length === 2)
         for (var r, s = 0, o = t.length; s < o; s++) !r && s in t || (r || (r = Array.prototype.slice.call(t, 0, s)), r[s] = t[s]);
     return e.concat(r || Array.prototype.slice.call(t))
 }
-var ce = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+var ue = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-function sc(e) {
+function nc(e) {
     return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e
 }
 
 function lr(e, t) {
     return e(t = {
         exports: {}
     }, t.exports), t.exports
 }
 var Ne, Li, bi = function(e) {
         return e && e.Math == Math && e
     },
-    M = bi(typeof globalThis == "object" && globalThis) || bi(typeof window == "object" && window) || bi(typeof self == "object" && self) || bi(typeof ce == "object" && ce) || function() {
+    M = bi(typeof globalThis == "object" && globalThis) || bi(typeof window == "object" && window) || bi(typeof self == "object" && self) || bi(typeof ue == "object" && ue) || function() {
         return this
     }() || Function("return this")(),
     nt = function(e) {
         try {
             return !!e()
         } catch {
             return !0
@@ -11065,309 +11065,309 @@
         var e = function() {}.bind();
         return typeof e != "function" || e.hasOwnProperty("prototype")
     }),
     mi = Function.prototype.call,
     St = ii ? mi.bind(mi) : function() {
         return mi.apply(mi, arguments)
     },
-    fu = {}.propertyIsEnumerable,
-    hu = Object.getOwnPropertyDescriptor,
-    h0 = hu && !fu.call({
+    du = {}.propertyIsEnumerable,
+    pu = Object.getOwnPropertyDescriptor,
+    d0 = pu && !du.call({
         1: 2
     }, 1) ? function(e) {
-        var t = hu(this, e);
+        var t = pu(this, e);
         return !!t && t.enumerable
-    } : fu,
-    oc = {
-        f: h0
+    } : du,
+    rc = {
+        f: d0
     },
-    gn = function(e, t) {
+    vn = function(e, t) {
         return {
             enumerable: !(1 & e),
             configurable: !(2 & e),
             writable: !(4 & e),
             value: t
         }
     },
-    Fh = Function.prototype,
-    d0 = Fh.bind,
-    Uo = Fh.call,
-    p0 = ii && d0.bind(Uo, Uo),
+    Lh = Function.prototype,
+    p0 = Lh.bind,
+    Uo = Lh.call,
+    y0 = ii && p0.bind(Uo, Uo),
     P = ii ? function(e) {
-        return e && p0(e)
+        return e && y0(e)
     } : function(e) {
         return e && function() {
             return Uo.apply(e, arguments)
         }
     },
-    y0 = P({}.toString),
-    b0 = P("".slice),
+    b0 = P({}.toString),
+    m0 = P("".slice),
     Te = function(e) {
-        return b0(y0(e), 8, -1)
+        return m0(b0(e), 8, -1)
     },
     eo = Object,
-    m0 = P("".split),
-    xh = nt(function() {
+    g0 = P("".split),
+    Dh = nt(function() {
         return !eo("z").propertyIsEnumerable(0)
     }) ? function(e) {
-        return Te(e) == "String" ? m0(e, "") : eo(e)
+        return Te(e) == "String" ? g0(e, "") : eo(e)
     } : eo,
-    g0 = TypeError,
+    v0 = TypeError,
     si = function(e) {
-        if (e == null) throw g0("Can't call method on " + e);
+        if (e == null) throw v0("Can't call method on " + e);
         return e
     },
     be = function(e) {
-        return xh(si(e))
+        return Dh(si(e))
     },
     rt = function(e) {
         return typeof e == "function"
     },
     st = function(e) {
         return typeof e == "object" ? e !== null : rt(e)
     },
-    v0 = function(e) {
+    w0 = function(e) {
         return rt(e) ? e : void 0
     },
-    ie = function(e, t) {
-        return arguments.length < 2 ? v0(M[e]) : M[e] && M[e][t]
+    se = function(e, t) {
+        return arguments.length < 2 ? w0(M[e]) : M[e] && M[e][t]
     },
-    vn = P({}.isPrototypeOf),
-    no = ie("navigator", "userAgent") || "",
-    du = M.process,
-    pu = M.Deno,
-    yu = du && du.versions || pu && pu.version,
-    bu = yu && yu.v8;
-bu && (Li = (Ne = bu.split("."))[0] > 0 && Ne[0] < 4 ? 1 : +(Ne[0] + Ne[1])), !Li && no && (!(Ne = no.match(/Edge\/(\d+)/)) || Ne[1] >= 74) && (Ne = no.match(/Chrome\/(\d+)/)) && (Li = +Ne[1]);
+    wn = P({}.isPrototypeOf),
+    no = se("navigator", "userAgent") || "",
+    yu = M.process,
+    bu = M.Deno,
+    mu = yu && yu.versions || bu && bu.version,
+    gu = mu && mu.v8;
+gu && (Li = (Ne = gu.split("."))[0] > 0 && Ne[0] < 4 ? 1 : +(Ne[0] + Ne[1])), !Li && no && (!(Ne = no.match(/Edge\/(\d+)/)) || Ne[1] >= 74) && (Ne = no.match(/Chrome\/(\d+)/)) && (Li = +Ne[1]);
 var Qi = Li,
-    Vt = !!Object.getOwnPropertySymbols && !nt(function() {
+    jt = !!Object.getOwnPropertySymbols && !nt(function() {
         var e = Symbol();
         return !String(e) || !(Object(e) instanceof Symbol) || !Symbol.sham && Qi && Qi < 41
     }),
-    ac = Vt && !Symbol.sham && typeof Symbol.iterator == "symbol",
-    w0 = Object,
-    sr = ac ? function(e) {
+    ic = jt && !Symbol.sham && typeof Symbol.iterator == "symbol",
+    _0 = Object,
+    sr = ic ? function(e) {
         return typeof e == "symbol"
     } : function(e) {
-        var t = ie("Symbol");
-        return rt(t) && vn(t.prototype, w0(e))
+        var t = se("Symbol");
+        return rt(t) && wn(t.prototype, _0(e))
     },
-    _0 = String,
+    S0 = String,
     fr = function(e) {
         try {
-            return _0(e)
+            return S0(e)
         } catch {
             return "Object"
         }
     },
-    S0 = TypeError,
-    cc = function(e) {
+    I0 = TypeError,
+    sc = function(e) {
         if (rt(e)) return e;
-        throw S0(fr(e) + " is not a function")
+        throw I0(fr(e) + " is not a function")
     },
     ts = function(e, t) {
         var n = e[t];
-        return n == null ? void 0 : cc(n)
+        return n == null ? void 0 : sc(n)
     },
-    I0 = TypeError,
-    T0 = Object.defineProperty,
-    uc = function(e, t) {
+    T0 = TypeError,
+    A0 = Object.defineProperty,
+    oc = function(e, t) {
         try {
-            T0(M, e, {
+            A0(M, e, {
                 value: t,
                 configurable: !0,
                 writable: !0
             })
         } catch {
             M[e] = t
         }
         return t
     },
-    We = M["__core-js_shared__"] || uc("__core-js_shared__", {}),
-    Qe = lr(function(e) {
+    $e = M["__core-js_shared__"] || oc("__core-js_shared__", {}),
+    en = lr(function(e) {
         (e.exports = function(t, n) {
-            return We[t] || (We[t] = n !== void 0 ? n : {})
+            return $e[t] || ($e[t] = n !== void 0 ? n : {})
         })("versions", []).push({
             version: "3.24.0",
             mode: "global",
             copyright: "\xA9 2014-2022 Denis Pushkarev (zloirock.ru)",
             license: "https://github.com/zloirock/core-js/blob/v3.24.0/LICENSE",
             source: "https://github.com/zloirock/core-js"
         })
     }),
-    A0 = Object,
+    B0 = Object,
     hr = function(e) {
-        return A0(si(e))
+        return B0(si(e))
     },
-    B0 = P({}.hasOwnProperty),
+    O0 = P({}.hasOwnProperty),
     A = Object.hasOwn || function(e, t) {
-        return B0(hr(e), t)
+        return O0(hr(e), t)
     },
-    O0 = 0,
-    F0 = Math.random(),
-    x0 = P(1 .toString),
+    F0 = 0,
+    x0 = Math.random(),
+    L0 = P(1 .toString),
     or = function(e) {
-        return "Symbol(" + (e === void 0 ? "" : e) + ")_" + x0(++O0 + F0, 36)
+        return "Symbol(" + (e === void 0 ? "" : e) + ")_" + L0(++F0 + x0, 36)
     },
-    mr = Qe("wks"),
-    ln = M.Symbol,
-    mu = ln && ln.for,
-    L0 = ac ? ln : ln && ln.withoutSetter || or,
+    mr = en("wks"),
+    hn = M.Symbol,
+    vu = hn && hn.for,
+    D0 = ic ? hn : hn && hn.withoutSetter || or,
     ut = function(e) {
-        if (!A(mr, e) || !Vt && typeof mr[e] != "string") {
+        if (!A(mr, e) || !jt && typeof mr[e] != "string") {
             var t = "Symbol." + e;
-            Vt && A(ln, e) ? mr[e] = ln[e] : mr[e] = ac && mu ? mu(t) : L0(t)
+            jt && A(hn, e) ? mr[e] = hn[e] : mr[e] = ic && vu ? vu(t) : D0(t)
         }
         return mr[e]
     },
-    D0 = TypeError,
-    k0 = ut("toPrimitive"),
-    E0 = function(e, t) {
+    k0 = TypeError,
+    E0 = ut("toPrimitive"),
+    U0 = function(e, t) {
         if (!st(e) || sr(e)) return e;
-        var n, r = ts(e, k0);
+        var n, r = ts(e, E0);
         if (r) {
             if (t === void 0 && (t = "default"), n = St(r, e, t), !st(n) || sr(n)) return n;
-            throw D0("Can't convert object to primitive value")
+            throw k0("Can't convert object to primitive value")
         }
         return t === void 0 && (t = "number"),
             function(s, o) {
                 var i, a;
                 if (o === "string" && rt(i = s.toString) && !st(a = St(i, s)) || rt(i = s.valueOf) && !st(a = St(i, s)) || o !== "string" && rt(i = s.toString) && !st(a = St(i, s))) return a;
-                throw I0("Can't convert object to primitive value")
+                throw T0("Can't convert object to primitive value")
             }(e, t)
     },
-    wn = function(e) {
-        var t = E0(e, "string");
+    _n = function(e) {
+        var t = U0(e, "string");
         return sr(t) ? t : t + ""
     },
     No = M.document,
-    U0 = st(No) && st(No.createElement),
-    Lh = function(e) {
-        return U0 ? No.createElement(e) : {}
+    N0 = st(No) && st(No.createElement),
+    kh = function(e) {
+        return N0 ? No.createElement(e) : {}
     },
-    Dh = !J && !nt(function() {
-        return Object.defineProperty(Lh("div"), "a", {
+    Eh = !J && !nt(function() {
+        return Object.defineProperty(kh("div"), "a", {
             get: function() {
                 return 7
             }
         }).a != 7
     }),
-    gu = Object.getOwnPropertyDescriptor,
+    wu = Object.getOwnPropertyDescriptor,
     oi = {
-        f: J ? gu : function(e, t) {
-            if (e = be(e), t = wn(t), Dh) try {
-                return gu(e, t)
+        f: J ? wu : function(e, t) {
+            if (e = be(e), t = _n(t), Eh) try {
+                return wu(e, t)
             } catch {}
-            if (A(e, t)) return gn(!St(oc.f, e, t), e[t])
+            if (A(e, t)) return vn(!St(rc.f, e, t), e[t])
         }
     },
-    kh = J && nt(function() {
+    Uh = J && nt(function() {
         return Object.defineProperty(function() {}, "prototype", {
             value: 42,
             writable: !1
         }).prototype != 42
     }),
-    N0 = String,
-    M0 = TypeError,
+    M0 = String,
+    C0 = TypeError,
     ht = function(e) {
         if (st(e)) return e;
-        throw M0(N0(e) + " is not an object")
+        throw C0(M0(e) + " is not an object")
     },
-    C0 = TypeError,
+    R0 = TypeError,
     ro = Object.defineProperty,
-    R0 = Object.getOwnPropertyDescriptor,
+    V0 = Object.getOwnPropertyDescriptor,
     vt = {
-        f: J ? kh ? function(e, t, n) {
-            if (ht(e), t = wn(t), ht(n), typeof e == "function" && t === "prototype" && "value" in n && "writable" in n && !n.writable) {
-                var r = R0(e, t);
+        f: J ? Uh ? function(e, t, n) {
+            if (ht(e), t = _n(t), ht(n), typeof e == "function" && t === "prototype" && "value" in n && "writable" in n && !n.writable) {
+                var r = V0(e, t);
                 r && r.writable && (e[t] = n.value, n = {
                     configurable: "configurable" in n ? n.configurable : r.configurable,
                     enumerable: "enumerable" in n ? n.enumerable : r.enumerable,
                     writable: !1
                 })
             }
             return ro(e, t, n)
         } : ro : function(e, t, n) {
-            if (ht(e), t = wn(t), ht(n), Dh) try {
+            if (ht(e), t = _n(t), ht(n), Eh) try {
                 return ro(e, t, n)
             } catch {}
-            if ("get" in n || "set" in n) throw C0("Accessors not supported");
+            if ("get" in n || "set" in n) throw R0("Accessors not supported");
             return "value" in n && (e[t] = n.value), e
         }
     },
     Us = J ? function(e, t, n) {
-        return vt.f(e, t, gn(1, n))
+        return vt.f(e, t, vn(1, n))
     } : function(e, t, n) {
         return e[t] = n, e
     },
-    Eh = Function.prototype,
-    V0 = J && Object.getOwnPropertyDescriptor,
-    io = A(Eh, "name"),
-    lc = {
+    Nh = Function.prototype,
+    j0 = J && Object.getOwnPropertyDescriptor,
+    io = A(Nh, "name"),
+    ac = {
         EXISTS: io,
         PROPER: io && function() {}.name === "something",
-        CONFIGURABLE: io && (!J || J && V0(Eh, "name").configurable)
+        CONFIGURABLE: io && (!J || J && j0(Nh, "name").configurable)
     },
-    j0 = P(Function.toString);
-rt(We.inspectSource) || (We.inspectSource = function(e) {
-    return j0(e)
+    P0 = P(Function.toString);
+rt($e.inspectSource) || ($e.inspectSource = function(e) {
+    return P0(e)
 });
-var es, Or, ns, fc = We.inspectSource,
-    vu = M.WeakMap,
-    P0 = rt(vu) && /native code/.test(fc(vu)),
-    wu = Qe("keys"),
+var es, Or, ns, cc = $e.inspectSource,
+    _u = M.WeakMap,
+    z0 = rt(_u) && /native code/.test(cc(_u)),
+    Su = en("keys"),
     Ns = function(e) {
-        return wu[e] || (wu[e] = or(e))
+        return Su[e] || (Su[e] = or(e))
     },
     dr = {},
     Mo = M.TypeError,
-    z0 = M.WeakMap;
-if (P0 || We.state) {
-    var rn = We.state || (We.state = new z0),
-        W0 = P(rn.get),
-        _u = P(rn.has),
-        $0 = P(rn.set);
+    W0 = M.WeakMap;
+if (z0 || $e.state) {
+    var on = $e.state || ($e.state = new W0),
+        $0 = P(on.get),
+        Iu = P(on.has),
+        Y0 = P(on.set);
     es = function(e, t) {
-        if (_u(rn, e)) throw new Mo("Object already initialized");
-        return t.facade = e, $0(rn, e, t), t
+        if (Iu(on, e)) throw new Mo("Object already initialized");
+        return t.facade = e, Y0(on, e, t), t
     }, Or = function(e) {
-        return W0(rn, e) || {}
+        return $0(on, e) || {}
     }, ns = function(e) {
-        return _u(rn, e)
+        return Iu(on, e)
     }
 } else {
-    var xn = Ns("state");
-    dr[xn] = !0, es = function(e, t) {
-        if (A(e, xn)) throw new Mo("Object already initialized");
-        return t.facade = e, Us(e, xn, t), t
+    var Ln = Ns("state");
+    dr[Ln] = !0, es = function(e, t) {
+        if (A(e, Ln)) throw new Mo("Object already initialized");
+        return t.facade = e, Us(e, Ln, t), t
     }, Or = function(e) {
-        return A(e, xn) ? e[xn] : {}
+        return A(e, Ln) ? e[Ln] : {}
     }, ns = function(e) {
-        return A(e, xn)
+        return A(e, Ln)
     }
 }
-var Wt = {
+var $t = {
         set: es,
         get: Or,
         has: ns,
         enforce: function(e) {
             return ns(e) ? Or(e) : es(e, {})
         },
         getterFor: function(e) {
             return function(t) {
                 var n;
                 if (!st(t) || (n = Or(t)).type !== e) throw Mo("Incompatible receiver, " + e + " required");
                 return n
             }
         }
     },
-    Y0 = lr(function(e) {
-        var t = lc.CONFIGURABLE,
-            n = Wt.enforce,
-            r = Wt.get,
+    G0 = lr(function(e) {
+        var t = ac.CONFIGURABLE,
+            n = $t.enforce,
+            r = $t.get,
             s = Object.defineProperty,
             o = J && !nt(function() {
                 return s(function() {}, "length", {
                     value: 8
                 }).length !== 8
             }),
             i = String(String).split("String"),
@@ -11383,413 +11383,413 @@
                         writable: !1
                     }) : c.prototype && (c.prototype = void 0)
                 } catch {}
                 var f = n(c);
                 return A(f, "source") || (f.source = i.join(typeof u == "string" ? u : "")), c
             };
         Function.prototype.toString = a(function() {
-            return rt(this) && r(this).source || fc(this)
+            return rt(this) && r(this).source || cc(this)
         }, "toString")
     }),
     It = function(e, t, n, r) {
         r || (r = {});
         var s = r.enumerable,
             o = r.name !== void 0 ? r.name : t;
-        if (rt(n) && Y0(n, o, r), r.global) s ? e[t] = n : uc(t, n);
+        if (rt(n) && G0(n, o, r), r.global) s ? e[t] = n : oc(t, n);
         else {
             try {
                 r.unsafe ? e[t] && (s = !0) : delete e[t]
             } catch {}
             s ? e[t] = n : vt.f(e, t, {
                 value: n,
                 enumerable: !1,
                 configurable: !r.nonConfigurable,
                 writable: !r.nonWritable
             })
         }
         return e
     },
-    G0 = Math.ceil,
-    K0 = Math.floor,
-    Z0 = Math.trunc || function(e) {
+    K0 = Math.ceil,
+    Z0 = Math.floor,
+    H0 = Math.trunc || function(e) {
         var t = +e;
-        return (t > 0 ? K0 : G0)(t)
+        return (t > 0 ? Z0 : K0)(t)
     },
-    hc = function(e) {
+    uc = function(e) {
         var t = +e;
-        return t != t || t === 0 ? 0 : Z0(t)
+        return t != t || t === 0 ? 0 : H0(t)
     },
-    H0 = Math.max,
-    J0 = Math.min,
+    J0 = Math.max,
+    X0 = Math.min,
     Co = function(e, t) {
-        var n = hc(e);
-        return n < 0 ? H0(n + t, 0) : J0(n, t)
+        var n = uc(e);
+        return n < 0 ? J0(n + t, 0) : X0(n, t)
     },
-    X0 = Math.min,
-    Uh = function(e) {
-        return e > 0 ? X0(hc(e), 9007199254740991) : 0
+    q0 = Math.min,
+    Mh = function(e) {
+        return e > 0 ? q0(uc(e), 9007199254740991) : 0
     },
     pr = function(e) {
-        return Uh(e.length)
+        return Mh(e.length)
     },
-    Su = function(e) {
+    Tu = function(e) {
         return function(t, n, r) {
             var s, o = be(t),
                 i = pr(o),
                 a = Co(r, i);
             if (e && n != n) {
                 for (; i > a;)
                     if ((s = o[a++]) != s) return !0
             } else
                 for (; i > a; a++)
                     if ((e || a in o) && o[a] === n) return e || a || 0;
             return !e && -1
         }
     },
-    Nh = {
-        includes: Su(!0),
-        indexOf: Su(!1)
-    },
-    q0 = Nh.indexOf,
-    Iu = P([].push),
-    Mh = function(e, t) {
+    Ch = {
+        includes: Tu(!0),
+        indexOf: Tu(!1)
+    },
+    Q0 = Ch.indexOf,
+    Au = P([].push),
+    Rh = function(e, t) {
         var n, r = be(e),
             s = 0,
             o = [];
-        for (n in r) !A(dr, n) && A(r, n) && Iu(o, n);
-        for (; t.length > s;) A(r, n = t[s++]) && (~q0(o, n) || Iu(o, n));
+        for (n in r) !A(dr, n) && A(r, n) && Au(o, n);
+        for (; t.length > s;) A(r, n = t[s++]) && (~Q0(o, n) || Au(o, n));
         return o
     },
     rs = ["constructor", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "toLocaleString", "toString", "valueOf"],
-    Q0 = rs.concat("length", "prototype"),
+    tv = rs.concat("length", "prototype"),
     Vr = {
         f: Object.getOwnPropertyNames || function(e) {
-            return Mh(e, Q0)
+            return Rh(e, tv)
         }
     },
     Ms = {
         f: Object.getOwnPropertySymbols
     },
-    tv = P([].concat),
-    ev = ie("Reflect", "ownKeys") || function(e) {
+    ev = P([].concat),
+    nv = se("Reflect", "ownKeys") || function(e) {
         var t = Vr.f(ht(e)),
             n = Ms.f;
-        return n ? tv(t, n(e)) : t
+        return n ? ev(t, n(e)) : t
     },
-    Ch = function(e, t, n) {
-        for (var r = ev(t), s = vt.f, o = oi.f, i = 0; i < r.length; i++) {
+    Vh = function(e, t, n) {
+        for (var r = nv(t), s = vt.f, o = oi.f, i = 0; i < r.length; i++) {
             var a = r[i];
             A(e, a) || n && A(n, a) || s(e, a, o(t, a))
         }
     },
-    nv = /#|\.prototype\./,
+    rv = /#|\.prototype\./,
     ai = function(e, t) {
-        var n = iv[rv(e)];
-        return n == ov || n != sv && (rt(t) ? nt(t) : !!t)
+        var n = sv[iv(e)];
+        return n == av || n != ov && (rt(t) ? nt(t) : !!t)
     },
-    rv = ai.normalize = function(e) {
-        return String(e).replace(nv, ".").toLowerCase()
+    iv = ai.normalize = function(e) {
+        return String(e).replace(rv, ".").toLowerCase()
     },
-    iv = ai.data = {},
-    sv = ai.NATIVE = "N",
-    ov = ai.POLYFILL = "P",
+    sv = ai.data = {},
+    ov = ai.NATIVE = "N",
+    av = ai.POLYFILL = "P",
     Ro = ai,
-    av = oi.f,
+    cv = oi.f,
     dt = function(e, t) {
         var n, r, s, o, i, a = e.target,
             c = e.global,
             u = e.stat;
-        if (n = c ? M : u ? M[a] || uc(a, {}) : (M[a] || {}).prototype)
+        if (n = c ? M : u ? M[a] || oc(a, {}) : (M[a] || {}).prototype)
             for (r in t) {
-                if (o = t[r], s = e.dontCallGetSet ? (i = av(n, r)) && i.value : n[r], !Ro(c ? r : a + (u ? "." : "#") + r, e.forced) && s !== void 0) {
+                if (o = t[r], s = e.dontCallGetSet ? (i = cv(n, r)) && i.value : n[r], !Ro(c ? r : a + (u ? "." : "#") + r, e.forced) && s !== void 0) {
                     if (typeof o == typeof s) continue;
-                    Ch(o, s)
+                    Vh(o, s)
                 }(e.sham || s && s.sham) && Us(o, "sham", !0), It(n, r, o, e)
             }
     },
-    Rh = {};
-Rh[ut("toStringTag")] = "z";
-var so, dc = String(Rh) === "[object z]",
-    cv = ut("toStringTag"),
-    uv = Object,
-    lv = Te(function() {
+    jh = {};
+jh[ut("toStringTag")] = "z";
+var so, lc = String(jh) === "[object z]",
+    uv = ut("toStringTag"),
+    lv = Object,
+    fv = Te(function() {
         return arguments
     }()) == "Arguments",
-    Bn = dc ? Te : function(e) {
+    On = lc ? Te : function(e) {
         var t, n, r;
         return e === void 0 ? "Undefined" : e === null ? "Null" : typeof(n = function(s, o) {
             try {
                 return s[o]
             } catch {}
-        }(t = uv(e), cv)) == "string" ? n : lv ? Te(t) : (r = Te(t)) == "Object" && rt(t.callee) ? "Arguments" : r
+        }(t = lv(e), uv)) == "string" ? n : fv ? Te(t) : (r = Te(t)) == "Object" && rt(t.callee) ? "Arguments" : r
     },
-    fv = String,
+    hv = String,
     Oe = function(e) {
-        if (Bn(e) === "Symbol") throw TypeError("Cannot convert a Symbol value to a string");
-        return fv(e)
+        if (On(e) === "Symbol") throw TypeError("Cannot convert a Symbol value to a string");
+        return hv(e)
     },
-    hv = ut("match"),
-    dv = TypeError,
-    Vh = function(e) {
+    dv = ut("match"),
+    pv = TypeError,
+    Ph = function(e) {
         if (function(t) {
                 var n;
-                return st(t) && ((n = t[hv]) !== void 0 ? !!n : Te(t) == "RegExp")
-            }(e)) throw dv("The method doesn't accept regular expressions");
+                return st(t) && ((n = t[dv]) !== void 0 ? !!n : Te(t) == "RegExp")
+            }(e)) throw pv("The method doesn't accept regular expressions");
         return e
     },
-    pv = ut("match"),
-    jh = function(e) {
+    yv = ut("match"),
+    zh = function(e) {
         var t = /./;
         try {
             "/./" [e](t)
         } catch {
             try {
-                return t[pv] = !1, "/./" [e](t)
+                return t[yv] = !1, "/./" [e](t)
             } catch {}
         }
         return !1
     },
-    yv = oi.f,
-    Tu = P("".startsWith),
-    bv = P("".slice),
-    mv = Math.min,
-    Ph = jh("startsWith"),
-    gv = !(Ph || (so = yv(String.prototype, "startsWith"), !so || so.writable));
+    bv = oi.f,
+    Bu = P("".startsWith),
+    mv = P("".slice),
+    gv = Math.min,
+    Wh = zh("startsWith"),
+    vv = !(Wh || (so = bv(String.prototype, "startsWith"), !so || so.writable));
 dt({
     target: "String",
     proto: !0,
-    forced: !gv && !Ph
+    forced: !vv && !Wh
 }, {
     startsWith: function(e) {
         var t = Oe(si(this));
-        Vh(e);
-        var n = Uh(mv(arguments.length > 1 ? arguments[1] : void 0, t.length)),
+        Ph(e);
+        var n = Mh(gv(arguments.length > 1 ? arguments[1] : void 0, t.length)),
             r = Oe(e);
-        return Tu ? Tu(t, r, n) : bv(t, n, n + r.length) === r
+        return Bu ? Bu(t, r, n) : mv(t, n, n + r.length) === r
     }
 });
-var pc = function(e, t) {
+var fc = function(e, t) {
     return P(M[e].prototype[t])
 };
-pc("String", "startsWith");
+fc("String", "startsWith");
 var is = Array.isArray || function(e) {
         return Te(e) == "Array"
     },
-    vv = TypeError,
-    Au = function(e) {
-        if (e > 9007199254740991) throw vv("Maximum allowed index exceeded");
+    wv = TypeError,
+    Ou = function(e) {
+        if (e > 9007199254740991) throw wv("Maximum allowed index exceeded");
         return e
     },
     jr = function(e, t, n) {
-        var r = wn(t);
-        r in e ? vt.f(e, r, gn(0, n)) : e[r] = n
+        var r = _n(t);
+        r in e ? vt.f(e, r, vn(0, n)) : e[r] = n
     },
-    zh = function() {},
-    wv = [],
-    Wh = ie("Reflect", "construct"),
-    yc = /^\s*(?:class|function)\b/,
-    _v = P(yc.exec),
-    Sv = !yc.exec(zh),
+    $h = function() {},
+    _v = [],
+    Yh = se("Reflect", "construct"),
+    hc = /^\s*(?:class|function)\b/,
+    Sv = P(hc.exec),
+    Iv = !hc.exec($h),
     gr = function(e) {
         if (!rt(e)) return !1;
         try {
-            return Wh(zh, wv, e), !0
+            return Yh($h, _v, e), !0
         } catch {
             return !1
         }
     },
-    $h = function(e) {
+    Gh = function(e) {
         if (!rt(e)) return !1;
-        switch (Bn(e)) {
+        switch (On(e)) {
             case "AsyncFunction":
             case "GeneratorFunction":
             case "AsyncGeneratorFunction":
                 return !1
         }
         try {
-            return Sv || !!_v(yc, fc(e))
+            return Iv || !!Sv(hc, cc(e))
         } catch {
             return !0
         }
     };
-$h.sham = !0;
-var Bu, bc = !Wh || nt(function() {
+Gh.sham = !0;
+var Fu, dc = !Yh || nt(function() {
         var e;
         return gr(gr.call) || !gr(Object) || !gr(function() {
             e = !0
         }) || e
-    }) ? $h : gr,
-    Iv = ut("species"),
-    Ou = Array,
-    Yh = function(e, t) {
+    }) ? Gh : gr,
+    Tv = ut("species"),
+    xu = Array,
+    Kh = function(e, t) {
         return new(function(n) {
             var r;
-            return is(n) && (r = n.constructor, (bc(r) && (r === Ou || is(r.prototype)) || st(r) && (r = r[Iv]) === null) && (r = void 0)), r === void 0 ? Ou : r
+            return is(n) && (r = n.constructor, (dc(r) && (r === xu || is(r.prototype)) || st(r) && (r = r[Tv]) === null) && (r = void 0)), r === void 0 ? xu : r
         }(e))(t === 0 ? 0 : t)
     },
-    Tv = ut("species"),
-    Gh = ut("isConcatSpreadable"),
-    Av = Qi >= 51 || !nt(function() {
+    Av = ut("species"),
+    Zh = ut("isConcatSpreadable"),
+    Bv = Qi >= 51 || !nt(function() {
         var e = [];
-        return e[Gh] = !1, e.concat()[0] !== e
+        return e[Zh] = !1, e.concat()[0] !== e
     }),
-    Bv = (Bu = "concat", Qi >= 51 || !nt(function() {
+    Ov = (Fu = "concat", Qi >= 51 || !nt(function() {
         var e = [];
-        return (e.constructor = {})[Tv] = function() {
+        return (e.constructor = {})[Av] = function() {
             return {
                 foo: 1
             }
-        }, e[Bu](Boolean).foo !== 1
+        }, e[Fu](Boolean).foo !== 1
     })),
-    Ov = function(e) {
+    Fv = function(e) {
         if (!st(e)) return !1;
-        var t = e[Gh];
+        var t = e[Zh];
         return t !== void 0 ? !!t : is(e)
     };
 dt({
     target: "Array",
     proto: !0,
     arity: 1,
-    forced: !Av || !Bv
+    forced: !Bv || !Ov
 }, {
     concat: function(e) {
         var t, n, r, s, o, i = hr(this),
-            a = Yh(i, 0),
+            a = Kh(i, 0),
             c = 0;
         for (t = -1, r = arguments.length; t < r; t++)
-            if (Ov(o = t === -1 ? i : arguments[t]))
-                for (s = pr(o), Au(c + s), n = 0; n < s; n++, c++) n in o && jr(a, c, o[n]);
-            else Au(c + 1), jr(a, c++, o);
+            if (Fv(o = t === -1 ? i : arguments[t]))
+                for (s = pr(o), Ou(c + s), n = 0; n < s; n++, c++) n in o && jr(a, c, o[n]);
+            else Ou(c + 1), jr(a, c++, o);
         return a.length = c, a
     }
 });
-var Fv = dc ? {}.toString : function() {
-    return "[object " + Bn(this) + "]"
+var xv = lc ? {}.toString : function() {
+    return "[object " + On(this) + "]"
 };
-dc || It(Object.prototype, "toString", Fv, {
+lc || It(Object.prototype, "toString", xv, {
     unsafe: !0
 });
-var gi, mc = Object.keys || function(e) {
-        return Mh(e, rs)
+var gi, pc = Object.keys || function(e) {
+        return Rh(e, rs)
     },
-    xv = J && !kh ? Object.defineProperties : function(e, t) {
+    Lv = J && !Uh ? Object.defineProperties : function(e, t) {
         ht(e);
-        for (var n, r = be(t), s = mc(t), o = s.length, i = 0; o > i;) vt.f(e, n = s[i++], r[n]);
+        for (var n, r = be(t), s = pc(t), o = s.length, i = 0; o > i;) vt.f(e, n = s[i++], r[n]);
         return e
     },
-    Kh = {
-        f: xv
+    Hh = {
+        f: Lv
     },
-    Lv = ie("document", "documentElement"),
-    Zh = Ns("IE_PROTO"),
+    Dv = se("document", "documentElement"),
+    Jh = Ns("IE_PROTO"),
     oo = function() {},
-    Hh = function(e) {
+    Xh = function(e) {
         return "<script>" + e + "<\/script>"
     },
-    Fu = function(e) {
-        e.write(Hh("")), e.close();
+    Lu = function(e) {
+        e.write(Xh("")), e.close();
         var t = e.parentWindow.Object;
         return e = null, t
     },
     Di = function() {
         try {
             gi = new ActiveXObject("htmlfile")
         } catch {}
         var e, t;
-        Di = typeof document < "u" ? document.domain && gi ? Fu(gi) : ((t = Lh("iframe")).style.display = "none", Lv.appendChild(t), t.src = String("javascript:"), (e = t.contentWindow.document).open(), e.write(Hh("document.F=Object")), e.close(), e.F) : Fu(gi);
+        Di = typeof document < "u" ? document.domain && gi ? Lu(gi) : ((t = kh("iframe")).style.display = "none", Dv.appendChild(t), t.src = String("javascript:"), (e = t.contentWindow.document).open(), e.write(Xh("document.F=Object")), e.close(), e.F) : Lu(gi);
         for (var n = rs.length; n--;) delete Di.prototype[rs[n]];
         return Di()
     };
-dr[Zh] = !0;
-var He = Object.create || function(e, t) {
+dr[Jh] = !0;
+var Xe = Object.create || function(e, t) {
         var n;
-        return e !== null ? (oo.prototype = ht(e), n = new oo, oo.prototype = null, n[Zh] = e) : n = Di(), t === void 0 ? n : Kh.f(n, t)
+        return e !== null ? (oo.prototype = ht(e), n = new oo, oo.prototype = null, n[Jh] = e) : n = Di(), t === void 0 ? n : Hh.f(n, t)
     },
-    Dv = Array,
-    kv = Math.max,
-    Jh = Vr.f,
-    Xh = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
-    Ev = function(e) {
+    kv = Array,
+    Ev = Math.max,
+    qh = Vr.f,
+    Qh = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
+    Uv = function(e) {
         try {
-            return Jh(e)
+            return qh(e)
         } catch {
             return function(n, r, s) {
-                for (var o = pr(n), i = Co(r, o), a = Co(s === void 0 ? o : s, o), c = Dv(kv(a - i, 0)), u = 0; i < a; i++, u++) jr(c, u, n[i]);
+                for (var o = pr(n), i = Co(r, o), a = Co(s === void 0 ? o : s, o), c = kv(Ev(a - i, 0)), u = 0; i < a; i++, u++) jr(c, u, n[i]);
                 return c.length = u, c
-            }(Xh)
+            }(Qh)
         }
     },
-    gc = {
+    yc = {
         f: function(e) {
-            return Xh && Te(e) == "Window" ? Ev(e) : Jh(be(e))
+            return Qh && Te(e) == "Window" ? Uv(e) : qh(be(e))
         }
     },
-    qh = {
+    td = {
         f: ut
     },
     Pr = M,
-    Uv = vt.f,
+    Nv = vt.f,
     At = function(e) {
         var t = Pr.Symbol || (Pr.Symbol = {});
-        A(t, e) || Uv(t, e, {
-            value: qh.f(e)
+        A(t, e) || Nv(t, e, {
+            value: td.f(e)
         })
     },
-    Qh = function() {
-        var e = ie("Symbol"),
+    ed = function() {
+        var e = se("Symbol"),
             t = e && e.prototype,
             n = t && t.valueOf,
             r = ut("toPrimitive");
         t && !t[r] && It(t, r, function(s) {
             return St(n, this)
         }, {
             arity: 1
         })
     },
-    Nv = vt.f,
-    xu = ut("toStringTag"),
+    Mv = vt.f,
+    Du = ut("toStringTag"),
     Pe = function(e, t, n) {
-        e && !n && (e = e.prototype), e && !A(e, xu) && Nv(e, xu, {
+        e && !n && (e = e.prototype), e && !A(e, Du) && Mv(e, Du, {
             configurable: !0,
             value: t
         })
     },
-    Mv = P(P.bind),
+    Cv = P(P.bind),
     Cs = function(e, t) {
-        return cc(e), t === void 0 ? e : ii ? Mv(e, t) : function() {
+        return sc(e), t === void 0 ? e : ii ? Cv(e, t) : function() {
             return e.apply(t, arguments)
         }
     },
-    Lu = P([].push),
+    ku = P([].push),
     Me = function(e) {
         var t = e == 1,
             n = e == 2,
             r = e == 3,
             s = e == 4,
             o = e == 6,
             i = e == 7,
             a = e == 5 || o;
         return function(c, u, l, f) {
-            for (var h, p, w = hr(c), _ = xh(w), b = Cs(u, l), g = pr(_), v = 0, I = f || Yh, it = t ? I(c, g) : n || i ? I(c, 0) : void 0; g > v; v++)
+            for (var h, p, w = hr(c), _ = Dh(w), b = Cs(u, l), g = pr(_), v = 0, I = f || Kh, it = t ? I(c, g) : n || i ? I(c, 0) : void 0; g > v; v++)
                 if ((a || v in _) && (p = b(h = _[v], v, w), e))
                     if (t) it[v] = p;
                     else if (p) switch (e) {
                 case 3:
                     return !0;
                 case 5:
                     return h;
                 case 6:
                     return v;
                 case 2:
-                    Lu(it, h)
+                    ku(it, h)
             } else switch (e) {
                 case 4:
                     return !1;
                 case 7:
-                    Lu(it, h)
+                    ku(it, h)
             }
             return o ? -1 : r || s ? s : it
         }
     },
     Rs = {
         forEach: Me(0),
         map: Me(1),
@@ -11797,361 +11797,361 @@
         some: Me(3),
         every: Me(4),
         find: Me(5),
         findIndex: Me(6),
         filterReject: Me(7)
     }.forEach,
     Bt = Ns("hidden"),
-    Cv = Wt.set,
-    Du = Wt.getterFor("Symbol"),
-    jt = Object.prototype,
-    Vn = M.Symbol,
-    _r = Vn && Vn.prototype,
-    Rv = M.TypeError,
+    Rv = $t.set,
+    Eu = $t.getterFor("Symbol"),
+    Pt = Object.prototype,
+    Rn = M.Symbol,
+    _r = Rn && Rn.prototype,
+    Vv = M.TypeError,
     ao = M.QObject,
-    td = oi.f,
+    nd = oi.f,
     Ve = vt.f,
-    ed = gc.f,
-    Vv = oc.f,
-    nd = P([].push),
-    Fe = Qe("symbols"),
-    ci = Qe("op-symbols"),
-    jv = Qe("wks"),
+    rd = yc.f,
+    jv = rc.f,
+    id = P([].push),
+    Fe = en("symbols"),
+    ci = en("op-symbols"),
+    Pv = en("wks"),
     co = !ao || !ao.prototype || !ao.prototype.findChild,
     Vo = J && nt(function() {
-        return He(Ve({}, "a", {
+        return Xe(Ve({}, "a", {
             get: function() {
                 return Ve(this, "a", {
                     value: 7
                 }).a
             }
         })).a != 7
     }) ? function(e, t, n) {
-        var r = td(jt, t);
-        r && delete jt[t], Ve(e, t, n), r && e !== jt && Ve(jt, t, r)
+        var r = nd(Pt, t);
+        r && delete Pt[t], Ve(e, t, n), r && e !== Pt && Ve(Pt, t, r)
     } : Ve,
     uo = function(e, t) {
-        var n = Fe[e] = He(_r);
-        return Cv(n, {
+        var n = Fe[e] = Xe(_r);
+        return Rv(n, {
             type: "Symbol",
             tag: e,
             description: t
         }), J || (n.description = t), n
     },
     ss = function(e, t, n) {
-        e === jt && ss(ci, t, n), ht(e);
-        var r = wn(t);
-        return ht(n), A(Fe, r) ? (n.enumerable ? (A(e, Bt) && e[Bt][r] && (e[Bt][r] = !1), n = He(n, {
-            enumerable: gn(0, !1)
-        })) : (A(e, Bt) || Ve(e, Bt, gn(1, {})), e[Bt][r] = !0), Vo(e, r, n)) : Ve(e, r, n)
+        e === Pt && ss(ci, t, n), ht(e);
+        var r = _n(t);
+        return ht(n), A(Fe, r) ? (n.enumerable ? (A(e, Bt) && e[Bt][r] && (e[Bt][r] = !1), n = Xe(n, {
+            enumerable: vn(0, !1)
+        })) : (A(e, Bt) || Ve(e, Bt, vn(1, {})), e[Bt][r] = !0), Vo(e, r, n)) : Ve(e, r, n)
     },
     lo = function(e, t) {
         ht(e);
         var n = be(t),
-            r = mc(n).concat(rd(n));
+            r = pc(n).concat(sd(n));
         return Rs(r, function(s) {
             J && !St(jo, n, s) || ss(e, s, n[s])
         }), e
     },
     jo = function(e) {
-        var t = wn(e),
-            n = St(Vv, this, t);
-        return !(this === jt && A(Fe, t) && !A(ci, t)) && (!(n || !A(this, t) || !A(Fe, t) || A(this, Bt) && this[Bt][t]) || n)
+        var t = _n(e),
+            n = St(jv, this, t);
+        return !(this === Pt && A(Fe, t) && !A(ci, t)) && (!(n || !A(this, t) || !A(Fe, t) || A(this, Bt) && this[Bt][t]) || n)
     },
-    ku = function(e, t) {
+    Uu = function(e, t) {
         var n = be(e),
-            r = wn(t);
-        if (n !== jt || !A(Fe, r) || A(ci, r)) {
-            var s = td(n, r);
+            r = _n(t);
+        if (n !== Pt || !A(Fe, r) || A(ci, r)) {
+            var s = nd(n, r);
             return !s || !A(Fe, r) || A(n, Bt) && n[Bt][r] || (s.enumerable = !0), s
         }
     },
-    Eu = function(e) {
-        var t = ed(be(e)),
+    Nu = function(e) {
+        var t = rd(be(e)),
             n = [];
         return Rs(t, function(r) {
-            A(Fe, r) || A(dr, r) || nd(n, r)
+            A(Fe, r) || A(dr, r) || id(n, r)
         }), n
     },
-    rd = function(e) {
-        var t = e === jt,
-            n = ed(t ? ci : be(e)),
+    sd = function(e) {
+        var t = e === Pt,
+            n = rd(t ? ci : be(e)),
             r = [];
         return Rs(n, function(s) {
-            !A(Fe, s) || t && !A(jt, s) || nd(r, Fe[s])
+            !A(Fe, s) || t && !A(Pt, s) || id(r, Fe[s])
         }), r
     };
-Vt || (_r = (Vn = function() {
-    if (vn(_r, this)) throw Rv("Symbol is not a constructor");
+jt || (_r = (Rn = function() {
+    if (wn(_r, this)) throw Vv("Symbol is not a constructor");
     var e = arguments.length && arguments[0] !== void 0 ? Oe(arguments[0]) : void 0,
         t = or(e),
         n = function(r) {
-            this === jt && St(n, ci, r), A(this, Bt) && A(this[Bt], t) && (this[Bt][t] = !1), Vo(this, t, gn(1, r))
+            this === Pt && St(n, ci, r), A(this, Bt) && A(this[Bt], t) && (this[Bt][t] = !1), Vo(this, t, vn(1, r))
         };
-    return J && co && Vo(jt, t, {
+    return J && co && Vo(Pt, t, {
         configurable: !0,
         set: n
     }), uo(t, e)
 }).prototype, It(_r, "toString", function() {
-    return Du(this).tag
-}), It(Vn, "withoutSetter", function(e) {
+    return Eu(this).tag
+}), It(Rn, "withoutSetter", function(e) {
     return uo(or(e), e)
-}), oc.f = jo, vt.f = ss, Kh.f = lo, oi.f = ku, Vr.f = gc.f = Eu, Ms.f = rd, qh.f = function(e) {
+}), rc.f = jo, vt.f = ss, Hh.f = lo, oi.f = Uu, Vr.f = yc.f = Nu, Ms.f = sd, td.f = function(e) {
     return uo(ut(e), e)
 }, J && (Ve(_r, "description", {
     configurable: !0,
     get: function() {
-        return Du(this).description
+        return Eu(this).description
     }
-}), It(jt, "propertyIsEnumerable", jo, {
+}), It(Pt, "propertyIsEnumerable", jo, {
     unsafe: !0
 }))), dt({
     global: !0,
     constructor: !0,
     wrap: !0,
-    forced: !Vt,
-    sham: !Vt
+    forced: !jt,
+    sham: !jt
 }, {
-    Symbol: Vn
-}), Rs(mc(jv), function(e) {
+    Symbol: Rn
+}), Rs(pc(Pv), function(e) {
     At(e)
 }), dt({
     target: "Symbol",
     stat: !0,
-    forced: !Vt
+    forced: !jt
 }, {
     useSetter: function() {
         co = !0
     },
     useSimple: function() {
         co = !1
     }
 }), dt({
     target: "Object",
     stat: !0,
-    forced: !Vt,
+    forced: !jt,
     sham: !J
 }, {
     create: function(e, t) {
-        return t === void 0 ? He(e) : lo(He(e), t)
+        return t === void 0 ? Xe(e) : lo(Xe(e), t)
     },
     defineProperty: ss,
     defineProperties: lo,
-    getOwnPropertyDescriptor: ku
+    getOwnPropertyDescriptor: Uu
 }), dt({
     target: "Object",
     stat: !0,
-    forced: !Vt
+    forced: !jt
 }, {
-    getOwnPropertyNames: Eu
-}), Qh(), Pe(Vn, "Symbol"), dr[Bt] = !0;
-var id = Vt && !!Symbol.for && !!Symbol.keyFor,
-    fo = Qe("string-to-symbol-registry"),
-    Pv = Qe("symbol-to-string-registry");
+    getOwnPropertyNames: Nu
+}), ed(), Pe(Rn, "Symbol"), dr[Bt] = !0;
+var od = jt && !!Symbol.for && !!Symbol.keyFor,
+    fo = en("string-to-symbol-registry"),
+    zv = en("symbol-to-string-registry");
 dt({
     target: "Symbol",
     stat: !0,
-    forced: !id
+    forced: !od
 }, {
     for: function(e) {
         var t = Oe(e);
         if (A(fo, t)) return fo[t];
-        var n = ie("Symbol")(t);
-        return fo[t] = n, Pv[n] = t, n
+        var n = se("Symbol")(t);
+        return fo[t] = n, zv[n] = t, n
     }
 });
-var Uu = Qe("symbol-to-string-registry");
+var Mu = en("symbol-to-string-registry");
 dt({
     target: "Symbol",
     stat: !0,
-    forced: !id
+    forced: !od
 }, {
     keyFor: function(e) {
         if (!sr(e)) throw TypeError(fr(e) + " is not a symbol");
-        if (A(Uu, e)) return Uu[e]
+        if (A(Mu, e)) return Mu[e]
     }
 });
-var sd = Function.prototype,
-    Nu = sd.apply,
-    Mu = sd.call,
-    od = typeof Reflect == "object" && Reflect.apply || (ii ? Mu.bind(Nu) : function() {
-        return Mu.apply(Nu, arguments)
+var ad = Function.prototype,
+    Cu = ad.apply,
+    Ru = ad.call,
+    cd = typeof Reflect == "object" && Reflect.apply || (ii ? Ru.bind(Cu) : function() {
+        return Ru.apply(Cu, arguments)
     }),
-    vc = P([].slice),
-    $e = ie("JSON", "stringify"),
+    bc = P([].slice),
+    Ye = se("JSON", "stringify"),
     vi = P(/./.exec),
-    Cu = P("".charAt),
-    zv = P("".charCodeAt),
-    Wv = P("".replace),
-    $v = P(1 .toString),
-    Yv = /[\uD800-\uDFFF]/g,
-    Ru = /^[\uD800-\uDBFF]$/,
-    Vu = /^[\uDC00-\uDFFF]$/,
-    ju = !Vt || nt(function() {
-        var e = ie("Symbol")();
-        return $e([e]) != "[null]" || $e({
+    Vu = P("".charAt),
+    Wv = P("".charCodeAt),
+    $v = P("".replace),
+    Yv = P(1 .toString),
+    Gv = /[\uD800-\uDFFF]/g,
+    ju = /^[\uD800-\uDBFF]$/,
+    Pu = /^[\uDC00-\uDFFF]$/,
+    zu = !jt || nt(function() {
+        var e = se("Symbol")();
+        return Ye([e]) != "[null]" || Ye({
             a: e
-        }) != "{}" || $e(Object(e)) != "{}"
+        }) != "{}" || Ye(Object(e)) != "{}"
     }),
-    Pu = nt(function() {
-        return $e("\uDF06\uD834") !== '"\\udf06\\ud834"' || $e("\uDEAD") !== '"\\udead"'
+    Wu = nt(function() {
+        return Ye("\uDF06\uD834") !== '"\\udf06\\ud834"' || Ye("\uDEAD") !== '"\\udead"'
     }),
-    Gv = function(e, t) {
-        var n = vc(arguments),
+    Kv = function(e, t) {
+        var n = bc(arguments),
             r = t;
         if ((st(t) || e !== void 0) && !sr(e)) return is(t) || (t = function(s, o) {
             if (rt(r) && (o = St(r, this, s, o)), !sr(o)) return o
-        }), n[1] = t, od($e, null, n)
+        }), n[1] = t, cd(Ye, null, n)
     },
-    Kv = function(e, t, n) {
-        var r = Cu(n, t - 1),
-            s = Cu(n, t + 1);
-        return vi(Ru, e) && !vi(Vu, s) || vi(Vu, e) && !vi(Ru, r) ? "\\u" + $v(zv(e, 0), 16) : e
+    Zv = function(e, t, n) {
+        var r = Vu(n, t - 1),
+            s = Vu(n, t + 1);
+        return vi(ju, e) && !vi(Pu, s) || vi(Pu, e) && !vi(ju, r) ? "\\u" + Yv(Wv(e, 0), 16) : e
     };
-$e && dt({
+Ye && dt({
     target: "JSON",
     stat: !0,
     arity: 3,
-    forced: ju || Pu
+    forced: zu || Wu
 }, {
     stringify: function(e, t, n) {
-        var r = vc(arguments),
-            s = od(ju ? Gv : $e, null, r);
-        return Pu && typeof s == "string" ? Wv(s, Yv, Kv) : s
+        var r = bc(arguments),
+            s = cd(zu ? Kv : Ye, null, r);
+        return Wu && typeof s == "string" ? $v(s, Gv, Zv) : s
     }
 });
-var Zv = !Vt || nt(function() {
+var Hv = !jt || nt(function() {
     Ms.f(1)
 });
 dt({
     target: "Object",
     stat: !0,
-    forced: Zv
+    forced: Hv
 }, {
     getOwnPropertySymbols: function(e) {
         var t = Ms.f;
         return t ? t(hr(e)) : []
     }
 }), At("asyncIterator");
-var Hv = vt.f,
+var Jv = vt.f,
     we = M.Symbol,
-    sn = we && we.prototype;
-if (J && rt(we) && (!("description" in sn) || we().description !== void 0)) {
-    var zu = {},
+    an = we && we.prototype;
+if (J && rt(we) && (!("description" in an) || we().description !== void 0)) {
+    var $u = {},
         wi = function() {
             var e = arguments.length < 1 || arguments[0] === void 0 ? void 0 : Oe(arguments[0]),
-                t = vn(sn, this) ? new we(e) : e === void 0 ? we() : we(e);
-            return e === "" && (zu[t] = !0), t
+                t = wn(an, this) ? new we(e) : e === void 0 ? we() : we(e);
+            return e === "" && ($u[t] = !0), t
         };
-    Ch(wi, we), wi.prototype = sn, sn.constructor = wi;
-    var Jv = String(we("test")) == "Symbol(test)",
-        Xv = P(sn.toString),
-        qv = P(sn.valueOf),
-        Qv = /^Symbol\((.*)\)[^)]+$/,
-        tw = P("".replace),
-        ew = P("".slice);
-    Hv(sn, "description", {
+    Vh(wi, we), wi.prototype = an, an.constructor = wi;
+    var Xv = String(we("test")) == "Symbol(test)",
+        qv = P(an.toString),
+        Qv = P(an.valueOf),
+        tw = /^Symbol\((.*)\)[^)]+$/,
+        ew = P("".replace),
+        nw = P("".slice);
+    Jv(an, "description", {
         configurable: !0,
         get: function() {
-            var e = qv(this),
-                t = Xv(e);
-            if (A(zu, e)) return "";
-            var n = Jv ? ew(t, 7, -1) : tw(t, Qv, "$1");
+            var e = Qv(this),
+                t = qv(e);
+            if (A($u, e)) return "";
+            var n = Xv ? nw(t, 7, -1) : ew(t, tw, "$1");
             return n === "" ? void 0 : n
         }
     }), dt({
         global: !0,
         constructor: !0,
         forced: !0
     }, {
         Symbol: wi
     })
 }
-At("hasInstance"), At("isConcatSpreadable"), At("iterator"), At("match"), At("matchAll"), At("replace"), At("search"), At("species"), At("split"), At("toPrimitive"), Qh(), At("toStringTag"), Pe(ie("Symbol"), "Symbol"), At("unscopables"), Pe(M.JSON, "JSON", !0), Pe(Math, "Math", !0), dt({
+At("hasInstance"), At("isConcatSpreadable"), At("iterator"), At("match"), At("matchAll"), At("replace"), At("search"), At("species"), At("split"), At("toPrimitive"), ed(), At("toStringTag"), Pe(se("Symbol"), "Symbol"), At("unscopables"), Pe(M.JSON, "JSON", !0), Pe(Math, "Math", !0), dt({
     global: !0
 }, {
     Reflect: {}
 }), Pe(M.Reflect, "Reflect", !0), Pr.Symbol;
-var fn, Wu, $u, nw = P("".charAt),
-    Yu = P("".charCodeAt),
-    rw = P("".slice),
-    Gu = function(e) {
+var dn, Yu, Gu, rw = P("".charAt),
+    Ku = P("".charCodeAt),
+    iw = P("".slice),
+    Zu = function(e) {
         return function(t, n) {
             var r, s, o = Oe(si(t)),
-                i = hc(n),
+                i = uc(n),
                 a = o.length;
-            return i < 0 || i >= a ? e ? "" : void 0 : (r = Yu(o, i)) < 55296 || r > 56319 || i + 1 === a || (s = Yu(o, i + 1)) < 56320 || s > 57343 ? e ? nw(o, i) : r : e ? rw(o, i, i + 2) : s - 56320 + (r - 55296 << 10) + 65536
+            return i < 0 || i >= a ? e ? "" : void 0 : (r = Ku(o, i)) < 55296 || r > 56319 || i + 1 === a || (s = Ku(o, i + 1)) < 56320 || s > 57343 ? e ? rw(o, i) : r : e ? iw(o, i, i + 2) : s - 56320 + (r - 55296 << 10) + 65536
         }
     },
-    iw = {
-        codeAt: Gu(!1),
-        charAt: Gu(!0)
+    sw = {
+        codeAt: Zu(!1),
+        charAt: Zu(!0)
     },
-    sw = !nt(function() {
+    ow = !nt(function() {
         function e() {}
         return e.prototype.constructor = null, Object.getPrototypeOf(new e) !== e.prototype
     }),
-    Ku = Ns("IE_PROTO"),
+    Hu = Ns("IE_PROTO"),
     Po = Object,
-    ow = Po.prototype,
-    Je = sw ? Po.getPrototypeOf : function(e) {
+    aw = Po.prototype,
+    qe = ow ? Po.getPrototypeOf : function(e) {
         var t = hr(e);
-        if (A(t, Ku)) return t[Ku];
+        if (A(t, Hu)) return t[Hu];
         var n = t.constructor;
-        return rt(n) && t instanceof n ? n.prototype : t instanceof Po ? ow : null
+        return rt(n) && t instanceof n ? n.prototype : t instanceof Po ? aw : null
     },
     zo = ut("iterator"),
-    ad = !1;
-[].keys && ("next" in ($u = [].keys()) ? (Wu = Je(Je($u))) !== Object.prototype && (fn = Wu) : ad = !0);
-var aw = fn == null || nt(function() {
+    ud = !1;
+[].keys && ("next" in (Gu = [].keys()) ? (Yu = qe(qe(Gu))) !== Object.prototype && (dn = Yu) : ud = !0);
+var cw = dn == null || nt(function() {
     var e = {};
-    return fn[zo].call(e) !== e
+    return dn[zo].call(e) !== e
 });
-aw && (fn = {}), rt(fn[zo]) || It(fn, zo, function() {
+cw && (dn = {}), rt(dn[zo]) || It(dn, zo, function() {
     return this
 });
-var wc = {
-        IteratorPrototype: fn,
-        BUGGY_SAFARI_ITERATORS: ad
+var mc = {
+        IteratorPrototype: dn,
+        BUGGY_SAFARI_ITERATORS: ud
     },
     ar = {},
-    cw = wc.IteratorPrototype,
-    uw = function() {
+    uw = mc.IteratorPrototype,
+    lw = function() {
         return this
     },
-    lw = String,
-    fw = TypeError,
+    fw = String,
+    hw = TypeError,
     he = Object.setPrototypeOf || ("__proto__" in {} ? function() {
         var e, t = !1,
             n = {};
         try {
             (e = P(Object.getOwnPropertyDescriptor(Object.prototype, "__proto__").set))(n, []), t = n instanceof Array
         } catch {}
         return function(r, s) {
             return ht(r),
                 function(o) {
                     if (typeof o == "object" || rt(o)) return o;
-                    throw fw("Can't set " + lw(o) + " as a prototype")
+                    throw hw("Can't set " + fw(o) + " as a prototype")
                 }(s), t ? e(r, s) : r.__proto__ = s, r
         }
     }() : void 0),
-    hw = lc.PROPER,
-    dw = lc.CONFIGURABLE,
-    Zu = wc.IteratorPrototype,
-    _i = wc.BUGGY_SAFARI_ITERATORS,
+    dw = ac.PROPER,
+    pw = ac.CONFIGURABLE,
+    Ju = mc.IteratorPrototype,
+    _i = mc.BUGGY_SAFARI_ITERATORS,
     vr = ut("iterator"),
-    pw = function() {
+    yw = function() {
         return this
     },
-    _c = function(e, t, n, r, s, o, i) {
+    gc = function(e, t, n, r, s, o, i) {
         (function(g, v, I, it) {
             var yt = v + " Iterator";
-            g.prototype = He(cw, {
-                next: gn(+!it, I)
-            }), Pe(g, yt, !1), ar[yt] = uw
+            g.prototype = Xe(uw, {
+                next: vn(+!it, I)
+            }), Pe(g, yt, !1), ar[yt] = lw
         })(n, t, r);
         var a, c, u, l = function(g) {
                 if (g === s && _) return _;
                 if (!_i && g in p) return p[g];
                 switch (g) {
                     case "keys":
                     case "values":
@@ -12166,15 +12166,15 @@
             },
             f = t + " Iterator",
             h = !1,
             p = e.prototype,
             w = p[vr] || p["@@iterator"] || s && p[s],
             _ = !_i && w || l(s),
             b = t == "Array" && p.entries || w;
-        if (b && (a = Je(b.call(new e))) !== Object.prototype && a.next && (Je(a) !== Zu && (he ? he(a, Zu) : rt(a[vr]) || It(a, vr, pw)), Pe(a, f, !0)), hw && s == "values" && w && w.name !== "values" && (dw ? Us(p, "name", "values") : (h = !0, _ = function() {
+        if (b && (a = qe(b.call(new e))) !== Object.prototype && a.next && (qe(a) !== Ju && (he ? he(a, Ju) : rt(a[vr]) || It(a, vr, yw)), Pe(a, f, !0)), dw && s == "values" && w && w.name !== "values" && (pw ? Us(p, "name", "values") : (h = !0, _ = function() {
                 return St(w, this)
             })), s)
             if (c = {
                     values: l("values"),
                     keys: o ? _ : l("keys"),
                     entries: l("entries")
                 }, i)
@@ -12184,31 +12184,31 @@
                 proto: !0,
                 forced: _i || h
             }, c);
         return p[vr] !== _ && It(p, vr, _, {
             name: s
         }), ar[t] = _, c
     },
-    yw = iw.charAt,
-    bw = Wt.set,
-    mw = Wt.getterFor("String Iterator");
-_c(String, "String", function(e) {
-    bw(this, {
+    bw = sw.charAt,
+    mw = $t.set,
+    gw = $t.getterFor("String Iterator");
+gc(String, "String", function(e) {
+    mw(this, {
         type: "String Iterator",
         string: Oe(e),
         index: 0
     })
 }, function() {
-    var e, t = mw(this),
+    var e, t = gw(this),
         n = t.string,
         r = t.index;
     return r >= n.length ? {
         value: void 0,
         done: !0
-    } : (e = yw(n, r), t.index += e.length, {
+    } : (e = bw(n, r), t.index += e.length, {
         value: e,
         done: !1
     })
 });
 var Wo = function(e, t, n) {
         var r, s;
         ht(e);
@@ -12221,164 +12221,164 @@
         } catch (o) {
             s = !0, r = o
         }
         if (t === "throw") throw n;
         if (s) throw r;
         return ht(r), n
     },
-    gw = function(e, t, n, r) {
+    vw = function(e, t, n, r) {
         try {
             return r ? t(ht(n)[0], n[1]) : t(n)
         } catch (s) {
             Wo(e, "throw", s)
         }
     },
-    vw = ut("iterator"),
-    ww = Array.prototype,
-    cd = function(e) {
-        return e !== void 0 && (ar.Array === e || ww[vw] === e)
-    },
-    _w = ut("iterator"),
-    Sc = function(e) {
-        if (e != null) return ts(e, _w) || ts(e, "@@iterator") || ar[Bn(e)]
-    },
-    Sw = TypeError,
-    ud = function(e, t) {
-        var n = arguments.length < 2 ? Sc(e) : t;
-        if (cc(n)) return ht(St(n, e));
-        throw Sw(fr(e) + " is not iterable")
-    },
-    Hu = Array,
-    ld = ut("iterator"),
-    fd = !1;
+    ww = ut("iterator"),
+    _w = Array.prototype,
+    ld = function(e) {
+        return e !== void 0 && (ar.Array === e || _w[ww] === e)
+    },
+    Sw = ut("iterator"),
+    vc = function(e) {
+        if (e != null) return ts(e, Sw) || ts(e, "@@iterator") || ar[On(e)]
+    },
+    Iw = TypeError,
+    fd = function(e, t) {
+        var n = arguments.length < 2 ? vc(e) : t;
+        if (sc(n)) return ht(St(n, e));
+        throw Iw(fr(e) + " is not iterable")
+    },
+    Xu = Array,
+    hd = ut("iterator"),
+    dd = !1;
 try {
-    var Iw = 0,
-        Ju = {
+    var Tw = 0,
+        qu = {
             next: function() {
                 return {
-                    done: !!Iw++
+                    done: !!Tw++
                 }
             },
             return: function() {
-                fd = !0
+                dd = !0
             }
         };
-    Ju[ld] = function() {
+    qu[hd] = function() {
         return this
-    }, Array.from(Ju, function() {
+    }, Array.from(qu, function() {
         throw 2
     })
 } catch {}
-var hd = function(e, t) {
-        if (!t && !fd) return !1;
+var pd = function(e, t) {
+        if (!t && !dd) return !1;
         var n = !1;
         try {
             var r = {};
-            r[ld] = function() {
+            r[hd] = function() {
                 return {
                     next: function() {
                         return {
                             done: n = !0
                         }
                     }
                 }
             }, e(r)
         } catch {}
         return n
     },
-    Tw = !hd(function(e) {
+    Aw = !pd(function(e) {
         Array.from(e)
     });
 dt({
     target: "Array",
     stat: !0,
-    forced: Tw
+    forced: Aw
 }, {
     from: function(e) {
         var t = hr(e),
-            n = bc(this),
+            n = dc(this),
             r = arguments.length,
             s = r > 1 ? arguments[1] : void 0,
             o = s !== void 0;
         o && (s = Cs(s, r > 2 ? arguments[2] : void 0));
-        var i, a, c, u, l, f, h = Sc(t),
+        var i, a, c, u, l, f, h = vc(t),
             p = 0;
-        if (!h || this === Hu && cd(h))
-            for (i = pr(t), a = n ? new this(i) : Hu(i); i > p; p++) f = o ? s(t[p], p) : t[p], jr(a, p, f);
+        if (!h || this === Xu && ld(h))
+            for (i = pr(t), a = n ? new this(i) : Xu(i); i > p; p++) f = o ? s(t[p], p) : t[p], jr(a, p, f);
         else
-            for (l = (u = ud(t, h)).next, a = n ? new this : []; !(c = St(l, u)).done; p++) f = o ? gw(u, s, [c.value, p], !0) : c.value, jr(a, p, f);
+            for (l = (u = fd(t, h)).next, a = n ? new this : []; !(c = St(l, u)).done; p++) f = o ? vw(u, s, [c.value, p], !0) : c.value, jr(a, p, f);
         return a.length = p, a
     }
 }), Pr.Array.from;
-var Ft, Gn, os, Aw = typeof ArrayBuffer < "u" && typeof DataView < "u",
-    Bw = vt.f,
-    dd = Wt.enforce,
-    Ow = Wt.get,
+var Ft, Gn, os, Bw = typeof ArrayBuffer < "u" && typeof DataView < "u",
+    Ow = vt.f,
+    yd = $t.enforce,
+    Fw = $t.get,
     as = M.Int8Array,
     $o = as && as.prototype,
-    Xu = M.Uint8ClampedArray,
-    qu = Xu && Xu.prototype,
-    oe = as && Je(as),
-    Zt = $o && Je($o),
-    Fw = Object.prototype,
+    Qu = M.Uint8ClampedArray,
+    tl = Qu && Qu.prototype,
+    ae = as && qe(as),
+    Ht = $o && qe($o),
+    xw = Object.prototype,
     Yo = M.TypeError,
-    Qu = ut("toStringTag"),
+    el = ut("toStringTag"),
     Go = or("TYPED_ARRAY_TAG"),
-    Ae = Aw && !!he && Bn(M.opera) !== "Opera",
-    pd = !1,
+    Ae = Bw && !!he && On(M.opera) !== "Opera",
+    bd = !1,
     Ie = {
         Int8Array: 1,
         Uint8Array: 1,
         Uint8ClampedArray: 1,
         Int16Array: 2,
         Uint16Array: 2,
         Int32Array: 4,
         Uint32Array: 4,
         Float32Array: 4,
         Float64Array: 8
     },
-    Ic = {
+    wc = {
         BigInt64Array: 8,
         BigUint64Array: 8
     },
-    yd = function(e) {
-        var t = Je(e);
+    md = function(e) {
+        var t = qe(e);
         if (st(t)) {
-            var n = Ow(t);
-            return n && A(n, "TypedArrayConstructor") ? n.TypedArrayConstructor : yd(t)
+            var n = Fw(t);
+            return n && A(n, "TypedArrayConstructor") ? n.TypedArrayConstructor : md(t)
         }
     },
-    tl = function(e) {
+    nl = function(e) {
         if (!st(e)) return !1;
-        var t = Bn(e);
-        return A(Ie, t) || A(Ic, t)
+        var t = On(e);
+        return A(Ie, t) || A(wc, t)
     };
-for (Ft in Ie)(os = (Gn = M[Ft]) && Gn.prototype) ? dd(os).TypedArrayConstructor = Gn : Ae = !1;
-for (Ft in Ic)(os = (Gn = M[Ft]) && Gn.prototype) && (dd(os).TypedArrayConstructor = Gn);
-if ((!Ae || !rt(oe) || oe === Function.prototype) && (oe = function() {
+for (Ft in Ie)(os = (Gn = M[Ft]) && Gn.prototype) ? yd(os).TypedArrayConstructor = Gn : Ae = !1;
+for (Ft in wc)(os = (Gn = M[Ft]) && Gn.prototype) && (yd(os).TypedArrayConstructor = Gn);
+if ((!Ae || !rt(ae) || ae === Function.prototype) && (ae = function() {
         throw Yo("Incorrect invocation")
     }, Ae))
-    for (Ft in Ie) M[Ft] && he(M[Ft], oe);
-if ((!Ae || !Zt || Zt === Fw) && (Zt = oe.prototype, Ae))
-    for (Ft in Ie) M[Ft] && he(M[Ft].prototype, Zt);
-if (Ae && Je(qu) !== Zt && he(qu, Zt), J && !A(Zt, Qu))
-    for (Ft in pd = !0, Bw(Zt, Qu, {
+    for (Ft in Ie) M[Ft] && he(M[Ft], ae);
+if ((!Ae || !Ht || Ht === xw) && (Ht = ae.prototype, Ae))
+    for (Ft in Ie) M[Ft] && he(M[Ft].prototype, Ht);
+if (Ae && qe(tl) !== Ht && he(tl, Ht), J && !A(Ht, el))
+    for (Ft in bd = !0, Ow(Ht, el, {
             get: function() {
                 return st(this) ? this[Go] : void 0
             }
         }), Ie) M[Ft] && Us(M[Ft], Go, Ft);
 var Vs = {
         NATIVE_ARRAY_BUFFER_VIEWS: Ae,
-        TYPED_ARRAY_TAG: pd && Go,
+        TYPED_ARRAY_TAG: bd && Go,
         aTypedArray: function(e) {
-            if (tl(e)) return e;
+            if (nl(e)) return e;
             throw Yo("Target is not a typed array")
         },
         aTypedArrayConstructor: function(e) {
-            if (rt(e) && (!he || vn(oe, e))) return e;
+            if (rt(e) && (!he || wn(ae, e))) return e;
             throw Yo(fr(e) + " is not a typed array constructor")
         },
         exportTypedArrayMethod: function(e, t, n, r) {
             if (J) {
                 if (n)
                     for (var s in Ie) {
                         var o = M[s];
@@ -12386,108 +12386,108 @@
                             delete o.prototype[e]
                         } catch {
                             try {
                                 o.prototype[e] = t
                             } catch {}
                         }
                     }
-                Zt[e] && !n || It(Zt, e, n ? t : Ae && $o[e] || t, r)
+                Ht[e] && !n || It(Ht, e, n ? t : Ae && $o[e] || t, r)
             }
         },
         exportTypedArrayStaticMethod: function(e, t, n) {
             var r, s;
             if (J) {
                 if (he) {
                     if (n) {
                         for (r in Ie)
                             if ((s = M[r]) && A(s, e)) try {
                                 delete s[e]
                             } catch {}
                     }
-                    if (oe[e] && !n) return;
+                    if (ae[e] && !n) return;
                     try {
-                        return It(oe, e, n ? t : Ae && oe[e] || t)
+                        return It(ae, e, n ? t : Ae && ae[e] || t)
                     } catch {}
                 }
                 for (r in Ie) !(s = M[r]) || s[e] && !n || It(s, e, t)
             }
         },
-        getTypedArrayConstructor: yd,
+        getTypedArrayConstructor: md,
         isView: function(e) {
             if (!st(e)) return !1;
-            var t = Bn(e);
-            return t === "DataView" || A(Ie, t) || A(Ic, t)
+            var t = On(e);
+            return t === "DataView" || A(Ie, t) || A(wc, t)
         },
-        isTypedArray: tl,
-        TypedArray: oe,
-        TypedArrayPrototype: Zt
-    },
-    xw = TypeError,
-    Lw = ut("species"),
-    Dw = function(e, t) {
+        isTypedArray: nl,
+        TypedArray: ae,
+        TypedArrayPrototype: Ht
+    },
+    Lw = TypeError,
+    Dw = ut("species"),
+    kw = function(e, t) {
         var n, r = ht(e).constructor;
-        return r === void 0 || (n = ht(r)[Lw]) == null ? t : function(s) {
-            if (bc(s)) return s;
-            throw xw(fr(s) + " is not a constructor")
+        return r === void 0 || (n = ht(r)[Dw]) == null ? t : function(s) {
+            if (dc(s)) return s;
+            throw Lw(fr(s) + " is not a constructor")
         }(n)
     },
-    kw = Vs.aTypedArrayConstructor,
-    Ew = Vs.getTypedArrayConstructor,
-    Uw = Vs.aTypedArray;
+    Ew = Vs.aTypedArrayConstructor,
+    Uw = Vs.getTypedArrayConstructor,
+    Nw = Vs.aTypedArray;
 (0, Vs.exportTypedArrayMethod)("slice", function(e, t) {
-    for (var n, r = vc(Uw(this), e, t), s = kw(Dw(n = this, Ew(n))), o = 0, i = r.length, a = new s(i); i > o;) a[o] = r[o++];
+    for (var n, r = bc(Nw(this), e, t), s = Ew(kw(n = this, Uw(n))), o = 0, i = r.length, a = new s(i); i > o;) a[o] = r[o++];
     return a
 }, nt(function() {
     new Int8Array(1).slice()
 }));
-var Nw = vt.f,
+var Mw = vt.f,
     Ko = ut("unscopables"),
     Zo = Array.prototype;
-Zo[Ko] == null && Nw(Zo, Ko, {
+Zo[Ko] == null && Mw(Zo, Ko, {
     configurable: !0,
-    value: He(null)
+    value: Xe(null)
 });
 var ki = function(e) {
         Zo[Ko][e] = !0
     },
-    Mw = Nh.includes,
-    Cw = nt(function() {
+    Cw = Ch.includes,
+    Rw = nt(function() {
         return !Array(1).includes()
     });
 dt({
     target: "Array",
     proto: !0,
-    forced: Cw
+    forced: Rw
 }, {
     includes: function(e) {
-        return Mw(this, e, arguments.length > 1 ? arguments[1] : void 0)
+        return Cw(this, e, arguments.length > 1 ? arguments[1] : void 0)
     }
-}), ki("includes"), pc("Array", "includes");
-var Rw = P("".indexOf);
+}), ki("includes"), fc("Array", "includes");
+var Vw = P("".indexOf);
 dt({
     target: "String",
     proto: !0,
-    forced: !jh("includes")
+    forced: !zh("includes")
 }, {
     includes: function(e) {
-        return !!~Rw(Oe(si(this)), Oe(Vh(e)), arguments.length > 1 ? arguments[1] : void 0)
+        return !!~Vw(Oe(si(this)), Oe(Ph(e)), arguments.length > 1 ? arguments[1] : void 0)
     }
-}), pc("String", "includes");
-var Vw = vt.f,
-    jw = Wt.set,
-    Pw = Wt.getterFor("Array Iterator");
-_c(Array, "Array", function(e, t) {
-    jw(this, {
+}), fc("String", "includes");
+var jw = vt.f,
+    Pw = $t.set,
+    zw = $t.getterFor("Array Iterator");
+gc(Array, "Array", function(e, t) {
+    Pw(this, {
         type: "Array Iterator",
         target: be(e),
         index: 0,
         kind: t
     })
 }, function() {
-    var e = Pw(this),
+    var e = zw(this),
         t = e.target,
         n = e.kind,
         r = e.index++;
     return !t || r >= t.length ? (e.target = void 0, {
         value: void 0,
         done: !0
     }) : n == "keys" ? {
@@ -12497,38 +12497,38 @@
         value: t[r],
         done: !1
     } : {
         value: [r, t[r]],
         done: !1
     }
 }, "values");
-var el = ar.Arguments = ar.Array;
-if (ki("keys"), ki("values"), ki("entries"), J && el.name !== "values") try {
-    Vw(el, "name", {
+var rl = ar.Arguments = ar.Array;
+if (ki("keys"), ki("values"), ki("entries"), J && rl.name !== "values") try {
+    jw(rl, "name", {
         value: "values"
     })
 } catch {}
-var nl = nt(function() {
+var il = nt(function() {
         if (typeof ArrayBuffer == "function") {
             var e = new ArrayBuffer(8);
             Object.isExtensible(e) && Object.defineProperty(e, "a", {
                 value: 8
             })
         }
     }),
     Si = Object.isExtensible,
     ho = nt(function() {
         Si(1)
-    }) || nl ? function(e) {
-        return !!st(e) && (!nl || Te(e) != "ArrayBuffer") && (!Si || Si(e))
+    }) || il ? function(e) {
+        return !!st(e) && (!il || Te(e) != "ArrayBuffer") && (!Si || Si(e))
     } : Si,
-    zw = !nt(function() {
+    Ww = !nt(function() {
         return Object.isExtensible(Object.preventExtensions({}))
     }),
-    jn = lr(function(e) {
+    Vn = lr(function(e) {
         var t = vt.f,
             n = !1,
             r = or("meta"),
             s = 0,
             o = function(a) {
                 t(a, r, {
                     value: {
@@ -12550,15 +12550,15 @@
                                 break
                             } return f
                     }, dt({
                         target: "Object",
                         stat: !0,
                         forced: !0
                     }, {
-                        getOwnPropertyNames: gc.f
+                        getOwnPropertyNames: yc.f
                     }))
                 },
                 fastKey: function(a, c) {
                     if (!st(a)) return typeof a == "symbol" ? a : (typeof a == "string" ? "S" : "P") + a;
                     if (!A(a, r)) {
                         if (!ho(a)) return "F";
                         if (!c) return "E";
@@ -12571,26 +12571,26 @@
                         if (!ho(a)) return !0;
                         if (!c) return !1;
                         o(a)
                     }
                     return a[r].weakData
                 },
                 onFreeze: function(a) {
-                    return zw && n && ho(a) && !A(a, r) && o(a), a
+                    return Ww && n && ho(a) && !A(a, r) && o(a), a
                 }
             };
         dr[r] = !0
     });
-jn.enable, jn.fastKey, jn.getWeakData, jn.onFreeze;
-var Ww = TypeError,
+Vn.enable, Vn.fastKey, Vn.getWeakData, Vn.onFreeze;
+var $w = TypeError,
     Ei = function(e, t) {
         this.stopped = e, this.result = t
     },
-    rl = Ei.prototype,
-    bd = function(e, t, n) {
+    sl = Ei.prototype,
+    gd = function(e, t, n) {
         var r, s, o, i, a, c, u, l = n && n.that,
             f = !(!n || !n.AS_ENTRIES),
             h = !(!n || !n.IS_RECORD),
             p = !(!n || !n.IS_ITERATOR),
             w = !(!n || !n.INTERRUPTED),
             _ = Cs(t, l),
             b = function(v) {
@@ -12598,82 +12598,82 @@
             },
             g = function(v) {
                 return f ? (ht(v), w ? _(v[0], v[1], b) : _(v[0], v[1])) : w ? _(v, b) : _(v)
             };
         if (h) r = e.iterator;
         else if (p) r = e;
         else {
-            if (!(s = Sc(e))) throw Ww(fr(e) + " is not iterable");
-            if (cd(s)) {
+            if (!(s = vc(e))) throw $w(fr(e) + " is not iterable");
+            if (ld(s)) {
                 for (o = 0, i = pr(e); i > o; o++)
-                    if ((a = g(e[o])) && vn(rl, a)) return a;
+                    if ((a = g(e[o])) && wn(sl, a)) return a;
                 return new Ei(!1)
             }
-            r = ud(e, s)
+            r = fd(e, s)
         }
         for (c = h ? e.next : r.next; !(u = St(c, r)).done;) {
             try {
                 a = g(u.value)
             } catch (v) {
                 Wo(r, "throw", v)
             }
-            if (typeof a == "object" && a && vn(rl, a)) return a
+            if (typeof a == "object" && a && wn(sl, a)) return a
         }
         return new Ei(!1)
     },
-    $w = TypeError,
-    md = function(e, t) {
-        if (vn(t, e)) return e;
-        throw $w("Incorrect invocation")
+    Yw = TypeError,
+    vd = function(e, t) {
+        if (wn(t, e)) return e;
+        throw Yw("Incorrect invocation")
     },
-    il = function(e, t, n) {
+    ol = function(e, t, n) {
         for (var r in t) It(e, r, t[r], n);
         return e
     },
-    sl = ut("species"),
-    Yw = vt.f,
-    ol = jn.fastKey,
-    al = Wt.set,
-    po = Wt.getterFor,
-    Gw = {
+    al = ut("species"),
+    Gw = vt.f,
+    cl = Vn.fastKey,
+    ul = $t.set,
+    po = $t.getterFor,
+    Kw = {
         getConstructor: function(e, t, n, r) {
             var s = e(function(u, l) {
-                    md(u, o), al(u, {
+                    vd(u, o), ul(u, {
                         type: t,
-                        index: He(null),
+                        index: Xe(null),
                         first: void 0,
                         last: void 0,
                         size: 0
-                    }), J || (u.size = 0), l != null && bd(l, u[r], {
+                    }), J || (u.size = 0), l != null && gd(l, u[r], {
                         that: u,
                         AS_ENTRIES: n
                     })
                 }),
                 o = s.prototype,
                 i = po(t),
                 a = function(u, l, f) {
                     var h, p, w = i(u),
                         _ = c(u, l);
                     return _ ? _.value = f : (w.last = _ = {
-                        index: p = ol(l, !0),
+                        index: p = cl(l, !0),
                         key: l,
                         value: f,
                         previous: h = w.last,
                         next: void 0,
                         removed: !1
                     }, w.first || (w.first = _), h && (h.next = _), J ? w.size++ : u.size++, p !== "F" && (w.index[p] = _)), u
                 },
                 c = function(u, l) {
                     var f, h = i(u),
-                        p = ol(l);
+                        p = cl(l);
                     if (p !== "F") return h.index[p];
                     for (f = h.first; f; f = f.next)
                         if (f.key == l) return f
                 };
-            return il(o, {
+            return ol(o, {
                 clear: function() {
                     for (var u = i(this), l = u.index, f = u.first; f;) f.removed = !0, f.previous && (f.previous = f.previous.next = void 0), delete l[f.index], f = f.next;
                     u.first = u.last = void 0, J ? u.size = 0 : this.size = 0
                 },
                 delete: function(u) {
                     var l = this,
                         f = i(l),
@@ -12688,38 +12688,38 @@
                 forEach: function(u) {
                     for (var l, f = i(this), h = Cs(u, arguments.length > 1 ? arguments[1] : void 0); l = l ? l.next : f.first;)
                         for (h(l.value, l.key, this); l && l.removed;) l = l.previous
                 },
                 has: function(u) {
                     return !!c(this, u)
                 }
-            }), il(o, n ? {
+            }), ol(o, n ? {
                 get: function(u) {
                     var l = c(this, u);
                     return l && l.value
                 },
                 set: function(u, l) {
                     return a(this, u === 0 ? 0 : u, l)
                 }
             } : {
                 add: function(u) {
                     return a(this, u = u === 0 ? 0 : u, u)
                 }
-            }), J && Yw(o, "size", {
+            }), J && Gw(o, "size", {
                 get: function() {
                     return i(this).size
                 }
             }), s
         },
         setStrong: function(e, t, n) {
             var r = t + " Iterator",
                 s = po(t),
                 o = po(r);
-            _c(e, t, function(i, a) {
-                    al(this, {
+            gc(e, t, function(i, a) {
+                    ul(this, {
                         type: r,
                         target: i,
                         state: s(i),
                         kind: a,
                         last: void 0
                     })
                 }, function() {
@@ -12735,40 +12735,40 @@
                         done: !1
                     } : (i.target = void 0, {
                         value: void 0,
                         done: !0
                     })
                 }, n ? "entries" : "values", !n, !0),
                 function(i) {
-                    var a = ie(i),
+                    var a = se(i),
                         c = vt.f;
-                    J && a && !a[sl] && c(a, sl, {
+                    J && a && !a[al] && c(a, al, {
                         configurable: !0,
                         get: function() {
                             return this
                         }
                     })
                 }(t)
         }
     };
 
-function gd(e) {
+function wd(e) {
     var t = this.constructor;
     return this.then(function(n) {
         return t.resolve(e()).then(function() {
             return n
         })
     }, function(n) {
         return t.resolve(e()).then(function() {
             return t.reject(n)
         })
     })
 }
 
-function vd(e) {
+function _d(e) {
     return new this(function(t, n) {
         if (!e || e.length === void 0) return n(new TypeError(typeof e + " " + e + " is not iterable(cannot read property Symbol(Symbol.iterator))"));
         var r = Array.prototype.slice.call(e);
         if (r.length === 0) return t([]);
         var s = r.length;
 
         function o(a, c) {
@@ -12810,65 +12810,65 @@
                 return !(s && !st(v)) && g(this, v === 0 ? 0 : v)
             } : function(v, I) {
                 return g(this, v === 0 ? 0 : v, I), this
             })
         };
     if (Ro(e, !rt(i) || !(s || a.forEach && !nt(function() {
             new i().entries().next()
-        })))) c = n.getConstructor(t, e, r, o), jn.enable();
+        })))) c = n.getConstructor(t, e, r, o), Vn.enable();
     else if (Ro(e, !0)) {
         var f = new c,
             h = f[o](s ? {} : -0, 1) != f,
             p = nt(function() {
                 f.has(1)
             }),
-            w = hd(function(b) {
+            w = pd(function(b) {
                 new i(b)
             }),
             _ = !s && nt(function() {
                 for (var b = new i, g = 5; g--;) b[o](g, g);
                 return !b.has(-0)
             });
         w || ((c = t(function(b, g) {
-            md(b, a);
+            vd(b, a);
             var v = function(I, it, yt) {
                 var Dt, me;
                 return he && rt(Dt = it.constructor) && Dt !== yt && st(me = Dt.prototype) && me !== yt.prototype && he(I, me), I
             }(new i, b, c);
-            return g != null && bd(g, v[o], {
+            return g != null && gd(g, v[o], {
                 that: v,
                 AS_ENTRIES: r
             }), v
         })).prototype = a, a.constructor = c), (p || _) && (l("delete"), l("has"), r && l("get")), (_ || h) && l(o), s && a.clear && delete a.clear
     }
     u[e] = c, dt({
         global: !0,
         constructor: !0,
         forced: c != i
     }, u), Pe(c, e), s || n.setStrong(c, e, r)
 })("Set", function(e) {
     return function() {
         return e(this, arguments.length ? arguments[0] : void 0)
     }
-}, Gw), Pr.Set;
-var Kw = setTimeout;
+}, Kw), Pr.Set;
+var Zw = setTimeout;
 
-function cl(e) {
+function ll(e) {
     return Boolean(e && e.length !== void 0)
 }
 
-function Zw() {}
+function Hw() {}
 
 function ct(e) {
     if (!(this instanceof ct)) throw new TypeError("Promises must be constructed via new");
     if (typeof e != "function") throw new TypeError("not a function");
-    this._state = 0, this._handled = !1, this._value = void 0, this._deferreds = [], _d(e, this)
+    this._state = 0, this._handled = !1, this._value = void 0, this._deferreds = [], Id(e, this)
 }
 
-function wd(e, t) {
+function Sd(e, t) {
     for (; e._state === 3;) e = e._value;
     e._state !== 0 ? (e._handled = !0, ct._immediateFn(function() {
         var n = e._state === 1 ? t.onFulfilled : t.onRejected;
         if (n !== null) {
             var r;
             try {
                 r = n(e._value)
@@ -12882,15 +12882,15 @@
 
 function Ho(e, t) {
     try {
         if (t === e) throw new TypeError("A promise cannot be resolved with itself.");
         if (t && (typeof t == "object" || typeof t == "function")) {
             var n = t.then;
             if (t instanceof ct) return e._state = 3, e._value = t, void Jo(e);
-            if (typeof n == "function") return void _d((r = n, s = t, function() {
+            if (typeof n == "function") return void Id((r = n, s = t, function() {
                 r.apply(s, arguments)
             }), e)
         }
         e._state = 1, e._value = t, Jo(e)
     } catch (o) {
         zr(e, o)
     }
@@ -12901,23 +12901,23 @@
     e._state = 2, e._value = t, Jo(e)
 }
 
 function Jo(e) {
     e._state === 2 && e._deferreds.length === 0 && ct._immediateFn(function() {
         e._handled || ct._unhandledRejectionFn(e._value)
     });
-    for (var t = 0, n = e._deferreds.length; t < n; t++) wd(e, e._deferreds[t]);
+    for (var t = 0, n = e._deferreds.length; t < n; t++) Sd(e, e._deferreds[t]);
     e._deferreds = null
 }
 
-function Hw(e, t, n) {
+function Jw(e, t, n) {
     this.onFulfilled = typeof e == "function" ? e : null, this.onRejected = typeof t == "function" ? t : null, this.promise = n
 }
 
-function _d(e, t) {
+function Id(e, t) {
     var n = !1;
     try {
         e(function(r) {
             n || (n = !0, Ho(t, r))
         }, function(r) {
             n || (n = !0, zr(t, r))
         })
@@ -12925,19 +12925,19 @@
         if (n) return;
         n = !0, zr(t, r)
     }
 }
 ct.prototype.catch = function(e) {
     return this.then(null, e)
 }, ct.prototype.then = function(e, t) {
-    var n = new this.constructor(Zw);
-    return wd(this, new Hw(e, t, n)), n
-}, ct.prototype.finally = gd, ct.all = function(e) {
+    var n = new this.constructor(Hw);
+    return Sd(this, new Jw(e, t, n)), n
+}, ct.prototype.finally = wd, ct.all = function(e) {
     return new ct(function(t, n) {
-        if (!cl(e)) return n(new TypeError("Promise.all accepts an array"));
+        if (!ll(e)) return n(new TypeError("Promise.all accepts an array"));
         var r = Array.prototype.slice.call(e);
         if (r.length === 0) return t([]);
         var s = r.length;
 
         function o(a, c) {
             try {
                 if (c && (typeof c == "object" || typeof c == "function")) {
@@ -12949,41 +12949,41 @@
                 r[a] = c, --s == 0 && t(r)
             } catch (l) {
                 n(l)
             }
         }
         for (var i = 0; i < r.length; i++) o(i, r[i])
     })
-}, ct.allSettled = vd, ct.resolve = function(e) {
+}, ct.allSettled = _d, ct.resolve = function(e) {
     return e && typeof e == "object" && e.constructor === ct ? e : new ct(function(t) {
         t(e)
     })
 }, ct.reject = function(e) {
     return new ct(function(t, n) {
         n(e)
     })
 }, ct.race = function(e) {
     return new ct(function(t, n) {
-        if (!cl(e)) return n(new TypeError("Promise.race accepts an array"));
+        if (!ll(e)) return n(new TypeError("Promise.race accepts an array"));
         for (var r = 0, s = e.length; r < s; r++) ct.resolve(e[r]).then(t, n)
     })
 }, ct._immediateFn = typeof setImmediate == "function" && function(e) {
     setImmediate(e)
 } || function(e) {
-    Kw(e, 0)
+    Zw(e, 0)
 }, ct._unhandledRejectionFn = function(e) {
     typeof console < "u" && console && console.warn("Possible Unhandled Promise Rejection:", e)
 };
-var Ln = function() {
+var Dn = function() {
     if (typeof self < "u") return self;
     if (typeof window < "u") return window;
     if (typeof global < "u") return global;
     throw new Error("unable to locate global object")
 }();
-typeof Ln.Promise != "function" ? Ln.Promise = ct : (Ln.Promise.prototype.finally || (Ln.Promise.prototype.finally = gd), Ln.Promise.allSettled || (Ln.Promise.allSettled = vd)),
+typeof Dn.Promise != "function" ? Dn.Promise = ct : (Dn.Promise.prototype.finally || (Dn.Promise.prototype.finally = wd), Dn.Promise.allSettled || (Dn.Promise.allSettled = _d)),
     function(e) {
         function t() {}
 
         function n(i, a) {
             if (i = i === void 0 ? "utf-8" : i, a = a === void 0 ? {
                     fatal: !1
                 } : a, s.indexOf(i.toLowerCase()) === -1) throw new RangeError("Failed to construct 'TextDecoder': The encoding label provided ('" + i + "') is invalid.");
@@ -13062,15 +13062,15 @@
             }
         }), n.prototype.decode = function(i, a) {
             if ((a = a === void 0 ? {
                     stream: !1
                 } : a).stream) throw Error("Failed to decode: the 'stream' option is unsupported.");
             return i = i instanceof Uint8Array ? i : i.buffer instanceof ArrayBuffer ? new Uint8Array(i.buffer) : new Uint8Array(i), o(i)
         }, e.TextEncoder = t, e.TextDecoder = n
-    }(typeof window < "u" ? window : ce),
+    }(typeof window < "u" ? window : ue),
     function() {
         function e(b, g) {
             if (!(b instanceof g)) throw new TypeError("Cannot call a class as a function")
         }
 
         function t(b, g) {
             for (var v = 0; v < g.length; v++) {
@@ -13256,17 +13256,17 @@
 
         function _(b) {
             return b.__FORCE_INSTALL_ABORTCONTROLLER_POLYFILL ? (console.log("__FORCE_INSTALL_ABORTCONTROLLER_POLYFILL=true is set, will force install polyfill"), !0) : typeof b.Request == "function" && !b.Request.prototype.hasOwnProperty("signal") || !b.AbortController
         }
         typeof Symbol < "u" && Symbol.toStringTag && (w.prototype[Symbol.toStringTag] = "AbortController", p.prototype[Symbol.toStringTag] = "AbortSignal"),
             function(b) {
                 _(b) && (b.AbortController = w, b.AbortSignal = p)
-            }(typeof self < "u" ? self : ce)
+            }(typeof self < "u" ? self : ue)
     }();
-var on = lr(function(e, t) {
+var cn = lr(function(e, t) {
     Object.defineProperty(t, "__esModule", {
         value: !0
     });
     var n = function() {
         function r() {
             var s = this;
             this.locked = new Map, this.addToLocked = function(o, i) {
@@ -13290,17 +13290,17 @@
             return r.instance === void 0 && (r.instance = new r), r.instance
         }, r
     }();
     t.default = function() {
         return n.getInstance()
     }
 });
-sc(on);
-var Jw = lr(function(e, t) {
-        var n = ce && ce.__awaiter || function(c, u, l, f) {
+nc(cn);
+var Xw = lr(function(e, t) {
+        var n = ue && ue.__awaiter || function(c, u, l, f) {
                 return new(l || (l = Promise))(function(h, p) {
                     function w(g) {
                         try {
                             b(f.next(g))
                         } catch (v) {
                             p(v)
                         }
@@ -13318,15 +13318,15 @@
                         g.done ? h(g.value) : new l(function(v) {
                             v(g.value)
                         }).then(w, _)
                     }
                     b((f = f.apply(c, u || [])).next())
                 })
             },
-            r = ce && ce.__generator || function(c, u) {
+            r = ue && ue.__generator || function(c, u) {
                 var l, f, h, p, w = {
                     label: 0,
                     sent: function() {
                         if (1 & h[0]) throw h[1];
                         return h[1]
                     },
                     trys: [],
@@ -13454,17 +13454,17 @@
                     return r(this, function(h) {
                         return setTimeout(function() {
                             return n(f, void 0, void 0, function() {
                                 var p, w;
                                 return r(this, function(_) {
                                     switch (_.label) {
                                         case 0:
-                                            return [4, on.default().lock(l)];
+                                            return [4, cn.default().lock(l)];
                                         case 1:
-                                            return _.sent(), this.acquiredIatSet.has(l) ? (p = window.localStorage, (w = p.getItem(u)) === null ? (on.default().unlock(l), [2]) : ((w = JSON.parse(w)).timeRefreshed = Date.now(), p.setItem(u, JSON.stringify(w)), on.default().unlock(l), this.refreshLockWhileAcquired(u, l), [2])) : (on.default().unlock(l), [2])
+                                            return _.sent(), this.acquiredIatSet.has(l) ? (p = window.localStorage, (w = p.getItem(u)) === null ? (cn.default().unlock(l), [2]) : ((w = JSON.parse(w)).timeRefreshed = Date.now(), p.setItem(u, JSON.stringify(w)), cn.default().unlock(l), this.refreshLockWhileAcquired(u, l), [2])) : (cn.default().unlock(l), [2])
                                     }
                                 })
                             })
                         }, 1e3), [2]
                     })
                 })
             }, c.prototype.waitForSomethingToChange = function(u) {
@@ -13515,17 +13515,17 @@
                 })
             }, c.prototype.releaseLock__private__ = function(u) {
                 return n(this, void 0, void 0, function() {
                     var l, f, h;
                     return r(this, function(p) {
                         switch (p.label) {
                             case 0:
-                                return l = window.localStorage, f = s + "-" + u, (h = l.getItem(f)) === null ? [2] : (h = JSON.parse(h)).id !== this.id ? [3, 2] : [4, on.default().lock(h.iat)];
+                                return l = window.localStorage, f = s + "-" + u, (h = l.getItem(f)) === null ? [2] : (h = JSON.parse(h)).id !== this.id ? [3, 2] : [4, cn.default().lock(h.iat)];
                             case 1:
-                                p.sent(), this.acquiredIatSet.delete(h.iat), l.removeItem(f), on.default().unlock(h.iat), c.notifyWaiters(), p.label = 2;
+                                p.sent(), this.acquiredIatSet.delete(h.iat), l.removeItem(f), cn.default().unlock(h.iat), c.notifyWaiters(), p.label = 2;
                             case 2:
                                 return [2]
                         }
                     })
                 })
             }, c.lockCorrector = function() {
                 for (var u = Date.now() - 5e3, l = window.localStorage, f = Object.keys(l), h = !1, p = 0; p < f.length; p++) {
@@ -13536,109 +13536,109 @@
                     }
                 }
                 h && c.notifyWaiters()
             }, c.waiters = void 0, c
         }();
         t.default = a
     }),
-    Xw = sc(Jw),
-    qw = {
+    qw = nc(Xw),
+    Qw = {
         timeoutInSeconds: 60
     },
-    Qw = ["login_required", "consent_required", "interaction_required", "account_selection_required", "access_denied"],
-    Sd = {
+    t_ = ["login_required", "consent_required", "interaction_required", "account_selection_required", "access_denied"],
+    Td = {
         name: "auth0-spa-js",
         version: "1.22.4"
     },
-    Id = function() {
+    Ad = function() {
         return Date.now()
     },
     xe = function(e) {
         function t(n, r) {
             var s = e.call(this, r) || this;
             return s.error = n, s.error_description = r, Object.setPrototypeOf(s, t.prototype), s
         }
-        return An(t, e), t.fromPayload = function(n) {
+        return Bn(t, e), t.fromPayload = function(n) {
             return new t(n.error, n.error_description)
         }, t
     }(Error),
-    t_ = function(e) {
+    e_ = function(e) {
         function t(n, r, s, o) {
             o === void 0 && (o = null);
             var i = e.call(this, n, r) || this;
             return i.state = s, i.appState = o, Object.setPrototypeOf(i, t.prototype), i
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(xe),
     Xo = function(e) {
         function t() {
             var n = e.call(this, "timeout", "Timeout") || this;
             return Object.setPrototypeOf(n, t.prototype), n
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(xe),
-    e_ = function(e) {
+    n_ = function(e) {
         function t(n) {
             var r = e.call(this) || this;
             return r.popup = n, Object.setPrototypeOf(r, t.prototype), r
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(Xo),
-    n_ = function(e) {
+    r_ = function(e) {
         function t(n) {
             var r = e.call(this, "cancelled", "Popup closed") || this;
             return r.popup = n, Object.setPrototypeOf(r, t.prototype), r
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(xe),
-    r_ = function(e) {
+    i_ = function(e) {
         function t(n, r, s) {
             var o = e.call(this, n, r) || this;
             return o.mfa_token = s, Object.setPrototypeOf(o, t.prototype), o
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(xe),
-    i_ = function(e) {
+    s_ = function(e) {
         function t(n, r) {
-            var s = e.call(this, "missing_refresh_token", "Missing Refresh Token (audience: '".concat(ll(n, ["default"]), "', scope: '").concat(ll(r), "')")) || this;
+            var s = e.call(this, "missing_refresh_token", "Missing Refresh Token (audience: '".concat(hl(n, ["default"]), "', scope: '").concat(hl(r), "')")) || this;
             return s.audience = n, s.scope = r, Object.setPrototypeOf(s, t.prototype), s
         }
-        return An(t, e), t
+        return Bn(t, e), t
     }(xe),
-    s_ = function(e) {
+    o_ = function(e) {
         return new Promise(function(t, n) {
             var r, s = setInterval(function() {
-                    e.popup && e.popup.closed && (clearInterval(s), clearTimeout(o), window.removeEventListener("message", r, !1), n(new n_(e.popup)))
+                    e.popup && e.popup.closed && (clearInterval(s), clearTimeout(o), window.removeEventListener("message", r, !1), n(new r_(e.popup)))
                 }, 1e3),
                 o = setTimeout(function() {
-                    clearInterval(s), n(new e_(e.popup)), window.removeEventListener("message", r, !1)
+                    clearInterval(s), n(new n_(e.popup)), window.removeEventListener("message", r, !1)
                 }, 1e3 * (e.timeoutInSeconds || 60));
             r = function(i) {
                 if (i.data && i.data.type === "authorization_response") {
                     if (clearTimeout(o), clearInterval(s), window.removeEventListener("message", r, !1), e.popup.close(), i.data.response.error) return n(xe.fromPayload(i.data.response));
                     t(i.data.response)
                 }
             }, window.addEventListener("message", r)
         })
     },
-    Tc = function() {
+    _c = function() {
         return window.crypto || window.msCrypto
     },
-    Td = function() {
-        var e = Tc();
+    Bd = function() {
+        var e = _c();
         return e.subtle || e.webkitSubtle
     },
     ge = function() {
         var e = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz-_~.",
             t = "";
-        return Array.from(Tc().getRandomValues(new Uint8Array(43))).forEach(function(n) {
+        return Array.from(_c().getRandomValues(new Uint8Array(43))).forEach(function(n) {
             return t += e[n % e.length]
         }), t
     },
-    Dn = function(e) {
+    kn = function(e) {
         return btoa(e)
     },
     qo = function(e) {
         return Object.keys(e).filter(function(t) {
             return e[t] !== void 0
         }).map(function(t) {
             return encodeURIComponent(t) + "=" + encodeURIComponent(e[t])
@@ -13646,15 +13646,15 @@
     },
     yo = function(e) {
         return $(void 0, void 0, void 0, function() {
             var t;
             return Y(this, function(n) {
                 switch (n.label) {
                     case 0:
-                        return t = Td().digest({
+                        return t = Bd().digest({
                             name: "SHA-256"
                         }, new TextEncoder().encode(e)), window.msCrypto ? [2, new Promise(function(r, s) {
                             t.oncomplete = function(o) {
                                 r(o.target.result)
                             }, t.onerror = function(o) {
                                 s(o.error)
                             }, t.onabort = function() {
@@ -13663,15 +13663,15 @@
                         })] : [4, t];
                     case 1:
                         return [2, n.sent()]
                 }
             })
         })
     },
-    ul = function(e) {
+    fl = function(e) {
         return function(t) {
             return decodeURIComponent(atob(t).split("").map(function(n) {
                 return "%" + ("00" + n.charCodeAt(0).toString(16)).slice(-2)
             }).join(""))
         }(e.replace(/_/g, "/").replace(/-/g, "+"))
     },
     bo = function(e) {
@@ -13684,18 +13684,18 @@
             };
             return n.replace(/[+/=]/g, function(s) {
                 return r[s]
             })
         }(window.btoa(String.fromCharCode.apply(String, Eo([], ir(Array.from(t)), !1))))
     };
 
-function ll(e, t) {
+function hl(e, t) {
     return t === void 0 && (t = []), e && !t.includes(e) ? e : ""
 }
-var o_ = function(e, t) {
+var a_ = function(e, t) {
         return $(void 0, void 0, void 0, function() {
             var n, r;
             return Y(this, function(s) {
                 switch (s.label) {
                     case 0:
                         return [4, (o = e, i = t, i = i || {}, new Promise(function(a, c) {
                             var u = new XMLHttpRequest,
@@ -13748,29 +13748,29 @@
                     case 2:
                         return [2, (r.json = s.sent(), r)]
                 }
                 var o, i
             })
         })
     },
-    a_ = function(e, t, n) {
+    c_ = function(e, t, n) {
         return $(void 0, void 0, void 0, function() {
             var r, s;
             return Y(this, function(o) {
-                return r = new AbortController, t.signal = r.signal, [2, Promise.race([o_(e, t), new Promise(function(i, a) {
+                return r = new AbortController, t.signal = r.signal, [2, Promise.race([a_(e, t), new Promise(function(i, a) {
                     s = setTimeout(function() {
                         r.abort(), a(new Error("Timeout when executing 'fetch'"))
                     }, n)
                 })]).finally(function() {
                     clearTimeout(s)
                 })]
             })
         })
     },
-    c_ = function(e, t, n, r, s, o, i) {
+    u_ = function(e, t, n, r, s, o, i) {
         return $(void 0, void 0, void 0, function() {
             return Y(this, function(a) {
                 return [2, (c = {
                     auth: {
                         audience: t,
                         scope: n
                     },
@@ -13784,43 +13784,43 @@
                         p.data.error ? f(new Error(p.data.error)) : l(p.data)
                     }, u.postMessage(c, [h.port2])
                 }))];
                 var c, u
             })
         })
     },
-    u_ = function(e, t, n, r, s, o, i) {
+    l_ = function(e, t, n, r, s, o, i) {
         return i === void 0 && (i = 1e4), $(void 0, void 0, void 0, function() {
             return Y(this, function(a) {
-                return s ? [2, c_(e, t, n, r, i, s, o)] : [2, a_(e, r, i)]
+                return s ? [2, u_(e, t, n, r, i, s, o)] : [2, c_(e, r, i)]
             })
         })
     };
 
-function l_(e, t, n, r, s, o, i) {
+function f_(e, t, n, r, s, o, i) {
     return $(this, void 0, void 0, function() {
         var a, c, u, l, f, h, p, w, _;
         return Y(this, function(b) {
             switch (b.label) {
                 case 0:
                     a = null, u = 0, b.label = 1;
                 case 1:
                     if (!(u < 3)) return [3, 6];
                     b.label = 2;
                 case 2:
-                    return b.trys.push([2, 4, , 5]), [4, u_(e, n, r, s, o, i, t)];
+                    return b.trys.push([2, 4, , 5]), [4, l_(e, n, r, s, o, i, t)];
                 case 3:
                     return c = b.sent(), a = null, [3, 6];
                 case 4:
                     return l = b.sent(), a = l, [3, 5];
                 case 5:
                     return u++, [3, 1];
                 case 6:
                     if (a) throw a.message = a.message || "Failed to fetch", a;
-                    if (f = c.json, h = f.error, p = f.error_description, w = Tt(f, ["error", "error_description"]), !c.ok) throw _ = p || "HTTP error. Unable to fetch ".concat(e), h === "mfa_required" ? new r_(h, _, w.mfa_token) : new xe(h || "request_error", _);
+                    if (f = c.json, h = f.error, p = f.error_description, w = Tt(f, ["error", "error_description"]), !c.ok) throw _ = p || "HTTP error. Unable to fetch ".concat(e), h === "mfa_required" ? new i_(h, _, w.mfa_token) : new xe(h || "request_error", _);
                     return [2, w]
             }
         })
     })
 }
 
 function Ii(e, t) {
@@ -13832,36 +13832,36 @@
         a = e.useFormData,
         c = Tt(e, ["baseUrl", "timeout", "audience", "scope", "auth0Client", "useFormData"]);
     return $(this, void 0, void 0, function() {
         var u;
         return Y(this, function(l) {
             switch (l.label) {
                 case 0:
-                    return u = a ? qo(c) : JSON.stringify(c), [4, l_("".concat(n, "/oauth/token"), r, s || "default", o, {
+                    return u = a ? qo(c) : JSON.stringify(c), [4, f_("".concat(n, "/oauth/token"), r, s || "default", o, {
                         method: "POST",
                         body: u,
                         headers: {
                             "Content-Type": a ? "application/x-www-form-urlencoded" : "application/json",
-                            "Auth0-Client": btoa(JSON.stringify(i || Sd))
+                            "Auth0-Client": btoa(JSON.stringify(i || Td))
                         }
                     }, t, a)];
                 case 1:
                     return [2, l.sent()]
             }
         })
     })
 }
-var f_ = function(e) {
+var h_ = function(e) {
         return Array.from(new Set(e))
     },
     Ce = function() {
         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-        return f_(e.join(" ").trim().split(/\s+/)).join(" ")
+        return h_(e.join(" ").trim().split(/\s+/)).join(" ")
     },
-    an = function() {
+    un = function() {
         function e(t, n) {
             n === void 0 && (n = "@@auth0spajs@@"), this.prefix = n, this.client_id = t.client_id, this.scope = t.scope, this.audience = t.audience
         }
         return e.prototype.toKey = function() {
             return "".concat(this.prefix, "::").concat(this.client_id, "::").concat(this.audience, "::").concat(this.scope)
         }, e.fromKey = function(t) {
             var n = ir(t.split("::"), 4),
@@ -13877,15 +13877,15 @@
             return new e({
                 scope: t.scope,
                 audience: t.audience,
                 client_id: t.client_id
             })
         }, e
     }(),
-    h_ = function() {
+    d_ = function() {
         function e() {}
         return e.prototype.set = function(t, n) {
             localStorage.setItem(t, JSON.stringify(n))
         }, e.prototype.get = function(t) {
             var n = window.localStorage.getItem(t);
             if (n) try {
                 return JSON.parse(n)
@@ -13896,15 +13896,15 @@
             localStorage.removeItem(t)
         }, e.prototype.allKeys = function() {
             return Object.keys(window.localStorage).filter(function(t) {
                 return t.startsWith("@@auth0spajs@@")
             })
         }, e
     }(),
-    d_ = function() {
+    p_ = function() {
         var e;
         this.enclosedCache = (e = {}, {
             set: function(t, n) {
                 e[t] = n
             },
             get: function(t) {
                 var n = e[t];
@@ -13914,17 +13914,17 @@
                 delete e[t]
             },
             allKeys: function() {
                 return Object.keys(e)
             }
         })
     },
-    p_ = function() {
+    y_ = function() {
         function e(t, n, r) {
-            this.cache = t, this.keyManifest = n, this.nowProvider = r, this.nowProvider = this.nowProvider || Id
+            this.cache = t, this.keyManifest = n, this.nowProvider = r, this.nowProvider = this.nowProvider || Ad
         }
         return e.prototype.get = function(t, n) {
             var r;
             return n === void 0 && (n = 0), $(this, void 0, void 0, function() {
                 var s, o, i, a, c;
                 return Y(this, function(u) {
                     switch (u.label) {
@@ -13958,15 +13958,15 @@
         }, e.prototype.set = function(t) {
             var n;
             return $(this, void 0, void 0, function() {
                 var r, s;
                 return Y(this, function(o) {
                     switch (o.label) {
                         case 0:
-                            return r = new an({
+                            return r = new un({
                                 client_id: t.client_id,
                                 scope: t.scope,
                                 audience: t.audience
                             }), [4, this.wrapCacheEntry(t)];
                         case 1:
                             return s = o.sent(), [4, this.cache.set(r.toKey(), s)];
                         case 2:
@@ -14048,25 +14048,25 @@
                         case 4:
                             return [2, n]
                     }
                 })
             })
         }, e.prototype.matchExistingCacheKey = function(t, n) {
             return n.filter(function(r) {
-                var s = an.fromKey(r),
+                var s = un.fromKey(r),
                     o = new Set(s.scope && s.scope.split(" ")),
                     i = t.scope.split(" "),
                     a = s.scope && i.reduce(function(c, u) {
                         return c && o.has(u)
                     }, !0);
                 return s.prefix === "@@auth0spajs@@" && s.client_id === t.client_id && s.audience === t.audience && a
             })[0]
         }, e
     }(),
-    y_ = function() {
+    b_ = function() {
         function e(t, n) {
             this.storage = t, this.clientId = n, this.storageKey = "".concat("a0.spajs.txs", ".").concat(this.clientId), this.transaction = this.storage.get(this.storageKey)
         }
         return e.prototype.create = function(t) {
             this.transaction = t, this.storage.save(this.storageKey, t, {
                 daysUntilExpire: 1
             })
@@ -14075,38 +14075,38 @@
         }, e.prototype.remove = function() {
             delete this.transaction, this.storage.remove(this.storageKey)
         }, e
     }(),
     wr = function(e) {
         return typeof e == "number"
     },
-    b_ = ["iss", "aud", "exp", "nbf", "iat", "jti", "azp", "nonce", "auth_time", "at_hash", "c_hash", "acr", "amr", "sub_jwk", "cnf", "sip_from_tag", "sip_date", "sip_callid", "sip_cseq_num", "sip_via_branch", "orig", "dest", "mky", "events", "toe", "txn", "rph", "sid", "vot", "vtm"],
-    m_ = function(e) {
+    m_ = ["iss", "aud", "exp", "nbf", "iat", "jti", "azp", "nonce", "auth_time", "at_hash", "c_hash", "acr", "amr", "sub_jwk", "cnf", "sip_from_tag", "sip_date", "sip_callid", "sip_cseq_num", "sip_via_branch", "orig", "dest", "mky", "events", "toe", "txn", "rph", "sid", "vot", "vtm"],
+    g_ = function(e) {
         if (!e.id_token) throw new Error("ID token is required but missing");
         var t = function(a) {
             var c = a.split("."),
                 u = ir(c, 3),
                 l = u[0],
                 f = u[1],
                 h = u[2];
             if (c.length !== 3 || !l || !f || !h) throw new Error("ID token could not be decoded");
-            var p = JSON.parse(ul(f)),
+            var p = JSON.parse(fl(f)),
                 w = {
                     __raw: a
                 },
                 _ = {};
             return Object.keys(p).forEach(function(b) {
-                w[b] = p[b], b_.includes(b) || (_[b] = p[b])
+                w[b] = p[b], m_.includes(b) || (_[b] = p[b])
             }), {
                 encoded: {
                     header: l,
                     payload: f,
                     signature: h
                 },
-                header: JSON.parse(ul(l)),
+                header: JSON.parse(fl(l)),
                 claims: w,
                 user: _
             }
         }(e.id_token);
         if (!t.claims.iss) throw new Error("Issuer (iss) claim must be a string present in the ID token");
         if (t.claims.iss !== e.iss) throw new Error('Issuer (iss) claim mismatch in the ID token; expected "'.concat(e.iss, '", found "').concat(t.claims.iss, '"'));
         if (!t.user.sub) throw new Error("Subject (sub) claim must be a string present in the ID token");
@@ -14136,16 +14136,16 @@
         if (wr(t.claims.auth_time) && r > i) throw new Error("Authentication Time (auth_time) claim in the ID token indicates that too much time has passed since the last end-user authentication. Currrent time (".concat(r, ") is after last auth at ").concat(i));
         if (e.organizationId) {
             if (!t.claims.org_id) throw new Error("Organization ID (org_id) claim must be a string present in the ID token");
             if (e.organizationId !== t.claims.org_id) throw new Error('Organization ID (org_id) claim mismatch in the ID token; expected "'.concat(e.organizationId, '", found "').concat(t.claims.org_id, '"'))
         }
         return t
     },
-    un = lr(function(e, t) {
-        var n = ce && ce.__assign || function() {
+    fn = lr(function(e, t) {
+        var n = ue && ue.__assign || function() {
             return n = Object.assign || function(c) {
                 for (var u, l = 1, f = arguments.length; l < f; l++)
                     for (var h in u = arguments[l]) Object.prototype.hasOwnProperty.call(u, h) && (c[h] = u[h]);
                 return c
             }, n.apply(this, arguments)
         };
 
@@ -14190,67 +14190,67 @@
             return i()[c]
         }, t.set = a, t.remove = function(c, u) {
             a(c, "", n(n({}, u), {
                 expires: -1
             }))
         }
     });
-sc(un), un.encode, un.parse, un.getAll;
-var g_ = un.get,
-    Ad = un.set,
-    Bd = un.remove,
-    Un = {
+nc(fn), fn.encode, fn.parse, fn.getAll;
+var v_ = fn.get,
+    Od = fn.set,
+    Fd = fn.remove,
+    Nn = {
         get: function(e) {
-            var t = g_(e);
+            var t = v_(e);
             if (t !== void 0) return JSON.parse(t)
         },
         save: function(e, t, n) {
             var r = {};
             window.location.protocol === "https:" && (r = {
                 secure: !0,
                 sameSite: "none"
-            }), n != null && n.daysUntilExpire && (r.expires = n.daysUntilExpire), n != null && n.cookieDomain && (r.domain = n.cookieDomain), Ad(e, JSON.stringify(t), r)
+            }), n != null && n.daysUntilExpire && (r.expires = n.daysUntilExpire), n != null && n.cookieDomain && (r.domain = n.cookieDomain), Od(e, JSON.stringify(t), r)
         },
         remove: function(e, t) {
             var n = {};
-            t != null && t.cookieDomain && (n.domain = t.cookieDomain), Bd(e, n)
+            t != null && t.cookieDomain && (n.domain = t.cookieDomain), Fd(e, n)
         }
     },
-    v_ = {
+    w_ = {
         get: function(e) {
-            var t = Un.get(e);
-            return t || Un.get("".concat("_legacy_").concat(e))
+            var t = Nn.get(e);
+            return t || Nn.get("".concat("_legacy_").concat(e))
         },
         save: function(e, t, n) {
             var r = {};
             window.location.protocol === "https:" && (r = {
                 secure: !0
-            }), n != null && n.daysUntilExpire && (r.expires = n.daysUntilExpire), Ad("".concat("_legacy_").concat(e), JSON.stringify(t), r), Un.save(e, t, n)
+            }), n != null && n.daysUntilExpire && (r.expires = n.daysUntilExpire), Od("".concat("_legacy_").concat(e), JSON.stringify(t), r), Nn.save(e, t, n)
         },
         remove: function(e, t) {
             var n = {};
-            t != null && t.cookieDomain && (n.domain = t.cookieDomain), Bd(e, n), Un.remove(e, t), Un.remove("".concat("_legacy_").concat(e), t)
+            t != null && t.cookieDomain && (n.domain = t.cookieDomain), Fd(e, n), Nn.remove(e, t), Nn.remove("".concat("_legacy_").concat(e), t)
         }
     },
-    w_ = {
+    __ = {
         get: function(e) {
             if (typeof sessionStorage < "u") {
                 var t = sessionStorage.getItem(e);
                 if (t !== void 0) return JSON.parse(t)
             }
         },
         save: function(e, t) {
             sessionStorage.setItem(e, JSON.stringify(t))
         },
         remove: function(e) {
             sessionStorage.removeItem(e)
         }
     };
 
-function __(e, t, n) {
+function S_(e, t, n) {
     var r = t === void 0 ? null : t,
         s = function(c, u) {
             var l = atob(c);
             if (u) {
                 for (var f = new Uint8Array(l.length), h = 0, p = l.length; h < p; ++h) f[h] = l.charCodeAt(h);
                 return String.fromCharCode.apply(null, new Uint16Array(f.buffer))
             }
@@ -14260,19 +14260,19 @@
 `, 10) + 1,
         i = s.substring(o) + (r ? "//# sourceMappingURL=" + r : ""),
         a = new Blob([i], {
             type: "application/javascript"
         });
     return URL.createObjectURL(a)
 }
-var fl, hl, dl, mo, S_ = (fl = "Lyogcm9sbHVwLXBsdWdpbi13ZWItd29ya2VyLWxvYWRlciAqLwohZnVuY3Rpb24oKXsidXNlIHN0cmljdCI7dmFyIHQ9ZnVuY3Rpb24oZSxyKXtyZXR1cm4gdD1PYmplY3Quc2V0UHJvdG90eXBlT2Z8fHtfX3Byb3RvX186W119aW5zdGFuY2VvZiBBcnJheSYmZnVuY3Rpb24odCxlKXt0Ll9fcHJvdG9fXz1lfXx8ZnVuY3Rpb24odCxlKXtmb3IodmFyIHIgaW4gZSlPYmplY3QucHJvdG90eXBlLmhhc093blByb3BlcnR5LmNhbGwoZSxyKSYmKHRbcl09ZVtyXSl9LHQoZSxyKX07ZnVuY3Rpb24gZShlLHIpe2lmKCJmdW5jdGlvbiIhPXR5cGVvZiByJiZudWxsIT09cil0aHJvdyBuZXcgVHlwZUVycm9yKCJDbGFzcyBleHRlbmRzIHZhbHVlICIrU3RyaW5nKHIpKyIgaXMgbm90IGEgY29uc3RydWN0b3Igb3IgbnVsbCIpO2Z1bmN0aW9uIG4oKXt0aGlzLmNvbnN0cnVjdG9yPWV9dChlLHIpLGUucHJvdG90eXBlPW51bGw9PT1yP09iamVjdC5jcmVhdGUocik6KG4ucHJvdG90eXBlPXIucHJvdG90eXBlLG5ldyBuKX12YXIgcj1mdW5jdGlvbigpe3JldHVybiByPU9iamVjdC5hc3NpZ258fGZ1bmN0aW9uKHQpe2Zvcih2YXIgZSxyPTEsbj1hcmd1bWVudHMubGVuZ3RoO3I8bjtyKyspZm9yKHZhciBvIGluIGU9YXJndW1lbnRzW3JdKU9iamVjdC5wcm90b3R5cGUuaGFzT3duUHJvcGVydHkuY2FsbChlLG8pJiYodFtvXT1lW29dKTtyZXR1cm4gdH0sci5hcHBseSh0aGlzLGFyZ3VtZW50cyl9O2Z1bmN0aW9uIG4odCxlLHIsbil7cmV0dXJuIG5ldyhyfHwocj1Qcm9taXNlKSkoKGZ1bmN0aW9uKG8sYyl7ZnVuY3Rpb24gaSh0KXt0cnl7cyhuLm5leHQodCkpfWNhdGNoKHQpe2ModCl9fWZ1bmN0aW9uIGEodCl7dHJ5e3Mobi50aHJvdyh0KSl9Y2F0Y2godCl7Yyh0KX19ZnVuY3Rpb24gcyh0KXt2YXIgZTt0LmRvbmU/byh0LnZhbHVlKTooZT10LnZhbHVlLGUgaW5zdGFuY2VvZiByP2U6bmV3IHIoKGZ1bmN0aW9uKHQpe3QoZSl9KSkpLnRoZW4oaSxhKX1zKChuPW4uYXBwbHkodCxlfHxbXSkpLm5leHQoKSl9KSl9ZnVuY3Rpb24gbyh0LGUpe3ZhciByLG4sbyxjLGk9e2xhYmVsOjAsc2VudDpmdW5jdGlvbigpe2lmKDEmb1swXSl0aHJvdyBvWzFdO3JldHVybiBvWzFdfSx0cnlzOltdLG9wczpbXX07cmV0dXJuIGM9e25leHQ6YSgwKSx0aHJvdzphKDEpLHJldHVybjphKDIpfSwiZnVuY3Rpb24iPT10eXBlb2YgU3ltYm9sJiYoY1tTeW1ib2wuaXRlcmF0b3JdPWZ1bmN0aW9uKCl7cmV0dXJuIHRoaXN9KSxjO2Z1bmN0aW9uIGEoYyl7cmV0dXJuIGZ1bmN0aW9uKGEpe3JldHVybiBmdW5jdGlvbihjKXtpZihyKXRocm93IG5ldyBUeXBlRXJyb3IoIkdlbmVyYXRvciBpcyBhbHJlYWR5IGV4ZWN1dGluZy4iKTtmb3IoO2k7KXRyeXtpZihyPTEsbiYmKG89MiZjWzBdP24ucmV0dXJuOmNbMF0/bi50aHJvd3x8KChvPW4ucmV0dXJuKSYmby5jYWxsKG4pLDApOm4ubmV4dCkmJiEobz1vLmNhbGwobixjWzFdKSkuZG9uZSlyZXR1cm4gbztzd2l0Y2gobj0wLG8mJihjPVsyJmNbMF0sby52YWx1ZV0pLGNbMF0pe2Nhc2UgMDpjYXNlIDE6bz1jO2JyZWFrO2Nhc2UgNDpyZXR1cm4gaS5sYWJlbCsrLHt2YWx1ZTpjWzFdLGRvbmU6ITF9O2Nhc2UgNTppLmxhYmVsKyssbj1jWzFdLGM9WzBdO2NvbnRpbnVlO2Nhc2UgNzpjPWkub3BzLnBvcCgpLGkudHJ5cy5wb3AoKTtjb250aW51ZTtkZWZhdWx0OmlmKCEobz1pLnRyeXMsKG89by5sZW5ndGg+MCYmb1tvLmxlbmd0aC0xXSl8fDYhPT1jWzBdJiYyIT09Y1swXSkpe2k9MDtjb250aW51ZX1pZigzPT09Y1swXSYmKCFvfHxjWzFdPm9bMF0mJmNbMV08b1szXSkpe2kubGFiZWw9Y1sxXTticmVha31pZig2PT09Y1swXSYmaS5sYWJlbDxvWzFdKXtpLmxhYmVsPW9bMV0sbz1jO2JyZWFrfWlmKG8mJmkubGFiZWw8b1syXSl7aS5sYWJlbD1vWzJdLGkub3BzLnB1c2goYyk7YnJlYWt9b1syXSYmaS5vcHMucG9wKCksaS50cnlzLnBvcCgpO2NvbnRpbnVlfWM9ZS5jYWxsKHQsaSl9Y2F0Y2godCl7Yz1bNix0XSxuPTB9ZmluYWxseXtyPW89MH1pZig1JmNbMF0pdGhyb3cgY1sxXTtyZXR1cm57dmFsdWU6Y1swXT9jWzFdOnZvaWQgMCxkb25lOiEwfX0oW2MsYV0pfX19ZnVuY3Rpb24gYyh0LGUpe3JldHVybiB2b2lkIDA9PT1lJiYoZT1bXSksdCYmIWUuaW5jbHVkZXModCk/dDoiIn12YXIgaT1mdW5jdGlvbih0KXtmdW5jdGlvbiByKGUsbil7dmFyIG89dC5jYWxsKHRoaXMsbil8fHRoaXM7cmV0dXJuIG8uZXJyb3I9ZSxvLmVycm9yX2Rlc2NyaXB0aW9uPW4sT2JqZWN0LnNldFByb3RvdHlwZU9mKG8sci5wcm90b3R5cGUpLG99cmV0dXJuIGUocix0KSxyLmZyb21QYXlsb2FkPWZ1bmN0aW9uKHQpe3JldHVybiBuZXcgcih0LmVycm9yLHQuZXJyb3JfZGVzY3JpcHRpb24pfSxyfShFcnJvcik7IWZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSxuLG8sYyl7dm9pZCAwPT09YyYmKGM9bnVsbCk7dmFyIGk9dC5jYWxsKHRoaXMsZSxuKXx8dGhpcztyZXR1cm4gaS5zdGF0ZT1vLGkuYXBwU3RhdGU9YyxPYmplY3Quc2V0UHJvdG90eXBlT2YoaSxyLnByb3RvdHlwZSksaX1lKHIsdCl9KGkpLGZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSl7dmFyIG49dC5jYWxsKHRoaXMpfHx0aGlzO3JldHVybiBuLnBvcHVwPWUsT2JqZWN0LnNldFByb3RvdHlwZU9mKG4sci5wcm90b3R5cGUpLG59ZShyLHQpfShmdW5jdGlvbih0KXtmdW5jdGlvbiByKCl7dmFyIGU9dC5jYWxsKHRoaXMsInRpbWVvdXQiLCJUaW1lb3V0Iil8fHRoaXM7cmV0dXJuIE9iamVjdC5zZXRQcm90b3R5cGVPZihlLHIucHJvdG90eXBlKSxlfXJldHVybiBlKHIsdCkscn0oaSkpLGZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSl7dmFyIG49dC5jYWxsKHRoaXMsImNhbmNlbGxlZCIsIlBvcHVwIGNsb3NlZCIpfHx0aGlzO3JldHVybiBuLnBvcHVwPWUsT2JqZWN0LnNldFByb3RvdHlwZU9mKG4sci5wcm90b3R5cGUpLG59ZShyLHQpfShpKSxmdW5jdGlvbih0KXtmdW5jdGlvbiByKGUsbixvKXt2YXIgYz10LmNhbGwodGhpcyxlLG4pfHx0aGlzO3JldHVybiBjLm1mYV90b2tlbj1vLE9iamVjdC5zZXRQcm90b3R5cGVPZihjLHIucHJvdG90eXBlKSxjfWUocix0KX0oaSk7dmFyIGE9ZnVuY3Rpb24odCl7ZnVuY3Rpb24gcihlLG4pe3ZhciBvPXQuY2FsbCh0aGlzLCJtaXNzaW5nX3JlZnJlc2hfdG9rZW4iLCJNaXNzaW5nIFJlZnJlc2ggVG9rZW4gKGF1ZGllbmNlOiAnIi5jb25jYXQoYyhlLFsiZGVmYXVsdCJdKSwiJywgc2NvcGU6ICciKS5jb25jYXQoYyhuKSwiJykiKSl8fHRoaXM7cmV0dXJuIG8uYXVkaWVuY2U9ZSxvLnNjb3BlPW4sT2JqZWN0LnNldFByb3RvdHlwZU9mKG8sci5wcm90b3R5cGUpLG99cmV0dXJuIGUocix0KSxyfShpKSxzPXt9LHU9ZnVuY3Rpb24odCxlKXtyZXR1cm4iIi5jb25jYXQodCwifCIpLmNvbmNhdChlKX07YWRkRXZlbnRMaXN0ZW5lcigibWVzc2FnZSIsKGZ1bmN0aW9uKHQpe3ZhciBlPXQuZGF0YSxjPWUudGltZW91dCxpPWUuYXV0aCxmPWUuZmV0Y2hVcmwsbD1lLmZldGNoT3B0aW9ucyxwPWUudXNlRm9ybURhdGEsaD1mdW5jdGlvbih0LGUpe3ZhciByPSJmdW5jdGlvbiI9PXR5cGVvZiBTeW1ib2wmJnRbU3ltYm9sLml0ZXJhdG9yXTtpZighcilyZXR1cm4gdDt2YXIgbixvLGM9ci5jYWxsKHQpLGk9W107dHJ5e2Zvcig7KHZvaWQgMD09PWV8fGUtLSA+MCkmJiEobj1jLm5leHQoKSkuZG9uZTspaS5wdXNoKG4udmFsdWUpfWNhdGNoKHQpe289e2Vycm9yOnR9fWZpbmFsbHl7dHJ5e24mJiFuLmRvbmUmJihyPWMucmV0dXJuKSYmci5jYWxsKGMpfWZpbmFsbHl7aWYobyl0aHJvdyBvLmVycm9yfX1yZXR1cm4gaX0odC5wb3J0cywxKVswXTtyZXR1cm4gbih2b2lkIDAsdm9pZCAwLHZvaWQgMCwoZnVuY3Rpb24oKXt2YXIgdCxlLG4seSx2LGIsZCx3LE8sXztyZXR1cm4gbyh0aGlzLChmdW5jdGlvbihvKXtzd2l0Y2goby5sYWJlbCl7Y2FzZSAwOm49KGU9aXx8e30pLmF1ZGllbmNlLHk9ZS5zY29wZSxvLmxhYmVsPTE7Y2FzZSAxOmlmKG8udHJ5cy5wdXNoKFsxLDcsLDhdKSwhKHY9cD8obT1sLmJvZHksaz1uZXcgVVJMU2VhcmNoUGFyYW1zKG0pLFA9e30say5mb3JFYWNoKChmdW5jdGlvbih0LGUpe1BbZV09dH0pKSxQKTpKU09OLnBhcnNlKGwuYm9keSkpLnJlZnJlc2hfdG9rZW4mJiJyZWZyZXNoX3Rva2VuIj09PXYuZ3JhbnRfdHlwZSl7aWYoYj1mdW5jdGlvbih0LGUpe3JldHVybiBzW3UodCxlKV19KG4seSksIWIpdGhyb3cgbmV3IGEobix5KTtsLmJvZHk9cD9uZXcgVVJMU2VhcmNoUGFyYW1zKHIocih7fSx2KSx7cmVmcmVzaF90b2tlbjpifSkpLnRvU3RyaW5nKCk6SlNPTi5zdHJpbmdpZnkocihyKHt9LHYpLHtyZWZyZXNoX3Rva2VuOmJ9KSl9ZD12b2lkIDAsImZ1bmN0aW9uIj09dHlwZW9mIEFib3J0Q29udHJvbGxlciYmKGQ9bmV3IEFib3J0Q29udHJvbGxlcixsLnNpZ25hbD1kLnNpZ25hbCksdz12b2lkIDAsby5sYWJlbD0yO2Nhc2UgMjpyZXR1cm4gby50cnlzLnB1c2goWzIsNCwsNV0pLFs0LFByb21pc2UucmFjZShbKGc9YyxuZXcgUHJvbWlzZSgoZnVuY3Rpb24odCl7cmV0dXJuIHNldFRpbWVvdXQodCxnKX0pKSksZmV0Y2goZixyKHt9LGwpKV0pXTtjYXNlIDM6cmV0dXJuIHc9by5zZW50KCksWzMsNV07Y2FzZSA0OnJldHVybiBPPW8uc2VudCgpLGgucG9zdE1lc3NhZ2Uoe2Vycm9yOk8ubWVzc2FnZX0pLFsyXTtjYXNlIDU6cmV0dXJuIHc/WzQsdy5qc29uKCldOihkJiZkLmFib3J0KCksaC5wb3N0TWVzc2FnZSh7ZXJyb3I6IlRpbWVvdXQgd2hlbiBleGVjdXRpbmcgJ2ZldGNoJyJ9KSxbMl0pO2Nhc2UgNjpyZXR1cm4odD1vLnNlbnQoKSkucmVmcmVzaF90b2tlbj8oZnVuY3Rpb24odCxlLHIpe3NbdShlLHIpXT10fSh0LnJlZnJlc2hfdG9rZW4sbix5KSxkZWxldGUgdC5yZWZyZXNoX3Rva2VuKTpmdW5jdGlvbih0LGUpe2RlbGV0ZSBzW3UodCxlKV19KG4seSksaC5wb3N0TWVzc2FnZSh7b2s6dy5vayxqc29uOnR9KSxbMyw4XTtjYXNlIDc6cmV0dXJuIF89by5zZW50KCksaC5wb3N0TWVzc2FnZSh7b2s6ITEsanNvbjp7ZXJyb3JfZGVzY3JpcHRpb246Xy5tZXNzYWdlfX0pLFszLDhdO2Nhc2UgODpyZXR1cm5bMl19dmFyIGcsbSxrLFB9KSl9KSl9KSl9KCk7Cgo=", hl = null, dl = !1, function(e) {
-        return mo = mo || __(fl, hl, dl), new Worker(mo, e)
+var dl, pl, yl, mo, I_ = (dl = "Lyogcm9sbHVwLXBsdWdpbi13ZWItd29ya2VyLWxvYWRlciAqLwohZnVuY3Rpb24oKXsidXNlIHN0cmljdCI7dmFyIHQ9ZnVuY3Rpb24oZSxyKXtyZXR1cm4gdD1PYmplY3Quc2V0UHJvdG90eXBlT2Z8fHtfX3Byb3RvX186W119aW5zdGFuY2VvZiBBcnJheSYmZnVuY3Rpb24odCxlKXt0Ll9fcHJvdG9fXz1lfXx8ZnVuY3Rpb24odCxlKXtmb3IodmFyIHIgaW4gZSlPYmplY3QucHJvdG90eXBlLmhhc093blByb3BlcnR5LmNhbGwoZSxyKSYmKHRbcl09ZVtyXSl9LHQoZSxyKX07ZnVuY3Rpb24gZShlLHIpe2lmKCJmdW5jdGlvbiIhPXR5cGVvZiByJiZudWxsIT09cil0aHJvdyBuZXcgVHlwZUVycm9yKCJDbGFzcyBleHRlbmRzIHZhbHVlICIrU3RyaW5nKHIpKyIgaXMgbm90IGEgY29uc3RydWN0b3Igb3IgbnVsbCIpO2Z1bmN0aW9uIG4oKXt0aGlzLmNvbnN0cnVjdG9yPWV9dChlLHIpLGUucHJvdG90eXBlPW51bGw9PT1yP09iamVjdC5jcmVhdGUocik6KG4ucHJvdG90eXBlPXIucHJvdG90eXBlLG5ldyBuKX12YXIgcj1mdW5jdGlvbigpe3JldHVybiByPU9iamVjdC5hc3NpZ258fGZ1bmN0aW9uKHQpe2Zvcih2YXIgZSxyPTEsbj1hcmd1bWVudHMubGVuZ3RoO3I8bjtyKyspZm9yKHZhciBvIGluIGU9YXJndW1lbnRzW3JdKU9iamVjdC5wcm90b3R5cGUuaGFzT3duUHJvcGVydHkuY2FsbChlLG8pJiYodFtvXT1lW29dKTtyZXR1cm4gdH0sci5hcHBseSh0aGlzLGFyZ3VtZW50cyl9O2Z1bmN0aW9uIG4odCxlLHIsbil7cmV0dXJuIG5ldyhyfHwocj1Qcm9taXNlKSkoKGZ1bmN0aW9uKG8sYyl7ZnVuY3Rpb24gaSh0KXt0cnl7cyhuLm5leHQodCkpfWNhdGNoKHQpe2ModCl9fWZ1bmN0aW9uIGEodCl7dHJ5e3Mobi50aHJvdyh0KSl9Y2F0Y2godCl7Yyh0KX19ZnVuY3Rpb24gcyh0KXt2YXIgZTt0LmRvbmU/byh0LnZhbHVlKTooZT10LnZhbHVlLGUgaW5zdGFuY2VvZiByP2U6bmV3IHIoKGZ1bmN0aW9uKHQpe3QoZSl9KSkpLnRoZW4oaSxhKX1zKChuPW4uYXBwbHkodCxlfHxbXSkpLm5leHQoKSl9KSl9ZnVuY3Rpb24gbyh0LGUpe3ZhciByLG4sbyxjLGk9e2xhYmVsOjAsc2VudDpmdW5jdGlvbigpe2lmKDEmb1swXSl0aHJvdyBvWzFdO3JldHVybiBvWzFdfSx0cnlzOltdLG9wczpbXX07cmV0dXJuIGM9e25leHQ6YSgwKSx0aHJvdzphKDEpLHJldHVybjphKDIpfSwiZnVuY3Rpb24iPT10eXBlb2YgU3ltYm9sJiYoY1tTeW1ib2wuaXRlcmF0b3JdPWZ1bmN0aW9uKCl7cmV0dXJuIHRoaXN9KSxjO2Z1bmN0aW9uIGEoYyl7cmV0dXJuIGZ1bmN0aW9uKGEpe3JldHVybiBmdW5jdGlvbihjKXtpZihyKXRocm93IG5ldyBUeXBlRXJyb3IoIkdlbmVyYXRvciBpcyBhbHJlYWR5IGV4ZWN1dGluZy4iKTtmb3IoO2k7KXRyeXtpZihyPTEsbiYmKG89MiZjWzBdP24ucmV0dXJuOmNbMF0/bi50aHJvd3x8KChvPW4ucmV0dXJuKSYmby5jYWxsKG4pLDApOm4ubmV4dCkmJiEobz1vLmNhbGwobixjWzFdKSkuZG9uZSlyZXR1cm4gbztzd2l0Y2gobj0wLG8mJihjPVsyJmNbMF0sby52YWx1ZV0pLGNbMF0pe2Nhc2UgMDpjYXNlIDE6bz1jO2JyZWFrO2Nhc2UgNDpyZXR1cm4gaS5sYWJlbCsrLHt2YWx1ZTpjWzFdLGRvbmU6ITF9O2Nhc2UgNTppLmxhYmVsKyssbj1jWzFdLGM9WzBdO2NvbnRpbnVlO2Nhc2UgNzpjPWkub3BzLnBvcCgpLGkudHJ5cy5wb3AoKTtjb250aW51ZTtkZWZhdWx0OmlmKCEobz1pLnRyeXMsKG89by5sZW5ndGg+MCYmb1tvLmxlbmd0aC0xXSl8fDYhPT1jWzBdJiYyIT09Y1swXSkpe2k9MDtjb250aW51ZX1pZigzPT09Y1swXSYmKCFvfHxjWzFdPm9bMF0mJmNbMV08b1szXSkpe2kubGFiZWw9Y1sxXTticmVha31pZig2PT09Y1swXSYmaS5sYWJlbDxvWzFdKXtpLmxhYmVsPW9bMV0sbz1jO2JyZWFrfWlmKG8mJmkubGFiZWw8b1syXSl7aS5sYWJlbD1vWzJdLGkub3BzLnB1c2goYyk7YnJlYWt9b1syXSYmaS5vcHMucG9wKCksaS50cnlzLnBvcCgpO2NvbnRpbnVlfWM9ZS5jYWxsKHQsaSl9Y2F0Y2godCl7Yz1bNix0XSxuPTB9ZmluYWxseXtyPW89MH1pZig1JmNbMF0pdGhyb3cgY1sxXTtyZXR1cm57dmFsdWU6Y1swXT9jWzFdOnZvaWQgMCxkb25lOiEwfX0oW2MsYV0pfX19ZnVuY3Rpb24gYyh0LGUpe3JldHVybiB2b2lkIDA9PT1lJiYoZT1bXSksdCYmIWUuaW5jbHVkZXModCk/dDoiIn12YXIgaT1mdW5jdGlvbih0KXtmdW5jdGlvbiByKGUsbil7dmFyIG89dC5jYWxsKHRoaXMsbil8fHRoaXM7cmV0dXJuIG8uZXJyb3I9ZSxvLmVycm9yX2Rlc2NyaXB0aW9uPW4sT2JqZWN0LnNldFByb3RvdHlwZU9mKG8sci5wcm90b3R5cGUpLG99cmV0dXJuIGUocix0KSxyLmZyb21QYXlsb2FkPWZ1bmN0aW9uKHQpe3JldHVybiBuZXcgcih0LmVycm9yLHQuZXJyb3JfZGVzY3JpcHRpb24pfSxyfShFcnJvcik7IWZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSxuLG8sYyl7dm9pZCAwPT09YyYmKGM9bnVsbCk7dmFyIGk9dC5jYWxsKHRoaXMsZSxuKXx8dGhpcztyZXR1cm4gaS5zdGF0ZT1vLGkuYXBwU3RhdGU9YyxPYmplY3Quc2V0UHJvdG90eXBlT2YoaSxyLnByb3RvdHlwZSksaX1lKHIsdCl9KGkpLGZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSl7dmFyIG49dC5jYWxsKHRoaXMpfHx0aGlzO3JldHVybiBuLnBvcHVwPWUsT2JqZWN0LnNldFByb3RvdHlwZU9mKG4sci5wcm90b3R5cGUpLG59ZShyLHQpfShmdW5jdGlvbih0KXtmdW5jdGlvbiByKCl7dmFyIGU9dC5jYWxsKHRoaXMsInRpbWVvdXQiLCJUaW1lb3V0Iil8fHRoaXM7cmV0dXJuIE9iamVjdC5zZXRQcm90b3R5cGVPZihlLHIucHJvdG90eXBlKSxlfXJldHVybiBlKHIsdCkscn0oaSkpLGZ1bmN0aW9uKHQpe2Z1bmN0aW9uIHIoZSl7dmFyIG49dC5jYWxsKHRoaXMsImNhbmNlbGxlZCIsIlBvcHVwIGNsb3NlZCIpfHx0aGlzO3JldHVybiBuLnBvcHVwPWUsT2JqZWN0LnNldFByb3RvdHlwZU9mKG4sci5wcm90b3R5cGUpLG59ZShyLHQpfShpKSxmdW5jdGlvbih0KXtmdW5jdGlvbiByKGUsbixvKXt2YXIgYz10LmNhbGwodGhpcyxlLG4pfHx0aGlzO3JldHVybiBjLm1mYV90b2tlbj1vLE9iamVjdC5zZXRQcm90b3R5cGVPZihjLHIucHJvdG90eXBlKSxjfWUocix0KX0oaSk7dmFyIGE9ZnVuY3Rpb24odCl7ZnVuY3Rpb24gcihlLG4pe3ZhciBvPXQuY2FsbCh0aGlzLCJtaXNzaW5nX3JlZnJlc2hfdG9rZW4iLCJNaXNzaW5nIFJlZnJlc2ggVG9rZW4gKGF1ZGllbmNlOiAnIi5jb25jYXQoYyhlLFsiZGVmYXVsdCJdKSwiJywgc2NvcGU6ICciKS5jb25jYXQoYyhuKSwiJykiKSl8fHRoaXM7cmV0dXJuIG8uYXVkaWVuY2U9ZSxvLnNjb3BlPW4sT2JqZWN0LnNldFByb3RvdHlwZU9mKG8sci5wcm90b3R5cGUpLG99cmV0dXJuIGUocix0KSxyfShpKSxzPXt9LHU9ZnVuY3Rpb24odCxlKXtyZXR1cm4iIi5jb25jYXQodCwifCIpLmNvbmNhdChlKX07YWRkRXZlbnRMaXN0ZW5lcigibWVzc2FnZSIsKGZ1bmN0aW9uKHQpe3ZhciBlPXQuZGF0YSxjPWUudGltZW91dCxpPWUuYXV0aCxmPWUuZmV0Y2hVcmwsbD1lLmZldGNoT3B0aW9ucyxwPWUudXNlRm9ybURhdGEsaD1mdW5jdGlvbih0LGUpe3ZhciByPSJmdW5jdGlvbiI9PXR5cGVvZiBTeW1ib2wmJnRbU3ltYm9sLml0ZXJhdG9yXTtpZighcilyZXR1cm4gdDt2YXIgbixvLGM9ci5jYWxsKHQpLGk9W107dHJ5e2Zvcig7KHZvaWQgMD09PWV8fGUtLSA+MCkmJiEobj1jLm5leHQoKSkuZG9uZTspaS5wdXNoKG4udmFsdWUpfWNhdGNoKHQpe289e2Vycm9yOnR9fWZpbmFsbHl7dHJ5e24mJiFuLmRvbmUmJihyPWMucmV0dXJuKSYmci5jYWxsKGMpfWZpbmFsbHl7aWYobyl0aHJvdyBvLmVycm9yfX1yZXR1cm4gaX0odC5wb3J0cywxKVswXTtyZXR1cm4gbih2b2lkIDAsdm9pZCAwLHZvaWQgMCwoZnVuY3Rpb24oKXt2YXIgdCxlLG4seSx2LGIsZCx3LE8sXztyZXR1cm4gbyh0aGlzLChmdW5jdGlvbihvKXtzd2l0Y2goby5sYWJlbCl7Y2FzZSAwOm49KGU9aXx8e30pLmF1ZGllbmNlLHk9ZS5zY29wZSxvLmxhYmVsPTE7Y2FzZSAxOmlmKG8udHJ5cy5wdXNoKFsxLDcsLDhdKSwhKHY9cD8obT1sLmJvZHksaz1uZXcgVVJMU2VhcmNoUGFyYW1zKG0pLFA9e30say5mb3JFYWNoKChmdW5jdGlvbih0LGUpe1BbZV09dH0pKSxQKTpKU09OLnBhcnNlKGwuYm9keSkpLnJlZnJlc2hfdG9rZW4mJiJyZWZyZXNoX3Rva2VuIj09PXYuZ3JhbnRfdHlwZSl7aWYoYj1mdW5jdGlvbih0LGUpe3JldHVybiBzW3UodCxlKV19KG4seSksIWIpdGhyb3cgbmV3IGEobix5KTtsLmJvZHk9cD9uZXcgVVJMU2VhcmNoUGFyYW1zKHIocih7fSx2KSx7cmVmcmVzaF90b2tlbjpifSkpLnRvU3RyaW5nKCk6SlNPTi5zdHJpbmdpZnkocihyKHt9LHYpLHtyZWZyZXNoX3Rva2VuOmJ9KSl9ZD12b2lkIDAsImZ1bmN0aW9uIj09dHlwZW9mIEFib3J0Q29udHJvbGxlciYmKGQ9bmV3IEFib3J0Q29udHJvbGxlcixsLnNpZ25hbD1kLnNpZ25hbCksdz12b2lkIDAsby5sYWJlbD0yO2Nhc2UgMjpyZXR1cm4gby50cnlzLnB1c2goWzIsNCwsNV0pLFs0LFByb21pc2UucmFjZShbKGc9YyxuZXcgUHJvbWlzZSgoZnVuY3Rpb24odCl7cmV0dXJuIHNldFRpbWVvdXQodCxnKX0pKSksZmV0Y2goZixyKHt9LGwpKV0pXTtjYXNlIDM6cmV0dXJuIHc9by5zZW50KCksWzMsNV07Y2FzZSA0OnJldHVybiBPPW8uc2VudCgpLGgucG9zdE1lc3NhZ2Uoe2Vycm9yOk8ubWVzc2FnZX0pLFsyXTtjYXNlIDU6cmV0dXJuIHc/WzQsdy5qc29uKCldOihkJiZkLmFib3J0KCksaC5wb3N0TWVzc2FnZSh7ZXJyb3I6IlRpbWVvdXQgd2hlbiBleGVjdXRpbmcgJ2ZldGNoJyJ9KSxbMl0pO2Nhc2UgNjpyZXR1cm4odD1vLnNlbnQoKSkucmVmcmVzaF90b2tlbj8oZnVuY3Rpb24odCxlLHIpe3NbdShlLHIpXT10fSh0LnJlZnJlc2hfdG9rZW4sbix5KSxkZWxldGUgdC5yZWZyZXNoX3Rva2VuKTpmdW5jdGlvbih0LGUpe2RlbGV0ZSBzW3UodCxlKV19KG4seSksaC5wb3N0TWVzc2FnZSh7b2s6dy5vayxqc29uOnR9KSxbMyw4XTtjYXNlIDc6cmV0dXJuIF89by5zZW50KCksaC5wb3N0TWVzc2FnZSh7b2s6ITEsanNvbjp7ZXJyb3JfZGVzY3JpcHRpb246Xy5tZXNzYWdlfX0pLFszLDhdO2Nhc2UgODpyZXR1cm5bMl19dmFyIGcsbSxrLFB9KSl9KSl9KSl9KCk7Cgo=", pl = null, yl = !1, function(e) {
+        return mo = mo || S_(dl, pl, yl), new Worker(mo, e)
     }),
     go = {},
-    I_ = function() {
+    T_ = function() {
         function e(t, n) {
             this.cache = t, this.clientId = n, this.manifestKey = this.createManifestKeyFrom(this.clientId)
         }
         return e.prototype.add = function(t) {
             var n;
             return $(this, void 0, void 0, function() {
                 var r, s;
@@ -14314,65 +14314,65 @@
             return this.cache.get(this.manifestKey)
         }, e.prototype.clear = function() {
             return this.cache.remove(this.manifestKey)
         }, e.prototype.createManifestKeyFrom = function(t) {
             return "".concat("@@auth0spajs@@", "::").concat(t)
         }, e
     }(),
-    vo = new Xw,
-    T_ = {
+    vo = new qw,
+    A_ = {
         memory: function() {
-            return new d_().enclosedCache
+            return new p_().enclosedCache
         },
         localstorage: function() {
-            return new h_
+            return new d_
         }
     },
-    pl = function(e) {
-        return T_[e]
+    bl = function(e) {
+        return A_[e]
     },
-    A_ = function() {
+    B_ = function() {
         return !/Trident.*rv:11\.0/.test(navigator.userAgent)
     },
-    B_ = function() {
+    O_ = function() {
         function e(t) {
             var n, r, s, o, i = this;
             if (this.options = t, this._releaseLockOnPageHide = function() {
                     return $(i, void 0, void 0, function() {
                         return Y(this, function(u) {
                             switch (u.label) {
                                 case 0:
                                     return [4, vo.releaseLock("auth0.lock.getTokenSilently")];
                                 case 1:
                                     return u.sent(), window.removeEventListener("pagehide", this._releaseLockOnPageHide), [2]
                             }
                         })
                     })
                 }, typeof window < "u" && function() {
-                    if (!Tc()) throw new Error("For security reasons, `window.crypto` is required to run `auth0-spa-js`.");
-                    if (Td() === void 0) throw new Error(`
+                    if (!_c()) throw new Error("For security reasons, `window.crypto` is required to run `auth0-spa-js`.");
+                    if (Bd() === void 0) throw new Error(`
       auth0-spa-js must run on a secure origin. See https://github.com/auth0/auth0-spa-js/blob/master/FAQ.md#why-do-i-get-auth0-spa-js-must-run-on-a-secure-origin for more information.
     `)
                 }(), t.cache && t.cacheLocation && console.warn("Both `cache` and `cacheLocation` options have been specified in the Auth0Client configuration; ignoring `cacheLocation` and using `cache`."), t.cache) s = t.cache;
             else {
-                if (this.cacheLocation = t.cacheLocation || "memory", !pl(this.cacheLocation)) throw new Error('Invalid cache location "'.concat(this.cacheLocation, '"'));
-                s = pl(this.cacheLocation)()
+                if (this.cacheLocation = t.cacheLocation || "memory", !bl(this.cacheLocation)) throw new Error('Invalid cache location "'.concat(this.cacheLocation, '"'));
+                s = bl(this.cacheLocation)()
             }
-            this.httpTimeoutMs = t.httpTimeoutInSeconds ? 1e3 * t.httpTimeoutInSeconds : 1e4, this.cookieStorage = t.legacySameSiteCookie === !1 ? Un : v_, this.orgHintCookieName = (o = this.options.client_id, "auth0.".concat(o, ".organization_hint")), this.isAuthenticatedCookieName = function(u) {
+            this.httpTimeoutMs = t.httpTimeoutInSeconds ? 1e3 * t.httpTimeoutInSeconds : 1e4, this.cookieStorage = t.legacySameSiteCookie === !1 ? Nn : w_, this.orgHintCookieName = (o = this.options.client_id, "auth0.".concat(o, ".organization_hint")), this.isAuthenticatedCookieName = function(u) {
                 return "auth0.".concat(u, ".is.authenticated")
             }(this.options.client_id), this.sessionCheckExpiryDays = t.sessionCheckExpiryDays || 1;
-            var a, c = t.useCookiesForTransactions ? this.cookieStorage : w_;
-            this.scope = this.options.scope, this.transactionManager = new y_(c, this.options.client_id), this.nowProvider = this.options.nowProvider || Id, this.cacheManager = new p_(s, s.allKeys ? null : new I_(s, this.options.client_id), this.nowProvider), this.domainUrl = (a = this.options.domain, /^https?:\/\//.test(a) ? a : "https://".concat(a)), this.tokenIssuer = function(u, l) {
+            var a, c = t.useCookiesForTransactions ? this.cookieStorage : __;
+            this.scope = this.options.scope, this.transactionManager = new b_(c, this.options.client_id), this.nowProvider = this.options.nowProvider || Ad, this.cacheManager = new y_(s, s.allKeys ? null : new T_(s, this.options.client_id), this.nowProvider), this.domainUrl = (a = this.options.domain, /^https?:\/\//.test(a) ? a : "https://".concat(a)), this.tokenIssuer = function(u, l) {
                 return u ? u.startsWith("https://") ? u : "https://".concat(u, "/") : "".concat(l, "/")
-            }(this.options.issuer, this.domainUrl), this.defaultScope = Ce("openid", ((r = (n = this.options) === null || n === void 0 ? void 0 : n.advancedOptions) === null || r === void 0 ? void 0 : r.defaultScope) !== void 0 ? this.options.advancedOptions.defaultScope : "openid profile email"), this.options.useRefreshTokens && (this.scope = Ce(this.scope, "offline_access")), typeof window < "u" && window.Worker && this.options.useRefreshTokens && this.cacheLocation === "memory" && A_() && (this.worker = new S_), this.customOptions = function(u) {
+            }(this.options.issuer, this.domainUrl), this.defaultScope = Ce("openid", ((r = (n = this.options) === null || n === void 0 ? void 0 : n.advancedOptions) === null || r === void 0 ? void 0 : r.defaultScope) !== void 0 ? this.options.advancedOptions.defaultScope : "openid profile email"), this.options.useRefreshTokens && (this.scope = Ce(this.scope, "offline_access")), typeof window < "u" && window.Worker && this.options.useRefreshTokens && this.cacheLocation === "memory" && B_() && (this.worker = new I_), this.customOptions = function(u) {
                 return u.advancedOptions, u.audience, u.auth0Client, u.authorizeTimeoutInSeconds, u.cacheLocation, u.cache, u.client_id, u.domain, u.issuer, u.leeway, u.max_age, u.nowProvider, u.redirect_uri, u.scope, u.useRefreshTokens, u.useRefreshTokensFallback, u.useCookiesForTransactions, u.useFormData, Tt(u, ["advancedOptions", "audience", "auth0Client", "authorizeTimeoutInSeconds", "cacheLocation", "cache", "client_id", "domain", "issuer", "leeway", "max_age", "nowProvider", "redirect_uri", "scope", "useRefreshTokens", "useRefreshTokensFallback", "useCookiesForTransactions", "useFormData"])
             }(t), this.useRefreshTokensFallback = this.options.useRefreshTokensFallback !== !1
         }
         return e.prototype._url = function(t) {
-            var n = encodeURIComponent(btoa(JSON.stringify(this.options.auth0Client || Sd)));
+            var n = encodeURIComponent(btoa(JSON.stringify(this.options.auth0Client || Td)));
             return "".concat(this.domainUrl).concat(t, "&auth0Client=").concat(n)
         }, e.prototype._getParams = function(t, n, r, s, o) {
             var i = this.options;
             i.useRefreshTokens, i.useCookiesForTransactions, i.useFormData, i.auth0Client, i.cacheLocation, i.advancedOptions, i.detailedResponse, i.nowProvider, i.authorizeTimeoutInSeconds, i.legacySameSiteCookie, i.sessionCheckExpiryDays, i.domain, i.leeway, i.httpTimeoutInSeconds;
             var a = Tt(i, ["useRefreshTokens", "useCookiesForTransactions", "useFormData", "auth0Client", "cacheLocation", "advancedOptions", "detailedResponse", "nowProvider", "authorizeTimeoutInSeconds", "legacySameSiteCookie", "sessionCheckExpiryDays", "domain", "leeway", "httpTimeoutInSeconds"]);
             return N(N(N({}, a), t), {
                 scope: Ce(this.defaultScope, this.scope, t.scope),
@@ -14390,15 +14390,15 @@
             return $(this, void 0, void 0, function() {
                 var s;
                 return Y(this, function(o) {
                     switch (o.label) {
                         case 0:
                             return [4, this.nowProvider()];
                         case 1:
-                            return s = o.sent(), [2, m_({
+                            return s = o.sent(), [2, g_({
                                 iss: this.tokenIssuer,
                                 aud: this.options.client_id,
                                 id_token: t,
                                 nonce: n,
                                 organizationId: r,
                                 leeway: this.options.leeway,
                                 max_age: this._parseNumber(this.options.max_age),
@@ -14418,15 +14418,15 @@
             })
         }, e.prototype.buildAuthorizeUrl = function(t) {
             return t === void 0 && (t = {}), $(this, void 0, void 0, function() {
                 var n, r, s, o, i, a, c, u, l, f, h, p;
                 return Y(this, function(w) {
                     switch (w.label) {
                         case 0:
-                            return n = t.redirect_uri, r = t.appState, s = Tt(t, ["redirect_uri", "appState"]), o = Dn(ge()), i = Dn(ge()), a = ge(), [4, yo(a)];
+                            return n = t.redirect_uri, r = t.appState, s = Tt(t, ["redirect_uri", "appState"]), o = kn(ge()), i = kn(ge()), a = ge(), [4, yo(a)];
                         case 1:
                             return c = w.sent(), u = bo(c), l = t.fragment ? "#".concat(t.fragment) : "", f = this._getParams(s, o, i, u, n), h = this._authorizeUrl(f), p = t.organization || this.options.organization, this.transactionManager.create(N({
                                 nonce: i,
                                 code_verifier: a,
                                 appState: r,
                                 scope: f.scope,
                                 audience: f.audience || "default",
@@ -14445,19 +14445,19 @@
                     switch (b.label) {
                         case 0:
                             if (t = t || {}, !(n = n || {}).popup && (n.popup = function(g) {
                                     var v = window.screenX + (window.innerWidth - 400) / 2,
                                         I = window.screenY + (window.innerHeight - 600) / 2;
                                     return window.open(g, "auth0:authorize:popup", "left=".concat(v, ",top=").concat(I, ",width=").concat(400, ",height=").concat(600, ",resizable,scrollbars=yes,status=1"))
                                 }(""), !n.popup)) throw new Error("Unable to open a popup for loginWithPopup - window.open returned `null`");
-                            return r = Tt(t, []), s = Dn(ge()), o = Dn(ge()), i = ge(), [4, yo(i)];
+                            return r = Tt(t, []), s = kn(ge()), o = kn(ge()), i = ge(), [4, yo(i)];
                         case 1:
                             return a = b.sent(), c = bo(a), u = this._getParams(r, s, o, c, this.options.redirect_uri || window.location.origin), l = this._authorizeUrl(N(N({}, u), {
                                 response_mode: "web_message"
-                            })), n.popup.location.href = l, [4, s_(N(N({}, n), {
+                            })), n.popup.location.href = l, [4, o_(N(N({}, n), {
                                 timeoutInSeconds: n.timeoutInSeconds || this.options.authorizeTimeoutInSeconds || 60
                             }))];
                         case 2:
                             if (f = b.sent(), s !== f.state) throw new Error("Invalid state");
                             return [4, Ii({
                                 audience: u.audience,
                                 scope: u.scope,
@@ -14490,15 +14490,15 @@
             })
         }, e.prototype.getUser = function(t) {
             return t === void 0 && (t = {}), $(this, void 0, void 0, function() {
                 var n, r, s;
                 return Y(this, function(o) {
                     switch (o.label) {
                         case 0:
-                            return n = t.audience || this.options.audience || "default", r = Ce(this.defaultScope, this.scope, t.scope), [4, this.cacheManager.get(new an({
+                            return n = t.audience || this.options.audience || "default", r = Ce(this.defaultScope, this.scope, t.scope), [4, this.cacheManager.get(new un({
                                 client_id: this.options.client_id,
                                 audience: n,
                                 scope: r
                             }))];
                         case 1:
                             return [2, (s = o.sent()) && s.decodedToken && s.decodedToken.user]
                     }
@@ -14506,15 +14506,15 @@
             })
         }, e.prototype.getIdTokenClaims = function(t) {
             return t === void 0 && (t = {}), $(this, void 0, void 0, function() {
                 var n, r, s;
                 return Y(this, function(o) {
                     switch (o.label) {
                         case 0:
-                            return n = t.audience || this.options.audience || "default", r = Ce(this.defaultScope, this.scope, t.scope), [4, this.cacheManager.get(new an({
+                            return n = t.audience || this.options.audience || "default", r = Ce(this.defaultScope, this.scope, t.scope), [4, this.cacheManager.get(new un({
                                 client_id: this.options.client_id,
                                 audience: n,
                                 scope: r
                             }))];
                         case 1:
                             return [2, (s = o.sent()) && s.decodedToken && s.decodedToken.claims]
                     }
@@ -14546,15 +14546,15 @@
                                     return w.forEach(function(b) {
                                         var g = ir(b.split("="), 2),
                                             v = g[0],
                                             I = g[1];
                                         _[v] = decodeURIComponent(I)
                                     }), _.expires_in && (_.expires_in = parseInt(_.expires_in)), _
                                 }(n.join("")), s = r.state, o = r.code, i = r.error, a = r.error_description, !(c = this.transactionManager.get())) throw new Error("Invalid state");
-                            if (this.transactionManager.remove(), i) throw new t_(i, a, s, c.appState);
+                            if (this.transactionManager.remove(), i) throw new e_(i, a, s, c.appState);
                             if (!c.code_verifier || c.state && c.state !== s) throw new Error("Invalid state");
                             return u = {
                                 audience: c.audience,
                                 scope: c.scope,
                                 baseUrl: this.domainUrl,
                                 client_id: this.options.client_id,
                                 code_verifier: c.code_verifier,
@@ -14601,15 +14601,15 @@
                             }
                             r.label = 1;
                         case 1:
                             return r.trys.push([1, 3, , 4]), [4, this.getTokenSilently(t)];
                         case 2:
                             return r.sent(), [3, 4];
                         case 3:
-                            if (n = r.sent(), !Qw.includes(n.error)) throw n;
+                            if (n = r.sent(), !t_.includes(n.error)) throw n;
                             return [3, 4];
                         case 4:
                             return [2]
                     }
                 })
             })
         }, e.prototype.getTokenSilently = function(t) {
@@ -14719,17 +14719,17 @@
                 })
             })
         }, e.prototype.getTokenWithPopup = function(t, n) {
             return t === void 0 && (t = {}), n === void 0 && (n = {}), $(this, void 0, void 0, function() {
                 return Y(this, function(r) {
                     switch (r.label) {
                         case 0:
-                            return t.audience = t.audience || this.options.audience, t.scope = Ce(this.defaultScope, this.scope, t.scope), n = N(N({}, qw), n), [4, this.loginWithPopup(t, n)];
+                            return t.audience = t.audience || this.options.audience, t.scope = Ce(this.defaultScope, this.scope, t.scope), n = N(N({}, Qw), n), [4, this.loginWithPopup(t, n)];
                         case 1:
-                            return r.sent(), [4, this.cacheManager.get(new an({
+                            return r.sent(), [4, this.cacheManager.get(new un({
                                 scope: t.scope,
                                 audience: t.audience || "default",
                                 client_id: this.options.client_id
                             }))];
                         case 2:
                             return [2, r.sent().access_token]
                     }
@@ -14774,37 +14774,37 @@
             this.cacheManager.clearSync(), o()
         }, e.prototype._getTokenFromIFrame = function(t) {
             return $(this, void 0, void 0, function() {
                 var n, r, s, o, i, a, c, u, l, f, h, p, w, _, b, g, v;
                 return Y(this, function(I) {
                     switch (I.label) {
                         case 0:
-                            return n = Dn(ge()), r = Dn(ge()), s = ge(), [4, yo(s)];
+                            return n = kn(ge()), r = kn(ge()), s = ge(), [4, yo(s)];
                         case 1:
                             o = I.sent(), i = bo(o), a = Tt(t, ["detailedResponse"]), c = this._getParams(a, n, r, i, t.redirect_uri || this.options.redirect_uri || window.location.origin), (u = this.cookieStorage.get(this.orgHintCookieName)) && !c.organization && (c.organization = u), l = this._authorizeUrl(N(N({}, c), {
                                 prompt: "none",
                                 response_mode: "web_message"
                             })), I.label = 2;
                         case 2:
                             if (I.trys.push([2, 6, , 7]), window.crossOriginIsolated) throw new xe("login_required", "The application is running in a Cross-Origin Isolated context, silently retrieving a token without refresh token is not possible.");
-                            return f = t.timeoutInSeconds || this.options.authorizeTimeoutInSeconds, [4, (it = l, yt = this.domainUrl, Dt = f, Dt === void 0 && (Dt = 60), new Promise(function(me, Oc) {
-                                var tn = window.document.createElement("iframe");
-                                tn.setAttribute("width", "0"), tn.setAttribute("height", "0"), tn.style.display = "none";
-                                var ui, Fc = function() {
-                                        window.document.body.contains(tn) && (window.document.body.removeChild(tn), window.removeEventListener("message", ui, !1))
+                            return f = t.timeoutInSeconds || this.options.authorizeTimeoutInSeconds, [4, (it = l, yt = this.domainUrl, Dt = f, Dt === void 0 && (Dt = 60), new Promise(function(me, xc) {
+                                var nn = window.document.createElement("iframe");
+                                nn.setAttribute("width", "0"), nn.setAttribute("height", "0"), nn.style.display = "none";
+                                var ui, Lc = function() {
+                                        window.document.body.contains(nn) && (window.document.body.removeChild(nn), window.removeEventListener("message", ui, !1))
                                     },
-                                    Fd = setTimeout(function() {
-                                        Oc(new Xo), Fc()
+                                    xd = setTimeout(function() {
+                                        xc(new Xo), Lc()
                                     }, 1e3 * Dt);
-                                ui = function(en) {
-                                    if (en.origin == yt && en.data && en.data.type === "authorization_response") {
-                                        var xc = en.source;
-                                        xc && xc.close(), en.data.response.error ? Oc(xe.fromPayload(en.data.response)) : me(en.data.response), clearTimeout(Fd), window.removeEventListener("message", ui, !1), setTimeout(Fc, 2e3)
+                                ui = function(rn) {
+                                    if (rn.origin == yt && rn.data && rn.data.type === "authorization_response") {
+                                        var Dc = rn.source;
+                                        Dc && Dc.close(), rn.data.response.error ? xc(xe.fromPayload(rn.data.response)) : me(rn.data.response), clearTimeout(xd), window.removeEventListener("message", ui, !1), setTimeout(Lc, 2e3)
                                     }
-                                }, window.addEventListener("message", ui, !1), window.document.body.appendChild(tn), tn.setAttribute("src", it)
+                                }, window.addEventListener("message", ui, !1), window.document.body.appendChild(nn), nn.setAttribute("src", it)
                             }))];
                         case 3:
                             if (h = I.sent(), n !== h.state) throw new Error("Invalid state");
                             return p = t.scope, w = t.audience, _ = Tt(t, ["scope", "audience", "redirect_uri", "ignoreCache", "timeoutInSeconds", "detailedResponse"]), [4, Ii(N(N(N({}, this.customOptions), _), {
                                 scope: p,
                                 audience: w,
                                 baseUrl: this.domainUrl,
@@ -14838,25 +14838,25 @@
             })
         }, e.prototype._getTokenUsingRefreshToken = function(t) {
             return $(this, void 0, void 0, function() {
                 var n, r, s, o, i, a, c, u, l;
                 return Y(this, function(f) {
                     switch (f.label) {
                         case 0:
-                            return t.scope = Ce(this.defaultScope, this.options.scope, t.scope), [4, this.cacheManager.get(new an({
+                            return t.scope = Ce(this.defaultScope, this.options.scope, t.scope), [4, this.cacheManager.get(new un({
                                 scope: t.scope,
                                 audience: t.audience || "default",
                                 client_id: this.options.client_id
                             }))];
                         case 1:
                             return (n = f.sent()) && n.refresh_token || this.worker ? [3, 4] : this.useRefreshTokensFallback ? [4, this._getTokenFromIFrame(t)] : [3, 3];
                         case 2:
                             return [2, f.sent()];
                         case 3:
-                            throw new i_(t.audience || "default", t.scope);
+                            throw new s_(t.audience || "default", t.scope);
                         case 4:
                             r = t.redirect_uri || this.options.redirect_uri || window.location.origin, o = t.scope, i = t.audience, a = Tt(t, ["scope", "audience", "ignoreCache", "timeoutInSeconds", "detailedResponse"]), c = typeof t.timeoutInSeconds == "number" ? 1e3 * t.timeoutInSeconds : null, f.label = 5;
                         case 5:
                             return f.trys.push([5, 7, , 10]), [4, Ii(N(N(N(N(N({}, this.customOptions), a), {
                                 audience: i,
                                 scope: o,
                                 baseUrl: this.domainUrl,
@@ -14898,15 +14898,15 @@
                 o = t.getDetailedEntry,
                 i = o !== void 0 && o;
             return $(this, void 0, void 0, function() {
                 var a, c, u, l, f;
                 return Y(this, function(h) {
                     switch (h.label) {
                         case 0:
-                            return [4, this.cacheManager.get(new an({
+                            return [4, this.cacheManager.get(new un({
                                 scope: n,
                                 audience: r,
                                 client_id: s
                             }), 60)];
                         case 1:
                             return (a = h.sent()) && a.access_token ? i ? (c = a.id_token, u = a.access_token, l = a.oauthTokenScope, f = a.expires_in, [2, N(N({
                                 id_token: c,
@@ -14918,41 +14918,41 @@
                             })]) : [2, a.access_token] : [2]
                     }
                 })
             })
         }, e
     }();
 
-function O_(e) {
+function F_(e) {
     return $(this, void 0, void 0, function() {
         var t;
         return Y(this, function(n) {
             switch (n.label) {
                 case 0:
-                    return [4, (t = new B_(e)).checkSession()];
+                    return [4, (t = new O_(e)).checkSession()];
                 case 1:
                     return n.sent(), [2, t]
             }
         })
     })
 }
-var F_ = {
+var x_ = {
     exports: {}
 };
 /*!
  * Toastify js 1.12.0
  * https://github.com/apvarun/toastify-js
  * @license MIT licensed
  *
  * Copyright (C) 2018 Varun A P
  */
 (function(e) {
     (function(t, n) {
         e.exports ? e.exports = n() : t.Toastify = n()
-    })(xd, function(t) {
+    })(Ld, function(t) {
         var n = function(i) {
                 return new n.lib.init(i)
             },
             r = "1.12.0";
         n.defaults = {
             oldestFirst: !0,
             text: "Toastify is awesome!",
@@ -15070,75 +15070,75 @@
         }
 
         function o(i, a) {
             return !i || typeof a != "string" ? !1 : !!(i.className && i.className.trim().split(/\s+/gi).indexOf(a) > -1)
         }
         return n.lib.init.prototype = n.lib, n
     })
-})(F_);
-const Ac = document.body.appendChild(document.createElement("div")),
-    ue = Ac.appendChild(document.createElement("button"));
-ue.className = "log";
-ue.textContent = "Login";
-Ac.style = "display: flex; flex-direction: column; color: rgb(104, 85, 224); font-weight: 600; margin: 0; padding: 10px";
-const yl = Ac.appendChild(document.createTextNode(""));
-let Qo, ta, Nn, Mn, Cn;
-const Od = async () => {
-    Cn.logout({
-        returnTo: ea()
-    }), ue.textContent = "Login", ue.removeEventListener("click", Od), ue.addEventListener("click", Bc)
-}, Bc = async () => {
-    Mn && console.log(`Configuration:
-  Client Id:` + Qo + `
-  Domain:`, ta + `
-  Audience:`, Nn + `
-  Callback urls set to: `, ea() + `
-`), ue.textContent = "working...", Cn = await O_({
-        domain: ta,
-        client_id: Qo,
-        redirect_uri: ea(),
-        audience: Nn,
-        useRefreshTokens: !0,
-        cacheLocation: "localstorage"
-    });
-    try {
-        await Cn.loginWithPopup(), yl.textContent = ""
-    } catch (r) {
-        console.log(r), yl.textContent = "Popup blocked, please try again or enable popups" + String.fromCharCode(160);
-        return
-    }
-    const e = await Cn.getUser();
-    Mn && (console.log(e), console.log({
-        audience: Nn,
-        scope: "read:current_user"
-    }));
-    let t = !1;
-    try {
-        t = await Cn.getTokenSilently({
-            audience: Nn,
-            scope: "read:current_user"
-        })
-    } catch (r) {
-        r.error === "consent_required" || r.error === "login_required" ? (Mn && console.log("asking user for permission to their profile"), t = await Cn.getTokenWithPopup({
-            audience: Nn,
+})(x_);
+const Sc = document.body.appendChild(document.createElement("div")),
+    Nt = Sc.appendChild(document.createElement("button"));
+Nt.className = "log";
+Nt.textContent = "Login";
+Sc.style = "display: flex; flex-direction: column; color: rgb(104, 85, 224); font-weight: 600; margin: 0; padding: 10px";
+const ml = Sc.appendChild(document.createTextNode(""));
+let Ic, Tc, jn, Mn, ze;
+const Ac = () => {
+        if (window.parent !== window) {
+            const e = new URL(document.location.href),
+                t = e.origin,
+                n = decodeURIComponent(e.pathname);
+            return t + n
+        } else return window.location.origin
+    },
+    Bc = async () => {
+        ze || (ze = await F_({
+            domain: Tc,
+            client_id: Ic,
+            redirect_uri: Ac(),
+            audience: jn,
+            useRefreshTokens: !0,
+            cacheLocation: "localstorage"
+        }))
+    }, Oc = async () => {
+        await Bc(), ze.logout({
+            returnTo: Ac()
+        }), Nt.textContent = "Login", Nt.removeEventListener("click", Oc), Nt.addEventListener("click", Fc), Je.setComponentValue(null)
+    }, Fc = async () => {
+        Mn && console.log(`Configuration:
+  Client Id:` + Ic + `
+  Domain:`, Tc + `
+  Audience:`, jn + `
+  Callback urls set to: `, Ac() + `
+`), Nt.textContent = "working...", await Bc();
+        try {
+            await ze.loginWithPopup(), ml.textContent = ""
+        } catch (r) {
+            console.log(r), ml.textContent = "Popup blocked, please try again or enable popups" + String.fromCharCode(160);
+            return
+        }
+        const e = await ze.getUser();
+        Mn && (console.log(e), console.log({
+            audience: jn,
             scope: "read:current_user"
-        }), Mn && console.log(t)) : console.error(r)
-    }
-    let n = JSON.parse(JSON.stringify(e));
-    n.token = t, Mn && console.log(n), mn.setComponentValue(n), ue.textContent = "Logout", ue.removeEventListener("click", Bc), ue.addEventListener("click", Od)
-};
-ue.onclick = Bc;
-
-function x_(e) {
+        }));
+        let t = !1;
+        try {
+            t = await ze.getTokenSilently({
+                audience: jn,
+                scope: "read:current_user"
+            })
+        } catch (r) {
+            r.error === "consent_required" || r.error === "login_required" ? (Mn && console.log("asking user for permission to their profile"), t = await ze.getTokenWithPopup({
+                audience: jn,
+                scope: "read:current_user"
+            }), Mn && console.log(t)) : console.error(r)
+        }
+        let n = JSON.parse(JSON.stringify(e));
+        n.token = t, Mn && console.log(n), Je.setComponentValue(n), Nt.textContent = "Logout", Nt.removeEventListener("click", Fc), Nt.addEventListener("click", Oc)
+    };
+async function L_(e) {
     const t = e.detail;
-    Qo = t.args.client_id, ta = t.args.domain, Nn = t.args.audience, Mn = t.args.debug_logs, mn.setFrameHeight()
+    Ic = t.args.client_id, Tc = t.args.domain, jn = t.args.audience, Mn = t.args.debug_logs, await Bc(), await ze.isAuthenticated() ? (Nt.textContent = "Logout", Nt.onclick = Oc) : (Nt.textContent = "Login", Nt.onclick = Fc), Je.setFrameHeight()
 }
-mn.events.addEventListener(mn.RENDER_EVENT, x_);
-mn.setComponentReady();
-const ea = () => {
-    if (window.parent !== window) {
-        const e = new URL(document.location.href),
-            t = e.origin,
-            n = decodeURIComponent(e.pathname);
-        return t + n
-    } else return window.location.origin
-};
+Je.events.addEventListener(Je.RENDER_EVENT, L_);
+Je.setComponentReady();
```

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/auth0_component/frontend/dist/assets/index.1dbfa948.css` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.1dbfa948.css`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.2.0.4.dev1689876708/setup.py` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.py`

 * *Files identical despite different names*

