# Comparing `tmp/pixel-font-builder-0.0.4.tar.gz` & `tmp/pixel-font-builder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.4.tar", last modified: Wed Jul 19 15:18:55 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.5.tar", last modified: Tue Jul 25 08:52:50 2023, max compression
```

## Comparing `pixel-font-builder-0.0.4.tar` & `pixel-font-builder-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.272489 pixel-font-builder-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.4/LICENSE` & `pixel-font-builder-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.4/PKG-INFO` & `pixel-font-builder-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

### Comparing `pixel-font-builder-0.0.4/README.md` & `pixel-font-builder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.4/pyproject.toml` & `pixel-font-builder-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
@@ -15,15 +15,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools>=4.41.0",
+    "fonttools>=4.41.1",
     "Brotli>=1.0.9",
     "bdffont>=0.0.13",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/pixel-font-builder"
 source = "https://github.com/TakWolf/pixel-font-builder"
```

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.5/src/pixel_font_builder/bdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     builder = BdfFont(
         point_size=context.size,
         resolution_xy=(context.bdf_configs.resolution_x, context.bdf_configs.resolution_y),
         bounding_box_size=(context.size, context.line_height),
         bounding_box_offset=(0, context.descent),
     )
 
-    logger.debug("Add 'Glyph': %s", '.notdef')
+    logger.debug("Add 'Glyph': .notdef")
     builder.add_glyph(_create_glyph(context, -1, '.notdef'))
     for code_point, glyph_name in context.character_mapping.items():
         logger.debug("Add 'Glyph': %s", glyph_name)
         builder.add_glyph(_create_glyph(context, code_point, glyph_name))
 
     logger.debug("Setup 'Properties'")
     builder.properties.foundry = context.meta_infos.manufacturer
```

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.5/src/pixel_font_builder/font.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import bdffont
 import fontTools.fontBuilder
+import fontTools.ttLib
 
 from pixel_font_builder import opentype, bdf
 from pixel_font_builder.glyph import Glyph
 from pixel_font_builder.info import MetaInfos
 
 
 class FontBuilder:
@@ -105,7 +106,34 @@
 
     def save_bdf(
             self,
             file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
             optimize_bitmap: bool = True,
     ):
         self.to_bdf_builder().save(file_path, optimize_bitmap)
+
+
+class FontCollectionBuilder:
+    def __init__(self, font_builders: list[FontBuilder] = None):
+        if font_builders is None:
+            font_builders = list[FontBuilder]()
+        self.font_builders = font_builders
+
+    def to_otc_builder(self) -> fontTools.ttLib.TTCollection:
+        return opentype.create_collection_builder(self, False)
+
+    def save_otc(
+            self,
+            file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
+            share_tables: bool = True,
+    ):
+        self.to_otc_builder().save(file_path, share_tables)
+
+    def to_ttc_builder(self) -> fontTools.ttLib.TTCollection:
+        return opentype.create_collection_builder(self, True)
+
+    def save_ttc(
+            self,
+            file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
+            share_tables: bool = True,
+    ):
+        self.to_ttc_builder().save(file_path, share_tables)
```

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.5/src/pixel_font_builder/glyph.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.5/src/pixel_font_builder/info.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.5/src/pixel_font_builder/opentype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from enum import StrEnum
 
 from fontTools.fontBuilder import FontBuilder
 from fontTools.misc.psCharStrings import T2CharString as OTFGlyph
 from fontTools.pens.t2CharStringPen import T2CharStringPen as OTFGlyphPen
 from fontTools.pens.ttGlyphPen import TTGlyphPen as TTFGlyphPen
+from fontTools.ttLib import TTCollection
 from fontTools.ttLib.tables._g_l_y_f import Glyph as TTFGlyph
 
 from pixel_font_builder import font
 from pixel_font_builder.glyph import Glyph
 from pixel_font_builder.info import MetaInfos
 
 logger = logging.getLogger('pixel_font_builder.opentype')
@@ -207,15 +208,15 @@
         pen.closePath()
     if is_ttf:
         return pen.glyph()
     else:
         return pen.getCharString()
 
 
-def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor) -> FontBuilder:
+def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor = None) -> FontBuilder:
     xtf_name = 'TTF' if is_ttf else 'OTF'
 
     logger.debug("Create '%sBuilder': %s", xtf_name, context.meta_infos.family_name)
     context.check_ready()
 
     units_per_em = context.size * context.opentype_configs.px_to_units
     builder = FontBuilder(units_per_em, isTTF=is_ttf)
@@ -302,7 +303,14 @@
 
     if flavor is not None:
         logger.debug("Setup 'Flavor': %s", flavor)
         builder.font.flavor = flavor
 
     logger.debug("Create '%sBuilder' finished", xtf_name)
     return builder
+
+
+def create_collection_builder(context: 'font.FontCollectionBuilder', is_ttf: bool) -> TTCollection:
+    collection_builder = TTCollection()
+    for font_context in context.font_builders:
+        collection_builder.fonts.append(create_builder(font_context, is_ttf).font)
+    return collection_builder
```

### Comparing `pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

