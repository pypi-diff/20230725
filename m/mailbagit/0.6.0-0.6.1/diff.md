# Comparing `tmp/mailbagit-0.6.0.tar.gz` & `tmp/mailbagit-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailbagit-0.6.0.tar", last modified: Thu Jun 22 18:07:49 2023, max compression
+gzip compressed data, was "mailbagit-0.6.1.tar", last modified: Tue Jul 25 14:34:55 2023, max compression
```

## Comparing `mailbagit-0.6.0.tar` & `mailbagit-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.844214 mailbagit-0.6.0/
--rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     5882 2023-06-22 18:07:49.843213 mailbagit-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.760215 mailbagit-0.6.0/mailbagit/
--rw-rw-rw-   0        0        0    12594 2023-06-22 14:02:26.000000 mailbagit-0.6.0/mailbagit/__init__.py
--rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/controller.py
--rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.6.0/mailbagit/derivative.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.799214 mailbagit-0.6.0/mailbagit/derivatives/
--rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/eml.py
--rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/example.py
--rw-rw-rw-   0        0        0     2773 2023-06-22 15:09:33.000000 mailbagit-0.6.0/mailbagit/derivatives/html.py
--rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/derivatives/mbox.py
--rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/pdf.py
--rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/pdf_chrome.py
--rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/derivatives/txt.py
--rw-rw-rw-   0        0        0    14611 2023-06-22 14:01:35.000000 mailbagit-0.6.0/mailbagit/derivatives/warc.py
--rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/email_account.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.813214 mailbagit-0.6.0/mailbagit/formats/
--rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/eml.py
--rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/example.py
--rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.6.0/mailbagit/formats/mbox.py
--rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/formats/msg.py
--rw-rw-rw-   0        0        0    20552 2023-06-22 17:36:18.000000 mailbagit-0.6.0/mailbagit/formats/pst.py
--rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/globals.py
--rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.6.0/mailbagit/guided.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.820217 mailbagit-0.6.0/mailbagit/helper/
--rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.6.0/mailbagit/helper/__init__.py
--rw-rw-rw-   0        0        0     3781 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/helper/common.py
--rw-rw-rw-   0        0        0     4808 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/helper/controller.py
--rw-rw-rw-   0        0        0     8257 2023-06-22 15:10:17.000000 mailbagit-0.6.0/mailbagit/helper/derivative.py
--rw-rw-rw-   0        0        0    16733 2023-06-22 17:10:09.000000 mailbagit-0.6.0/mailbagit/helper/format.py
--rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/loggerx.py
--rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.6.0/mailbagit/models.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.780213 mailbagit-0.6.0/mailbagit.egg-info/
--rw-rw-rw-   0        0        0     5882 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      455 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-06-22 18:07:49.000000 mailbagit-0.6.0/mailbagit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 18:07:49.844214 mailbagit-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2023-06-22 14:02:39.000000 mailbagit-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:07:49.841213 mailbagit-0.6.0/tests/
--rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.6.0/tests/test_controller.py
--rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.6.0/tests/test_formats.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.049769 mailbagit-0.6.1/
+-rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     5882 2023-07-25 14:34:55.048795 mailbagit-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:54.998776 mailbagit-0.6.1/mailbagit/
+-rw-rw-rw-   0        0        0    12594 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/__init__.py
+-rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/controller.py
+-rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.6.1/mailbagit/derivative.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.028782 mailbagit-0.6.1/mailbagit/derivatives/
+-rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/derivatives/eml.py
+-rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/derivatives/example.py
+-rw-rw-rw-   0        0        0     2773 2023-06-22 15:09:33.000000 mailbagit-0.6.1/mailbagit/derivatives/html.py
+-rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/derivatives/mbox.py
+-rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/derivatives/pdf.py
+-rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/derivatives/pdf_chrome.py
+-rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/derivatives/txt.py
+-rw-rw-rw-   0        0        0    14611 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/derivatives/warc.py
+-rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/email_account.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.035769 mailbagit-0.6.1/mailbagit/formats/
+-rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/formats/eml.py
+-rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/formats/example.py
+-rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.6.1/mailbagit/formats/mbox.py
+-rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/formats/msg.py
+-rw-rw-rw-   0        0        0    20552 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/formats/pst.py
+-rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/globals.py
+-rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.6.1/mailbagit/guided.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.042778 mailbagit-0.6.1/mailbagit/helper/
+-rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.6.1/mailbagit/helper/__init__.py
+-rw-rw-rw-   0        0        0     3787 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/helper/common.py
+-rw-rw-rw-   0        0        0     5606 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/helper/controller.py
+-rw-rw-rw-   0        0        0     8257 2023-06-22 15:10:17.000000 mailbagit-0.6.1/mailbagit/helper/derivative.py
+-rw-rw-rw-   0        0        0    16733 2023-07-25 14:30:15.000000 mailbagit-0.6.1/mailbagit/helper/format.py
+-rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/loggerx.py
+-rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.6.1/mailbagit/models.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.016774 mailbagit-0.6.1/mailbagit.egg-info/
+-rw-rw-rw-   0        0        0     5882 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      455 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-07-25 14:34:54.000000 mailbagit-0.6.1/mailbagit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:34:55.049769 mailbagit-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2023-07-25 14:30:15.000000 mailbagit-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:34:55.046772 mailbagit-0.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.6.1/tests/test_controller.py
+-rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.6.1/tests/test_formats.py
```

### Comparing `mailbagit-0.6.0/LICENSE` & `mailbagit-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/PKG-INFO` & `mailbagit-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.6.0
+Version: 0.6.1
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.6.0/README.md` & `mailbagit-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/__init__.py` & `mailbagit-0.6.1/mailbagit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version of the mailbagit package
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 import os
 from pathlib import Path
 from bagit import _make_parser, Bag, BagHeaderAction, DEFAULT_CHECKSUMS
 import importlib
 from mailbagit.loggerx import setup_logging, get_logger
 from argparse import ArgumentParser, FileType
