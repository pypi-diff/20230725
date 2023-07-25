# Comparing `tmp/excolor-0.0.1.tar.gz` & `tmp/excolor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excolor-0.0.1.tar", last modified: Tue Jul 18 09:18:37 2023, max compression
+gzip compressed data, was "excolor-0.0.2.tar", last modified: Tue Jul 25 13:41:40 2023, max compression
```

## Comparing `excolor-0.0.1.tar` & `excolor-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-18 09:18:37.440655 excolor-0.0.1/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.1/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     2522 2023-07-18 09:18:37.440473 excolor-0.0.1/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     2088 2023-07-18 09:14:21.000000 excolor-0.0.1/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-18 09:18:37.439225 excolor-0.0.1/excolor/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      339 2023-07-18 06:19:31.000000 excolor-0.0.1/excolor/__init__.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     3498 2023-07-17 15:09:32.000000 excolor-0.0.1/excolor/background.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)    18367 2023-07-18 06:19:29.000000 excolor-0.0.1/excolor/excolor.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4749 2023-07-18 06:55:38.000000 excolor-0.0.1/excolor/imagetools.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     3521 2023-07-17 12:04:43.000000 excolor-0.0.1/excolor/utils.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-18 09:18:37.440243 excolor-0.0.1/excolor.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     2522 2023-07-18 09:18:37.000000 excolor-0.0.1/excolor.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      280 2023-07-18 09:18:37.000000 excolor-0.0.1/excolor.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-18 09:18:37.000000 excolor-0.0.1/excolor.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       34 2023-07-18 09:18:37.000000 excolor-0.0.1/excolor.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-07-18 09:18:37.000000 excolor-0.0.1/excolor.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-18 09:18:37.440707 excolor-0.0.1/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      850 2023-07-18 06:27:48.000000 excolor-0.0.1/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.920121 excolor-0.0.2/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.2/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3068 2023-07-25 13:41:40.919948 excolor-0.0.2/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     2633 2023-07-18 11:05:42.000000 excolor-0.0.2/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.918769 excolor-0.0.2/excolor/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      350 2023-07-25 04:09:40.000000 excolor-0.0.2/excolor/__init__.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    11406 2023-07-25 13:28:40.000000 excolor-0.0.2/excolor/background.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    12593 2023-07-24 17:19:21.000000 excolor-0.0.2/excolor/excolor.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     2663 2023-07-25 12:27:34.000000 excolor-0.0.2/excolor/geometry.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     9085 2023-07-25 13:39:43.000000 excolor-0.0.2/excolor/imagetools.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     9461 2023-07-25 04:17:01.000000 excolor-0.0.2/excolor/utils.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.919723 excolor-0.0.2/excolor.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3068 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      300 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       61 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-25 13:41:40.920172 excolor-0.0.2/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      899 2023-07-25 13:20:04.000000 excolor-0.0.2/setup.py
```

### Comparing `excolor-0.0.1/LICENSE` & `excolor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `excolor-0.0.1/PKG-INFO` & `excolor-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-Metadata-Version: 2.1
-Name: excolor
-Version: 0.0.1
-Summary: Extended colors for python
-Home-page: https://github.com/timpyrkov/excolor
-Author: Tim Pyrkov
-Author-email: tim.pyrkov@gmail.com
-License: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Artistic Software
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![Python Versions](https://img.shields.io/pypi/pyversions/excolor?style=plastic)](https://pypi.org/project/excolor/)
+[![PyPI](https://img.shields.io/pypi/v/excolor?style=plastic)](https://pypi.org/project/excolor/)
+[![License](https://img.shields.io/pypi/l/excolor?style=plastic)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/excolor/badge/?version=latest)](https://excolor.readthedocs.io/en/latest/?badge=latest)
 
 # excolors
 
 ## Extexnded color utilities for python
 #
 
 # Installation
@@ -23,42 +13,44 @@
 pip install excolor
 ```
 
 
 # Extra colormaps
 
 ```
+import excolor
+
 cmap = plt.get_cmap("gruvbox")
 cmap
 ```
 
 ![](img/colormap.png)
 
 # Colorize black-and-white image
 
 - Hue and saturation cannot colorize black-and-white image. They only change pixels where levels of red, gree, blue are not the same. 
 
