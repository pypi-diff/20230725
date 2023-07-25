# Comparing `tmp/pyTermUI-1.2.2.tar.gz` & `tmp/pyTermUI-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTermUI-1.2.2.tar", last modified: Mon Jul 24 09:35:05 2023, max compression
+gzip compressed data, was "pyTermUI-1.2.3.tar", last modified: Tue Jul 25 07:11:59 2023, max compression
```

## Comparing `pyTermUI-1.2.2.tar` & `pyTermUI-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/
--rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      995 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-24 09:23:00.000000 pyTermUI-1.2.2/README.md
--rw-rw-rw-   0        0        0      681 2023-07-24 09:31:36.000000 pyTermUI-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.260666 pyTermUI-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.323893 pyTermUI-1.2.2/src/pyTermUI/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/src/pyTermUI/Toolkit/
--rw-rw-rw-   0        0        0     1253 2023-07-23 05:57:56.000000 pyTermUI-1.2.2/src/pyTermUI/Toolkit/asciiart.py
--rw-rw-rw-   0        0        0     2342 2023-07-23 08:27:42.000000 pyTermUI-1.2.2/src/pyTermUI/Toolkit/hover.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/__init__.py
--rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/button.py
--rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.2/src/pyTermUI/checkbox.py
--rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/colors.py
--rw-rw-rw-   0        0        0     2515 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/element.py
--rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/position.py
--rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/region.py
--rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/text.py
--rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.2/src/pyTermUI/textbox.py
--rw-rw-rw-   0        0        0     4856 2023-07-23 07:42:44.000000 pyTermUI-1.2.2/src/pyTermUI/ui.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/src/pyTermUI.egg-info/
--rw-rw-rw-   0        0        0      995 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:59.248355 pyTermUI-1.2.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      995 2023-07-25 07:11:59.247176 pyTermUI-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-24 09:23:00.000000 pyTermUI-1.2.3/README.md
+-rw-rw-rw-   0        0        0      681 2023-07-25 07:07:26.000000 pyTermUI-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 07:11:59.248355 pyTermUI-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:59.180544 pyTermUI-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:59.232622 pyTermUI-1.2.3/src/pyTermUI/
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:59.246147 pyTermUI-1.2.3/src/pyTermUI/Toolkit/
+-rw-rw-rw-   0        0        0     1289 2023-07-25 04:35:59.000000 pyTermUI-1.2.3/src/pyTermUI/Toolkit/asciiart.py
+-rw-rw-rw-   0        0        0     2421 2023-07-25 07:10:53.000000 pyTermUI-1.2.3/src/pyTermUI/Toolkit/hover.py
+-rw-rw-rw-   0        0        0     4459 2023-07-25 04:33:07.000000 pyTermUI-1.2.3/src/pyTermUI/Toolkit/taskhandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/__init__.py
+-rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/button.py
+-rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.3/src/pyTermUI/checkbox.py
+-rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/colors.py
+-rw-rw-rw-   0        0        0     3398 2023-07-25 07:05:39.000000 pyTermUI-1.2.3/src/pyTermUI/element.py
+-rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/position.py
+-rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/region.py
+-rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.3/src/pyTermUI/text.py
+-rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.3/src/pyTermUI/textbox.py
+-rw-rw-rw-   0        0        0     5477 2023-07-25 04:59:20.000000 pyTermUI-1.2.3/src/pyTermUI/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:11:59.242833 pyTermUI-1.2.3/src/pyTermUI.egg-info/
+-rw-rw-rw-   0        0        0      995 2023-07-25 07:11:59.000000 pyTermUI-1.2.3/src/pyTermUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-07-25 07:11:59.000000 pyTermUI-1.2.3/src/pyTermUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:11:59.000000 pyTermUI-1.2.3/src/pyTermUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-25 07:11:59.000000 pyTermUI-1.2.3/src/pyTermUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 07:11:59.000000 pyTermUI-1.2.3/src/pyTermUI.egg-info/top_level.txt
```

### Comparing `pyTermUI-1.2.2/LICENSE` & `pyTermUI-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/PKG-INFO` & `pyTermUI-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.2
+Version: 1.2.3
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
 Author-email: iiVeil <zhuebner03@gmail.com>
 Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyTermUI-1.2.2/pyproject.toml` & `pyTermUI-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 dynamic = ["dependencies"]
 name = "pyTermUI"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="iiVeil", email="zhuebner03@gmail.com" },
 ]
 description = "pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyTermUI-1.2.2/src/pyTermUI/Toolkit/asciiart.py` & `pyTermUI-1.2.3/src/pyTermUI/Toolkit/asciiart.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,8 +28,10 @@
         """
         for i, line in enumerate(self.lines):
             position = Position(self.center.x-floor(len(line)/2),
                                 self.center.y-len(self.lines)+i)
             element = Text(line, position)
             self.elements.append(element)
             self.region.add_element(element)
-        
+        
+    def end(self):
+        return
```

### Comparing `pyTermUI-1.2.2/src/pyTermUI/button.py` & `pyTermUI-1.2.3/src/pyTermUI/button.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/checkbox.py` & `pyTermUI-1.2.3/src/pyTermUI/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/colors.py` & `pyTermUI-1.2.3/src/pyTermUI/colors.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/element.py` & `pyTermUI-1.2.3/src/pyTermUI/element.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import curses
+from math import floor
 from .position import Position
 
 
 class Element:
     """
     ? Description
     * * An element that exists within a region