```

### Comparing `mailbagit-0.6.0/mailbagit/controller.py` & `mailbagit-0.6.1/mailbagit/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivative.py` & `mailbagit-0.6.1/mailbagit/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/eml.py` & `mailbagit-0.6.1/mailbagit/derivatives/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/example.py` & `mailbagit-0.6.1/mailbagit/derivatives/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/html.py` & `mailbagit-0.6.1/mailbagit/derivatives/html.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/mbox.py` & `mailbagit-0.6.1/mailbagit/derivatives/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/pdf.py` & `mailbagit-0.6.1/mailbagit/derivatives/pdf.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/pdf_chrome.py` & `mailbagit-0.6.1/mailbagit/derivatives/pdf_chrome.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/txt.py` & `mailbagit-0.6.1/mailbagit/derivatives/txt.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/derivatives/warc.py` & `mailbagit-0.6.1/mailbagit/derivatives/warc.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/email_account.py` & `mailbagit-0.6.1/mailbagit/email_account.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/formats/eml.py` & `mailbagit-0.6.1/mailbagit/formats/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/formats/example.py` & `mailbagit-0.6.1/mailbagit/formats/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/formats/mbox.py` & `mailbagit-0.6.1/mailbagit/formats/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/formats/msg.py` & `mailbagit-0.6.1/mailbagit/formats/msg.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/formats/pst.py` & `mailbagit-0.6.1/mailbagit/formats/pst.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/guided.py` & `mailbagit-0.6.1/mailbagit/guided.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/helper/common.py` & `mailbagit-0.6.1/mailbagit/helper/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     Parameters:
         path (str): Unsafe path/to/stuff
     Returns:
         out_path (str): Safe path/to/stuff
     """
     if os.name == "nt":
-        specials = ["<", ">", ":", '"', "/", "|", "?", "*"]
+        specials = ["<", ">", ":", '"', "/", "\\", "|", "?", "*"]
         special_names = [
             "CON",
             "PRN",
             "AUX",
             "NUL",
             "COM1",
             "COM2",
```

### Comparing `mailbagit-0.6.0/mailbagit/helper/controller.py` & `mailbagit-0.6.1/mailbagit/helper/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os, shutil, glob
 import datetime
 from time import time
 import csv
+import random
+import string
 
 import mailbagit.helper.common as common
 import mailbagit.globals as globals
 
 from mailbagit.loggerx import get_logger
 
 log = get_logger()
@@ -38,15 +40,15 @@
     dt = f"{e.year}-{e.month:02d}-{e.day:02d} {e.hour:02d}:{e.minute:02d}.{e.second:02d}"
     message_type = f'[{style["cy"][0]}{prefix}{style["b"][1]}]'
     # deco_prefix = f'{style["b"][0]}{prefix}{style["b"][1]}'
     # statusBar = f'|{bar}| {percent}% [{current}MB out of {total}MB] {suffix}'
     status = f"{percent}% [Processed {current} of {total} messages] {remaining_time}s remaining"
 
     # Originally printed timestamp and [Progress] first, which was eliminated for screen readers
-    #print(f"\r{dt} {message_type} {status}", end=print_End)
+    # print(f"\r{dt} {message_type} {status}", end=print_End)
     print(f"\r{status}", end=print_End)
 
 
 def progressMessage(msg, print_End="\r"):
     """
     Shows a message as progress. Useful since it make take awhile to save large bags
     even after all messages have been processed.