-- Colorize() function takes a greyscale or b&w image and adds colors to darg and light areas.
+- Colorize() function takes a greyscale or b&w image and adds colors to dark and light areas.
 
 
 ```
 fname = "pacman.png"
 
 img = excolor.load_image(fname)
 
 plt.figure(figsize=(2,2), facecolor="#00000000")
 plt.imshow(img)
-plt.gca().set_axis_off()
+plt.axis("off")
 plt.show()
 
 img = excolor.colorize(fname, "yellow", "green")
 
 plt.figure(figsize=(2,2), facecolor="#00000000")
 plt.imshow(img)
-plt.gca().set_axis_off()
+plt.axis("off")
 plt.show()
 
 ```
 
 ![](img/pacman.png)
 ![](img/arrow.png)
 ![](img/colorized.png)
@@ -119,7 +111,10 @@
 plt.imshow( np.abs(x), cmap=cmap)
 plt.axis("off")
 plt.show()
 ```
 
 ![](img/caustics.png)
 
+# Documentation
+
+[https://excolor.readthedocs.io](https://excolor.readthedocs.io)
```

### Comparing `excolor-0.0.1/excolor/excolor.py` & `excolor-0.0.2/excolor/excolor.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,61 +4,23 @@
 import numpy as np
 import pylab as plt
 from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 import seaborn as sns
 from matplotlib.patches import Rectangle
 import matplotlib.colors as mc
 from cycler import cycler
-from excolor.utils import _is_arraylike, _is_int, _is_exp, _is_log
-from excolor.utils import _is_qualitative, _is_cyclic, _is_divergent
+from excolor.utils import _is_arraylike, _is_int, _is_exp, _is_log, _is_cmap
+from excolor.utils import _is_qualitative, _is_cyclic, _is_divergent, _get_bgcolor_dict
+from excolor.utils import *
+
 
 import warnings
 warnings.filterwarnings("ignore")
 
 
-def get_colors(cmap, n=None, exclude_extreme=True, mode="hex"):
-    """
-    Gets colors from cmap
-
-    Parameters
-    ----------
-    cmap : str or matplotlib.colors.Colormap object
-        Colormap
-    n : int, optional
-        Number of colors
-    exclude_extreme : bool, default True
-        Whethr to exclude extreme (very dark/light) colors
-    mode : {"hex", "rgb", "rgba", "hsv"}, default "hex"
-        Format of colors
-
-    Returns
-    -------
-    colors : list
-        List of colors
-
-    """
-    assert mode in ["hex", "rgb", "rgba", "hsv"]
-    cmap = plt.get_cmap(cmap)
-    if _is_qualitative(cmap):
-        colors = cmap.colors
-    else:
-        n = 10 - _is_divergent(cmap) if n is None else n
-        dn = 1 if exclude_extreme else 0
-        idx = np.arange(dn, n + dn) / (n + 2 * dn - 1)
-        colors = cmap(idx)
-    colors = [mc.to_hex(c, keep_alpha=False).upper() for c in colors]
-    if mode == "rgb":
-        colors = [mc.to_rgb(c) for c in colors]
-    elif mode == "rgba":
-        colors = [mc.to_rgba(c) for c in colors]
-    elif mode == "hsv":
-        colors = [mc.rgb_to_hsv(mc.to_rgb(c)) for c in colors]
-    return colors
-
-
 def logscale_cmap(cmap, norders=3):
     """
     Extends list of colors by adding colors inbetween
 
     Parameters
     ----------
     cmap : str or matplotlib.colors.Colormap object
@@ -142,18 +104,16 @@
         List of color names
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, exclude_extreme=False)
         title = c.name
-        is_cmap = True
     except:
         colors = c if _is_arraylike(c) else [c]
-        is_cmap = False
     d = 0.05
     width = 1  -2 * d
     n, m = aspect_ratio(len(colors), lmin=12)
     plt.figure(figsize=(2*n+4,2*m), facecolor="#00000000")
     plt.title(title, fontsize=20, color="grey")
     for k, color in enumerate(colors):
         i = k % n
@@ -211,25 +171,23 @@
     cmod : list or matplotlib.colors.Colormap object
         List of modified colors or colormap
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, 256, exclude_extreme=False)
-        is_cmap = True
     except:
         colors = c if _is_arraylike(c) else [c]
-        is_cmap = False
     hsv = np.array([mc.rgb_to_hsv(mc.to_rgb(color)) for color in colors]).T
     hsv[2] = hsv[2] + scale * (1 - hsv[2])
     cmod = [mc.to_hex(mc.hsv_to_rgb(color)).upper() for color in hsv.T]
-    if is_cmap:
+    if _is_cmap(c):
         name = c.name + "_light"
         cmod = LinearSegmentedColormap.from_list(name, cmod)
-    elif len(cmod) < 2:
+    elif len(cmod) == 1:
         cmod = cmod[0]
     return cmod
 
 
 def darken(c, scale=0.5):
     """
     Darkens colors or colormap
