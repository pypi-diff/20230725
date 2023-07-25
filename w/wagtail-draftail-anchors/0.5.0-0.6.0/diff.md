# Comparing `tmp/wagtail_draftail_anchors-0.5.0-py3-none-any.whl.zip` & `tmp/wagtail_draftail_anchors-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13585 bytes, number of entries: 12
+Zip file size: 13774 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       85 b- defN 20-May-13 10:07 wagtail_draftail_anchors/__init__.py
 -rw-rw-r--  2.0 unx      266 b- defN 22-Mar-30 08:10 wagtail_draftail_anchors/apps.py
--rw-rw-r--  2.0 unx     3698 b- defN 23-Jan-05 10:46 wagtail_draftail_anchors/rich_text.py
--rw-rw-r--  2.0 unx     4071 b- defN 23-Jan-05 10:46 wagtail_draftail_anchors/wagtail_hooks.py
+-rw-rw-r--  2.0 unx     3698 b- defN 23-Jul-25 10:39 wagtail_draftail_anchors/rich_text.py
+-rw-rw-r--  2.0 unx     4071 b- defN 23-Jul-25 10:39 wagtail_draftail_anchors/wagtail_hooks.py
 -rw-r--r--  2.0 unx      269 b- defN 20-May-05 13:51 wagtail_draftail_anchors/static/wagtaildraftailanchors/css/wagtail-draftail-anchor.css
 -rw-r--r--  2.0 unx     1396 b- defN 20-May-05 13:51 wagtail_draftail_anchors/static/wagtaildraftailanchors/fonts/wagtail-draftail-anchor.woff
--rw-rw-r--  2.0 unx    13404 b- defN 23-Jan-05 10:46 wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js
+-rw-rw-r--  2.0 unx    13771 b- defN 23-Jul-25 10:39 wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js
 -rw-r--r--  2.0 unx      899 b- defN 20-Jun-12 13:40 wagtail_draftail_anchors/templates/wagtaildraftailanchors/icons/anchor.svg
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jan-05 11:02 wagtail_draftail_anchors-0.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-05 11:02 wagtail_draftail_anchors-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Jan-05 11:02 wagtail_draftail_anchors-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1297 b- defN 23-Jan-05 11:02 wagtail_draftail_anchors-0.5.0.dist-info/RECORD
-12 files, 28038 bytes uncompressed, 11301 bytes compressed:  59.7%
+-rw-rw-r--  2.0 unx     2573 b- defN 23-Jul-25 10:42 wagtail_draftail_anchors-0.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 10:42 wagtail_draftail_anchors-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-25 10:42 wagtail_draftail_anchors-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1297 b- defN 23-Jul-25 10:42 wagtail_draftail_anchors-0.6.0.dist-info/RECORD
+12 files, 28442 bytes uncompressed, 11490 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js
 Comment: 
 
 Filename: wagtail_draftail_anchors/templates/wagtaildraftailanchors/icons/anchor.svg
 Comment: 
 
-Filename: wagtail_draftail_anchors-0.5.0.dist-info/METADATA
+Filename: wagtail_draftail_anchors-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: wagtail_draftail_anchors-0.5.0.dist-info/WHEEL
+Filename: wagtail_draftail_anchors-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: wagtail_draftail_anchors-0.5.0.dist-info/top_level.txt
+Filename: wagtail_draftail_anchors-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wagtail_draftail_anchors-0.5.0.dist-info/RECORD
+Filename: wagtail_draftail_anchors-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js

### js-beautify {}