@@ -94,23 +96,37 @@
                 writtenName = attachment.WrittenName
             attachment_row = [attachment.Name, writtenName, attachment.MimeType, attachment.Content_ID]
         else:
             # If there is no filename available, just use and integer
             # The format parsers raise an error about this
             writtenName = attachment.WrittenName
             attachment_row = ["", writtenName, attachment.MimeType, attachment.Content_ID]
-        attachment_data.append(attachment_row)
 
         log.debug("Saving Attachment:" + str(attachment.Name))
         log.debug("Type:" + str(attachment.MimeType))
         if not dry_run:
             attachment_path = os.path.join(message_attachments_dir, writtenName)
-            f = open(attachment_path, "wb")
-            f.write(attachment.File)
-            f.close()
+            try:
+                f = open(attachment_path, "wb")
+                f.write(attachment.File)
+                f.close()
+            except Exception as e:
+                random_name = "".join(random.choices(string.ascii_letters + string.digits, k=8))
+                desc = (
+                    f"Failed to write attachment {attachment.Name} even as normalized name {writtenName}. Instead writing as {random_name}."
+                )
+                errors = common.handle_error(errors, None, desc, "error")
+                attachment_row = [attachment.Name, random_name, attachment.MimeType, attachment.Content_ID]
+                attachment_path = os.path.join(message_attachments_dir, random_name)
+                f = open(attachment_path, "wb")
+                f.write(attachment.File)
+                f.close()
+
+        # add line to CSV for attachment
+        attachment_data.append(attachment_row)
 
     # Write attachments.csv
     if not dry_run:
         with open(attachments_csv, "w", encoding="utf-8", newline="") as csv_file:
             writer = csv.writer(csv_file)
             writer.writerows(attachment_data)
             csv_file.close()
```

### Comparing `mailbagit-0.6.0/mailbagit/helper/derivative.py` & `mailbagit-0.6.1/mailbagit/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/helper/format.py` & `mailbagit-0.6.1/mailbagit/helper/format.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/loggerx.py` & `mailbagit-0.6.1/mailbagit/loggerx.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit/models.py` & `mailbagit-0.6.1/mailbagit/models.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/mailbagit.egg-info/PKG-INFO` & `mailbagit-0.6.1/mailbagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.6.0
+Version: 0.6.1
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mailbagit-0.6.0/mailbagit.egg-info/SOURCES.txt` & `mailbagit-0.6.1/mailbagit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/setup.py` & `mailbagit-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mailbagit",
-    version="0.6.0",
+    version="0.6.1",
     author="Gregory Wiedeman",
     author_email="gwiedeman@albany.edu",
     description="A tool for preserving email with multiple masters.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UAlbanyArchives/mailbag",
     packages=setuptools.find_namespace_packages(exclude=("tests")),
```

### Comparing `mailbagit-0.6.0/tests/test_controller.py` & `mailbagit-0.6.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.6.0/tests/test_formats.py` & `mailbagit-0.6.1/tests/test_formats.py`

 * *Files identical despite different names*