@@ -246,25 +204,23 @@
     cmod : list or matplotlib.colors.Colormap object
         List of modified colors or colormap
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, 256, exclude_extreme=False)
-        is_cmap = True
     except:
         colors = c if _is_arraylike(c) else [c]
-        is_cmap = False
     hsv = np.array([mc.rgb_to_hsv(mc.to_rgb(color)) for color in colors]).T
     hsv[2] = (1 - scale) * hsv[2]
     cmod = [mc.to_hex(mc.hsv_to_rgb(color)).upper() for color in hsv.T]
-    if is_cmap:
+    if _is_cmap(c):
         name = c.name + "_dark"
         cmod = LinearSegmentedColormap.from_list(name, cmod)
-    elif len(cmod) < 2:
+    elif len(cmod) == 1:
         cmod = cmod[0]
     return cmod
 
 
 def saturate(c, scale=0.5):
     """
     Saturates colors or colormap
@@ -281,25 +237,23 @@
     cmod : list or matplotlib.colors.Colormap object
         List of modified colors or colormap
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, 256, exclude_extreme=False)
-        is_cmap = True
     except:
         colors = c if _is_arraylike(c) else [c]
-        is_cmap = False
     hsv = np.array([mc.rgb_to_hsv(mc.to_rgb(color)) for color in colors]).T
     hsv[1] = hsv[1] + scale * (1 - hsv[1])
     cmod = [mc.to_hex(mc.hsv_to_rgb(color)).upper() for color in hsv.T]
-    if is_cmap:
+    if _is_cmap(c):
         name = c.name + "_saturated"
         cmod = LinearSegmentedColormap.from_list(name, cmod)
-    elif len(cmod) < 2:
+    elif len(cmod) == 1:
         cmod = cmod[0]
     return cmod
 
 
 def desaturate(c, scale=0.5):
     """
     Desaturates colors or colormap
@@ -316,25 +270,23 @@
     cmod : list or matplotlib.colors.Colormap object
         List of modified colors or colormap
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, 256, exclude_extreme=False)
-        is_cmap = True
     except:
         colors = c if _is_arraylike(c) else [c]
-        is_cmap = False
     hsv = np.array([mc.rgb_to_hsv(mc.to_rgb(color)) for color in colors]).T
     hsv[1] = (1 - scale) * hsv[1]
     cmod = [mc.to_hex(mc.hsv_to_rgb(color)).upper() for color in hsv.T]
-    if is_cmap:
+    if _is_cmap(c):
         name = c.name + "_desaturated"
         cmod = LinearSegmentedColormap.from_list(name, cmod)
-    elif len(cmod) < 2:
+    elif len(cmod) == 1:
         cmod = cmod[0]
     return cmod
 
 
 def color_to_hex(c, keep_alpha=False):
     """
     Converts color(s) to hex names
@@ -380,25 +332,14 @@
         except:
             try:
                 # rgb-int to hex then to rgb
                 hcolor = "#" + "".join(["{:02X}".format(c_) for c_ in c])
                 rgb = mc.to_rgb(hcolor)
             except:
                 rgb = None
-    # if _is_arraylike(c) and len(c) >=3 and len(c) <= 4:
-    #     rgb = np.array([c_ for c_ in c])
-    #     if rgb.min() >= 0 and rgb.max() > 1 and rgb.max() <= 255:
-    #         # rgb-int to hex then to rgb
-    #         hcolor = "#" + "".join(["{:02X}".format(c_) for c_ in c])
-    #         rgb = mc.to_rgb(hcolor)
-    #     else:
-    #         rgb = mc.to_rgb(c)
-    # else:
-    #     # default matplotlib func
-    #     rgb = mc.to_rgb(c)
     return rgb
 
 
 def extend_colors(c, n=5):
     """
     Extends list of colors by adding colors inbetween
 
