# Comparing `tmp/webpty-3.7.tar.gz` & `tmp/webpty-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpty-3.7.tar", max compression
+gzip compressed data, was "webpty-3.8.tar", max compression
```

## Comparing `webpty-3.7.tar` & `webpty-3.8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1071 2022-12-22 09:48:14.480245 webpty-3.7/LICENSE
--rw-r--r--   0        0        0     1531 2022-12-22 09:48:14.480245 webpty-3.7/README.md
--rw-r--r--   0        0        0      513 2022-12-22 09:48:14.480245 webpty-3.7/pyproject.toml
--rw-r--r--   0        0        0      181 2022-12-22 09:48:14.480245 webpty-3.7/webpty/__init__.py
--rw-r--r--   0        0        0     1011 2022-12-22 09:48:14.480245 webpty-3.7/webpty/index.html
--rw-r--r--   0        0        0     6267 2022-12-22 09:48:14.480245 webpty-3.7/webpty/server.py
--rw-r--r--   0        0        0      232 2022-12-22 09:48:14.480245 webpty-3.7/webpty/static/webpty.css
--rw-r--r--   0        0        0     2993 2022-12-22 09:48:14.480245 webpty-3.7/webpty/static/webpty.js
--rw-r--r--   0        0        0      200 2022-12-22 09:48:14.480245 webpty-3.7/webpty/static/webpty.min.css
--rw-r--r--   0        0        0     1685 2022-12-22 09:48:14.480245 webpty-3.7/webpty/static/webpty.min.js
--rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 webpty-3.7/setup.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 webpty-3.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-12-16 06:19:27.884454 webpty-3.8/LICENSE
+-rw-r--r--   0        0        0     1531 2022-12-16 06:19:27.884968 webpty-3.8/README.md
+-rw-r--r--   0        0        0      514 2023-07-25 06:07:12.333576 webpty-3.8/pyproject.toml
+-rw-r--r--   0        0        0      181 2022-12-16 11:42:16.018623 webpty-3.8/webpty/__init__.py
+-rw-r--r--   0        0        0     1011 2023-07-25 06:05:13.399487 webpty-3.8/webpty/index.html
+-rw-r--r--   0        0        0     6267 2022-12-16 11:42:16.019541 webpty-3.8/webpty/server.py
+-rw-r--r--   0        0        0      232 2022-12-16 11:42:16.019787 webpty-3.8/webpty/static/webpty.css
+-rw-r--r--   0        0        0     3043 2023-07-25 06:02:28.894895 webpty-3.8/webpty/static/webpty.js
+-rw-r--r--   0        0        0      200 2022-12-16 11:42:16.020425 webpty-3.8/webpty/static/webpty.min.css
+-rw-r--r--   0        0        0     1767 2023-07-25 06:05:02.484896 webpty-3.8/webpty/static/webpty.min.js
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 webpty-3.8/PKG-INFO
```

### Comparing `webpty-3.7/LICENSE` & `webpty-3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webpty-3.7/README.md` & `webpty-3.8/README.md`

 * *Files identical despite different names*

### Comparing `webpty-3.7/pyproject.toml` & `webpty-3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "webpty"
-version = "3.7"
+version = "3.8"
 description = "A web-based application to access shell & shell based applications via a browser"
 readme = "README.md"
 authors = ["Satheesh Kumar <mail@satheesh.dev>"]
 license = "OSI Approved :: MIT License"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<=3.9"
+python = ">=3.7,<=3.10"
 tornado = "6.2"
 requests = "2.28.1"
 importlib-metadata = "^5.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
```

### Comparing `webpty-3.7/webpty/index.html` & `webpty-3.8/webpty/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="utf-8">
   <title>webpty v{{app_version}}</title>
   <link rel="preconnect" href="https://fonts.gstatic.com">
   <link href="https://fonts.googleapis.com/css2?family=Source+Code+Pro&display=swap" rel="stylesheet">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/xterm@5.0.0/css/xterm.css" />
