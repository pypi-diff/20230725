# Comparing `tmp/pydelorean-1.5.0.tar.gz` & `tmp/pydelorean-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.5.0.tar", last modified: Tue Jul 25 03:35:57 2023, max compression
+gzip compressed data, was "pydelorean-1.5.1.tar", last modified: Tue Jul 25 04:06:46 2023, max compression
```

## Comparing `pydelorean-1.5.0.tar` & `pydelorean-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.909291 pydelorean-1.5.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-1.5.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 03:35:57.909291 pydelorean-1.5.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1979 2023-07-09 04:04:35.000000 pydelorean-1.5.0/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.906291 pydelorean-1.5.0/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1602 2023-07-16 23:17:50.000000 pydelorean-1.5.0/pydelorean/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/base/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-16 23:33:35.000000 pydelorean-1.5.0/pydelorean/base/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1927 2023-07-16 23:56:46.000000 pydelorean-1.5.0/pydelorean/base/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1832 2023-07-16 23:36:20.000000 pydelorean-1.5.0/pydelorean/base/node.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3190 2023-07-16 23:57:26.000000 pydelorean-1.5.0/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      191 2023-07-09 03:51:43.000000 pydelorean-1.5.0/pydelorean/errors.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      604 2023-07-09 03:51:12.000000 pydelorean-1.5.0/pydelorean/files.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      672 2023-07-16 23:34:45.000000 pydelorean-1.5.0/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1889 2023-07-18 02:20:26.000000 pydelorean-1.5.0/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5306 2023-07-25 03:31:41.000000 pydelorean-1.5.0/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2735 2023-07-16 23:21:02.000000 pydelorean-1.5.0/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.907291 pydelorean-1.5.0/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 03:35:57.909291 pydelorean-1.5.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-07-25 03:33:51.000000 pydelorean-1.5.0/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.649681 pydelorean-1.5.1/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-1.5.1/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 04:06:46.649681 pydelorean-1.5.1/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1979 2023-07-09 04:04:35.000000 pydelorean-1.5.1/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.647681 pydelorean-1.5.1/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1602 2023-07-16 23:17:50.000000 pydelorean-1.5.1/pydelorean/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.648681 pydelorean-1.5.1/pydelorean/base/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-16 23:33:35.000000 pydelorean-1.5.1/pydelorean/base/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1927 2023-07-16 23:56:46.000000 pydelorean-1.5.1/pydelorean/base/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1269 2023-07-25 03:59:42.000000 pydelorean-1.5.1/pydelorean/base/node.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3190 2023-07-16 23:57:26.000000 pydelorean-1.5.1/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      191 2023-07-09 03:51:43.000000 pydelorean-1.5.1/pydelorean/errors.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      604 2023-07-09 03:51:12.000000 pydelorean-1.5.1/pydelorean/files.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.648681 pydelorean-1.5.1/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      672 2023-07-16 23:34:45.000000 pydelorean-1.5.1/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1943 2023-07-25 03:58:57.000000 pydelorean-1.5.1/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5209 2023-07-25 04:00:07.000000 pydelorean-1.5.1/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.649681 pydelorean-1.5.1/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2735 2023-07-16 23:21:02.000000 pydelorean-1.5.1/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 04:06:46.648681 pydelorean-1.5.1/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 04:06:46.000000 pydelorean-1.5.1/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-25 04:06:46.000000 pydelorean-1.5.1/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 04:06:46.000000 pydelorean-1.5.1/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 04:06:46.000000 pydelorean-1.5.1/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 04:06:46.000000 pydelorean-1.5.1/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 04:06:46.649681 pydelorean-1.5.1/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-07-25 04:03:31.000000 pydelorean-1.5.1/setup.py
```

### Comparing `pydelorean-1.5.0/LICENSE` & `pydelorean-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/PKG-INFO` & `pydelorean-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.0
+Version: 1.5.1
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.0.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
```

### Comparing `pydelorean-1.5.0/README.rst` & `pydelorean-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/__init__.py` & `pydelorean-1.5.1/pydelorean/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/base/forest.py` & `pydelorean-1.5.1/pydelorean/base/forest.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/base/node.py` & `pydelorean-1.5.1/pydelorean/base/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,67 +9,42 @@
 
 class TextNode(Node):
     
     FRACTION_PRINTABLE = 0.25   
     
     def __init__(self, name:str, text:str, **kwargs):
         self.text = text