@@ -44,14 +45,35 @@
             string (str): The string to add
             options (int, optional): Other options: color, formatting, etc. Defaults to 0.
         """
         if y >= curses.LINES-1 or x >= curses.COLS-1:
             return
         self.region.ui.window.addstr(y, x, string, options)
 
+    def centerX(self):
+        """Center this element on the horizontal axis in its region."""
+        if self.region == None:
+            return
+        center = self.region.size.half() - Position(floor(self.size.x/2), 0)
+        self.move(center)
+        
+    def centerY(self):
+        """Center this element on the vertical axis in its region."""
+        if self.region == None:
+            return
+        center = self.region.size.half() - Position(0, floor(self.size.y/2))
+        self.move(center)
+        
+    def centerXY(self):
+        """Center this element on both axi in its region."""
+        if self.region == None:
+            return
+        center = self.region.size.half() - Position(floor(self.size.x/2), floor(self.size.y/2))
+        self.move(center)
+    
     def move(self, position: Position):
         """Move a element
 
         Args:
             position (Position): The new position
         """
         self.start = position
@@ -70,15 +92,16 @@
 
     def calc_pack(self):
         """Recalculate an elements relative placement packing."""
         self.pack = {
             "right": Position(
                 self.size.x+self.start.x+1, self.start.y),
             "down": Position(self.start.x, self.start.y+self.size.y+1),
-            "up": Position(self.start.x, self.start.y-1)
+            "up": Position(self.start.x, self.start.y-1),
+            "left": Position(self.start.x-1, self.start.y)
         }
 
     def event_mask(self, *args):
         """An event mask for allowing other elements click events to emulate a click on this element. 
 
         This should only be used as a callback for another element.
```

### Comparing `pyTermUI-1.2.2/src/pyTermUI/position.py` & `pyTermUI-1.2.3/src/pyTermUI/position.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/region.py` & `pyTermUI-1.2.3/src/pyTermUI/region.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/text.py` & `pyTermUI-1.2.3/src/pyTermUI/text.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/textbox.py` & `pyTermUI-1.2.3/src/pyTermUI/textbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.2/src/pyTermUI/ui.py` & `pyTermUI-1.2.3/src/pyTermUI/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,52 +4,55 @@
 from .position import Position
 from .textbox import Textbox
 
 
 class UI:
     """The main UI component
     """
-    count = 0
+    class CursesInterrupt(Exception):
+        """Keyboard Interrupt within a curses input"""
+        ...
+    
     screen_initialized = False
     last_element_clicked = 0
     clickable_cooldown = 300
     last_cursor_pos = (0, 0)
     "The amount of the time in milliseconds between registered clicks. default is 300"
 
     @staticmethod
     def init_screen():
         """Initialize the curses screen. This will happen the first time any UI is created. This also adds color support.
         """
         curses.curs_set(0)
         curses.start_color()
         curses.use_default_colors()
         curses.mousemask(1)
+        curses.raw()
         # Initialize color pairs
         for i in range(0, curses.COLORS):
             if i < 255:
                 curses.init_pair(i + 1, i, -1)
         UI.screen_initialized = True
 
     def __init__(self, stdscr):
         self.window = stdscr
-        self.id = UI.count
 
         self.screen = Position(120, 30)
         self.half = self.screen.half()
         self._active = False
         self.default_color = 232
         self.draw_callback = None
         self.event_callback = None
 
         self.regions = []
+        self.toolkits = []
         
         self.cursor = Position(0,0)
         if not UI.screen_initialized:
             UI.init_screen()
-        UI.count += 1
 
     """
     This setter functions as the second half of deactivate and activate, it will hold the UI instance open until the new UI takes over
     """
     @property
     def active(self):
         return self._active
@@ -80,14 +83,23 @@
         self.regions.append(region)
         region.ui = self
         if region.color == -1:
             region.color = self.default_color
             region.echo_color()
         self.draw()
 
+    def add_toolkits(self, *args):
+        """Add toolkits to the working UI, allowing proper closing of them.
+        
+        Assuming the toolkit has a end() method. If the toolkit does not need to be cleaned up, there is no reason to add it here.
+        """
+        
+        for arg in args:
+            self.toolkits.append(arg)
+
     def swap(self, new_ui):
         """
         Swap control of the main UI loop to another UI object.
 
         This will also hide the current UI, and reveal the new UI as only one can be active at a time.
 
         Args:
@@ -133,14 +145,19 @@
                     element = self.get_clickable(position)
                     if type(element) not in [Textbox, type(None)]:
                         self.draw()
             if event == curses.KEY_RESIZE:
                 y, x = self.window.getmaxyx()
                 curses.resize_term(y, x)
                 self.draw()
+            if event == 3:
+                for toolkit in self.toolkits:
+                    toolkit.end()
+                self.deactivate()
+                curses.endwin()
             if self.event_callback is not None:
                 self.event_callback(event)
 
     def set_curs(self):
         x, y = self.cursor.x, self.cursor.y
         
         curses.setsyx(y,x)
```

### Comparing `pyTermUI-1.2.2/src/pyTermUI.egg-info/PKG-INFO` & `pyTermUI-1.2.3/src/pyTermUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.2
+Version: 1.2.3
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
 Author-email: iiVeil <zhuebner03@gmail.com>
 Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyTermUI-1.2.2/src/pyTermUI.egg-info/SOURCES.txt` & `pyTermUI-1.2.3/src/pyTermUI.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/pyTermUI/ui.py
 src/pyTermUI.egg-info/PKG-INFO
 src/pyTermUI.egg-info/SOURCES.txt
 src/pyTermUI.egg-info/dependency_links.txt
 src/pyTermUI.egg-info/requires.txt
 src/pyTermUI.egg-info/top_level.txt
 src/pyTermUI/Toolkit/asciiart.py
-src/pyTermUI/Toolkit/hover.py
+src/pyTermUI/Toolkit/hover.py
+src/pyTermUI/Toolkit/taskhandler.py
```