@@ -525,109 +466,18 @@
         if length <= lmin or n > length:
             n = length
     else:
         n, m = 0, 0
     return n, m
 
 
-def _register_cmap(cmap):
-    try:
-        plt.colormaps.register(cmap)
-    except:
-        pass
-
-def _add_cool_warm_colormaps():
-    """
-    Extends list of registered colormaps by modifications of 'coolwarm'
-
-    """
-    # Divergent to sequential
-    gradient = np.linspace(0.5, 1, 128)
-    dct = {"cool": "cold", "warm": "warm"}
-    warm_colors = plt.get_cmap("coolwarm")(gradient)
-    cool_colors = plt.get_cmap("coolwarm_r")(gradient)
-    cmap = LinearSegmentedColormap.from_list("warm", warm_colors)
-    _register_cmap(cmap)
-    cmap = LinearSegmentedColormap.from_list("warm_r", warm_colors[::-1])
-    _register_cmap(cmap)
-    cmap = LinearSegmentedColormap.from_list("cold", cool_colors)
-    _register_cmap(cmap)
-    cmap = LinearSegmentedColormap.from_list("cold_r", cool_colors[::-1])
-    _register_cmap(cmap)
-    # Log-scaled
-    gradient = np.logspace(0, -10, 128)
-    logwarm_colors = plt.get_cmap("warm")(gradient)
-    logwarm_r_colors = plt.get_cmap("warm_r")(gradient)
-    cmap = LinearSegmentedColormap.from_list("logwarm", logwarm_colors)
-    _register_cmap(cmap)
-    cmap = LinearSegmentedColormap.from_list("logwarm_r", logwarm_r_colors)
-    _register_cmap(cmap)
-    logcool_colors = plt.get_cmap("cold")(gradient)
-    logcool_r_colors = plt.get_cmap("cold_r")(gradient)
-    cmap = LinearSegmentedColormap.from_list("logcool", logcool_colors)
-    _register_cmap(cmap)
-    cmap = LinearSegmentedColormap.from_list("logcool_r", logcool_r_colors)
-    _register_cmap(cmap)
-    return
-
-
-def _add_extended_colormaps():
-    """
-    Extends list of registered colormaps by modifications of 'coolwarm'
-    and manually hardcoded colormaps
-
-    """
-    try:
-        add_cool_warm_colormaps()
-    except:
-        pass
-    aquamarine = grey_to_aquamarine()
-    aquamarine_light = lighten(aquamarine, 0.8)
-    aquamarine_dark = darken(aquamarine, 0.4)
-    color_dict = {
-        "BrBu": ["#9B2227", "#BA3F04", "#CA6705", "#EE9B04", "#EAD7A4", "#93D3BD", "#4BB3A9", "#039396", "#027984", "#015F72"],
-        "BrGn": ["#9B2227", "#BA3F04", "#CA6705", "#EE9B04", "#EAD7A4", "#CAB67B", "#A99945", "#897C0F", "#736E12", "#5E6014"],
-        "OrBu": ["#B97401", "#DC8D01", "#FAC316", "#F8E584", "#F8FFC9", "#638094", "#4C6E83", "#3E596D", "#374053"],
-        "OrGn": ["#B97401", "#DC8D01", "#FAC316", "#F8E584", "#F1FFC1", "#7DA4A4", "#628E8E", "#467171", "#284C4C"],
-        "PiBu": ["#7D433D", "#A45040", "#C45D47", "#DD6850", "#CAA59F", "#4C8A9A", "#427283", "#385B6C", "#2E4355"],
-        "gruvbox_light": ["#FB4934", "#FE8019", "#FABD2F", "#B8BB26", "#8EC07C", "#83A598", "#D3869B"],
-        "gruvbox": ["#CC241D", "#D65D0E", "#D79921", "#98971A", "#689D6A", "#458588", "#B16286"],
-        "gruvbox_dark": ["#9D0006", "#AF3A03", "#B57614", "#79740E", "#427B58", "#076678", "#8F3F71"],
-        "artdeco": ["#9F1B10", "#D88533", "#E8B055", "#D9B97B", "#B6BEAA", "#768C86", "#365861", "#204755", "#0A3649"],
-        "cyberpunk": ["#55D6F5", "#5C9BE8", "#6260DC", "#522FAA", "#42007A", "#4F057A", "#5D097C", "#A917BE", "#F225FF"],
-        "synthwave": ["#5C9BE8", "#5368C4", "#4B35A0", "#42007A", "#550584", "#680B8E", "#7B1098", "#A75466", "#D19536", "#FBD606"],
-        "aquamarine_light": ["#7E3FE8", "#439BDF", "#00E8BE"],
-        "aquamarine": ["#7239D2", "#3985BF", "#00D2AC"],
-        "aquamarine_dark": ["#391C69", "#1C4360", "#006956"],
-        # "aquamarine_light": aquamarine_light,
-        # "aquamarine": aquamarine,
-        # "aquamarine_dark": aquamarine_dark,
-    }
-    for name, colors in color_dict.items():
-        try:
-            colors_ = colors[::-1]
-            name_ = name.split("_")[0] + "_r"
-            if name.find("_") > 0:
-                name_ = name_ + "_" + "_".join(name.split("_")[1:])
-            cmap = ListedColormap(colors_, name_)
-            _register_cmap(cmap)
-        except:
-            pass
-    for name, colors in color_dict.items():
-        try:
-            cmap = ListedColormap(colors, name)
-            _register_cmap(cmap)
-        except:
-            pass
-    return
-
 
 """ Aliases for functions """
