# Comparing `tmp/pixel-font-builder-0.0.5.tar.gz` & `tmp/pixel-font-builder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.5.tar", last modified: Tue Jul 25 08:52:50 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.6.tar", last modified: Tue Jul 25 14:21:46 2023, max compression
```

## Comparing `pixel-font-builder-0.0.5.tar` & `pixel-font-builder-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 08:52:50.000000 pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:52:50.455217 pixel-font-builder-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 08:52:39.000000 pixel-font-builder-0.0.5/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.770327 pixel-font-builder-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.774327 pixel-font-builder-0.0.6/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.774327 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.5/LICENSE` & `pixel-font-builder-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/PKG-INFO` & `pixel-font-builder-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

### Comparing `pixel-font-builder-0.0.5/README.md` & `pixel-font-builder-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/pyproject.toml` & `pixel-font-builder-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.5"
+version = "0.0.6"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.6/src/pixel_font_builder/bdf.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.6/src/pixel_font_builder/font.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.6/src/pixel_font_builder/glyph.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.6/src/pixel_font_builder/info.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.6/src/pixel_font_builder/opentype.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 _CACHE_NAME_TTF_GLYPH = '_opentype_cache_ttf_glyph'
 
 
 class Configs:
     def __init__(
             self,
             px_to_units: int = 100,
+            cff_family_name: str = None,
     ):
         self.px_to_units = px_to_units
+        self.cff_family_name = cff_family_name
 
 
 class Flavor(StrEnum):
     WOFF = 'woff'
     WOFF2 = 'woff2'
 
 
@@ -63,15 +65,15 @@
     variationsPostScriptNamePrefix (nameID 25)
     """
     unique_name = meta_infos.family_name.replace(' ', '-')
     name_strings = {
         'familyName': meta_infos.family_name,
         'styleName': meta_infos.style_name,
         'uniqueFontIdentifier': f'{unique_name}-{meta_infos.style_name};{meta_infos.version}',
-        'fullName': meta_infos.family_name,
+        'fullName': f'{meta_infos.family_name} {meta_infos.style_name}',
         'version': meta_infos.version,
         'psName': f'{unique_name}-{meta_infos.style_name}',
     }
     if meta_infos.copyright_info is not None:
         name_strings['copyright'] = meta_infos.copyright_info
     if meta_infos.manufacturer is not None:
         name_strings['manufacturer'] = meta_infos.manufacturer
@@ -232,17 +234,15 @@
             glyph_order.append(glyph_name)
     builder.setupGlyphOrder(glyph_order)
     logger.debug("Setup 'Character Mapping'")
     builder.setupCharacterMap(context.character_mapping)
 
     logger.debug("Setup 'Glyphs'")
     glyphs = {}
-    for glyph_name in glyph_order:
-        glyph_context = context.get_glyph(glyph_name)
-
+    for glyph_context in context.get_glyphs():
         cache_tag = f'{glyph_context.advance_width}#{glyph_context.offset}#{glyph_context.data}'.replace(' ', '')
         if getattr(glyph_context, _CACHE_NAME_TAG, None) != cache_tag:
             setattr(glyph_context, _CACHE_NAME_OUTLINES, None)
             setattr(glyph_context, _CACHE_NAME_OTF_GLYPH, None)
             setattr(glyph_context, _CACHE_NAME_TTF_GLYPH, None)
             setattr(glyph_context, _CACHE_NAME_TAG, cache_tag)
 
@@ -258,19 +258,31 @@
         glyph = getattr(glyph_context, cache_name_xtf_glyph, None)
         if glyph is None:
             logger.debug("Create '%sGlyph': %s", xtf_name, glyph_context.name)
             glyph = _create_glyph(outlines, glyph_context, context.opentype_configs.px_to_units, is_ttf)
             setattr(glyph_context, cache_name_xtf_glyph, glyph)
         else:
             logger.debug("Use cached '%sGlyph': %s", xtf_name, glyph_context.name)
-        glyphs[glyph_name] = glyph
+        glyphs[glyph_context.name] = glyph
     if is_ttf:
         builder.setupGlyf(glyphs)
     else:
-        builder.setupCFF(name_strings['psName'], {'FullName': name_strings['fullName']}, glyphs, {})
+        if context.opentype_configs.cff_family_name is not None:
+            cff_family_name = context.opentype_configs.cff_family_name
+        else:
+            cff_family_name = context.meta_infos.family_name
+        cff_ps_name = f'{cff_family_name.replace(" ", "-")}-{context.meta_infos.style_name}'
+        cff_font_infos = {
+            'FamilyName': cff_family_name,
+            'FullName': f'{cff_family_name} {context.meta_infos.style_name}',
+            'Weight': context.meta_infos.style_name,
+        }
+        if context.meta_infos.copyright_info is not None:
+            cff_font_infos['Notice'] = context.meta_infos.copyright_info
+        builder.setupCFF(cff_ps_name, cff_font_infos, glyphs, {})
 
     logger.debug("Setup 'Horizontal Metrics'")
     horizontal_metrics = {}
     for glyph_name in glyph_order:
         advance_width = context.get_glyph(glyph_name).advance_width * context.opentype_configs.px_to_units
         if is_ttf:
             lsb = glyphs[glyph_name].xMin
```

### Comparing `pixel-font-builder-0.0.5/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

