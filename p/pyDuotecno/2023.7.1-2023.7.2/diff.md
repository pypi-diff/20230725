# Comparing `tmp/pyDuotecno-2023.7.1.tar.gz` & `tmp/pyDuotecno-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.7.1.tar", last modified: Tue Jul 11 13:25:29 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.7.2.tar", last modified: Tue Jul 25 05:30:42 2023, max compression
```

## Comparing `pyDuotecno-2023.7.1.tar` & `pyDuotecno-2023.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/
--rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.1/LICENSE
--rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.1/MANIFEST.in
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      155 2023-05-05 12:02:57.000000 pyDuotecno-2023.7.1/README.md
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.233271 pyDuotecno-2023.7.1/duotecno/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     5254 2023-07-11 13:07:49.000000 pyDuotecno-2023.7.1/duotecno/controller.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)      126 2023-05-26 08:51:17.000000 pyDuotecno-2023.7.1/duotecno/exceptions.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.1/duotecno/node.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.1/duotecno/protocol.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     3668 2023-05-26 08:51:18.000000 pyDuotecno-2023.7.1/duotecno/unit.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.236605 pyDuotecno-2023.7.1/examples/
--rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.1/examples/read.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.243272 pyDuotecno-2023.7.1/pyDuotecno.egg-info/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-11 13:25:29.000000 pyDuotecno-2023.7.1/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-11 13:23:21.000000 pyDuotecno-2023.7.1/pyproject.toml
--rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.1/requirements.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/setup.cfg
--rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.1/setup.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.223271 pyDuotecno-2023.7.1/venv/
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-11 13:25:29.259940 pyDuotecno-2023.7.1/venv/bin/
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2man.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.2/LICENSE
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.2/MANIFEST.in
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      155 2023-05-05 12:02:57.000000 pyDuotecno-2023.7.2/README.md
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.503950 pyDuotecno-2023.7.2/duotecno/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     5254 2023-07-11 13:07:49.000000 pyDuotecno-2023.7.2/duotecno/controller.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      125 2023-07-25 04:44:21.000000 pyDuotecno-2023.7.2/duotecno/exceptions.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.2/duotecno/node.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.2/duotecno/protocol.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     4395 2023-07-25 04:46:29.000000 pyDuotecno-2023.7.2/duotecno/unit.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.503950 pyDuotecno-2023.7.2/examples/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.2/examples/read.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.510617 pyDuotecno-2023.7.2/pyDuotecno.egg-info/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-25 04:44:46.000000 pyDuotecno-2023.7.2/pyproject.toml
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.2/requirements.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/setup.cfg
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.2/setup.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.493949 pyDuotecno-2023.7.2/venv/
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/venv/bin/
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rstpep2html.py
```

### Comparing `pyDuotecno-2023.7.1/LICENSE` & `pyDuotecno-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/PKG-INFO` & `pyDuotecno-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.7.1/duotecno/controller.py` & `pyDuotecno-2023.7.2/duotecno/controller.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/duotecno/node.py` & `pyDuotecno-2023.7.2/duotecno/node.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/duotecno/protocol.py` & `pyDuotecno-2023.7.2/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/duotecno/unit.py` & `pyDuotecno-2023.7.2/duotecno/unit.py`

 * *Files 15% similar despite different names*

```diff
@@ -125,11 +125,40 @@
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITDUOSWITCHSTATUS_0):
             await self._update({"state": packet.state})
             return
         await super().handlePacket(packet)
 
+    def is_opening(self):
+        if self._state == 4:
+            return True
+        return False
+
+    def is_closing(self):
+        if self._state == 3:
+            return True
+        return False
+
+    def is_closed(self):
+        if self._state == 1:
+            return True
+        return False
+
+    async def up(self):
+        """Move up."""
+        await self.stop()
+        await self.writer(f"[182,0,{self.node.address},{self.unit},4]")
+
+    async def down(self):
+        """Move down."""
+        await self.stop()
+        await self.writer(f"[182,0,{self.node.address},{self.unit},5]")
+
+    async def stop(self):
+        """Stop the motor."""
+        await self.writer(f"[182,0,{self.node.address},{self.unit},3]")
+
 
 class VirtualUnit(BaseUnit):
     _unitType: final = 7
     pass
```

### Comparing `pyDuotecno-2023.7.1/examples/read.py` & `pyDuotecno-2023.7.2/examples/read.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.7.2/pyDuotecno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.7.1/pyDuotecno.egg-info/SOURCES.txt` & `pyDuotecno-2023.7.2/pyDuotecno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/pyproject.toml` & `pyDuotecno-2023.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name        = "pyDuotecno"
 license     = {text = "Apache"}
-version     = "2023.7.1"
+version     = "2023.7.2"
 description = "Open-source home automation platform running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords    = ["home", "duotecno", "automation"]
 classifiers = [
@@ -38,15 +38,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
 
 [tool.bumpver]
-current_version = "2023.7.1"
+current_version = "2023.7.2"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2html.py` & `pyDuotecno-2023.7.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2html4.py` & `pyDuotecno-2023.7.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2html5.py` & `pyDuotecno-2023.7.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2latex.py` & `pyDuotecno-2023.7.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2man.py` & `pyDuotecno-2023.7.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2odt.py` & `pyDuotecno-2023.7.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2odt_prepstyles.py` & `pyDuotecno-2023.7.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2pseudoxml.py` & `pyDuotecno-2023.7.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2s5.py` & `pyDuotecno-2023.7.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2xetex.py` & `pyDuotecno-2023.7.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rst2xml.py` & `pyDuotecno-2023.7.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.1/venv/bin/rstpep2html.py` & `pyDuotecno-2023.7.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