-show_colormap = show_cmap
-show_colorbar = show_cbar
+# show_colormap = show_cmap
+# show_colorbar = show_cbar
 gray_to_hue = grey_to_hue
 gray_to_aquamarine = grey_to_aquamarine
 
 import types
 __all__ = [name for name, thing in globals().items()
           if not (name.startswith("_") or isinstance(thing, types.ModuleType))]
 del types
```

### Comparing `excolor-0.0.1/excolor.egg-info/PKG-INFO` & `excolor-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 Metadata-Version: 2.1
 Name: excolor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extended colors for python
 Home-page: https://github.com/timpyrkov/excolor
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Artistic Software
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Python Versions](https://img.shields.io/pypi/pyversions/excolor?style=plastic)](https://pypi.org/project/excolor/)
+[![PyPI](https://img.shields.io/pypi/v/excolor?style=plastic)](https://pypi.org/project/excolor/)
+[![License](https://img.shields.io/pypi/l/excolor?style=plastic)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/excolor/badge/?version=latest)](https://excolor.readthedocs.io/en/latest/?badge=latest)
+
 # excolors
 
 ## Extexnded color utilities for python
 #
 
 # Installation
 ```
 pip install excolor
 ```
 
 
 # Extra colormaps
 
 ```
+import excolor
+
 cmap = plt.get_cmap("gruvbox")
 cmap
 ```
 
 ![](img/colormap.png)
 
 # Colorize black-and-white image
 
 - Hue and saturation cannot colorize black-and-white image. They only change pixels where levels of red, gree, blue are not the same. 
 
-- Colorize() function takes a greyscale or b&w image and adds colors to darg and light areas.
+- Colorize() function takes a greyscale or b&w image and adds colors to dark and light areas.
 
 
 ```
 fname = "pacman.png"
 
 img = excolor.load_image(fname)
 
 plt.figure(figsize=(2,2), facecolor="#00000000")
 plt.imshow(img)
-plt.gca().set_axis_off()
+plt.axis("off")
 plt.show()
 
 img = excolor.colorize(fname, "yellow", "green")
 
 plt.figure(figsize=(2,2), facecolor="#00000000")
 plt.imshow(img)
-plt.gca().set_axis_off()
+plt.axis("off")
 plt.show()
 
 ```
 
 ![](img/pacman.png)
 ![](img/arrow.png)
 ![](img/colorized.png)
@@ -119,7 +126,10 @@
 plt.imshow( np.abs(x), cmap=cmap)
 plt.axis("off")
 plt.show()
 ```
 
 ![](img/caustics.png)
 
+# Documentation
+
+[https://excolor.readthedocs.io](https://excolor.readthedocs.io)
```

### Comparing `excolor-0.0.1/setup.py` & `excolor-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="excolor",
-    version="0.0.1",
+    version="0.0.2",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Extended colors for python",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/excolor",
@@ -22,12 +22,14 @@
         "Topic :: Artistic Software",
     ],
     python_requires=">=3.6",
     include_package_data=True,
     install_requires=[
         "numpy",
         "matplotlib",
+        "opencv-python",
+        "pythonperlin",
         "seaborn",
         "requests",
     ],
 )
```

