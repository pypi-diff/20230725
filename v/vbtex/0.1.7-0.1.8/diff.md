# Comparing `tmp/vbtex-0.1.7.tar.gz` & `tmp/vbtex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.7.tar", max compression
+gzip compressed data, was "vbtex-0.1.8.tar", max compression
```

## Comparing `vbtex-0.1.7.tar` & `vbtex-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.7/README.md
--rw-r--r--   0        0        0      370 2023-07-20 13:38:56.440648 vbtex-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.7/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.7/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.7/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.7/vbtex/choice_option.py
--rw-r--r--   0        0        0     1798 2023-07-20 13:38:48.707557 vbtex-0.1.7/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.7/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.7/vbtex/padded.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.8/README.md
+-rw-r--r--   0        0        0      370 2023-07-25 05:00:58.594573 vbtex-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.8/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.8/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.8/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.8/vbtex/choice_option.py
+-rw-r--r--   0        0        0     2893 2023-07-25 05:00:45.304273 vbtex-0.1.8/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.8/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.8/vbtex/padded.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.8/PKG-INFO
```

### Comparing `vbtex-0.1.7/vbtex/.DS_Store` & `vbtex-0.1.8/vbtex/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.7/vbtex/choice_option.py` & `vbtex-0.1.8/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.7/vbtex/framed.py` & `vbtex-0.1.8/vbtex/framed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import click
 import os
 import sys
 from rich.console import Console
 from .choice_option import ChoiceOption
 
+from datetime import datetime
 
 
 @click.command(
     help="Renders tex expressions into pdf"
 )
 @click.option(
     '-i',
@@ -18,31 +19,50 @@
     show_default=True,
     help="It takes std inputs and try to render as pdf"
 )
 @click.option(
     '-s',
     '--size',
     prompt='Format',
-    type=click.Choice(['SQUARE', 'VRECT', 'HRECT']),
+    type=click.Choice(['SQUARE + VRECT', 'SQUARE', 'VRECT', 'HRECT']),
     cls=ChoiceOption,
     default=1,
     show_default=True,
     help="Format of the output"
 )
 def framed(input_text, size):
-    
+   
+    def get_file_name_png(size):
+        now = datetime.now()
+        file_name = now.strftime("%Y_%m_%d@%H:%M:%S")
+        return f'{file_name}_{size.lower()}.png'
+
     if input_text is None:
         tex = click.edit()
     else:
         tex = input_text
 
     click.echo(tex)
+
+    with open(f'./content.tex', 'w') as file:
+        file.write(tex)
     
-    os.makedirs(f'./vbtex', exist_ok=True)
-    path_main = os.path.join(f'./vbtex', 'main.tex')
+#
+#    if size == 'SQUARE + VRECT':
+#        os.makedirs(f'./square', exist_ok=True)
+#        os.makedirs(f'./vrect', exist_ok=True)
+#        path_main_square = os.path.join(f'./square', 'main.tex')
+#        path_main_vrect = os.path.join(f'./vrect', 'main.tex')
+#    else:
+#        os.makedirs(f'./{size.lower()}', exist_ok=True)
+#        path_main = os.path.join(f'./{size.lower()}', 'main.tex')
+#
+    os.makedirs(f'./{size.lower()}', exist_ok=True)
+    path_main = os.path.join(f'./{size.lower()}', 'main.tex')
+
 
     
     with open(path_main, 'w') as file:
         file.write(f'\\documentclass{{article}}\n')
         file.write(f'\\usepackage{{v-equation}}\n')
         if size == 'SQUARE':
             file.write(f'\\vgeometry[5][5][0]\n')
@@ -54,25 +74,33 @@
             file.write(f'\\vgeometry[5][5][0]\n')
             
 
         file.write(f'\\begin{{document}}\n')
 
         file.write(f'\\vspace*{{\\fill}}\n\n')
         file.write(f'\\begin{{center}}\n')
-        file.write(f'{tex}\n')
+        file.write(f'\\include{{../content.tex}}\n')
         file.write(f'\\end{{center}}\n')
         file.write(f'\\vspace*{{\\fill}}\n\n')
         file.write(f'\\end{{document}}')
 
 
 
     try:
-        os.chdir("./vbtex")
+        os.chdir(f'./{size.lower()}')
         try:
             os.system("pdflatex -shell-escape main.tex")
+            try:
+                os.system(f'vbpdf instagram -r 1 1 -b {background}')
+                try:
+                    os.system(f'cp ./downloads/main_f.png ../archive/{get_file_name_png(size)}')
+                except:
+                    click.echo("Failed to archive")
+            except:
+                click.echo("Failed to run vbpdf instagram")
         except:
             click.echo("Failed to rum pdflatex")
     except:
         click.echo("Failed to run cddir")
```

### Comparing `vbtex-0.1.7/vbtex/padded.py` & `vbtex-0.1.8/vbtex/padded.py`

 * *Files identical despite different names*

