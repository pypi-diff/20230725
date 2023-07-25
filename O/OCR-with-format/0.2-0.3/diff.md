# Comparing `tmp/OCR_with_format-0.2.tar.gz` & `tmp/OCR_with_format-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCR_with_format-0.2.tar", last modified: Tue Jul 25 15:33:28 2023, max compression
+gzip compressed data, was "OCR_with_format-0.3.tar", last modified: Tue Jul 25 15:40:37 2023, max compression
```

## Comparing `OCR_with_format-0.2.tar` & `OCR_with_format-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:33:28.030728 OCR_with_format-0.2/
--rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.2/LICENSE
--rw-rw-r--   0 g         (1000) g         (1000)    44630 2023-07-25 15:33:28.030728 OCR_with_format-0.2/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     3510 2023-07-25 14:44:31.000000 OCR_with_format-0.2/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:32:10.000000 OCR_with_format-0.2/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:33:28.030728 OCR_with_format-0.2/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:33:28.030728 OCR_with_format-0.2/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:33:28.030728 OCR_with_format-0.2/src/OCR_with_format/
--rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:33:11.000000 OCR_with_format-0.2/src/OCR_with_format/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.2/src/OCR_with_format/__main__.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:33:28.030728 OCR_with_format-0.2/src/OCR_with_format.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)    44630 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:33:28.000000 OCR_with_format-0.2/src/OCR_with_format.egg-info/top_level.txt
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.197165 OCR_with_format-0.3/
+-rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.3/LICENSE
+-rw-rw-r--   0 g         (1000) g         (1000)    44734 2023-07-25 15:40:37.197165 OCR_with_format-0.3/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     3614 2023-07-25 15:38:31.000000 OCR_with_format-0.3/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:39:49.000000 OCR_with_format-0.3/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:40:37.197165 OCR_with_format-0.3/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.193165 OCR_with_format-0.3/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.193165 OCR_with_format-0.3/src/OCR_with_format/
+-rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:40:00.000000 OCR_with_format-0.3/src/OCR_with_format/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.3/src/OCR_with_format/__main__.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:40:37.197165 OCR_with_format-0.3/src/OCR_with_format.egg-info/
+-rw-rw-r--   0 g         (1000) g         (1000)    44734 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:40:37.000000 OCR_with_format-0.3/src/OCR_with_format.egg-info/top_level.txt
```

### Comparing `OCR_with_format-0.2/LICENSE` & `OCR_with_format-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OCR_with_format-0.2/PKG-INFO` & `OCR_with_format-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR_with_format
-Version: 0.2
+Version: 0.3
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,15 +693,15 @@
 ## How to
 * install `python -m pip install OCR_with_format`
 * see usage `python -m OCR_with_format --help`
 
 ## Example
 
 * Image:
-  * ![image](./screenshot.png)
+  * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
```

### Comparing `OCR_with_format-0.2/README.md` & `OCR_with_format-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## How to
 * install `python -m pip install OCR_with_format`
 * see usage `python -m OCR_with_format --help`
 
 ## Example
 
 * Image:
-  * ![image](./screenshot.png)
+  * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
```

### Comparing `OCR_with_format-0.2/pyproject.toml` & `OCR_with_format-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OCR_with_format"
-version = "0.2"
+version = "0.3"
 description = "Wrapper to pytesseract to preserve space and formatting"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `OCR_with_format-0.2/src/OCR_with_format/__init__.py` & `OCR_with_format-0.3/src/OCR_with_format/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textwrap import dedent
 
 # pre compiled regex
 bbox_regex = re.compile(r'bbox\s(\d+)\s(\d+)\s(\d+)\s(\d+)')
 confidence_regex = re.compile(r'x_wconf\s(\d+)')
 newlines_regex = re.compile(r'\n\s*\n')
 
-__version__ = "0.2"
+__version__ = "0.3"
 
 # msic
 
 def _get_wdim(ocrx_word):
     "parse the dimansion of the word from the ocrx object"
     return [int(x) for x in re.findall(bbox_regex, ocrx_word["title"])[0]]
```

### Comparing `OCR_with_format-0.2/src/OCR_with_format.egg-info/PKG-INFO` & `OCR_with_format-0.3/src/OCR_with_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR-with-format
-Version: 0.2
+Version: 0.3
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,15 +693,15 @@
 ## How to
 * install `python -m pip install OCR_with_format`
 * see usage `python -m OCR_with_format --help`
 
 ## Example
 
 * Image:
-  * ![image](./screenshot.png)
+  * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `python ./__init__.py ./screenshot.png --thresholding_method="all"  --quiet`
 ```
                                                                     @Unwateh (1) ~        Fork (3)                  (©
     OCR_with_format                          [     Pir ][                   | [  &            <) [     s        -]
                                                                                           About
                                                                                                                               &
                                                                                           Wrapper around pytesseract to
```