```diff
@@ -139,36 +139,36 @@
         }
     }
 
     function p(t, e, n) {
         return e && s(t.prototype, e), n && s(t, n), t
     }
 
-    function y(t, e) {
+    function d(t, e) {
         if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function");
         t.prototype = Object.create(e && e.prototype, {
             constructor: {
                 value: t,
                 writable: !0,
                 configurable: !0
             }
-        }), e && d(t, e)
+        }), e && y(t, e)
     }
 
-    function d(t, e) {
-        return (d = Object.setPrototypeOf || function(t, e) {
+    function y(t, e) {
+        return (y = Object.setPrototypeOf || function(t, e) {
             return t.__proto__ = e, t
         })(t, e)
     }
 
     function h(t) {
         return function() {
-            var e, n = b(t);
-            if (w()) {
-                var r = b(this).constructor;
+            var e, n = w(t);
+            if (b()) {
+                var r = w(this).constructor;
                 e = Reflect.construct(n, arguments, r)
             } else e = n.apply(this, arguments);
             return g(this, e)
         }
     }
 
     function g(t, e) {
@@ -176,58 +176,58 @@
     }
 
     function m(t) {
         if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return t
     }
 
-    function w() {
+    function b() {
         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
         if (Reflect.construct.sham) return !1;
         if ("function" == typeof Proxy) return !0;
         try {
             return Date.prototype.toString.call(Reflect.construct(Date, [], (function() {}))), !0
         } catch (t) {
             return !1
         }
     }
 
-    function b(t) {
-        return (b = Object.setPrototypeOf ? Object.getPrototypeOf : function(t) {
+    function w(t) {
+        return (w = Object.setPrototypeOf ? Object.getPrototypeOf : function(t) {
             return t.__proto__ || Object.getPrototypeOf(t)
         })(t)
     }
     var v = window.React,
         E = window.DraftJS.RichUtils,
         O = window.DraftJS.Modifier,
         S = window.DraftJS.SelectionState,
         A = window.draftail.TooltipEntity,
         T = window.wagtail.components.Icon,
-        j = window.DraftJS.EditorState,
-        C = window.wagtail.components.Portal,
+        C = window.DraftJS.EditorState,
+        j = window.wagtail.components.Portal,
         U = window.draftail.Tooltip,
-        I = [],
         k = [],
+        I = [],
         D = [],
-        R = window.draftail.initEditor;
+        x = window.draftail.initEditor;
     window.draftail.registerControl = function(t) {
-        return k.push(t), k
-    }, window.draftail.registerDecorator = function(t) {
         return I.push(t), I
+    }, window.draftail.registerDecorator = function(t) {
+        return k.push(t), k
     }, window.draftail.initEditor = function(t, e, n) {
         var r = {
-                decorators: I.concat(e.decorators || []),
-                controls: k.concat(e.controls || []),
+                decorators: k.concat(e.decorators || []),
+                controls: I.concat(e.controls || []),
                 plugins: D.concat(e.plugins || [])
             },
             o = Object.assign({}, e, r);
-        return R(t, o, n)
+        return x(t, o, n)
     };
-    var x = function(t) {
-        y(n, t);
+    var L = function(t) {
+        d(n, t);
         var e = h(n);
 
         function n() {
             return f(this, n), e.apply(this, arguments)
         }
         return p(n, [{
             key: "componentDidMount",
@@ -251,15 +251,15 @@
             value: function() {
                 return null
             }
         }]), n
     }(v.Component);
     window.draftail.registerPlugin({
         type: "ANCHOR-IDENTIFIER",
-        source: x,
+        source: L,
         decorator: function(t) {
             var e = t.entityKey,
                 n = t.contentState.getEntity(e).getData();
             return v.createElement(A, c({}, t, function(t) {
                 var e = t.anchor || null;
                 return {
                     url: e,
@@ -267,85 +267,106 @@
                         name: "anchor"
                     }),
                     label: "#".concat(e)
                 }
             }(n)))
         }
     });
-    var L, P = function(t) {
-        y(n, t);
-        var e = h(n);
+    var R, P = function(t) {
+            var e = t.identifier,
+                n = i(v.useState(!1), 2),
+                r = n[0],
+                o = n[1];
+            return v.createElement("button", {
+                class: "button button-small",
+                style: {
+                    marginLeft: "1rem"
+                },
+                "aria-label": "Copy anchor identifier",
+                "aria-live": "polite",
+                role: "button",
+                onClick: function(t) {
+                    t.preventDefault(), navigator.clipboard.writeText(e), o(!0)
+                }
+            }, r ? "Copied" : "Copy")
+        },
+        _ = function(t) {
+            d(n, t);
+            var e = h(n);
 
-        function n(t) {
-            var r;
-            return f(this, n), (r = e.call(this, t)).state = {
-                showTooltipAt: null
-            }, r.openTooltip = r.openTooltip.bind(m(r)), r.closeTooltip = r.closeTooltip.bind(m(r)), r
-        }
-        return p(n, [{
-            key: "openTooltip",
-            value: function(t) {
-                var e = t.target.closest("[data-draftail-trigger]");
-                if (e) {
-                    var n = e.closest("[data-draftail-editor-wrapper]"),
-                        r = n.getBoundingClientRect(),
-                        o = e.getBoundingClientRect();
+            function n(t) {
+                var r;
+                return f(this, n), (r = e.call(this, t)).state = {
+                    showTooltipAt: null
+                }, r.openTooltip = r.openTooltip.bind(m(r)), r.closeTooltip = r.closeTooltip.bind(m(r)), r
+            }
+            return p(n, [{
+                key: "openTooltip",
+                value: function(t) {
+                    var e = t.target.closest("[data-draftail-trigger]");
+                    if (e) {
+                        var n = e.closest("[data-draftail-editor-wrapper]"),
+                            r = n.getBoundingClientRect(),
+                            o = e.getBoundingClientRect();
+                        this.setState({
+                            showTooltipAt: {
+                                container: n,
+                                top: o.top - r.top - (document.documentElement.scrollTop || document.body.scrollTop),
+                                left: o.left - r.left - (document.documentElement.scrollLeft || document.body.scrollLeft),
+                                width: o.width,
+                                height: o.height
+                            }
+                        })
+                    }
+                }
+            }, {
+                key: "closeTooltip",
+                value: function() {
                     this.setState({
-                        showTooltipAt: {
-                            container: n,
-                            top: o.top - r.top - (document.documentElement.scrollTop || document.body.scrollTop),
-                            left: o.left - r.left - (document.documentElement.scrollLeft || document.body.scrollLeft),
-                            width: o.width,
-                            height: o.height
-                        }
+                        showTooltipAt: null
                     })
                 }
-            }
-        }, {
-            key: "closeTooltip",
-            value: function() {
-                this.setState({
-                    showTooltipAt: null
-                })
-            }
-        }, {
-            key: "render",
-            value: function() {
-                var t = this.props.children,
-                    e = "#".concat(o()(this.props.decoratedText.toLowerCase())),
-                    n = this.state.showTooltipAt;
-                return v.createElement("a", {
-                    href: "",
-                    name: e,
-                    role: "button",
-                    onMouseUp: this.openTooltip,
-                    className: "TooltipEntity",
-                    "data-draftail-trigger": !0
-                }, v.createElement("sub", null, v.createElement(T, {
-                    name: "anchor",
-                    className: "TooltipEntity__icon"
-                })), t, n && v.createElement(C, {
-                    node: n.container,
-                    onClose: this.closeTooltip,
-                    closeOnClick: !0,
-                    closeOnType: !0,
-                    closeOnResize: !0
-                }, v.createElement(U, {
-                    target: n,
-                    direction: "top"
-                }, e)))
-            }
-        }]), n
-    }(v.Component);
-    L = {
+            }, {
+                key: "render",
+                value: function() {
+                    var t = this.props.children,
+                        e = o()(this.props.decoratedText.toLowerCase()),
+                        n = "#".concat(e),
+                        r = this.state.showTooltipAt;
+                    return v.createElement("a", {
+                        href: "",
+                        name: n,
+                        role: "button",
+                        onMouseUp: this.openTooltip,
+                        className: "TooltipEntity",
+                        "data-draftail-trigger": !0
+                    }, v.createElement("sub", null, v.createElement(T, {
+                        name: "anchor",
+                        className: "TooltipEntity__icon"
+                    })), t, r && v.createElement(j, {
+                        node: r.container,
+                        onClose: this.closeTooltip,
+                        closeOnClick: !0,
+                        closeOnType: !0,
+                        closeOnResize: !0
+                    }, v.createElement(U, {
+                        target: r,
+                        direction: "top"
+                    }, n, v.createElement(P, {
+                        identifier: e
+                    }))))
+                }
+            }]), n
+        }(v.Component);
+    R = {
         decorators: [{
             strategy: function(t, e, n) {
                 t.getType().includes("header") && e(0, t.getLength())
             },
-            component: P
+            component: _
         }],
         onChange: function(t, e) {
             var n = t.getCurrentContent();
             if (n == e.getEditorState().getCurrentContent()) return t;
             var r, u = n.getBlockMap(),
                 c = t.getSelection(),
                 l = t,
@@ -394,23 +415,23 @@
                         }
                     }
                 }(u.entries());
             try {
                 for (f.s(); !(r = f.n()).done;) {
                     var s = i(r.value, 2),
                         p = s[0],
-                        y = s[1];
-                    if (y.getType().includes("header")) {
-                        var d = S.createEmpty(p),
+                        d = s[1];
+                    if (d.getType().includes("header")) {
+                        var y = S.createEmpty(p),
                             h = new Map;
-                        h.set("anchor", o()(y.getText().toLowerCase())), n = O.mergeBlockData(n, d, h)
+                        h.set("anchor", o()(d.getText().toLowerCase())), n = O.mergeBlockData(n, y, h)
                     }
                 }
             } catch (t) {
                 f.e(t)
             } finally {
                 f.f()
             }
-            return l = j.push(t, n, t.getLastChangeType()), l = j.acceptSelection(l, c)
+            return l = C.push(t, n, t.getLastChangeType()), l = C.acceptSelection(l, c)
         }
-    }, D.push(L)
+    }, D.push(R)
 }]);
```