+  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/xterm@5.2.1/css/xterm.css" />
   <link rel="stylesheet" href=".{{ static_url("webpty.min.css") }}" />
 </head>
 <body>
     <div id="webpty"></div>
     <script>
         const APP_SECURED = {% if is_secured %} true {% else %} false {% end %};
         const KEEP_ALIVE = {{keepalive}};
     </script>
-    <script src="https://cdn.jsdelivr.net/npm/xterm@5.0.0/lib/xterm.min.js"></script>
-    <script src="https://cdn.jsdelivr.net/npm/xterm-addon-fit@0.6.0/lib/xterm-addon-fit.min.js"></script>
-    <script src="https://cdn.jsdelivr.net/npm/xterm-addon-web-links@0.7.0/lib/xterm-addon-web-links.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/xterm@5.2.1/lib/xterm.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/xterm-addon-fit@0.7.0/lib/xterm-addon-fit.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/xterm-addon-web-links@0.8.0/lib/xterm-addon-web-links.min.js"></script>
     <script src=".{{ static_url("webpty.min.js") }}"></script>
 </body>
 </html>
```

### Comparing `webpty-3.7/webpty/server.py` & `webpty-3.8/webpty/server.py`

 * *Files identical despite different names*

### Comparing `webpty-3.7/webpty/static/webpty.js` & `webpty-3.8/webpty/static/webpty.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,16 @@
+function callWithDelay(func, delay) {
+    let timeout;
+    return function(...args) {
+        const context = this;
+        clearTimeout(timeout);
+        timeout = setTimeout(() => func.apply(context, args), delay);
+    };
+}
+
 function startApp() {
     const delay = 50;
     const host = window.location.host;
     const pathname = window.location.pathname;
     const scrollBackLimit = 5000; // current limit is 5000, change it in future if required
     const fitAddon = new FitAddon.FitAddon();
     const terminal = new Terminal({
@@ -17,35 +26,27 @@
         "wss";
     const ws = new WebSocket(`${webSocketProtocol}://${host}${pathname}pty`);
 
     terminal.loadAddon(fitAddon);
 
     function fitToScreen() {
         fitAddon.fit();
+        console.log(terminal.cols, terminal.rows);
         ws.send(
             JSON.stringify({
                 action: "resize",
                 data: {
                     cols: terminal.cols,
                     rows: terminal.rows
                 },
             })
         );
     }
 
-    function resizeDelay(func, delay) {
-        let timeout;
-        return function(...args) {
-            const context = this;
-            clearTimeout(timeout);
-            timeout = setTimeout(() => func.apply(context, args), delay);
-        };
-    }
-
-    window.onresize = resizeDelay(fitToScreen, delay);
+    window.onresize = callWithDelay(fitToScreen, delay);
 
     ws.onopen = function() {
         terminal.open(document.getElementById(terminalDivId));
         terminal.options.scrollback = scrollBackLimit;
         fitToScreen();
     };
 
@@ -125,8 +126,9 @@
                 if (this.status === 200) {
                     location.reload();
                 }
             };
         }
     }
 }