+        self.corpus = text
         super().__init__(name, **kwargs)
         
         
     def __getitem__(self, index:int):
         if index < 0 or index >= len(self.text):
             raise IndexError("Index out of bounds")
         return self.text[index]
            
     def __str__(self):
         return self.text[0:min(10, int(self.FRACTION_PRINTABLE * len(self.text)))] + " ..."
 
     def __repr__(self) -> str:
         return "(Text) " + self.text[0:min(10, int(self.FRACTION_PRINTABLE * len(self.text)))] + " ..."
     
-    @property
-    def text(self):
-        return self._text
-    
-    @property
-    def corpus(self):
-        return self._text
-    
-    @text.setter
-    def text(self, text:str):
-        self._text = text
-
 
 class HeaderNode(Node):
     
     def __init__(self, header:str, headerNumber:int, **kwargs):
         self.header = header
-        self._header_level = headerNumber
-        self._corpus = []
+        self.header_level = headerNumber
+        self.corpus = header + "\n"
         super().__init__(header, **kwargs)
         
     def __str__(self):
         return self.header
     
     def __repr__(self):
         return f"(h{self._header_level}) {self.header}"
     
-    @property
-    def header_level(self) -> int:
-        return self._header_level
-    
-    @header_level.setter
-    def header_level(self, headerNumber:int) -> None:
-        self._header_level = headerNumber
-
-    def __pow__(self, other):
-        self._corpus.append(other)
-        
-    @property
-    def corpus(self) -> str:
-        final_text = self.header + "\n"
-        for child in self._corpus:
-            final_text += child.corpus + "\n"
-        return final_text    
+    def __and__(self, other):
+        self.corpus += "\n" + other.corpus
+
```

### Comparing `pydelorean-1.5.0/pydelorean/delorean.py` & `pydelorean-1.5.1/pydelorean/delorean.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/files.py` & `pydelorean-1.5.1/pydelorean/files.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/parser/__init__.py` & `pydelorean-1.5.1/pydelorean/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean/parser/parser.py` & `pydelorean-1.5.1/pydelorean/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
         HEADER_PATTERN = r"^(#+\s+)(.*)"
         
         tree = build_tree(self.text, document_name=self.document_name, header_pattern=HEADER_PATTERN)
+        build_corpus(tree)
         return tree
         
 
 class RestructuredParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
         HEADER_PATTERN = r"^(=+|-+|`+|'+|\^+|\*+|\.+|~+|\++)\s+(.+)\s+\1$"
         
         tree = build_tree(self.text, document_name=self.document_name, header_pattern=HEADER_PATTERN)
+        build_corpus(tree)
         return tree
    
 
 class AsciiDocParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
```

### Comparing `pydelorean-1.5.0/pydelorean/parser/utils.py` & `pydelorean-1.5.1/pydelorean/parser/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     
     for paragraph in paragraphs:
         print(paragraph)
         return_list.append(TextNode(name=paragraph, text=paragraph))
         
     return return_list
 
+
 def build_tree(inputText:str, *args, **kwargs) -> Node:
 
     assert isinstance(inputText, str), "inputText must be a string"
     if inputText == "":
         return None
     
     root = HeaderNode(header=kwargs["document_name"], headerNumber=0)
@@ -35,24 +36,24 @@
     
     # BASE CASE
     # Check if it is only text (since there are no header indices)
     if len(indices) == 0:
         list_of_text_nodes = parse_text(inputText)
         for text_node in list_of_text_nodes:
             root >> text_node