## Comparing `wagtail_draftail_anchors-0.5.0.dist-info/METADATA` & `wagtail_draftail_anchors-0.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: wagtail-draftail-anchors
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Draftail extension to add anchor identifiers to rich text
 Home-page: https://github.com/jacobtoppm/wagtail_draftail_anchors
 Author: Jacob Topp-Mugglestone, Quoc Duan
 Author-email: jacobtm@torchbox.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Wagtail :: 2
 Classifier: Framework :: Wagtail :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -62,7 +64,9 @@
 ``` python
 {"data-id": "my-anchor", "href": "#my-anchor", "id": "my-anchor", "linktype": "my-anchor"}
 ```
 
 If you define your own renderer, you should set the value of `DRAFTAIL_ANCHORS_RENDERER` to your custom renderer's import path.
 
 See `render_span` and `render_a` in `wagtail_draftail_anchors.rich_text` for examples.
+
+
```

### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: wagtail-draftail-anchors Version: 0.5.0 Summary: A
+Metadata-Version: 2.1 Name: wagtail-draftail-anchors Version: 0.6.0 Summary: A
 Draftail extension to add anchor identifiers to rich text Home-page: https://
 github.com/jacobtoppm/wagtail_draftail_anchors Author: Jacob Topp-Mugglestone,
-Quoc Duan Author-email: jacobtm@torchbox.com Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Requires-Dist: wagtail (>2.9) # Wagtail Draftail
-Anchors Adds the ability to add and edit anchors in the Draftail rich text
-editor, as well as automatically adding (slug-form) anchor ids to all headings.
-## Installation Install using `pip`: ``` pip install wagtail-draftail-anchors
-``` Add `'wagtail_draftail_anchors'` to `INSTALLED_APPS` below `wagtail.admin`.
-Add `'anchor-identifier'` to the features of any rich text field where you have
-overridden the default feature list. The feature must be added before any
-heading('h1',...,'h6') feature: ``` body = RichTextField(features=['anchor-
-identifier', 'h2', 'h3', 'bold', 'italic', 'link']) ``` ## Configuration ###
-Rendered representation of anchors By default, `anchor-identifier` rich text
-entities will be rendered as HTML `anchor` elements, e.g.: ``` html My_element
-``` This package provides an alternative renderer that renders `anchor-
-identifier` entities as HTML `span` elements, e.g.: ``` html My element ``` The
-desired renderer can be specified using the `DRAFTAIL_ANCHORS_RENDERER`
-setting. To use the `span` renderer, configure your application as follows: ```
-python DRAFTAIL_ANCHORS_RENDERER =
+Quoc Duan Author-email: jacobtm@torchbox.com License: UNKNOWN Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Framework :: Wagtail :: 2 Classifier: Framework :: Wagtail :: 3
+Requires-Python: >=3.6 Description-Content-Type: text/markdown Requires-Dist:
+wagtail (>2.9) # Wagtail Draftail Anchors Adds the ability to add and edit
+anchors in the Draftail rich text editor, as well as automatically adding
+(slug-form) anchor ids to all headings. ## Installation Install using `pip`:
+``` pip install wagtail-draftail-anchors ``` Add `'wagtail_draftail_anchors'`
+to `INSTALLED_APPS` below `wagtail.admin`. Add `'anchor-identifier'` to the
+features of any rich text field where you have overridden the default feature
+list. The feature must be added before any heading('h1',...,'h6') feature: ```
+body = RichTextField(features=['anchor-identifier', 'h2', 'h3', 'bold',
+'italic', 'link']) ``` ## Configuration ### Rendered representation of anchors
+By default, `anchor-identifier` rich text entities will be rendered as HTML
+`anchor` elements, e.g.: ``` html My_element ``` This package provides an
+alternative renderer that renders `anchor-identifier` entities as HTML `span`
+elements, e.g.: ``` html My element ``` The desired renderer can be specified
+using the `DRAFTAIL_ANCHORS_RENDERER` setting. To use the `span` renderer,
+configure your application as follows: ``` python DRAFTAIL_ANCHORS_RENDERER =
 "wagtail_draftail_anchors.rich_text.render_span" ``` It is possible to define
 your own renderer. It should be a callable that takes a `dict` of attributes,
 and returns a string containing the opening tag of the HTML element that
 represents the anchor target. The `dict` passed to the renderer, for an anchor
 with an identifier of `"my-anchor"`, would look like the following: ``` python
 {"data-id": "my-anchor", "href": "#my-anchor", "id": "my-anchor", "linktype":
 "my-anchor"} ``` If you define your own renderer, you should set the value of
```

## Comparing `wagtail_draftail_anchors-0.5.0.dist-info/RECORD` & `wagtail_draftail_anchors-0.6.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 wagtail_draftail_anchors/__init__.py,sha256=cl6roS_s0RlkJfC2cczMHBFoeXH__oa9a_yUn24jjmM,85
 wagtail_draftail_anchors/apps.py,sha256=XZsoM_3MVW3HVyYNMUjJyrzzr394LPa7n2OvZPoGiHk,266
 wagtail_draftail_anchors/rich_text.py,sha256=jXSmICfJaZNHg7soVOD3ziPOR5Y9lACZgEoFzr_GUS4,3698
 wagtail_draftail_anchors/wagtail_hooks.py,sha256=g7WMYLIDIIEPPjXsN7eGNNW9qYWIlkg-ytIhZThXp8Q,4071
 wagtail_draftail_anchors/static/wagtaildraftailanchors/css/wagtail-draftail-anchor.css,sha256=S21CJ2lCirabCaRp_RbUsW_AYpDKsMwQSSQKTxSlVas,269
 wagtail_draftail_anchors/static/wagtaildraftailanchors/fonts/wagtail-draftail-anchor.woff,sha256=S8XK7rgIYMUb7YP0ZMBwDentNm4cYWhR48qh6Y1KPrY,1396
-wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js,sha256=1j4taehhI7d5oFJb8s7JUHfJ6EZonmd_87TCgdt-aZM,13404
+wagtail_draftail_anchors/static/wagtaildraftailanchors/js/wagtail-draftail-anchor.js,sha256=nvvDhOG7mTkrQ8e3ffmpV9MmbY2CQnOgNHOeh8oA-PA,13771
 wagtail_draftail_anchors/templates/wagtaildraftailanchors/icons/anchor.svg,sha256=KHvsq26nAq1CGPIa9Tp6eWbfdBSqEeCe36UQnoZV-Ps,899
-wagtail_draftail_anchors-0.5.0.dist-info/METADATA,sha256=wW0vMtrkN_asuoEmSJmsU__C-CKEAX1uRQ6nge-YS7k,2536
-wagtail_draftail_anchors-0.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wagtail_draftail_anchors-0.5.0.dist-info/top_level.txt,sha256=X6HfDnVG27tVWfdTyHG-67mkuPOPG7mra4nKyjqmqhM,25
-wagtail_draftail_anchors-0.5.0.dist-info/RECORD,,
+wagtail_draftail_anchors-0.6.0.dist-info/METADATA,sha256=g4pCJ3_OIsS-CAABpOu48mOwYpXRxmrSLljRbLHmHEg,2573
+wagtail_draftail_anchors-0.6.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+wagtail_draftail_anchors-0.6.0.dist-info/top_level.txt,sha256=X6HfDnVG27tVWfdTyHG-67mkuPOPG7mra4nKyjqmqhM,25
+wagtail_draftail_anchors-0.6.0.dist-info/RECORD,,
```