-startApp();
+
+window.onload = startApp;
```

### Comparing `webpty-3.7/webpty/static/webpty.min.js` & `webpty-3.8/webpty/static/webpty.min.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,73 +1,75 @@
+function callWithDelay(t, e) {
+    let s;
+    return function(...o) {
+        let n = this;
+        clearTimeout(s), s = setTimeout(() => t.apply(n, o), e)
+    }
+}
+
 function startApp() {
-    var e;
     let t = window.location.host,
-        s = window.location.pathname,
-        o = new FitAddon.FitAddon,
-        n = new Terminal({
+        e = window.location.pathname,
+        s = new FitAddon.FitAddon,
+        o = new Terminal({
             screenKeys: !0,
             cursorBlink: !0,
             macOptionIsMeta: !0,
             scrollback: !0,
             fontFamily: "Source Code Pro"
         }),
-        a = window.location.protocol.indexOf("https") ? "ws" : "wss",
-        r = new WebSocket(`${a}://${t}${s}pty`);
+        n = window.location.protocol.indexOf("https") ? "ws" : "wss",
+        a = new WebSocket(`${n}://${t}${e}pty`);
 
     function i() {
-        o.fit(), r.send(JSON.stringify({
+        s.fit(), console.log(o.cols, o.rows), a.send(JSON.stringify({
             action: "resize",
             data: {
-                cols: n.cols,
-                rows: n.rows
+                cols: o.cols,
+                rows: o.rows
             }
         }))
     }
-    n.loadAddon(o);
-    let d;
-    window.onresize = (e = i, function(...t) {
-        let s = this;
-        clearTimeout(d), d = setTimeout(() => e.apply(s, t), 50)
-    }), r.onopen = function() {
-        n.open(document.getElementById("webpty")), n.options.scrollback = 5e3, i()
-    }, r.onmessage = function(e) {
-        n.write(e.data)
-    }, n.onKey(e => {
-        r.send(JSON.stringify({
+    o.loadAddon(s), window.onresize = callWithDelay(i, 50), a.onopen = function() {
+        o.open(document.getElementById("webpty")), o.options.scrollback = 5e3, i()
+    }, a.onmessage = function(t) {
+        o.write(t.data)
+    }, o.onKey(t => {
+        a.send(JSON.stringify({
             action: "input",
             data: {
-                key: e.key
+                key: t.key
             }
         }))
-    }), n.attachCustomKeyEventHandler(e => {
-        (e.ctrlKey || e.metaKey) && "KeyV" === e.code && "keydown" === e.type && (navigator.clipboard.readText().then(e => {
-            r.send(JSON.stringify({
+    }), o.attachCustomKeyEventHandler(t => {
+        (t.ctrlKey || t.metaKey) && "KeyV" === t.code && "keydown" === t.type && (navigator.clipboard.readText().then(t => {
+            a.send(JSON.stringify({
                 action: "input",
                 data: {
-                    key: e
+                    key: t
                 }
             }))
-        }), e.preventDefault())
-    }), KEEP_ALIVE && setInterval(function e() {
-        r.send(JSON.stringify({
+        }), t.preventDefault())
+    }), KEEP_ALIVE && setInterval(function t() {
+        a.send(JSON.stringify({
             action: "ping"
         }))
     }, 1e3 * KEEP_ALIVE)
 }
 
 function getPasswordFromCookie() {
-    let e = `; ${document.cookie}`,
-        t = e.split("; webptyPass=");
-    if (2 === t.length) return t.pop().split(";").shift()
+    let t = `; ${document.cookie}`,
+        e = t.split("; webptyPass=");
+    if (2 === e.length) return e.pop().split(";").shift()
 }
 if (APP_SECURED) {
     for (var userPassword = getPasswordFromCookie(); null === userPassword || "" === userPassword || void 0 === userPassword;)
         if (userPassword = prompt("This is a password protected shell. Please enter your password.")) {
-            var e = new XMLHttpRequest;
-            e.open("POST", "/auth", !0), e.setRequestHeader("Content-Type", "application/json"), e.send(JSON.stringify({
+            var t = new XMLHttpRequest;
+            t.open("POST", "/auth", !0), t.setRequestHeader("Content-Type", "application/json"), t.send(JSON.stringify({
                 webptyPass: userPassword
-            })), e.onreadystatechange = function() {
+            })), t.onreadystatechange = function() {
                 4 == this.readyState && (200 !== this.status && (userPassword = null), 200 === this.status && location.reload())
             }
         }
 }
-startApp();
+window.onload = startApp;
```

### Comparing `webpty-3.7/PKG-INFO` & `webpty-3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: webpty
-Version: 3.7
+Version: 3.8
 Summary: A web-based application to access shell & shell based applications via a browser
 License: OSI Approved :: MIT License
 Author: Satheesh Kumar
 Author-email: mail@satheesh.dev
-Requires-Python: >=3.7,<=3.9
+Requires-Python: >=3.7,<=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
 Requires-Dist: requests (==2.28.1)
 Requires-Dist: tornado (==6.2)
 Description-Content-Type: text/markdown
 
 # webpty
```