-            root ** text_node
+            # root ** text_node
         return root
     
     # Is there text before the first header?
     if indices[0][0] != 0:
         textBefore = inputText[0:indices[0][0]]
         list_of_text_nodes = parse_text(textBefore)
         for text_node in list_of_text_nodes:
             root >> text_node
-            root ** text_node
+            # root ** text_node
 
     # Use a stack to keep track of the header levels.
     stack = []
 
     # Iterate over all the headers and accordingly build the tree.
     for currHeader in indices:
 
@@ -61,15 +62,15 @@
         
         # If this is the first header then create the header node automatically.
         if len(stack) == 0:
             
             # Create the header node with the current header.
             node = HeaderNode(header=currHeaderText, headerNumber=currHeaderLevel)
             root >> node
-            root ** node
+            # root ** node
                         
             # Add the node to the stack
             stack.append((currHeaderLevel, currHeader, node))
             continue
         else:
             lastHeader = stack[-1]
         
@@ -78,63 +79,67 @@
             
             # Extract the text between the current header and the previous header
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
                 list_of_text_nodes = parse_text(textBetween)
                 for text_node in list_of_text_nodes:
                     lastHeader[-1] >> text_node
-                    lastHeader[-1] ** text_node
-                # node = TextNode(name=textBetween, text=textBetween)
-                # lastHeader[-1] >> node
-                # lastHeader[-1] ** node
+                    # lastHeader[-1] ** text_node
                 
             # Create the header node and add it to the stack
             node = HeaderNode(header=currHeaderText, headerNumber=currHeaderLevel)
             lastHeader[-1] >> node
-            lastHeader[-1] ** node
+            # lastHeader[-1] ** node
             
             stack.append((currHeaderLevel, currHeader, node))
             
         # CASE 2: If the current header level is less than or equal to the starting header level then we need to create a new tree.
         elif currHeaderLevel <= lastHeader[0]:
             
             # Get the text between 
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
                 list_of_text_nodes = parse_text(textBetween)
                 for text_node in list_of_text_nodes:
                     lastHeader[-1] >> text_node
-                    lastHeader[-1] ** text_node
+                    # lastHeader[-1] ** text_node
                                             
             # Pop off until you get to the node with a lower level than the current header level
             while len(stack) > 0:
                 if stack[-1][0] >= currHeaderLevel:
                     stack.pop()
                 else:
                     break
             
             if len(stack) == 0:
                 
                 node = HeaderNode(header=currHeaderText, headerNumber=currHeaderLevel)
                 root >> node
-                root ** node
+                # root ** node
             else:
                 node = HeaderNode(header=currHeaderText, headerNumber=currHeaderLevel)
                 stack[-1][-1] >> node
-                stack[-1][-1] ** node
+                # stack[-1][-1] ** node
                 
             stack.append((currHeaderLevel, currHeader, node))
 
 
     # Check if there is any text after the last header
     if indices[-1][1] != len(inputText):
         textEnd = inputText[indices[-1][1]:].strip()
         list_of_text_nodes = parse_text(textEnd)
         for text_node in list_of_text_nodes:
             stack[-1][-1] >> text_node
-            stack[-1][-1] ** text_node
-        # node = TextNode(name=textEnd, text=textEnd)
-        # stack[-1][-1] >> node
-        # stack[-1][-1] ** node
-        
+            # stack[-1][-1] ** text_node
     return root
 
+
+
+def build_corpus(root:Node):
+    
+    if root.is_leaf:
+        return 
+    
+    for child in root.children:
+        build_corpus(child)
+        root & child
+
```

### Comparing `pydelorean-1.5.0/pydelorean/tools/__init__.py` & `pydelorean-1.5.1/pydelorean/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.0/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.5.1/pydelorean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.0
+Version: 1.5.1
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.0.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
```

### Comparing `pydelorean-1.5.0/setup.py` & `pydelorean-1.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.5.0'
+VERSION = '1.5.1'
 DESCRIPTION = 'A package to convert between markup documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

