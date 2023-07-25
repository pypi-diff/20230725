# Comparing `tmp/pydelorean-1.3.5.tar.gz` & `tmp/pydelorean-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.3.5.tar", last modified: Fri Jul 14 22:25:34 2023, max compression
+gzip compressed data, was "pydelorean-1.5.0.tar", last modified: Tue Jul 25 03:35:57 2023, max compression
```

## Comparing `pydelorean-1.3.5.tar` & `pydelorean-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-1.3.5/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2422 2023-07-14 22:25:34.370834 pydelorean-1.3.5/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1979 2023-07-10 10:39:31.000000 pydelorean-1.3.5/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1602 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3887 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      191 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/errors.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      604 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/files.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       96 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1702 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4391 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2397 2023-07-14 22:23:49.000000 pydelorean-1.3.5/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1495 2023-07-10 10:39:31.000000 pydelorean-1.3.5/pydelorean/tree/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1829 2023-07-14 11:46:04.000000 pydelorean-1.3.5/pydelorean/tree/node.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-14 22:25:34.370834 pydelorean-1.3.5/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2422 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-14 22:25:34.000000 pydelorean-1.3.5/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-14 22:25:34.370834 pydelorean-1.3.5/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-14 22:25:20.000000 pydelorean-1.3.5/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.909291 pydelorean-1.5.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-1.5.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 03:35:57.909291 pydelorean-1.5.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1979 2023-07-09 04:04:35.000000 pydelorean-1.5.0/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.906291 pydelorean-1.5.0/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1602 2023-07-16 23:17:50.000000 pydelorean-1.5.0/pydelorean/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/base/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-16 23:33:35.000000 pydelorean-1.5.0/pydelorean/base/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1927 2023-07-16 23:56:46.000000 pydelorean-1.5.0/pydelorean/base/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1832 2023-07-16 23:36:20.000000 pydelorean-1.5.0/pydelorean/base/node.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3190 2023-07-16 23:57:26.000000 pydelorean-1.5.0/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      191 2023-07-09 03:51:43.000000 pydelorean-1.5.0/pydelorean/errors.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      604 2023-07-09 03:51:12.000000 pydelorean-1.5.0/pydelorean/files.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      672 2023-07-16 23:34:45.000000 pydelorean-1.5.0/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1889 2023-07-18 02:20:26.000000 pydelorean-1.5.0/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5306 2023-07-25 03:31:41.000000 pydelorean-1.5.0/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.908291 pydelorean-1.5.0/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2735 2023-07-16 23:21:02.000000 pydelorean-1.5.0/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 03:35:57.907291 pydelorean-1.5.0/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2394 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 03:35:57.000000 pydelorean-1.5.0/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 03:35:57.909291 pydelorean-1.5.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-07-25 03:33:51.000000 pydelorean-1.5.0/setup.py
```

### Comparing `pydelorean-1.3.5/LICENSE` & `pydelorean-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.3.5/PKG-INFO` & `pydelorean-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.3.5
-Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
+Version: 1.5.0
+Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.3.5.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -98,8 +97,7 @@
 documentation page here - [nil](nil)
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-1.3.5/README.rst` & `pydelorean-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydelorean-1.3.5/pydelorean/__init__.py` & `pydelorean-1.5.0/pydelorean/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup
 from .delorean import *
-from .tree import Forest
+from .base import Forest
 import re
 
 
 # TODO: Check the type of the input and call the appropriate function
 # Use the newly defined File classes for this. 
 def treeify(name:str, text:str, *args, **kwargs) -> Forest:
```

### Comparing `pydelorean-1.3.5/pydelorean/delorean.py` & `pydelorean-1.5.0/pydelorean/delorean.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,20 @@
 """ This file contains the main functions for the delorean package.
 """
-    
-import re
-
-import frontmatter
 from .files import *
-from .tree import *
+from .base import *
 from .parser import *
+from .tools import *
 
 # ==================================================================================================
 #                                           TREEIFY
 # ==================================================================================================
 
 # TODO: Rename to snake_case in the future.
 
