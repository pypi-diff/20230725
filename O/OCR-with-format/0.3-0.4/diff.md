# Comparing `tmp/OCR_with_format-0.3.tar.gz` & `tmp/OCR_with_format-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCR_with_format-0.3.tar", last modified: Tue Jul 25 15:40:37 2023, max compression
+gzip compressed data, was "OCR_with_format-0.4.tar", last modified: Tue Jul 25 15:44:45 2023, max compression
```

## Comparing `OCR_with_format-0.3.tar` & `OCR_with_format-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.197165 OCR_with_format-0.3/
--rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.3/LICENSE
--rw-rw-r--   0 g         (1000) g         (1000)    44734 2023-07-25 15:40:37.197165 OCR_with_format-0.3/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     3614 2023-07-25 15:38:31.000000 OCR_with_format-0.3/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:39:49.000000 OCR_with_format-0.3/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:40:37.197165 OCR_with_format-0.3/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.193165 OCR_with_format-0.3/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.193165 OCR_with_format-0.3/src/OCR_with_format/
--rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:40:00.000000 OCR_with_format-0.3/src/OCR_with_format/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.3/src/OCR_with_format/__main__.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.197165 OCR_with_format-0.3/src/OCR_with_format.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)    44734 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/top_level.txt
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:44:45.660848 OCR_with_format-0.4/
+-rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.4/LICENSE
+-rw-rw-r--   0 g         (1000) g         (1000)    44770 2023-07-25 15:44:45.660848 OCR_with_format-0.4/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     3650 2023-07-25 15:43:54.000000 OCR_with_format-0.4/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:44:19.000000 OCR_with_format-0.4/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:44:45.660848 OCR_with_format-0.4/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:44:45.656848 OCR_with_format-0.4/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:44:45.660848 OCR_with_format-0.4/src/OCR_with_format/
+-rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:44:26.000000 OCR_with_format-0.4/src/OCR_with_format/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.4/src/OCR_with_format/__main__.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:44:45.660848 OCR_with_format-0.4/src/OCR_with_format.egg-info/
+-rw-rw-r--   0 g         (1000) g         (1000)    44770 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:44:45.000000 OCR_with_format-0.4/src/OCR_with_format.egg-info/top_level.txt
```

### Comparing `OCR_with_format-0.3/LICENSE` & `OCR_with_format-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `OCR_with_format-0.3/PKG-INFO` & `OCR_with_format-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR_with_format
-Version: 0.3
+Version: 0.4
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,15 +688,15 @@
 License-File: LICENSE
 
 # OCR_with_format
 * simple wrapper that postprocesses pytesseract's hOCR output to maintain format and spacings.
 
 ## How to
 * install `python -m pip install OCR_with_format`
-* see usage `python -m OCR_with_format --help`
+* see usage `OCR_with_format --help` (executing with `python -m` is not supported)
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
```

### Comparing `OCR_with_format-0.3/README.md` & `OCR_with_format-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OCR_with_format
 * simple wrapper that postprocesses pytesseract's hOCR output to maintain format and spacings.
 
 ## How to
 * install `python -m pip install OCR_with_format`
-* see usage `python -m OCR_with_format --help`
+* see usage `OCR_with_format --help` (executing with `python -m` is not supported)
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
```

### Comparing `OCR_with_format-0.3/pyproject.toml` & `OCR_with_format-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OCR_with_format"
-version = "0.3"
+version = "0.4"
 description = "Wrapper to pytesseract to preserve space and formatting"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `OCR_with_format-0.3/src/OCR_with_format/__init__.py` & `OCR_with_format-0.4/src/OCR_with_format/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textwrap import dedent
 
 # pre compiled regex
 bbox_regex = re.compile(r'bbox\s(\d+)\s(\d+)\s(\d+)\s(\d+)')
 confidence_regex = re.compile(r'x_wconf\s(\d+)')
 newlines_regex = re.compile(r'\n\s*\n')
 
-__version__ = "0.3"
+__version__ = "0.4"
 
 # msic
 
 def _get_wdim(ocrx_word):
     "parse the dimansion of the word from the ocrx object"
     return [int(x) for x in re.findall(bbox_regex, ocrx_word["title"])[0]]
```

### Comparing `OCR_with_format-0.3/src/OCR_with_format.egg-info/PKG-INFO` & `OCR_with_format-0.4/src/OCR_with_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR-with-format
-Version: 0.3
+Version: 0.4
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,15 +688,15 @@
 License-File: LICENSE
 
 # OCR_with_format
 * simple wrapper that postprocesses pytesseract's hOCR output to maintain format and spacings.
 
 ## How to
 * install `python -m pip install OCR_with_format`
-* see usage `python -m OCR_with_format --help`
+* see usage `OCR_with_format --help` (executing with `python -m` is not supported)
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
```

