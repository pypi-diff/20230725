# Comparing `tmp/drawwithplt-0.3-py3-none-any.whl.zip` & `tmp/drawwithplt-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5904 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    14145 b- defN 23-Jul-24 02:22 drawwithplt.py
--rw-rw-rw-  2.0 fat     1032 b- defN 23-Jul-24 02:27 drawwithplt-0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 02:27 drawwithplt-0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-24 02:27 drawwithplt-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      378 b- defN 23-Jul-24 02:27 drawwithplt-0.3.dist-info/RECORD
-5 files, 15659 bytes uncompressed, 5202 bytes compressed:  66.8%
+Zip file size: 6034 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    14943 b- defN 23-Jul-25 02:35 drawwithplt.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-Jul-25 02:36 drawwithplt-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 02:36 drawwithplt-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-25 02:36 drawwithplt-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      386 b- defN 23-Jul-25 02:36 drawwithplt-0.3.1.dist-info/RECORD
+5 files, 16467 bytes uncompressed, 5316 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: drawwithplt.py
 Comment: 
 
-Filename: drawwithplt-0.3.dist-info/METADATA
+Filename: drawwithplt-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: drawwithplt-0.3.dist-info/WHEEL
+Filename: drawwithplt-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: drawwithplt-0.3.dist-info/top_level.txt
+Filename: drawwithplt-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: drawwithplt-0.3.dist-info/RECORD
+Filename: drawwithplt-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drawwithplt.py

```diff
@@ -309,40 +309,42 @@
         else:
             ax.plot(x,y,color=c,label=label)
     return p1
 
 def Initprop_forDrawMaps(prop, data):
     # 图片尺寸参数
     prop.setdefault("xl", 2.5)
-    prop.setdefault("yl", 2.5)
+    prop.setdefault("yl", 1.5)
+    prop.setdefault("aspect", "auto")
 
     # 图片横纵间隔
     prop.setdefault("space", (0.5, 0.5))
-    prop.setdefault("yl", 2.5)
     prop.setdefault("cbar_weight", 0.08)
 
     # 绘图参数-cbar
     prop.setdefault("c_labels", 'Cbar')
     prop.setdefault("cbar_str", 'seismic')
     prop.setdefault("vmin", np.min(data[(0,0)]))
     prop.setdefault("vmax", np.max(data[(0,0)]))
+    prop.setdefault("vs", 6)
+    prop.setdefault("v_fmt", "%.2f")
 
     # 刻度参数
     prop.setdefault("x0_ticks", [])
     prop.setdefault("x0_tlabels", [])
-    prop.setdefault("x0_labels", "x")
+    prop.setdefault("x0_labels", "x-%d")
 
     prop.setdefault("x_ticks", [])
     prop.setdefault("x_tlabels", [])
     prop.setdefault("x_labels", "")
     prop.setdefault("x_fmt", "%.2f")
 
     prop.setdefault("y0_ticks", [])
     prop.setdefault("y0_tlabels", [])
-    prop.setdefault("y0_labels", "y")
+    prop.setdefault("y0_labels", "y-%d")
     
     prop.setdefault("y_ticks", [])
     prop.setdefault("y_tlabels", [])
     prop.setdefault("y_labels", "")
     prop.setdefault("y_fmt", "%.2f")
 
     return prop
@@ -350,47 +352,61 @@
 
 
 def DrawMaps(xlist, ylist, data, prop = {}):
     x = len(xlist)
     y = len(ylist)
     prop = Initprop_forDrawMaps(prop, data)
 
-    fig = plt.figure(figsize=(prop["xl"]*x, prop["yl"]*y))
+    fig = plt.figure(figsize=(prop["yl"]*y, prop["xl"]*x))
     fig.subplots_adjust(hspace=prop["space"][0], wspace=prop["space"][1])
-    width_ratios = [1] * x
+    width_ratios = [1] * y
     width_ratios.append(prop["cbar_weight"])
     gs = gridspec.GridSpec(x, y+1, width_ratios=width_ratios)
     for xv, xi in enumerate(xlist):
         for yv, yi in enumerate(ylist):
             ax = plt.subplot(gs[xi,yi])
             tmpdata = data[(xi,yi)]
 
-            im = ax.imshow(tmpdata, cmap=prop["cbar_str"], origin='lower', vmin=prop["vmin"], vmax=prop["vmax"])
+            im = ax.imshow(tmpdata, cmap=prop["cbar_str"], origin='lower', vmin=prop["vmin"], vmax=prop["vmax"], aspect=prop["aspect"])
 
             if xi == x-1:
                 ax.set_xticks(prop["x0_ticks"])
                 ax.set_xticklabels([prop["x_fmt"]%i for i in prop["x0_tlabels"]])
-                ax.set_xlabel(prop["x0_labels"])
+                if "%" in prop["x0_labels"]:
+                    ax.set_xlabel(prop["x0_labels"]%xv)
+                else:
+                    ax.set_ylabel(prop["x0_labels"])
             else:
                 ax.set_xticks(prop["x_ticks"])
                 ax.set_xticklabels([prop["x_fmt"]%i for i in prop["x_tlabels"]])
-                ax.set_xlabel(prop["x_labels"])
+                if "%" in prop["x_labels"]:
+                    ax.set_xlabel(prop["x_labels"]%xv)
+                else:
+                    ax.set_ylabel(prop["x_labels"])
 
             if yi == 0:
                 ax.set_yticks(prop["y0_ticks"])
                 ax.set_yticklabels([prop["y_fmt"]%i for i in prop["y0_tlabels"]])
-                ax.set_ylabel(prop["y0_labels"])
+                if "%" in prop["y0_labels"]:
+                    ax.set_ylabel(prop["y0_labels"]%yv)
+                else:
+                    ax.set_ylabel(prop["y0_labels"])
             else:
                 ax.set_yticks(prop["y_ticks"])
                 ax.set_yticklabels([prop["y_fmt"]%i for i in prop["y_tlabels"]])
-                ax.set_ylabel(prop["y_labels"])
+                if "%" in prop["y_labels"]:
+                    ax.set_ylabel(prop["y_labels"]%yv)
+                else:
+                    ax.set_ylabel(prop["y_labels"])
 
     fig.align_ylabels()
     ax = plt.subplot(gs[:,-1])
     cbar = fig.colorbar(im, cax=ax)
+    cbar.set_ticks(np.linspace(prop["vmin"], prop["vmax"], prop["vs"]))
+    cbar.set_ticklabels([prop["v_fmt"]%i for i in np.linspace(prop["vmin"], prop["vmax"], prop["vs"])])
     cbar.set_label(prop["c_labels"])
 
 
 
 # 自定义色卡区
 CSL_4_1 = ["#384259","#f73859","#7ac7c4","#f07b3f"]
 CSL_4_2 = ["#2a557f","#44bd9d","#f04f75","#fdcd6e"]
```

## Comparing `drawwithplt-0.3.dist-info/METADATA` & `drawwithplt-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawwithplt
-Version: 0.3
+Version: 0.3.1
 Summary: More EASY to Draw SCI figure with PIL
 Home-page: https://github.com/liftes/PythonDraw
 Author: liftes
 Author-email: 21121598@bjtu.edu.cn
 Maintainer: liftes
 Maintainer-email: 21121598@bjtu.edu.cn
 License: BSD License
```

