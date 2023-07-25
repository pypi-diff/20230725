# Comparing `tmp/jupyter_viz_extension-0.2.0.tar.gz` & `tmp/jupyter_viz_extension-0.2.1.tar.gz`

## Comparing `jupyter_viz_extension-0.2.0.tar` & `jupyter_viz_extension-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/install.json
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter-config/nb-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter-config/server-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/_version.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/cmd.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/paraview.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/trame.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/user.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/package.json
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/remoteEntry.50eab919879261efcfd5.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/style.js
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/jupyter_viz_extension/share/launch_paraview.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/schema/plugin.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/components.tsx
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/dialogs.tsx
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/handler.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/index.tsx
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/paraview.tsx
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/src/trame.tsx
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/style/base.css
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/style/collapsible.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/style/index.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/LICENSE
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/.yarnrc.yml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/install.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter-config/nb-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter-config/server-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/_version.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/cmd.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/paraview.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/trame.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/user.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/package.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/remoteEntry.5dcc448ea4f84de302ab.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/jupyter_viz_extension/share/launch_paraview.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/schema/plugin.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/components.tsx
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/dialogs.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/handler.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/index.tsx
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/paraview.tsx
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/src/trame.tsx
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/base.css
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/collapsible.css
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/style/index.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.1/PKG-INFO
```

### Comparing `jupyter_viz_extension-0.2.0/package.json` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.5dcc448ea4f84de302ab.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -104,14 +104,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.5dcc448ea4f84de302ab.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
                 "managers": [
                     "pip"
@@ -178,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyter_viz_extension-0.2.0/tsconfig.json` & `jupyter_viz_extension-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/yarn.lock` & `jupyter_viz_extension-0.2.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/__init__.py` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/cmd.py` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/cmd.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/paraview.py` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/paraview.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/trame.py` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/trame.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/handlers/user.py` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/handlers/user.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/package.json` & `jupyter_viz_extension-0.2.1/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.2.1'"}*

```diff
@@ -104,19 +104,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.50eab919879261efcfd5.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
                 "managers": [
                     "pip"
@@ -183,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/remoteEntry.50eab919879261efcfd5.js` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/remoteEntry.5dcc448ea4f84de302ab.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, g, m, y = {
-            840: (e, r, t) => {
+            299: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./extension": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-viz-extension", "0.2.0", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-viz-extension", "0.2.1", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -284,10 +284,10 @@
                     u && u(j)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyter_viz_extension = self.webpackChunkjupyter_viz_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
-    var S = j(840);
+    var S = j(299);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyter-viz-extension"] = S
 })();
```

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/labextension/static/third-party-licenses.json` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/jupyter_viz_extension/share/launch_paraview.in` & `jupyter_viz_extension-0.2.1/jupyter_viz_extension/share/launch_paraview.in`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/src/dialogs.tsx` & `jupyter_viz_extension-0.2.1/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/src/handler.ts` & `jupyter_viz_extension-0.2.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/src/index.tsx` & `jupyter_viz_extension-0.2.1/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/src/paraview.tsx` & `jupyter_viz_extension-0.2.1/src/paraview.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/src/trame.tsx` & `jupyter_viz_extension-0.2.1/src/trame.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/style/collapsible.css` & `jupyter_viz_extension-0.2.1/style/collapsible.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/.gitignore` & `jupyter_viz_extension-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/LICENSE` & `jupyter_viz_extension-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/README.md` & `jupyter_viz_extension-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/pyproject.toml` & `jupyter_viz_extension-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.0/PKG-INFO` & `jupyter_viz_extension-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_viz_extension
-Version: 0.2.0
+Version: 0.2.1
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyter-viz-extension
 Project-URL: Bug Tracker, https://github.com/github_username/jupyter-viz-extension/issues
 Project-URL: Repository, https://github.com/github_username/jupyter-viz-extension.git
 Author-email: Jonathan Windgassen <j.windgassen@fz-juelich.de>
 License: BSD 3-Clause License
```

