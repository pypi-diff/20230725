# Comparing `tmp/colordemo-0.2.tar.gz` & `tmp/colordemo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colordemo-0.2.tar", last modified: Sun Jul 23 05:18:30 2023, max compression
+gzip compressed data, was "colordemo-0.2.1.tar", last modified: Tue Jul 25 05:00:48 2023, max compression
```

## Comparing `colordemo-0.2.tar` & `colordemo-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35147 2023-07-06 06:17:57.182174 colordemo-0.2/COPYING
--rw-r--r--   0        0        0     6317 2023-07-23 05:13:53.588444 colordemo-0.2/README.md
--rw-r--r--   0        0        0     1014 2023-07-23 04:19:34.075191 colordemo-0.2/colordemo/__init__.py
--rwxr-xr-x   0        0        0     5344 2023-07-23 04:19:34.075191 colordemo-0.2/colordemo/__main__.py
--rw-r--r--   0        0        0    13792 2023-07-23 04:24:27.225184 colordemo-0.2/colordemo/color_display.py
--rw-r--r--   0        0        0      820 2023-07-23 04:19:34.075191 colordemo-0.2/colordemo/colors.py
--rw-r--r--   0        0        0    14331 2023-07-23 04:19:34.075191 colordemo-0.2/colordemo/terminal_query.py
--rw-r--r--   0        0        0      837 2023-07-23 05:18:30.228437 colordemo-0.2/pyproject.toml
--rw-r--r--   0        0        0    47500 1970-01-01 00:00:00.000000 colordemo-0.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-06 06:17:57.182174 colordemo-0.2.1/COPYING
+-rw-r--r--   0        0        0     6358 2023-07-25 02:06:14.521093 colordemo-0.2.1/README.md
+-rw-r--r--   0        0        0     1014 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/__init__.py
+-rwxr-xr-x   0        0        0     5344 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/__main__.py
+-rw-r--r--   0        0        0    13792 2023-07-23 04:24:27.225184 colordemo-0.2.1/colordemo/color_display.py
+-rw-r--r--   0        0        0      820 2023-07-23 04:19:34.075191 colordemo-0.2.1/colordemo/colors.py
+-rw-r--r--   0        0        0    14220 2023-07-25 02:09:12.741089 colordemo-0.2.1/colordemo/terminal_query.py
+-rw-r--r--   0        0        0      839 2023-07-25 05:00:48.777500 colordemo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    47543 1970-01-01 00:00:00.000000 colordemo-0.2.1/PKG-INFO
```

### Comparing `colordemo-0.2/COPYING` & `colordemo-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `colordemo-0.2/README.md` & `colordemo-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 ### Unsupported terminals
 
 - Konsole-based terminals, which are buggy:
   - Konsole
   - yakuake
   - (etc.)
 - terminology
+- st (unpatched)
 - Linux basic TTY (text mode without X)
 - (etc.)
 
 Some terminals (like terminology) don't seem to allow their colors to be
 queried dynamically, so all RGB queries will fail, but the failure can
 be detected. The demo script will therefore be able to output a color
 table, but without RGB values.
@@ -181,9 +182,10 @@
 # Color components are floating-point numbers in the range [0, 1].
 # To convert these to two-digit hex codes:
 r_hex = '%02x' % (int(r * 0xffff) // 256)  # etc.
 ```
 
 ## Credits
 
-- dranjan (Darsh Ranjan): initial implementation
+- dranjan: main implementation
 - oblique: improved tmux support
+- Xyne: much useful discussion and review
```

### Comparing `colordemo-0.2/colordemo/__init__.py` & `colordemo-0.2.1/colordemo/__init__.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2/colordemo/__main__.py` & `colordemo-0.2.1/colordemo/__main__.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2/colordemo/color_display.py` & `colordemo-0.2.1/colordemo/color_display.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2/colordemo/colors.py` & `colordemo-0.2.1/colordemo/colors.py`

 * *Files identical despite different names*

### Comparing `colordemo-0.2/colordemo/terminal_query.py` & `colordemo-0.2.1/colordemo/terminal_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 #   along with termcolors.  If not, see
 #   <http://www.gnu.org/licenses/>.
 
 import os
 import re
 import select
 import termios
-from sys import version_info
 
 from .colors import RGBAColor
 
 #######################################################################
 # Query-related error conditions
 
 
@@ -444,19 +443,14 @@
             self.flush_input()
 
         os.write(self.fd, query.encode())
 
         response = ""
 
         while self.P.poll(timeout):
-            s = os.read(self.fd, 4096)
-            if version_info.major >= 3:
-                s = s.decode()
-            response += s
-
+            response += os.read(self.fd, 4096).decode()
             m = self.re_guard.match(response)
-
             if m:
                 return m.group(1)
         else:
             self.num_errors += 1
             raise NoResponseError(query)
```

### Comparing `colordemo-0.2/pyproject.toml` & `colordemo-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colordemo"
-version = "0.2"
+version = "0.2.1"
 description = "RGB queries on xterm-like terminals"
 authors = [
     { name = "Darsh Ranjan", email = "dranjan@berkeley.edu" },
 ]
 readme = "README.md"
 requires-python = ">=3.0"
 dependencies = []
```

### Comparing `colordemo-0.2/PKG-INFO` & `colordemo-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colordemo
-Version: 0.2
+Version: 0.2.1
 Summary: RGB queries on xterm-like terminals
 Author-Email: Darsh Ranjan <dranjan@berkeley.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -791,14 +791,15 @@
 ### Unsupported terminals
 
 - Konsole-based terminals, which are buggy:
   - Konsole
   - yakuake
   - (etc.)
 - terminology
+- st (unpatched)
 - Linux basic TTY (text mode without X)
 - (etc.)
 
 Some terminals (like terminology) don't seem to allow their colors to be
 queried dynamically, so all RGB queries will fail, but the failure can
 be detected. The demo script will therefore be able to output a color
 table, but without RGB values.
@@ -870,9 +871,10 @@
 # Color components are floating-point numbers in the range [0, 1].
 # To convert these to two-digit hex codes:
 r_hex = '%02x' % (int(r * 0xffff) // 256)  # etc.
 ```
 
 ## Credits
 
-- dranjan (Darsh Ranjan): initial implementation
+- dranjan: main implementation
 - oblique: improved tmux support
+- Xyne: much useful discussion and review
```