-
-def find_backlinks(input_text:str) -> list:
-    """ 
-    Function to find all backlinks in a given text.
-    """
-    
-    backlinks = []
-
-    # Regular expression pattern to match backlinks
-    pattern = r'\[\[(.*?)\]\]'
-    backlinks = re.findall(pattern, input_text)
-    return backlinks
-
-
-def find_tags(input_text:str) -> list:
-    """
-    Function to find all tags in a given text.
-    """
-    
-    tags = []
-
-    # Regular expression pattern to match backlinks
-    pattern = r'#([a-zA-Z0-9_]+)'
-    tags = re.findall(pattern, input_text)
-    return tags
-
-
-def find_metadata(input_text:str):
-    post = frontmatter.loads(input_text)
-    return post.metadata, post.content
-
-
 def mdtreeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
     """
     Converts markdown file to a MarkdownForest
     """
     
     meta, cont = find_metadata(md)
     
@@ -75,19 +40,19 @@
     return returnForest
 
 
 def rsttreeify(name:str, rst:str, *args, **kwargs) -> RestructuredForest:
     pass
 
 
-def asciidoc_treeify(name:str, asciidoc:str, *args, **kwargs) -> AsciidocForest:
+def asciidoc_treeify(name:str, adoc:str, *args, **kwargs) -> AsciiDocForest:
     pass
 
 
-def yaml_treeify(name:str, yaml:str, *args, **kwargs) -> YamlForest:
+def yaml_treeify(name:str, yaml:str, *args, **kwargs) -> YAMLForest:
     pass
 
 
 def jsontreeify(name:str, json:str, *args, **kwargs) -> JSONForest:
     pass
 
 
@@ -147,18 +112,18 @@
 
 
 def rsttextify(forest: RestructuredForest) -> str:
     
     pass
 
 
-def asciidoctextify(forest: AsciidocForest) -> str:
+def asciidoctextify(forest: AsciiDocForest) -> str:
     pass
 
 
-def yamltextify(forest: YamlForest) -> str:
+def yamltextify(forest: YAMLForest) -> str:
     pass
 
 
 def jsontextify(forest: JSONForest) -> str:
     pass
```

### Comparing `pydelorean-1.3.5/pydelorean/files.py` & `pydelorean-1.5.0/pydelorean/files.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.3.5/pydelorean/parser/parser.py` & `pydelorean-1.5.0/pydelorean/parser/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,24 @@
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
         HEADER_PATTERN = r"^(=+|-+|`+|'+|\^+|\*+|\.+|~+|\++)\s+(.+)\s+\1$"
         
         tree = build_tree(self.text, document_name=self.document_name, header_pattern=HEADER_PATTERN)
         return tree
+   
+
+class AsciiDocParser(Parser):
+    
+    def __init__(self, document_name:str, text:str):
+        super().__init__(document_name, text)
         
+    def parse(self) -> Node:
+        pass     
+
 
 class TextParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Node:
```

### Comparing `pydelorean-1.3.5/pydelorean/parser/utils.py` & `pydelorean-1.5.0/pydelorean/parser/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 import re
-from pydelorean.tree import TextNode, HeaderNode
+from pydelorean.base import TextNode, HeaderNode
 from bigtree import Node, print_tree
 
+
+def parse_text(input_text:str) -> list[TextNode]:
+    return_list = []
+    
+    # Split the text by newlines
+    input_text = input_text.strip()
+    paragraphs = input_text.split("\n\n")    
+    
+    for paragraph in paragraphs:
+        print(paragraph)
+        return_list.append(TextNode(name=paragraph, text=paragraph))
+        
+    return return_list
+
 def build_tree(inputText:str, *args, **kwargs) -> Node:
 
     assert isinstance(inputText, str), "inputText must be a string"
     if inputText == "":
         return None
     
     root = HeaderNode(header=kwargs["document_name"], headerNumber=0)
@@ -18,25 +32,27 @@
         
     # Get all the indices of the headers
     indices = [(match.start(), match.end()) for match in matches]
     
     # BASE CASE
     # Check if it is only text (since there are no header indices)
     if len(indices) == 0:
-        text_node = TextNode(name=inputText, text=inputText)
-        root >> text_node
-        root ** text_node
+        list_of_text_nodes = parse_text(inputText)
+        for text_node in list_of_text_nodes:
+            root >> text_node
+            root ** text_node
         return root
     
     # Is there text before the first header?
     if indices[0][0] != 0:
         textBefore = inputText[0:indices[0][0]]
