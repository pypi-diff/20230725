# Comparing `tmp/OCR_with_format-0.7.tar.gz` & `tmp/OCR_with_format-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCR_with_format-0.7.tar", last modified: Tue Jul 25 15:55:25 2023, max compression
+gzip compressed data, was "OCR_with_format-0.8.tar", last modified: Tue Jul 25 16:03:25 2023, max compression
```

## Comparing `OCR_with_format-0.7.tar` & `OCR_with_format-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:55:25.326247 OCR_with_format-0.7/
--rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.7/LICENSE
--rw-rw-r--   0 g         (1000) g         (1000)    46173 2023-07-25 15:55:25.326247 OCR_with_format-0.7/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     5053 2023-07-25 15:54:37.000000 OCR_with_format-0.7/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 15:55:04.000000 OCR_with_format-0.7/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 15:55:25.326247 OCR_with_format-0.7/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:55:25.326247 OCR_with_format-0.7/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:55:25.326247 OCR_with_format-0.7/src/OCR_with_format/
--rw-rw-r--   0 g         (1000) g         (1000)    10616 2023-07-25 15:55:01.000000 OCR_with_format-0.7/src/OCR_with_format/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.7/src/OCR_with_format/__main__.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 15:55:25.326247 OCR_with_format-0.7/src/OCR_with_format.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)    46173 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 15:55:25.000000 OCR_with_format-0.7/src/OCR_with_format.egg-info/top_level.txt
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/
+-rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.8/LICENSE
+-rw-rw-r--   0 g         (1000) g         (1000)    46195 2023-07-25 16:03:25.041263 OCR_with_format-0.8/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     5075 2023-07-25 16:02:37.000000 OCR_with_format-0.8/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 16:02:57.000000 OCR_with_format-0.8/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 16:03:25.041263 OCR_with_format-0.8/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.037263 OCR_with_format-0.8/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/src/OCR_with_format/
+-rw-rw-r--   0 g         (1000) g         (1000)    10639 2023-07-25 16:03:08.000000 OCR_with_format-0.8/src/OCR_with_format/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.8/src/OCR_with_format/__main__.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/src/OCR_with_format.egg-info/
+-rw-rw-r--   0 g         (1000) g         (1000)    46195 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/top_level.txt
```

### Comparing `OCR_with_format-0.7/LICENSE` & `OCR_with_format-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `OCR_with_format-0.7/PKG-INFO` & `OCR_with_format-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR_with_format
-Version: 0.7
+Version: 0.8
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,36 +697,37 @@
 
 ## Usage
 ```
 NAME
     OCR_with_format
 
 SYNOPSIS
-    OCR_with_format IMG_PATH THRESHOLDING_METHOD <flags>
+    OCR_with_format IMG_PATH <flags>
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
-    THRESHOLDING_METHOD
+
+FLAGS
+    --thresholding_method=THRESHOLDING_METHOD
         Type: str
+        Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
-
-FLAGS
     -l, --language=LANGUAGE
         Type: str
         Default: 'eng'
         language to look for in the image
     -o, --output_path=OUTPUT_PATH
         Type: Optional[str]
         Default: None
         if not None, will output to this path and erase its previous content.
-    -t, --tesseract_args=TESSERACT_ARGS
+    --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
     -c, --comparison_run=COMPARISON_RUN
```

### Comparing `OCR_with_format-0.7/README.md` & `OCR_with_format-0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 
 ## Usage
 ```
 NAME
     OCR_with_format
 
 SYNOPSIS
-    OCR_with_format IMG_PATH THRESHOLDING_METHOD <flags>
+    OCR_with_format IMG_PATH <flags>
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
-    THRESHOLDING_METHOD
+
+FLAGS
+    --thresholding_method=THRESHOLDING_METHOD
         Type: str
+        Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
-
-FLAGS
     -l, --language=LANGUAGE
         Type: str
         Default: 'eng'
         language to look for in the image
     -o, --output_path=OUTPUT_PATH
         Type: Optional[str]
         Default: None
         if not None, will output to this path and erase its previous content.
-    -t, --tesseract_args=TESSERACT_ARGS
+    --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
     -c, --comparison_run=COMPARISON_RUN
```

### Comparing `OCR_with_format-0.7/pyproject.toml` & `OCR_with_format-0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OCR_with_format"
-version = "0.7"
+version = "0.8"
 description = "Wrapper to pytesseract to preserve space and formatting"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `OCR_with_format-0.7/src/OCR_with_format/__init__.py` & `OCR_with_format-0.8/src/OCR_with_format/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textwrap import dedent
 
 # pre compiled regex
 bbox_regex = re.compile(r'bbox\s(\d+)\s(\d+)\s(\d+)\s(\d+)')
 confidence_regex = re.compile(r'x_wconf\s(\d+)')
 newlines_regex = re.compile(r'\n\s*\n')
 
-__version__ = "0.7"
+__version__ = "0.8"
 
 # msic
 
 def _get_wdim(ocrx_word):
     "parse the dimansion of the word from the ocrx object"
     return [int(x) for x in re.findall(bbox_regex, ocrx_word["title"])[0]]
 
@@ -35,28 +35,28 @@
             config=args,
             extension="hocr",
             )
 
 
 def OCR_with_format(
         img_path: str,
-        thresholding_method: str,
+        thresholding_method: str = "otsu",
         language: str = "eng",
         output_path: str = None,
         tesseract_args: str = "--oem 3 --psm 11 -c preserve_interword_spaces=1",
         quiet=False,
         comparison_run=False,
         ):
     """
     Parameters
     ----------
     img_path: str
         path to the image you want to do OCR on
 
-    thresholding_method: str
+    thresholding_method: str, default otsu
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be
         the one which maximizes the mean and median confidences over
         each parsed words.
 
     language: str, default eng
```

### Comparing `OCR_with_format-0.7/src/OCR_with_format.egg-info/PKG-INFO` & `OCR_with_format-0.8/src/OCR_with_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR-with-format
-Version: 0.7
+Version: 0.8
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,36 +697,37 @@
 
 ## Usage
 ```
 NAME
     OCR_with_format
 
 SYNOPSIS
-    OCR_with_format IMG_PATH THRESHOLDING_METHOD <flags>
+    OCR_with_format IMG_PATH <flags>
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
-    THRESHOLDING_METHOD
+
+FLAGS
+    --thresholding_method=THRESHOLDING_METHOD
         Type: str
+        Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
-
-FLAGS
     -l, --language=LANGUAGE
         Type: str
         Default: 'eng'
         language to look for in the image
     -o, --output_path=OUTPUT_PATH
         Type: Optional[str]
         Default: None
         if not None, will output to this path and erase its previous content.
-    -t, --tesseract_args=TESSERACT_ARGS
+    --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
     -c, --comparison_run=COMPARISON_RUN
```

