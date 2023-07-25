# Comparing `tmp/OCR_with_format-0.5.tar.gz` & `tmp/OCR_with_format-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCR_with_format-0.5.tar", last modified: Tue Jul 25 15:48:50 2023, max compression
+gzip compressed data, was "OCR_with_format-0.6.tar", last modified: Tue Jul 25 15:50:45 2023, max compression
```

## Comparing `OCR_with_format-0.5.tar` & `OCR_with_format-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:48:50.680458 OCR_with_format-0.5/
--rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.5/LICENSE
--rw-rw-r--   0 g         (1000) g         (1000)    46026 2023-07-25 15:48:50.680458 OCR_with_format-0.5/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     4906 2023-07-25 15:47:26.000000 OCR_with_format-0.5/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:48:34.000000 OCR_with_format-0.5/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:48:50.680458 OCR_with_format-0.5/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:48:50.680458 OCR_with_format-0.5/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:48:50.680458 OCR_with_format-0.5/src/OCR_with_format/
--rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:48:26.000000 OCR_with_format-0.5/src/OCR_with_format/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.5/src/OCR_with_format/__main__.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:48:50.680458 OCR_with_format-0.5/src/OCR_with_format.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)    46026 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:48:50.000000 OCR_with_format-0.5/src/OCR_with_format.egg-info/top_level.txt
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:50:45.758149 OCR_with_format-0.6/
+-rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.6/LICENSE
+-rw-rw-r--   0 g         (1000) g         (1000)    46016 2023-07-25 15:50:45.758149 OCR_with_format-0.6/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     4896 2023-07-25 15:50:13.000000 OCR_with_format-0.6/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:50:20.000000 OCR_with_format-0.6/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:50:45.758149 OCR_with_format-0.6/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:50:45.754149 OCR_with_format-0.6/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:50:45.754149 OCR_with_format-0.6/src/OCR_with_format/
+-rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:50:27.000000 OCR_with_format-0.6/src/OCR_with_format/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.6/src/OCR_with_format/__main__.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:50:45.758149 OCR_with_format-0.6/src/OCR_with_format.egg-info/
+-rw-rw-r--   0 g         (1000) g         (1000)    46016 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:50:45.000000 OCR_with_format-0.6/src/OCR_with_format.egg-info/top_level.txt
```

### Comparing `OCR_with_format-0.5/LICENSE` & `OCR_with_format-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OCR_with_format-0.5/PKG-INFO` & `OCR_with_format-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR_with_format
-Version: 0.5
+Version: 0.6
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -736,15 +736,15 @@
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
-* output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
+* output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
 ¥ Branches  © Tags                                                                     postprocess in a way that preserves
@@ -761,15 +761,15 @@
                                                                                           Packages
                                                                                           No packages published
                                                                                           Publish your first package
                                                                                           Languages
                                                                                           ———
                                                                                            ® Python 100.0%
 ```
-* output from `python ./__init__.py ./screenshot.png --quiet --comparison_run`
+* output from `OCR_with_format ./screenshot.png --quiet --comparison_run`
   *
 ```
 OCR_with_format
 
 [ pin | [ @unwateh (@) ~ | [ & Fork (O)
 
 -] [ ¢ s (0
```

### Comparing `OCR_with_format-0.5/README.md` & `OCR_with_format-0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
-* output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
+* output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
 ¥ Branches  © Tags                                                                     postprocess in a way that preserves
@@ -72,15 +72,15 @@
                                                                                           Packages
                                                                                           No packages published
                                                                                           Publish your first package
                                                                                           Languages
                                                                                           ———
                                                                                            ® Python 100.0%
 ```
-* output from `python ./__init__.py ./screenshot.png --quiet --comparison_run`
+* output from `OCR_with_format ./screenshot.png --quiet --comparison_run`
   *
 ```
 OCR_with_format
 
 [ pin | [ @unwateh (@) ~ | [ & Fork (O)
 
 -] [ ¢ s (0
```

### Comparing `OCR_with_format-0.5/pyproject.toml` & `OCR_with_format-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OCR_with_format"
-version = "0.5"
+version = "0.6"
 description = "Wrapper to pytesseract to preserve space and formatting"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `OCR_with_format-0.5/src/OCR_with_format/__init__.py` & `OCR_with_format-0.6/src/OCR_with_format/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textwrap import dedent
 
 # pre compiled regex
 bbox_regex = re.compile(r'bbox\s(\d+)\s(\d+)\s(\d+)\s(\d+)')
 confidence_regex = re.compile(r'x_wconf\s(\d+)')
 newlines_regex = re.compile(r'\n\s*\n')
 
-__version__ = "0.5"
+__version__ = "0.6"
 
 # msic
 
 def _get_wdim(ocrx_word):
     "parse the dimansion of the word from the ocrx object"
     return [int(x) for x in re.findall(bbox_regex, ocrx_word["title"])[0]]
```

### Comparing `OCR_with_format-0.5/src/OCR_with_format.egg-info/PKG-INFO` & `OCR_with_format-0.6/src/OCR_with_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR-with-format
-Version: 0.5
+Version: 0.6
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -736,15 +736,15 @@
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
-* output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
+* output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
 ¥ Branches  © Tags                                                                     postprocess in a way that preserves
@@ -761,15 +761,15 @@
                                                                                           Packages
                                                                                           No packages published
                                                                                           Publish your first package
                                                                                           Languages
                                                                                           ———
                                                                                            ® Python 100.0%
 ```
-* output from `python ./__init__.py ./screenshot.png --quiet --comparison_run`
+* output from `OCR_with_format ./screenshot.png --quiet --comparison_run`
   *
 ```
 OCR_with_format
 
 [ pin | [ @unwateh (@) ~ | [ & Fork (O)
 
 -] [ ¢ s (0
```