-        node = TextNode(name=textBefore, text=textBefore)
-        root >> node
-        root ** node
+        list_of_text_nodes = parse_text(textBefore)
+        for text_node in list_of_text_nodes:
+            root >> text_node
+            root ** text_node
 
     # Use a stack to keep track of the header levels.
     stack = []
 
     # Iterate over all the headers and accordingly build the tree.
     for currHeader in indices:
 
@@ -59,34 +75,39 @@
         
         # CASE 1: If the current header level is greater than the starting header level then keep going.
         if currHeaderLevel > lastHeader[0]:
             
             # Extract the text between the current header and the previous header
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
-                node = TextNode(name=textBetween, text=textBetween)
-                lastHeader[-1] >> node
-                lastHeader[-1] ** node
+                list_of_text_nodes = parse_text(textBetween)
+                for text_node in list_of_text_nodes:
+                    lastHeader[-1] >> text_node
+                    lastHeader[-1] ** text_node
+                # node = TextNode(name=textBetween, text=textBetween)
+                # lastHeader[-1] >> node
+                # lastHeader[-1] ** node
                 
             # Create the header node and add it to the stack
             node = HeaderNode(header=currHeaderText, headerNumber=currHeaderLevel)
             lastHeader[-1] >> node
             lastHeader[-1] ** node
             
             stack.append((currHeaderLevel, currHeader, node))
             
         # CASE 2: If the current header level is less than or equal to the starting header level then we need to create a new tree.
         elif currHeaderLevel <= lastHeader[0]:
             
             # Get the text between 
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
-                node = TextNode(name=textBetween, text=textBetween)
-                lastHeader[-1] >> node
-                lastHeader[-1] ** node
+                list_of_text_nodes = parse_text(textBetween)
+                for text_node in list_of_text_nodes:
+                    lastHeader[-1] >> text_node
+                    lastHeader[-1] ** text_node
                                             
             # Pop off until you get to the node with a lower level than the current header level
             while len(stack) > 0:
                 if stack[-1][0] >= currHeaderLevel:
                     stack.pop()
                 else:
                     break
@@ -103,13 +124,17 @@
                 
             stack.append((currHeaderLevel, currHeader, node))
 
 
     # Check if there is any text after the last header
     if indices[-1][1] != len(inputText):
         textEnd = inputText[indices[-1][1]:].strip()
-        node = TextNode(name=textEnd, text=textEnd)
-        stack[-1][-1] >> node
-        stack[-1][-1] ** node
+        list_of_text_nodes = parse_text(textEnd)
+        for text_node in list_of_text_nodes:
+            stack[-1][-1] >> text_node
+            stack[-1][-1] ** text_node
+        # node = TextNode(name=textEnd, text=textEnd)
+        # stack[-1][-1] >> node
+        # stack[-1][-1] ** node
         
     return root
```

### Comparing `pydelorean-1.3.5/pydelorean/tree/node.py` & `pydelorean-1.5.0/pydelorean/base/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from bigtree import Node
 
 # TODO: Add all the documentation and convert to snake case soon.
 
 
 class TextNode(Node):
     
-    FRACTION_PRINTABLE = 0.25
+    FRACTION_PRINTABLE = 0.25   
     
     def __init__(self, name:str, text:str, **kwargs):
         self.text = text
         super().__init__(name, **kwargs)
         
         
     def __getitem__(self, index:int):
```

### Comparing `pydelorean-1.3.5/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.5.0/pydelorean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.3.5
-Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
+Version: 1.5.0
+Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.3.5.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -98,8 +97,7 @@
 documentation page here - [nil](nil)
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-1.3.5/setup.py` & `pydelorean-1.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.3.5'
-DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
+VERSION = '1.5.0'
+DESCRIPTION = 'A package to convert between markup documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/delorean",
-    packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser', 'pydelorean.tools'],
+    packages = ['pydelorean', 'pydelorean.base', 'pydelorean.parser', 'pydelorean.tools'],
     tests_require = ['unittest'],
     install_requires = ['markdown', 'bigtree', 'beautifulsoup4'],
     download_url = 'https://github.com/kj3moraes/delorean/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

